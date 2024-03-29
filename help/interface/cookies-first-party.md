---
description: Hier erfahren Sie, wie Adobe Analytics Cookies verwendet, um Informationen über Variablen und Komponenten bereitzustellen, die zwischen Bildanforderungen und Browser-Sitzungen nicht bestehen bleiben.
solution: Experience Cloud,Analytics
title: "Erstanbieter-Cookies "
index: y
snippet: y
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: cef927ad0f9f875841d2acf670950de0a766df7e
workflow-type: tm+mt
source-wordcount: '1594'
ht-degree: 72%

---

# Informationen zu Erstanbieter-Cookies

Analytics verwendet Cookies, um Informationen zu Variablen und Komponenten zu liefern, die nicht zwischen Bildanfragen und Browsersitzungen bestehen bleiben. Wenn möglich, verwendet Adobe Erstanbieter-Cookies, um Aktivitäten auf Ihrer Website aufzuzeichnen. Um Aktivitäten auf verschiedenen Websites aufzuzeichnen, z. B. auf anderen Domains, deren Inhaber Sie sind, sind Drittanbieter-Cookies erforderlich.

Viele Browser und Anti-Spyware-Anwendungen sind dafür konzipiert, Drittanbieter-Cookies abzulehnen und zu löschen. Adobe stellt sicher, dass Cookies immer gesetzt werden können, auch wenn Drittanbieter-Cookies blockiert werden. Das spezifische Verhalten variiert je nachdem, ob Sie den Experience Platform Identity Service (ECID-Dienst) oder die Legacy-IDs von Analytics (auch s_vi-Cookie genannt) verwenden:

* [Experience Platform Identity Service (ECID-Service)](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=de) setzt automatisch Erstanbieter-Cookies, unabhängig davon, ob Ihre Erfassungs-Domain mit Ihrer Website-Domain übereinstimmt. Wenn sie nicht übereinstimmen, verwendet der Identity-Dienst JavaScript, um Cookies in der Domäne Ihrer Site festzulegen.
* Wenn Sie ältere [Legacy-Identifikatoren von Analytics](https://experienceleague.adobe.com/docs/core-services/interface/administration/ec-cookies/cookies-analytics.html?lang=de) (auch `s_vi`-Cookie genannt) verwenden, hängt dies von der Konfiguration Ihres Datenerfassungs-Servers ab. Wenn der Datenerfassungsserver mit der Domain Ihrer Website übereinstimmt, werden Cookies als First-Party gesetzt. Wenn der Erfassungsserver nicht mit Ihrer aktuellen Domain übereinstimmt, werden Cookies als Drittanbieter gesetzt. Wenn Drittanbieter-Cookies blockiert werden, setzt Analytics eine First-Party-[Ausweich-ID („s_fid“)](cookies-analytics.md) anstelle des standardmäßigen Cookies „s_vi“.

Wenn Sie sicherstellen möchten, dass Ihr Erfassungsserver mit der Domäne Ihrer Site übereinstimmt, können Sie eine CNAME-Implementierung verwenden, die die Weiterleitung von einer benutzerdefinierten Domäne ermöglicht, die in Ihrer CNAME-Implementierung an die Adobe-Erfassungsserver angegeben ist. Dazu gehören Änderungen an den DNS-Einstellungen Ihres Unternehmens, um einen CNAME-Alias zu konfigurieren, der auf eine von der Adobe gehostete Domain verweist. Beachten Sie, dass verschiedene Adobe-Produkte zwar CNAME verwenden, der CNAME jedoch in allen Fällen zum Erstellen eines vertrauenswürdigen First-Party-Endpunkts für einen bestimmten Kunden verwendet wird und sich im Besitz dieses Kunden befindet. Wenn Sie mehrere Domänen steuern, können sie einen einzelnen CNAME-Endpunkt verwenden, um Benutzer domänenübergreifend zu verfolgen. Wenn die Site-Domäne jedoch nicht mit den CNAME-Domänen-Cookies übereinstimmt, werden sie als Drittanbieter festgelegt.

>[!NOTE]
>
>Unabhängig davon, ob Ihre Erfassungsdomäne mit Ihrer Site-Domäne übereinstimmt, setzt das ITP-Programm (Intelligent Tracking Prevention) von Apple die Erstanbieter-Cookies, die von Adobe gesetzt werden, in Browsern mit kurzer Lebensdauer, die von ITP verwaltet werden. Dazu gehören Safari in macOS und alle Browser in iOS und iPadOS. Ab November 2020 laufen über CNAME gesetzte Cookies genauso ab wie über JavaScript gesetzte Cookies. Diese Ablaufzeit kann sich ändern.

Wenn Sie einen CNAME für die Datenerfassung einrichten möchten und Ihre Website sichere Seiten hat, welche das HTTPS-Protokoll verwenden, können Sie mithilfe von Adobe ein SSL-Zertifikat beantragen.

Der Bereitstellungsprozess von SSL-Zertifikaten kann verwirrend und zeitraubend sein. Daher ist Adobe eine Partnerschaft mit DigiCert, einer branchenführenden Zertifizierungsstelle (CA), eingegangen und hat einen integrierten Prozess entwickelt, durch den der Kauf und die Verwaltung dieser Zertifikate automatisiert werden.

Mit Ihrer Erlaubnis arbeiten wir mit einer Zertifizierungsstelle, um ein neues SHA-2-SSL-Zertifikat für Sie auszustellen, bereitzustellen und zu verwalten. Adobe verwaltet dieses Zertifikat und gewährleistet, dass die sichere Datenerfassung durch Ihr Unternehmen nicht durch ein unerwartetes Ablaufen der Gültigkeit, die Aberkennung oder ein Sicherheitsproblem gefährdet wird.

## Adobe-Managed Certificate Program

Das Adobe Managed Certificate Program (Programm für verwaltete Zertifikate) ist der empfohlene Prozess zum Einrichten des Erstanbieter-SSL-Zertifikats, das für eine CNAME-Implementierung erforderlich ist. Dadurch wird sichergestellt, dass Ihr Adobe-Erfassungs-Server mit Ihrer Website-Domain übereinstimmt.

Mit dem Adobe Managed Certificate Program können Sie ohne zusätzliche Kosten ein neues Erstanbieter-SSL-Zertifikat implementieren (für Ihre ersten 100 CNAMEs). Wenn Sie derzeit Ihr eigenes kundenverwaltetes SSL-Zertifikat haben, sprechen Sie mit der Adobe-Kundenunterstützung über den Umstieg zum Adobe-Managed Certificate Program.

### Implementierung

Folgen Sie unten stehenden Schritten, um ein neues Erstanbieter-SSL-Zertifikat für die Erstanbieter-Datenerfassung zu implementieren:

1. Füllen Sie die [Anforderungsformular für die Erstanbieterdomäne](/help/interface/cookies/assets/First_Part_Domain_Request_Form.xlsx) und öffnen Sie ein Ticket bei der Kundenunterstützung, um die Einrichtung der Erstanbieter-Datenerfassung im Adobe-Managed Program zu beantragen.

   Bei jedem Feld finden Sie eine Beschreibung anhand von Beispielen.

1. Erstellen Sie CNAME-Datensätze (siehe Anweisungen unten).

   Nach Erhalt des Tickets sollte Ihnen ein Kundenbetreuer einen CNAME-Eintrag zur Verfügung stellen. Diese Datensätze müssen auf dem DNS-Server Ihres Unternehmens konfiguriert werden, bevor Adobe das Zertifikat in Ihrem Namen erwerben kann. Der CNAME ähnelt dem folgenden:

   **Sicher** – Zum Beispiel verweist der Hostname `smetrics.example.com` auf: `[random-10-character-string].data.adobedc.net`.

   >[!NOTE]
   > In der Vergangenheit hat Adobe empfohlen, dass Kunden zwei CNAMEs einrichten: einen für HTTPS und einen für HTTP. Da es sich um eine Best Practice zur Traffic-Verschlüsselung handelt und die meisten Browser HTTP stark abhalten, empfehlen wir nicht mehr, einen CNAME für HTTP einzurichten. Es gilt nun als Best Practice, beide `trackingServer` und `trackingServerSecure` mit demselben CNAME. Beispielsweise können beide `trackingServer` und `trackingServerSecure` auf `smetrics.example.com`. HTTP ist nur für Hostnamen von Drittanbietern zulässig.

1. Wenn dieser CNAME eingerichtet ist, kauft und installiert Adobe gemeinsam mit DigiCert ein Zertifikat auf den Betreibungs-Servern von Adobe.

   Wenn Sie bereits ein Zertifikat implementiert haben, sollten Sie eine Besuchermigration erwägen, um Ihre vorhandenen Besucher beizubehalten. Nachdem das Zertifikat live in die Adobe-Produktionsumgebung übertragen wurde, können Sie Ihre Tracking-Server-Variablen in die neuen Hostnamen aktualisieren. Wenn die Site nicht sicher (HTTP) ist, aktualisieren Sie also `s.trackingServer`. Wenn die Site sicher ist (HTTPS), aktualisieren Sie die beiden Variablen `s.trackingServer` und `s.trackingServerSecure`.

1. [Validieren Sie die Weiterleitung von Hostnamen](#validate) (siehe unten).

1. [Aktualisieren Sie den Implementierungscode](#update) (siehe unten).

### Instandhaltung und Erneuerung

Dreißig Tage vor Ablauf Ihres Erstanbieter-Zertifikats überprüft Adobe, ob der CNAME noch gültig ist und verwendet wird. Ist dies der Fall, geht Adobe davon aus, dass Sie den Dienst weiterhin verwenden und das Zertifikat in Ihrem Namen automatisch verlängern möchten.

>[!NOTE]
> Wenn der CNAME entfernt wurde und/oder nicht mehr gültig ist (dem angegebenen Adobe-SSL-Hostnamen nicht zugeordnet ist), kann Adobe das Zertifikat nicht verlängern und der Eintrag in unserem System wird ohne weitere Kommunikation zum Entfernen markiert.

### Häufig gestellte Fragen

| Frage | Antwort |
|---|---|
| **Ist dieser Prozess sicher?** | Ja, das Adobe Managed-Programm ist sicherer als unsere frühere Methode, da weder Zertifikate noch private Schlüssel außerhalb von Adobe und der Zertifizierungsstelle ausgetauscht werden. |
| **Wie kann Adobe ein Zertifikat für unsere Domain erwerben?** | Das Zertifikat kann nur gekauft werden, wenn Sie mit dem jeweiligen Hostnamen (z. B. `telemetry.example.com`) auf Hostnamen von Adobe verweisen. Dadurch wird dieser Hostname an Adobe übertragen und Adobe kann das Zertifikat in Ihrem Namen erwerben. |
| **Kann ich verlangen, dass das Zertifikat entzogen wird?** | Ja, als Eigentümer der Domäne sind Sie berechtigt, die Sperrung des Zertifikats anzufordern. Öffnen Sie ein Ticket bei der Kundenunterstützung, um diesen Vorgang abzuschließen. |
| **Verwendet dieses Zertifikat SHA-2-Verschlüsselung?** | Ja, Adobe arbeitet mit DigiCert zusammen, um ein SHA-2-Zertifikat auszustellen. |
| **Verursacht dies Mehrkosten?** | Nein, Adobe stellt diesen Service allen aktuellen Adobe Digital Experience-Kunden kostenlos zur Verfügung. |

{style="table-layout:auto"}

## Erstellen von CNAME-Datensätzen

Das Netzwerkteam Ihres Unternehmens sollte Ihre DNS-Server konfigurieren, indem es CNAME-Datensätze erstellt. Jeder Hostname leitet Daten an die Datenerfassungsserver von Adobe weiter.

Der FPC-Spezialist stellt Ihnen den konfigurierten Host-Namen bereit und gibt an, auf welchen CNAME er verweisen soll. Beispiel:

* **SSL-Hostname**: `smetrics.example.com`
* **SSL-CNAME**: `[random-10-character-string].data.adobedc.net`

>[!NOTE]
> Wenn Sie immer noch das nicht sichere HTTP verwenden, sieht dies so aus:
>
> * **Nicht-SSL-Hostname**: `metrics.example.com`
> * **Nicht-SSL-CNAME**: `[random-10-character-string].data.adobedc.net`

Solange der Implementierungscode nicht verändert wird, beeinflusst dieser Schritt nicht die Datensammlung und kann zu einem beliebigen Zeitpunkt nach der Aktualisierung des Implementierungscodes vorgenommen werden.

## Überprüfen der Hostnamenweiterleitung {#validate}

Die folgenden Methoden stehen zur Überprüfung zur Verfügung:

### Validieren mithilfe eines Browsers

Wenn Sie einen CNAME eingerichtet haben und das Zertifikat installiert ist, können Sie den Browser zur Überprüfung verwenden:

`https://smetrics.adobe.com/_check`

>[!NOTE]
>
>Wenn kein Zertifikat installiert ist, wird eine Sicherheitswarnung angezeigt.

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

Sie können `nslookup` zur Überprüfung verwenden. Verwenden Sie `smetrics.adobe.com`als Beispiel, öffnen Sie eine Eingabeaufforderung und geben Sie `nslookup smetrics.adobe.com` ein.

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

Bevor Sie Code auf Ihrer Site bearbeiten, um Erstanbieter-Cookies zu verwenden, müssen folgende Voraussetzungen erfüllt sein:

* Fordern Sie ein SSL-Zertifikat an, indem Sie die oben im Abschnitt *Implementierung* des [Adobe-Managed Certificate Program](#adobe-managed-certificate-program) beschriebenen Schritte befolgen.
* Erstellen Sie CNAME-Datensätze (siehe oben).
* Validieren Sie die Hostnamen (siehe oben).

Nachdem Sie geprüft haben, dass Ihre Hostnamen reagieren und die Weiterleitung an die Adobe-Datensammlungsserver funktioniert, können Sie Ihre Implementierung ändern, damit diese zu Ihren eigenen Hostnamen für die Datensammlung weist.

1. Öffnen Sie Ihre JavaScript-Kerndatei (`s_code.js/AppMeasurement.js`).
1. Wenn Sie Ihre Codeversion aktualisieren möchten, ersetzen Sie die gesamte `s_code.js/AppMeasurement.js`-Datei mit der neueren Version und ersetzen Sie alle Plugins oder Einstellungen (falls vorhanden). **Alternativ haben Sie folgende Möglichkeit:** Wenn Sie den Code nur für die Erstanbieter-Datenerfassung aktualisieren möchten, suchen Sie die Variablen s.trackingServer und s.trackingServerSecure (bei Verwendung von SSL) und verweisen Sie sie auf Ihre neuen Datenerfassungs-Host-Namen. Beispiel:

   ```js
   s.trackingServer = "metrics.example.com";
   s.trackingServerSecure = "smetrics.example.com";
   ```

1. Laden Sie die aktualisierte JavaScript-Kerndatei auf Ihre Site.

1. Wenn Sie von einer älteren Implementierung zu einer Erstanbieter-Datenerfassung oder zu einem anderen Erstanbieter-Datenerfassungs-Host-Namen wechseln, empfiehlt Adobe, Besucher aus der vorherigen Domain in die neue Domain zu migrieren.

Siehe [Besuchermigration](https://experienceleague.adobe.com/docs/analytics/technotes/visitor-migration.html?lang=de) im Analytics-Implementierungshandbuch.

Nachdem Sie die JavaScript-Datei hochgeladen haben, ist die Konfiguration für die Erstanbieter-Cookie-Datenerfassung abgeschlossen. Adobe empfiehlt, Analytics Reporting in den nächsten Stunden zu überwachen, um sicherzustellen, dass die Datenerfassung wie üblich erfolgt. Ist dies nicht der Fall, stellen Sie sicher, dass alle oben genannten Schritte ausgeführt wurden und veranlassen Sie, dass ein unterstützter Mitarbeiter Ihrer Organisation die Kundenunterstützung kontaktiert.
