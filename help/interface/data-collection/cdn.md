---
title: Weiterleiten der Datenerfassung über ein CDN
description: Erfahren Sie, wie Sie ein Content Delivery Network (CDN) konfigurieren, um Datenerfassungsanfragen an Adobe weiterzuleiten, ohne die Datenqualität zu beeinträchtigen.
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
source-git-commit: e1185eeafc809b036b10955880536db7a576ca0b
workflow-type: tm+mt
source-wordcount: '1421'
ht-degree: 0%
---
# Weiterleiten der Datenerfassung über ein CDN

Einige Unternehmen leiten Datenerfassungsanfragen über ihr Content Delivery Network (CDN) weiter, anstatt sie direkt an Adobe zu senden. Häufige Gründe sind der Schutz vor Web Application Firewall (WAF), Unternehmensrichtlinien, die erfordern, dass der gesamte Website-Traffic durch ein CDN geleitet wird, und die Möglichkeit, den an Adobe gesendeten Traffic zu überprüfen. Das CDN empfängt Anfragen zu einem Host-Namen, dessen Eigentümer Ihr Unternehmen ist, und leitet sie dann an den Datenerfassungs-Host-Namen von Adobe weiter, der als Herkunft bezeichnet wird.

>[!IMPORTANT]
>
>Adobe kann Ihre CDN-Konfiguration nicht überprüfen oder validieren. Ihre Organisation und Ihr CDN-Anbieter sind für die korrekte Konfiguration des CDN verantwortlich. Wenden Sie sich an Ihren CDN-Anbieter, um Hilfe beim Konfigurieren Ihres CDN zu erhalten. Falsch konfigurierte CDNs können zu Datenverlust führen.

## Ursprungs-Typ auswählen {#origin-type}

| | Herkunft von Drittanbietern (empfohlen) | First-Party-Herkunft |
| --- | --- | --- |
| **Ursprungs-Host-Name** | Ihre Mandanten-ID-Subdomain von `data.adobedc.net`, z. B. `example.data.adobedc.net` | Der Hostname Ihres Erstanbieters, z. B. `data.example.com` |
| **Zertifikat auf Adobe-Servern** | Adobe-Zertifikat (`*.data.adobedc.net`) | [Kundenverwaltetes Zertifikat](customer-managed-cert.md) |
| **Zertifikatsverlängerungen** | Keine erforderlich | Ihr Unternehmen erneuert das Zertifikat und stellt es Adobe vor jedem Ablauf zur Verfügung |
| **Region-locked [RDC](rdc.md)** | Nicht unterstützt | „Unterstützt“ |
| **Verwendung** | Alle CDN-Implementierungen, es sei denn, Ihr Unternehmen benötigt einen Erstanbieter-Ursprung | Ihre Sicherheitsrichtlinie erfordert die direkte Kontrolle über das Ursprungszertifikat oder Ihr Unternehmen erfordert einen RDC-Typ mit Regionssperre |

>[!NOTE]
>
>Das von Adobe verwaltete Zertifikatprogramm [&#128279;](adobe-managed-cert.md) unterstützt keine CDN-Implementierungen. Adobe kann keine Domain-Eigentümerrechte überprüfen oder Zertifikate für Host-Namen erneuern, die auf Ihr CDN verweisen. Verwenden Sie eine Herkunft eines Drittanbieters oder eine Herkunft eines Erstanbieters mit einem [kundenverwalteten Zertifikat](customer-managed-cert.md).

## Anforderungen für alle CDN-Implementierungen {#requirements}

Adobe-Datenerfassungsbibliotheken wie AppMeasurement und die Web-SDK enthalten alles, was Adobe in jeder Anfrage benötigt. Konfigurieren Sie Ihr CDN so, dass diese Anfragen an Adobe weitergeleitet werden, ohne sie zu ändern.

>[!IMPORTANT]
>
>Ändern Sie nie den Endpunkt oder etwas, das bestimmt, wohin Daten gehen, einschließlich der Report Suite-ID (AppMeasurement) oder der Datenstrom-ID (Web SDK). Das Ändern dieser Werte verursacht Datenverlust.

Ihre CDN-Konfiguration muss:

* Leiten Sie die Anfragemethode, den URL-Pfad, die Abfragezeichenfolge und den Hauptteil ohne Änderungen weiter.
* Lassen Sie die `Host` unverändert.
* Lassen Sie die Domain, in der Adobe-Cookies gesetzt werden, unverändert.
* Behalten Sie alle Cookies bei, [&#x200B; im Abschnitt „Cookies](cookies/overview.md) dieses Handbuchs aufgeführt sind.
* Fügen Sie den `X-Forwarded-For`-Header hinzu, der die IP-Adresse des Besuchers enthält. Adobe verwendet diesen Header für die Geolocation. Ohne sie spiegeln die Geolokalisierungsdaten den Standort der CDN-Server Ihrer Besucher wider.
* Rückgabe der Adobe-Antworten an den Browser ohne Änderungen.

Ihre CDN-Konfiguration kann:

* Entfernen Sie Cookies, die Adobe nicht verwendet, z. B. Cookies von anderen Systemen auf Ihrer Site. Nicht verwandte Cookies belasten jede Anfrage zusätzlich.
* Verwenden Sie WAF, Bot-Filter oder Dienste zum Entfernen personenbezogener Daten, sofern sie nichts an den oben aufgeführten Änderungen ändern. Testen Sie diese Services mit einer Entwicklungs-Report Suite oder einem Datenstrom, bevor Sie sie auf den Produktions-Traffic anwenden. Übermäßig aggressive Filterung kann genügend Daten entfernen, um Berichte unbrauchbar zu machen.

Ihre CDN-Konfiguration darf nicht:

* Datenerfassungsanfragen oder -antworten zwischenspeichern. Jede Anfrage muss Adobe erreichen.
* Auf einen Ursprungs-Host-Namen verweisen, der nicht existiert.
* Akzeptieren abgelaufener Zertifikate oder Anheften eines bestimmten Zertifikats aus der Quelle. Adobe unterstützt die Bereitstellung abgelaufener Zertifikate nicht und kann diese jederzeit entfernen.

## Konfigurieren eines CDN mit Herkunft aus einem Drittanbieter {#third-party-origin}

Eine Drittquelle verwendet ein eigenes Zertifikat von Adobe, sodass Ihr Unternehmen kein Zertifikat auf Adobe-Servern verwalten muss.

1. Finden Sie die Mandanten-ID Ihrer Organisation. Siehe [Finden Ihrer Mandanten-ID](collection-domain.md#tenant-id).
1. Legen Sie in Ihrer CDN-Konfiguration den Ursprungs-Host-Namen auf Ihre Mandanten-ID-Subdomain von `data.adobedc.net` fest. Beispiel: `example.data.adobedc.net`.
1. Aktivieren Sie die Server-Namensangabe (SNI) für den Ursprung. Legen Sie den SNI-Hostnamen auf den Ursprungs-Hostnamen (z. B. `example.data.adobedc.net`) fest, nicht auf den Hostnamen Ihrer Website.
1. Konfigurieren Sie Ihr CDN so, dass es die [Anforderungen für alle CDN-Implementierungen](#requirements) oben erfüllt.
1. Wenn sich der Hostname, den Ihre Implementierung an sendet, ändert, [&#x200B; Sie Ihre Implementierung](collection-domain.md#update-implementation). Wenn Sie denselben Hostnamen beibehalten, sind keine Implementierungsänderungen erforderlich.

>[!WARNING]
>
>Legen Sie Ihre Herkunft nicht auf den Host-Namen fest, den Adobe als CNAME-Ziel angegeben hat, z. B. `hiodsibxvip01.data.adobedc.net`. Dieser Hostname ist an Ihr Erstanbieterzertifikat gebunden und kann nach dem Entfernen des Zertifikats nicht mehr funktionieren.

Drittanbieterquellen verwenden immer den standardmäßigen [RDC-Typ](rdc.md), sodass Daten an jedem Datenerfassungsspeicherort von Adobe erfasst werden können.

## Konfigurieren eines CDN mit Erstanbieter-Herkunft {#first-party-origin}

Verwenden Sie eine First-Party-Herkunft nur, wenn Ihr Unternehmen dies erfordert. Häufige Gründe sind:

* Ihre Sicherheitsrichtlinie erfordert die direkte Kontrolle über das Ursprungszertifikat. Beispielsweise muss Ihr Unternehmen in der Lage sein, das Zertifikat über seine eigene Zertifizierungsstelle zu widerrufen.
* Ihr Unternehmen benötigt einen regional gesperrten [RDC-Typ](rdc.md).

1. Wenden Sie sich an die Adobe-Kundenunterstützung, um ein [vom Kunden verwaltetes Zertifikat](customer-managed-cert.md) für Ihren Erstanbieter-Hostnamen einzurichten, z. B. `data.example.com`. Wenn Ihr Unternehmen einen regional gesperrten RDC-Typ benötigt, geben Sie ihn in Ihrer Anfrage an.
1. Legen Sie in Ihrer CDN-Konfiguration den Ursprungs-Host-Namen auf Ihren Erstanbieter-Host-Namen fest.
1. Aktivieren Sie die Server-Namensangabe (SNI) für den Ursprung. Legen Sie den SNI-Hostnamen auf Ihren Erstanbieter-Hostnamen fest und konfigurieren Sie Ihr CDN so, dass Ihr Erstanbieterzertifikat von der Quelle erwartet wird.
1. Konfigurieren Sie Ihr CDN so, dass es die [Anforderungen für alle CDN-Implementierungen](#requirements) oben erfüllt.
1. Wenn sich der Hostname, den Ihre Implementierung an sendet, ändert, [&#x200B; Sie Ihre Implementierung](collection-domain.md#update-implementation). Wenn Sie denselben Hostnamen beibehalten, sind keine Implementierungsänderungen erforderlich.

>[!IMPORTANT]
>
>Ihr Unternehmen ist für die Verlängerung Ihres vom Kunden verwalteten Zertifikats und dessen Bereitstellung bei der Adobe-Kundenunterstützung verantwortlich, bevor es abläuft. Wenn das Zertifikat auf Adobe-Servern abläuft, kann Ihr CDN die Verbindung ablehnen und Daten verwerfen, ohne Sie zu benachrichtigen. Siehe [Zertifikat erneuern](customer-managed-cert.md#renewals).

## Verschieben einer vorhandenen First-Party-Implementierung in ein CDN {#migrate}

Wenn Ihr Unternehmen derzeit Daten direkt an einen Erstanbieter-Host-Namen mit einem von Adobe gehosteten Zertifikat sendet, gehen Sie wie folgt vor, um zu einem CDN zu wechseln:

1. Identifizieren Sie jede Implementierung, die Daten über alle Adobe-Produkte hinweg an Ihren Erstanbieter-Host-Namen sendet. Andere Produkte wie Adobe Target oder Adobe Journey Optimizer verwenden möglicherweise denselben Hostnamen, und ein einzelnes Zertifikat kann viele Hostnamen abdecken.
1. Wählen Sie einen [Herkunftstyp](#origin-type). Wenn Sie einen Erstanbieter-Ursprung auswählen, wenden Sie sich an die Kundenunterstützung von Adobe, um Ihr Zertifikat in ein [kundenverwaltetes Zertifikat) &#x200B;](customer-managed-cert.md) konvertieren, bevor es abläuft.
1. Konfigurieren des CDN. Behalten Sie Ihren vorhandenen Hostnamen bei, damit Sie Ihre Implementierungen nicht aktualisieren müssen.
1. Bevor Ihr Zertifikat abläuft, verweisen Sie Ihren Hostnamen auf Ihr CDN und wechseln Sie alle Implementierungen, um es zu verwenden.
1. [Überprüfen Sie Ihre Daten](#check).
1. Wenn Sie die Herkunft eines Drittanbieters ausgewählt haben, wenden Sie sich an die Kundenunterstützung von Adobe, um Ihr Erstanbieterzertifikat zur Entfernung zu markieren.

Sobald Ihr Hostname auf Ihr CDN verweist, kann Adobe Ihr Erstanbieterzertifikat nicht mehr verlängern. Wenn eine Implementierung bei Ablauf immer noch auf das Zertifikat angewiesen ist, gehen Daten aus dieser Implementierung verloren. Wenn Sie sich an die Adobe-Kundenunterstützung wenden, kann Ihr Unternehmen steuern, wann das Zertifikat entfernt wird.

## Überprüfen der Daten {#check}

Adobe kann Ihre CDN-Konfiguration nicht validieren. Nachdem Sie die Datenerfassung durch Ihr CDN geroutet haben, vergleichen Sie Ihre Daten vor und nach der Änderung:

* Die Daten gelangen weiterhin im üblichen Volumen in die erwarteten Report Suites, Datenströme oder Datensätze.
* Geolokalisierungsberichte zeigen die Standorte Ihrer Besucher an, nicht eine geringe Anzahl von Städten, in denen sich die Server Ihres CDN befinden.
* Die Anzahl der Unique Visitors steigt nicht unerwartet an.
* In den Entwickler-Tools Ihres Browsers sind Datenerfassungsanfragen an Ihren Hostnamen erfolgreich, und Adobe-Cookies werden in derselben Domain wie zuvor gesetzt.

## Häufige Fehlkonfigurationen

Es ist bekannt, dass die folgenden Probleme Datenqualitätsprobleme oder Datenverluste verursachen. Diese Liste ist nicht vollständig.

| Symptom | Wahrscheinliche Ursache |
| --- | --- |
| Daten gelangen nicht mehr in eine Report Suite oder einen Datenstrom | Das CDN ändert die Anfrage-URL, oder der Ursprungs-Host-Name existiert nicht |
| Daten gelangen nicht mehr nach Ablauf eines Zertifikats | Das CDN erwartet ein Erstanbieterzertifikat aus der Quelle. Dieses Zertifikat ist abgelaufen |
| Geolokalisierungsdaten zeigen nur wenige Städte | Das CDN fügt die `X-Forwarded-For`-Kopfzeile nicht hinzu |
| Die Unique-Visitor-Anzahl steigt unerwartet an | Das CDN entfernt Adobe-Cookies, ändert die `Host` oder die Cookie-Domain |
| In Berichten fehlen große Datenmengen | Regeln zum Entfernen personenbezogener Daten oder zu WAF entfernen zu viel von jeder Anfrage |

## Häufig gestellte Fragen

+++Gilt diese Seite für andere Produkte als Adobe Analytics?

Ja. Diese Seite gilt für alle Adobe-Produkte, die Adobe-Datenerfassung verwenden, einschließlich Customer Journey Analytics, Adobe Experience Platform, Adobe Target und Adobe Journey Optimizer.

+++

+++Kann Adobe Daten ablehnen, die nicht über mein CDN gesendet werden?

Nein. Adobe bietet derzeit keine Möglichkeit, die Datenerfassung auf Anfragen aus Ihrem CDN zu beschränken.

+++

+++Kann Adobe eine Konfiguration für mein CDN bereitstellen oder validieren?

Nein. Die CDN-Konfigurationsoptionen unterscheiden sich je nach Anbieter und ändern sich im Laufe der Zeit. Wenden Sie sich an Ihren CDN-Anbieter, um Hilfe bei der Konfiguration Ihres CDN zu erhalten, und [&#x200B; Sie unter „Überprüfen Sie Ihre &#x200B;](#check)&quot;, wie Sie Probleme mit Ihrer Konfiguration identifizieren können.

+++
