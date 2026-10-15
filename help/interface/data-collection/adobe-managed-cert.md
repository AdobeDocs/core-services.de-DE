---
description: Erfahren Sie, wie Sie sichere Zertifikate für die Verwendung mit Adobe CX Enterprise-Erstanbieter-Cookies einrichten.
solution: Experience Cloud,Analytics
title: Adobe-Managed Certificate Program
index: true
snippet: 'y'
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
autotag-review: '2026-09-09T20:12:24.943Z'
TQID: 'https://experienceleague.adobe.com/8CSBLQaw3KOByyxxCYr1By4gyAQsDIhiofOdAzn38dg'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
    internal-label: Analytics
feature_v2:
  - id: b3f03848-ae12-48b2-8aab-cad18567eb32
    internal-label: Metrics
  - id: e9dbdbc5-3e52-40f0-a7bc-e18542967b7a
    internal-label: Implementations
  - id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
    internal-label: API
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
    internal-label: Administration
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
    internal-label: Support
  - id: c8add8f2-4250-4fd9-9cde-9707036c567d
    internal-label: Methods
  - id: d2311670-43bd-4c2e-bc98-1da2aaba9cef
    internal-label: Appmeasurement implementation
  - id: e992d880-33bc-4949-a648-aa7d410276cd
    internal-label: Validation
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 18fd590d6f0fd1800e3d5c62851453aa91d9db5f
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 2%
---
# Adobe Managed Certificate Program

Das Adobe-verwaltete Zertifikatsprogramm ist der empfohlene Prozess zum Einrichten von Erstanbieterzertifikaten, die für eine CNAME-Implementierung erforderlich sind. Das Programm ist nach der Konfiguration vollständig automatisiert. Zertifikate werden rechtzeitig erneuert, sodass sich die Datenerfassung aufgrund abgelaufener Zertifikate nicht auswirkt. Das Programm ist kostenlos für Ihre ersten 100 CNAMEs.

Das Adobe-verwaltete Zertifikatprogramm unterstützt nicht das Routing der Datenerfassung über ein Content Delivery Network (CDN). Wenn Sie ein CDN verwenden, finden Sie weitere Informationen unter [Routing der Datenerfassung über ein CDN](cdn.md). Organisationen, die ihre eigenen Zertifikate verwalten müssen, können stattdessen [kundenverwaltete Zertifikate](customer-managed-cert.md) verwenden. Wenn Sie derzeit Ihre eigenen Zertifikate verwalten und zum Adobe-verwalteten Zertifikatprogramm wechseln möchten, wenden Sie sich an die Kundenunterstützung von Adobe.

## Implementierung

Gehen Sie wie folgt vor, um ein neues Zertifikat für die Erstanbieter-Datenerfassung zu implementieren:

1. Laden Sie das Anforderungsformular für [-Domains herunter und füllen Sie es aus](cookies/assets/First_Party_Domain_Request_Form.xlsx)
1. Öffnen Sie ein Ticket bei der Adobe-Kundenunterstützung, um die Erstanbieter-Datenerfassung für das von Adobe verwaltete Zertifikatsprogramm einzurichten. Wenn Ihr Unternehmen Datenresidenz- oder Compliance-Anforderungen hat, geben Sie den gewünschten [RDC-Typ](rdc.md) in Ihrer Anfrage an.
1. Nach Erhalt des Tickets stellt Ihnen der Adobe-Support einen CNAME-Datensatz zur Verfügung. Dieser Eintrag muss auf dem DNS-Server Ihres Unternehmens konfiguriert werden, bevor Adobe das Zertifikat in Ihrem Namen erwerben kann. Beispielsweise verweist der Hostname-`data.example.com` auf `hiodsibxvip01.data.adobedc.net`. Wenn Ihr Unternehmen DNS-Zertifizierungsstellen-Einträge (CA) verwendet, stellen Sie sicher, dass Ihre CAA-Einträge DigiCert die Ausstellung von Zertifikaten ermöglichen. Siehe [Wartung und Erneuerung](#renewals).
1. Wenn der CNAME-Eintrag auf den Servern Ihres Unternehmens vorhanden ist, kauft und installiert Adobe gemeinsam mit DigiCert ein Zertifikat auf den Datenerfassungsservern von Adobe.
1. Wenn Sie eine Aktualisierung Ihrer `robots.txt` benötigen, wenn Sie von Adobe CNAME zu Erstanbieterzwecken gehostet werden, wenden Sie sich mit einer Anfrage an die Kundenunterstützung. Eine solche Anfrage ist relevant, wenn Sie die `robots.txt` aktualisieren möchten, um zu verhindern, dass Google Ihre Subdomains crawlen.

## Überprüfen der Hostnamenweiterleitung

Nachdem Adobe das Zertifikat installiert hat, können Sie eine der folgenden Methoden verwenden, um zu überprüfen, ob es funktioniert.

+++**Browser-Validierung**

Sie können jeden Browser verwenden, um zu überprüfen, ob ein Zertifikat korrekt installiert ist. Geben Sie Ihren CNAME mit `_check` als Pfad in die Adressleiste ein. Beispiel:

`data.example.com/_check`

Wenn alles funktioniert, zeigt der Browser `SUCCESS` an. Wenn das Zertifikat nicht korrekt installiert ist, wird eine Sicherheitswarnung ausgegeben.

+++

+++**Befehlszeile (`curl`)**

Die meisten modernen Betriebssysteme [`curl`](https://curl.se) bereits installiert.

Geben Sie Folgendes in die Befehlszeile ein:

```sh
curl data.example.com/_check
```

Wenn alles ordnungsgemäß funktioniert, gibt die Konsole `SUCCESS` zurück.

>[!TIP]
>
>Sie können die `-k`-Markierung verwenden, um die Sicherheitswarnung zu deaktivieren und so die Fehlerbehebung zu erleichtern.

+++

+++**Befehlszeile (`nslookup`)**

Geben Sie Folgendes in die Befehlszeile ein:

```sh
nslookup data.example.com
```

Wenn alles ordnungsgemäß funktioniert, werden die Datenerfassungs-Server von Adobe zurückgegeben:

```text
Server: hiodsibxvip01.corp.adobe.com
Address: 10.50.112.247

Name: example.com.ssl.d1.sc.omtrdc.net
Addresses: 63.140.37.126
    63.140.37.206
    63.140.36.51
    63.140.36.145
Aliases: data.example.com
```

+++

## Aktualisierung des Implementierungscodes

Um Ihren neuen CNAME-Hostnamen zu verwenden, aktualisieren Sie Ihre Adobe-Implementierung, sobald Sie überprüft haben, ob Ihr Zertifikat ordnungsgemäß funktioniert. Siehe [Aktualisieren Ihrer Implementierung](collection-domain.md#update-implementation).

## Wartung und Erneuerung {#renewals}

Adobe erneuert Ihr Zertifikat automatisch. Dreißig Tage vor Ablauf Ihres Zertifikats überprüft Adobe, ob der CNAME noch gültig und in Verwendung ist, und erneuert dann das Zertifikat in Ihrem Namen. Um Erneuerungen zu ermöglichen, vermeiden Sie die folgenden DNS-Änderungen:

* **CNAME-Eintrag entfernen oder neu verweisen**: Wenn der CNAME-Eintrag entfernt wurde oder nicht mehr auf den sicheren Hostnamen von Adobe verweist, kann Adobe das Zertifikat nicht verlängern. Diese Bedingung umfasst das Verweisen des CNAME-Eintrags auf ein Content Delivery Network (CDN). Wenn Sie beabsichtigen, ein CDN zu verwenden, lesen Sie [Verschieben einer vorhandenen Erstanbieterimplementierung in ein CDN](cdn.md#migrate) bevor Sie Ihre DNS-Einträge ändern.
* **Hinzufügen von CAA-Einträgen, die DigiCert nicht autorisieren**: Zertifizierungsstellen prüfen die CA-Einträge (Certificate Authority Authorization) auf Ihrem Hostnamen und den übergeordneten Domains. Wenn Sie CAA-Datensätze verwenden, schließen Sie `digicert.com` als autorisierten Aussteller ein. Beispiel: `example.com. IN CAA 0 issue "digicert.com"`.
* **DigiCert-Ausgabe auf ein bestimmtes Konto beschränken**: Die Domain-Sperrfunktion von DigiCert fügt einem CAA-Eintrag einen `account=` Parameter hinzu, z. B. `example.com. IN CAA 0 issue "digicert.com; account=<token>"`. Dieser Parameter beschränkt die Ausgabe auf das DigiCert-Konto Ihres Unternehmens, auch wenn `digicert.com` autorisiert ist. Dadurch kann Adobe kein Zertifikat erhalten. Wenn für Ihr Unternehmen eine DigiCert-Domain-Sperre erforderlich ist, verwenden Sie [kundenverwaltete Zertifikate](customer-managed-cert.md). Domain-Sperren, die von Ihrer Domain-Registrierungsstelle festgelegt werden (manchmal auch als Übertragungssperren bezeichnet), haben keinen Bezug zu Adobe-verwalteten Zertifikaten und wirken sich nicht auf diese aus.

>[!IMPORTANT]
>
>Wenn Ihr CNAME-Eintrag nicht mehr auf den sicheren Hostnamen von Adobe verweist, wird der Eintrag im System von Adobe zur Entfernung ohne weitere Kommunikation markiert.

## Häufig gestellte Fragen

+++Ist dieser Prozess sicher?

Ja. Das Adobe-verwaltete Zertifikatsprogramm ist sicherer als [kundenverwaltete Zertifikate](customer-managed-cert.md). Außerhalb von Adobe und der ausstellenden Zertifizierungsstelle wird kein Zertifikat oder privater Schlüssel übertragen.

+++

+++Wie kann Adobe ein Zertifikat für unsere Domain erwerben?

Das Zertifikat kann nur erworben werden, wenn der angegebene Hostname auf einen Adobe-eigenen Hostnamen verweist. Sie delegieren diesen Hostnamen an Adobe und erlauben Adobe, das Zertifikat in Ihrem Namen zu erwerben.

+++

+++Kann ich beantragen, dass das Zertifikat widerrufen wird?

Ja. Als Eigentümer der Domain sind Sie berechtigt, den Widerruf des Zertifikats zu verlangen. Wenden Sie sich an die Adobe-Kundenunterstützung, um diesen Prozess zu starten.

+++

+++Welcher Verschlüsselungstyp wird verwendet?

Adobe stellt in Zusammenarbeit mit DigiCert ein SHA-2-Zertifikat aus.

+++

+++Entstehen für dieses Programm zusätzliche Kosten?

Adobe bietet dieses Programm allen Adobe CX Enterprise-Kunden ohne zusätzliche Kosten für die ersten 100 CNAMEs an.

+++

+++Welche Chiffrier-Sicherheitsstufen bietet Adobe?

Adobe bietet zwei Chiffrier-Sicherheitsstufen, die den unterschiedlichen Sicherheitsanforderungen bei der Erfassung von First-Party-Daten gerecht werden. Diese Stufen bestimmen, welche Verschlüsselungsalgorithmen für HTTPS-Verbindungen mit Adobe-Servern unterstützt werden. Adobe überprüft und aktualisiert regelmäßig die unterstützten Algorithmen auf der Grundlage aktueller Sicherheitspraktiken. Wenden Sie sich an die Kundenunterstützung, um Ihre Chiffrier-Sicherheitseinstellungen zu ändern.

* **Standard** erfordert TLS 1.2 oder höher und mindestens 128-Bit-Verschlüsselung. Es wurde entwickelt, um die größtmögliche Gerätekompatibilität bei gleichzeitiger Beibehaltung einer sicheren Verschlüsselung zu gewährleisten.
* **Hoch** erfordert TLS 1.2 oder höher und entfernt die Unterstützung für schwächere Chiffren. Es wurde für Kunden entwickelt, die die stärkste Verschlüsselung wünschen. Clients, die vor 2015 veröffentlicht wurden, können in der Regel keine Verbindung herstellen, wenn die Chiffrier-Sicherheit auf **Hoch** eingestellt ist.

+++

+++Welche HTTPS-Zertifikatstypen werden unterstützt?

Adobe unterstützt sowohl RSA- als auch ECC-Zertifikate, und moderne Clients unterstützen beide Zertifikatstypen. ECC-Zertifikate erfordern sowohl auf dem Server als auch auf dem Client weniger Verarbeitungsaufwand. Für von Adobe verwaltete Zertifikate stellt Adobe sowohl RSA- als auch ECC-Zertifikate bereit. Für [kundenverwaltete Zertifikate](customer-managed-cert.md) ist RSA erforderlich und ECC wird empfohlen.

+++

