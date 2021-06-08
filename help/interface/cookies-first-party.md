---
description: Hier erfahren Sie, wie Adobe Analytics Cookies verwendet, um Informationen über Variablen und Komponenten bereitzustellen, die zwischen Bildanforderungen und Browser-Sitzungen nicht bestehen bleiben.
keywords: Cookies, Datenschutz
solution: Experience Cloud,Analytics
title: '"Erstanbieter-Cookies "'
index: y
snippet: y
feature: Cookies
topic: Administration
role: Administrator
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: 11b999ef0c0d4f258e8665eb9c5bf427f5d618c4
workflow-type: tm+mt
source-wordcount: '1576'
ht-degree: 55%

---

# Informationen zu Erstanbieter-Cookies

Analytics verwendet Cookies, um Informationen zu Variablen und Komponenten zu liefern, die nicht zwischen Bildanfragen und Browsersitzungen bestehen bleiben. Wenn möglich, verwendet Adobe Erstanbieter-Cookies, um Aktivitäten auf Ihrer Site aufzuzeichnen. Um Aktivitäten auf verschiedenen Sites aufzuzeichnen, z. B. auf anderen Domänen, deren Inhaber Sie sind, sind Drittanbieter-Cookies erforderlich.

Viele Browser und Anti-Spyware-Anwendungen sind dafür konzipiert, Drittanbieter-Cookies abzulehnen und zu löschen, einschließlich Cookies, die in der Datenerfassung von [!DNL Analytics] verwendet werden. Um das Tracking der Interaktion Ihrer Besucher mit Ihrer Website zu unterstützen, sollten Sie sicherstellen, dass Sie Ihre Datenerfassung für die Verwendung von Erstanbieter-Cookies konfiguriert haben:

Es stehen zwei Optionen zur Implementierung von Erstanbieter-Cookies zur Verfügung:

* Wenn Sie den Experience Platform Identity Service (ECID-Dienst) verwenden, werden Cookies mithilfe von JavaScript automatisch im Erstanbieterkontext gesetzt.
* Wenn Sie [!DNL Analytics] Legacy-IDs (auch `s_vi`-Cookie genannt) verwenden, hängt es davon ab, wie Sie Ihren Datenerfassungsserver konfiguriert haben. Wenn der Datenerfassungsserver mit der Domäne Ihrer Site übereinstimmt, werden Cookies als Erstanbieter gesetzt. Wenn der Erfassungsserver nicht mit Ihrer aktuellen Domäne übereinstimmt, werden Cookies als Drittanbieter gesetzt. Wenn Drittanbieter-Cookies blockiert werden, setzt [!DNL Analytics] anstelle des standardmäßigen &quot;s_vi&quot;-Cookies eine Erstanbieter-Ausweich-ID (s_fid)](cookies-analytics.md).[

Um sicherzustellen, dass Ihr Erfassungsserver mit der Domäne Ihrer Site übereinstimmt, können Sie eine CNAME-Implementierung verwenden, mit der Cookies in einem Erstanbieterkontext gesetzt werden können. Dazu gehören Änderungen an den DNS-Einstellungen Ihres Unternehmens, um einen CNAME-Alias zu konfigurieren, der auf eine von der Adobe gehostete Domäne verweist. Beachten Sie, dass verschiedene Adobe-Produkte zwar CNAME verwenden, der CNAME jedoch in allen Fällen zum Erstellen eines vertrauenswürdigen Erstanbieter-Endpunkts für einen bestimmten Kunden verwendet wird und sich im Besitz dieses Kunden befindet. Wenn Sie mehrere Domänen steuern, können sie einen einzelnen CNAME-Endpunkt verwenden, um Benutzer domänenübergreifend zu verfolgen. Wenn die Site-Domäne jedoch nicht mit den CNAME-Domänen-Cookies übereinstimmt, wird sie als Drittanbieter festgelegt.

>[!NOTE]
>
>Für beide Optionen sorgt das ITP-Programm (Intelligent Tracking Prevention) von Apple dafür, dass die Erstanbieter-Cookies in Browsern mit kurzer Lebensdauer verwendet werden, die von ITP verwaltet werden. Dazu gehören Safari unter macOS und alle Browser unter iOS und iPadOS. Ab November 2020 laufen Cookies beider Typen nach sieben Tagen ab. Diese Ablaufzeit kann sich ändern.

Bei der zweiten Option mit einem CNAME können Sie, wenn Ihre Site sichere Seiten mit dem HTTPS-Protokoll aufweist, mit Adobe ein SSL-Zertifikat abrufen, um Erstanbieter-Cookies zu implementieren. Adobe empfiehlt dringend, dass Sie ausschließlich HTTPS für die Datenerfassung verwenden, da Adobe die HTTP-Erfassung in der zweiten Jahreshälfte 2020 nicht mehr unterstützt.

Der Bereitstellungsprozess von SSL-Zertifikaten kann verwirrend und zeitraubend sein. Daher hat die Adobe eine Partnerschaft mit DigiCert, einer branchenführenden Zertifizierungsstelle (CA), aufgebaut und einen integrierten Prozess entwickelt, durch den der Erwerb und die Verwaltung dieser Zertifikate automatisiert werden.

Mit Ihrer Erlaubnis arbeiten wir mit CA, um ein neues SHA-2-SSL-Zertifikat für Sie auszustellen, bereitzustellen und zu verwalten. Adobe verwaltet dieses Zertifikat und stellt sicher, dass ein unerwarteter Ablauf, eine unerwartete Sperrung oder ein unerwartetes Sicherheitsproblem die sichere Erfassung Ihres Unternehmens nicht gefährdet.

## Adobe-Managed Certificate Program

Das Adobe Managed Certificate Program (Adobe-Programm für verwaltete Zertifikate) ist das empfohlene Verfahren zur Implementierung eines neuen Erstanbieter-SSL-Zertifikats für Erstanbieter-Cookies.

Mit diesem Programm können Sie ohne zusätzliche Kosten ein neues Erstanbieter-SSL-Zertifikat für Erstanbieter-Cookies implementieren (für Ihre ersten 100 CNAMEs). Wenn Sie derzeit über ein eigenes kundenverwaltetes SSL-Zertifikat verfügen, wenden Sie sich an die Adobe-Kundenunterstützung, um zum Adobe-Managed Certificate Program zu migrieren.

### Implementierung

So implementieren Sie ein neues Erstanbieter-SSL-Zertifikat für Erstanbieter-Cookies:

1. Füllen Sie das Anforderungsformular [Erstanbieter-Cookie](/help/interface/cookies/assets/First_Part_Domain_Request_Form.xlsx) aus und öffnen Sie ein Ticket für die Kundenunterstützung, um Erstanbieter-Cookies im Adobe-Managed Program einzurichten. Bei jedem Feld finden Sie eine Beschreibung anhand von Beispielen.

2. Erstellen Sie CNAME-Datensätze (siehe Anweisungen unten).

   Nach Erhalt des Tickets sollte Ihnen ein Mitarbeiter der Kundenunterstützung einen CNAME-Datensatz bereitstellen. Diese Datensätze müssen auf dem DNS-Server Ihres Unternehmens konfiguriert werden, bevor Adobe das Zertifikat in Ihrem Namen erwerben kann. Der CNAME ähnelt dem folgenden:

   **Sicher** – Zum Beispiel verweist der Hostname `smetrics.example.com` auf: `example.com.adobedc.net`.

>[!NOTE]
> In der Vergangenheit hat Adobe empfohlen, dass Kunden zwei CNAME-Einträge für HTTPS und einen für HTTP einrichten. Da es sich um eine Best Practice zur Verschlüsselung von Traffic handelt und die meisten Browser HTTP stark ablehnen, empfehlen wir nicht mehr, einen CNAME für HTTP einzurichten. Bei Bedarf würde dies wie folgt aussehen:
>    **Nicht sicher** – der Hostname `metrics.example.com` verweist auf: `example.com.adobedc.net`.

1. Wenn der CNAME eingerichtet ist, kauft und installiert Adobe gemeinsam mit DigiCert ein Zertifikat auf den Produktionsservern der Adobe.

   Wenn Sie bereits ein Zertifikat implementiert haben, sollten Sie eine Besuchermigration erwägen, um Ihre vorhandenen Besucher beizubehalten. Nachdem das Zertifikat live in die Produktionsumgebung von Adobe übermittelt wurde, können Sie Ihre Tracking-Server-Variablen gemäß den neuen Hostnamen aktualisieren. Wenn die Site nicht sicher (HTTP) ist, aktualisieren Sie also `s.trackingServer`. Wenn die Site sicher ist (HTTPS), aktualisieren Sie die beiden Variablen `s.trackingServer` und `s.trackingServerSecure`.

2. [Validieren Sie die Weiterleitung von Hostnamen](#validate) (siehe unten).

3. [Aktualisieren Sie den Implementierungscode](#update) (siehe unten).

### Wartung und Verlängerung

SSL-Zertifikate laufen jedes Jahr ab, d. h. Adobe muss jedes Jahr ein neues Zertifikat für jede Implementierung erwerben. Alle unterstützten Benutzer in Ihrem Unternehmen erhalten jedes Mal, wenn eine Implementierung kurz vor ihrem Ablauf steht, eine E-Mail-Benachrichtigung. Damit Adobe Ihren Hostnamen verlängert, muss ein unterstützter Benutzer auf die E-Mail von Adobe antworten und angeben, dass der ablaufende Hostname weiterhin für die Datenerfassung verwendet werden soll. Adobe kauft dann automatisch ein neues Zertifikat und installiert es.

### Häufig gestellte Fragen

| Frage | Antwort |
|---|---|
| **Ist dieser Prozess sicher?** | Ja, das Adobe-Managed Program ist sicherer als unsere alte Methode, da kein Zertifikat oder privater Schlüssel außerhalb der Adobe und der Zertifizierungsstelle wechselt. |
| **Wie kann Adobe ein Zertifikat für unsere Domäne erwerben?** | Das Zertifikat kann nur gekauft werden, wenn Sie mit dem jeweiligen Hostnamen (z. B. `telemetry.example.com`) auf Hostnamen von Adobe verweisen. Dadurch wird dieser Hostname an Adobe übertragen und Adobe kann das Zertifikat in Ihrem Namen erwerben. |
| **Kann ich verlangen, dass das Zertifikat entzogen wird?** | Ja, als Eigentümer der Domäne können Sie verlangen, dass uns das Zertifikat entzogen wird. Sie müssen dazu nur ein Ticket bei der Kundenunterstützung erstellen. |
| **Verwendet dieses Zertifikat SHA-2-Verschlüsselung?** | Ja, Adobe gibt in Zusammenarbeit mit DigiCert ein SHA-2-Zertifikat heraus. |
| **Verursacht dies Mehrkosten?** | Nein, Adobe stellt diesen Dienst allen aktuellen Adobe Digital Experience-Kunden kostenlos zur Verfügung. |

## Erstellen von CNAME-Datensätzen

Das Netzwerkteam Ihres Unternehmens sollte Ihre DNS-Server konfigurieren, indem es CNAME-Einträge erstellt. Jeder Hostname leitet Daten an die Datenerfassungsserver von Adobe weiter.

Der FPC-Spezialist stellt Ihnen den konfigurierten Host-Namen bereit und gibt an, auf welchen CNAME er verweisen soll. Beispiel:

* **SSL-Hostname**: `smetrics.mysite.com`
* **SSL-CNAME**: `mysite.com.adobedc.net`

>[!NOTE]
> Wenn Sie weiterhin nicht sicher verwenden, sieht es wie folgt aus:
> * **Nicht-SSL-Hostname**: `metrics.mysite.com`
> * **Nicht-SSL-CNAME**: `mysite.com.adobedc.net`


Solange der Implementierungscode nicht verändert wird, beeinflusst dieser Schritt nicht die Datensammlung und kann zu einem beliebigen Zeitpunkt nach der Aktualisierung des Implementierungscodes vorgenommen werden.

>[!NOTE]
>
>Hinweis: Der Besucher-ID-Dienst von Experience Cloud bietet eine Alternative zum Konfigurieren eines CNAME, um Erstanbieter-Cookies zu ermöglichen.

## Überprüfen der Hostnamenweiterleitung {#validate}

Die folgenden Methoden stehen zur Überprüfung zur Verfügung:

### Validieren mithilfe eines Browsers

Wenn Sie einen CNAME eingerichtet haben und das Zertifikat installiert ist, können Sie den Browser zur Überprüfung verwenden:

`https://smetrics.adobe.com/_check`

>[!NOTE]
>
>Sie erhalten eine Sicherheitswarnung, wenn kein Zertifikat installiert ist.

### Validieren mit [!DNL curl]

Adobe empfiehlt die Verwendung von [[!DNL curl]](https://curl.se/) über die Befehlszeile. ([!DNL Windows]-Benutzer können [!DNL curl] über folgenden Link installieren: <https://curl.se/windows/>)

Wenn Sie einen CNAME haben, aber kein Zertifikat installiert ist, führen Sie Folgendes aus:
`curl -k https://smetrics.adobe.com/_check`
Antwort: `SUCCESS`

(Der `-k`-Wert deaktiviert die Sicherheitswarnung.)

Wenn Sie einen CNAME eingerichtet haben und das Zertifikat installiert ist, führen Sie Folgendes aus:
`curl https://smetrics.adobe.com/_check`
Antwort: `SUCCESS`

### Validieren mit [!DNL nslookup]

Sie können `nslookup` zur Überprüfung verwenden. Verwenden Sie `smetrics.adobe.com` als Beispiel, öffnen Sie eine Eingabeaufforderung und geben Sie `nslookup smetrics.adobe.com` ein.

Wenn alles erfolgreich eingerichtet wurde, wird eine Rückgabe ähnlich der folgenden angezeigt:

```
nslookup smetrics.adobe.com
Server:             10.30.7.247
Address:     10.30.7.247#53

smetrics.adobe.com    canonical name = adobe.com.ssl.d1.sc.omtrdc.net.
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.218.180.161
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 52.39.8.230
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.187.216.46
```

## Aktualisierung des Implementierungscodes {#update}

Bevor Sie Code auf Ihrer Site bearbeiten, um Erstanbieter-Cookies zu verwenden, müssen Sie die folgenden Voraussetzungen erfüllen:

* Fordern Sie ein SSL-Zertifikat an, indem Sie die oben im Abschnitt *Implementieren* des [Adobe-Managed Certificate Program](#adobe-managed-certificate-program) beschriebenen Schritte befolgen.
* Erstellen Sie CNAME-Datensätze (siehe oben).
* Validieren Sie die Hostnamen (siehe oben).

Nachdem Sie überprüft haben, ob Ihre Hostnamen reagieren und an die Datenerfassungsserver der Adobe weiterleiten, können Sie Ihre Implementierung ändern, um auf Ihre eigenen Datenerfassungs-Hostnamen zu verweisen.

1. Öffnen Sie Ihre JavaScript-Kerndatei (`s_code.js/AppMeasurement.js`).
1. Wenn Sie Ihre Codeversion aktualisieren möchten, ersetzen Sie die gesamte `s_code.js/AppMeasurement.js`-Datei mit der neueren Version und ersetzen Sie alle Plugins oder Einstellungen (falls vorhanden). **Oder** wenn Sie den Code aktualisieren möchten, der nur für Erstanbieter-Cookies gilt, suchen Sie die Variablen s.trackingServer und s.trackingServerSecure (falls SSL verwendet wird) und verweisen Sie sie auf Ihre neuen Datenerfassungs-Hostnamen. Verwenden von mysite.com als Beispiel: `s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Laden Sie die aktualisierte JavaScript-Kerndatei auf Ihre Site.

1. Wenn Sie von einer älteren Implementierung zu Erstanbieter-Cookies wechseln oder zu einem anderen Erstanbieter-Erfassungshostnamen wechseln, empfiehlt Adobe die Migration von Besuchern aus der vorherigen Domäne in die neue Domäne.

Siehe [Besuchermigration](https://experienceleague.adobe.com/docs/analytics/implementation/javascript-implementation/visitor-migration.html?lang=en) im Analytics-Implementierungshandbuch.

Nachdem Sie die JavaScript-Datei hochgeladen haben, ist die Konfiguration für die Erstanbieter-Cookie-Datensammlung abgeschlossen. Adobe empfiehlt, die Analytics-Berichterstellung für die nächsten Stunden zu überwachen, um sicherzustellen, dass die Datenerfassung normal fortgesetzt wird. Ist dies nicht der Fall, stellen Sie sicher, dass alle oben genannten Schritte ausgeführt wurden und veranlassen Sie, dass ein unterstützter Mitarbeiter Ihrer Organisation die Kundenunterstützung kontaktiert.