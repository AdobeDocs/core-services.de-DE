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
level: Erfahren
translation-type: tm+mt
source-git-commit: 04f23f3b36b246aa1fe6d672aaeef1dc9140ef3a
workflow-type: tm+mt
source-wordcount: '1444'
ht-degree: 95%

---


# Informationen zu Erstanbieter-Cookies

Analytics verwendet Cookies, um Informationen zu Variablen und Komponenten zu liefern, die nicht zwischen Bildanfragen und Browsersitzungen bestehen bleiben. Diese harmlosen Cookies stammen aus einer von Adobe gehosteten Domäne und werden als Drittanbieter-Cookies bezeichnet.

Viele Browser und Anti-Spyware-Anwendungen sind dafür ausgelegt, Cookies von Drittanbietern abzuweisen und zu löschen, einschließlich der bei der Analytics-Datensammlung verwendeten Cookies. Um die Verfolgung der Interaktion Ihrer Besucher mit Ihrer Website zu unterstützen, können Sie Erstanbieter-Cookies implementieren.

Es stehen zwei Optionen zur Implementierung von Erstanbieter-Cookies zur Verfügung:

* Der ID-Dienst von Experience Platform. Der ID-Dienst kann das Cookie im Erstanbieterkontext mit JavaScript setzen.
* DNS-Einträge auf dem DNS-Server Ihres Unternehmens, um einen CNAME-Alias für eine von Adobe gehostete Domäne zu konfigurieren. Beachten Sie, dass verschiedene Adobe-Produkte zwar CNAME verwenden, der CNAME jedoch in allen Fällen zum Erstellen eines vertrauenswürdigen Erstanbieter-Endpunkts für einen bestimmten Kunden verwendet wird und sich im Besitz dieses Kunden befindet. Wenn der Kunde mehrere Domänen kontrolliert, kann er einen einzelnen CNAME-Endpunkt verwenden, um Benutzer domänenübergreifend zu verfolgen. Da dies jedoch Drittanbieter-Cookies für alle Domänen außerhalb der CNAME-Domäne erfordert, funktioniert dies nicht, wenn Drittanbieter-Cookies blockiert werden. Daher wird diese Vorgehensweise nicht empfohlen. Adobe-CNAMEs werden nie zur Verfolgung von Einzelpersonen oder Geräten über Domänen verschiedener Kunden hinweg verwendet.

>[!NOTE]
>
>Für beide Optionen macht das ITP-Programm (Intelligent Tracking Prevention) von Apple die Erstanbieter-Cookies in Browsern, die von ITP gesteuert werden, kurzlebig, einschließlich Safari unter MacOS und allen Browsern unter iOS und iPadOS. Ab November 2020 laufen beide Cookie-Typen sieben Tage ab. Dieser Ablauf kann sich ändern.

Bei der zweiten Option mit einem CNAME können Sie, wenn Ihre Site sichere Seiten mit dem HTTPS-Protokoll aufweist, mit Adobe ein SSL-Zertifikat abrufen, um Erstanbieter-Cookies zu implementieren. Adobe empfiehlt dringend, dass Sie ausschließlich HTTPS für die Datenerfassung verwenden, da die Unterstützung für die HTTP-Erfassung in der zweiten Jahreshälfte 2020 eingestellt wird.

Der Bereitstellungsprozess von SSL-Zertifikaten kann verwirrend und zeitraubend sein. Daher ist Adobe eine Partnerschaft mit DigiCert, einer branchenführenden Zertifizierungsstelle (CA), eingegangen und hat einen integrierten Prozess entwickelt, durch den der Kauf und die Verwaltung dieser Zertifikate automatisiert werden.

Mit Ihrer Einwilligung übernehmen wir gemeinsam mit unserer CA die Erstellung, Bereitstellung und Verwaltung eines neuen SHA-2-SSL-Zertifikats. Adobe verwaltet dieses Zertifikat und gewährleistet, dass die sichere Datenerfassung durch Ihr Unternehmen nicht durch ein unerwartetes Ablaufen der Gültigkeit, die Aberkennung oder ein Sicherheitsproblem gefährdet wird.

## Adobe Managed Certificate Program

Das Adobe Managed Certificate Program (Adobe-Programm für verwaltete Zertifikate) ist das empfohlene Verfahren zur Implementierung eines neuen Erstanbieter-SSL-Zertifikats für Erstanbieter-Cookies.

Mit diesem Programm können Sie ohne zusätzliche Kosten ein neues Erstanbieter-SSL-Zertifikat für Erstanbieter-Cookies implementieren (für Ihre ersten 100 CNAMEs). Wenn Sie derzeit Ihr eigenes kundenverwaltetes SSL-Zertifikat haben, sprechen Sie mit der Adobe-Kundenunterstützung über den Umstieg zum Adobe Managed Certificate Program.

### Implementierung

So implementieren Sie ein neues Erstanbieter-SSL-Zertifikat für Erstanbieter-Cookies:

1. Füllen Sie das [Anforderungsformular für Erstanbieter-Cookies](/help/interface/cookies/assets/FPC_Request_Form.xlsx) aus und erstellen Sie ein Ticket für die Kundenunterstützung, um Erstanbieter-Cookies im Adobe Managed Program einzurichten. Bei jedem Feld finden Sie eine Beschreibung anhand von Beispielen.

1. Erstellen Sie CNAME-Datensätze (siehe Anweisungen unten).

   Nach Erhalt des Tickets stellt Ihnen ein Mitarbeiter der Kundenunterstützung ein Paar CNAME-Datensätze bereit. Diese Datensätze müssen auf dem DNS-Server Ihres Unternehmens konfiguriert werden, bevor Adobe das Zertifikat in Ihrem Namen erwerben kann. Die CNAMES ähneln den folgenden:

   **Sicher** – Zum Beispiel verweist der Hostname `smetrics.example.com` auf: `example.com.ssl.d1.omtrdc.net`.

   **Nicht sicher** – Zum Beispiel verweist der Hostname `metrics.example.com` auf: `example.com.d1.omtrdc.net`.

1. Wenn diese CNAMEs eingerichtet sind, kauft und installiert Adobe gemeinsam mit DigiCert ein Zertifikat auf den Produktionsservern von Adobe.

   Wenn Sie bereits ein Zertifikat implementiert haben, sollten Sie eine Besuchermigration erwägen, um Ihre vorhandenen Besucher beizubehalten. Nachdem das Zertifikat live in die Produktionsumgebung von Adobe übermittelt wurde, können Sie Ihre Tracking-Server-Variablen gemäß den neuen Hostnamen aktualisieren. Wenn die Site nicht sicher (HTTP) ist, aktualisieren Sie also `s.trackingServer`. Wenn die Site sicher ist (HTTPS), aktualisieren Sie die beiden Variablen `s.trackingServer` und `s.trackingServerSecure`.

1. [Validieren Sie die Weiterleitung von Hostnamen](#validate) (siehe unten).

1. [Aktualisieren Sie den Implementierungscode](#update) (siehe unten).

### Wartung und Verlängerung

SSL-Zertifikate laufen jedes Jahr ab, d. h. Adobe muss jedes Jahr ein neues Zertifikat für jede Implementierung erwerben. Alle unterstützten Benutzer in Ihrem Unternehmen erhalten kurz von jedem Ablauf einer Implementierung eine E-Mail-Benachrichtigung. Damit Adobe Ihren Hostnamen verlängert, muss ein unterstützter Benutzer auf die E-Mail von Adobe antworten und angeben, dass der ablaufende Hostname weiterhin für die Datenerfassung verwendet werden soll. Adobe kauft dann automatisch ein neues Zertifikat und installiert es.

### Häufig gestellte Fragen

| Frage | Antwort |
|---|---|
| **Ist dieser Prozess sicher?** | Ja, das Adobe Managed-Programm ist sicherer als unsere frühere Methode, da weder Zertifikate noch private Schlüssel außerhalb von Adobe und der Zertifizierungsstelle ausgetauscht werden. |
| **Wie kann Adobe ein Zertifikat für unsere Domäne erwerben?** | Das Zertifikat kann nur gekauft werden, wenn Sie mit dem jeweiligen Hostnamen (z. B. `smetrics.example.com`) auf Hostnamen von Adobe verweisen. Dadurch wird dieser Hostname an Adobe übertragen und Adobe kann das Zertifikat in Ihrem Namen erwerben. |
| **Kann ich verlangen, dass das Zertifikat entzogen wird?** | Ja, als Eigentümer der Domäne können Sie verlangen, dass uns das Zertifikat entzogen wird. Sie müssen dazu nur ein Ticket bei der Kundenunterstützung erstellen. |
| **Verwendet dieses Zertifikat SHA-2-Verschlüsselung?** | Ja, Adobe gibt in Zusammenarbeit mit DigiCert ein SHA-2-Zertifikat heraus. |
| **Verursacht dies Mehrkosten?** | Nein, Adobe stellt diesen Dienst allen aktuellen Adobe Digital Experience-Kunden kostenlos zur Verfügung. |

## Erstellen von CNAME-Datensätzen

Das Netzwerkteam Ihres Unternehmens sollte Ihre DNS-Server konfigurieren, indem es neue CNAME-Datensätze erstellt. Jeder Hostname leitet Daten an die Datenerfassungsserver von Adobe weiter.

Der FPC-Spezialist stellt Ihnen die konfigurierten Hostnamen bereit und gibt an, auf welche CNAMEs sie verweisen sollen. Beispiel:

* **SSL-Hostname**: `smetrics.mysite.com`
* **SSL-CNAME**: `mysite.com.ssl.sc.omtrdc.net`
* **Nicht-SSL-Hostname**: `metrics.mysite.com`
* **Nicht-SSL-CNAME**: `mysite.com.sc.omtrdc.net`

Solange der Implementierungscode nicht verändert wird, beeinflusst dieser Schritt nicht die Datensammlung und kann zu einem beliebigen Zeitpunkt nach der Aktualisierung des Implementierungscodes vorgenommen werden.

>[!NOTE]
>
>Der Experience Cloud-Besucher-ID-Dienst bietet eine Alternative zum Konfigurieren eines CNAME, um Erstanbieter-Cookies zu aktivieren.

## Überprüfen der Hostnamenweiterleitung {#validate}

Die folgenden Methoden stehen zur Überprüfung zur Verfügung:

### Validieren mithilfe eines Browsers

Wenn Sie einen CNAME eingerichtet haben und das Zertifikat installiert ist, können Sie den Browser zur Überprüfung verwenden:

`https://sstats.adobe.com/_check`

>[!NOTE]
>
>Wenn kein Zertifikat installiert ist, wird eine Sicherheitswarnung angezeigt.

### Validieren mit [!DNL curl]

Adobe empfiehlt die Verwendung von [[!DNL curl]](https://curl.haxx.se/) über die Befehlszeile. ([!DNL Windows]-Benutzer können [!DNL curl] über folgenden Link installieren: <https://curl.haxx.se/windows/>)

Wenn Sie einen CNAME haben, aber kein Zertifikat installiert ist, führen Sie Folgendes aus:
`curl -k https://sstats.adobe.com/_check`
Antwort: `SUCCESS`

(Der `-k`-Wert deaktiviert die Sicherheitswarnung.)

Wenn Sie einen CNAME eingerichtet haben und das Zertifikat installiert ist, führen Sie Folgendes aus:
`curl https://sstats.adobe.com/_check`
Antwort: `SUCCESS`

### Validieren mit [!DNL nslookup]

Sie können `nslookup` zur Überprüfung verwenden. Verwenden Sie `sstats.adobe.com` als Beispiel, öffnen Sie eine Eingabeaufforderung und geben Sie `nslookup sstats.adobe.com` ein.

Wenn alles erfolgreich eingerichtet wurde, wird eine Rückgabe ähnlich der folgenden angezeigt:

```
nslookup sstats.adobe.com
Server:             10.30.7.247
Address:     10.30.7.247#53

sstats.adobe.com    canonical name = adobe.com.ssl.d1.sc.omtrdc.net.
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.218.180.161
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 52.39.8.230
Name:  adobe.com.ssl.d1.sc.omtrdc.net
Address: 54.187.216.46
```

## Aktualisierung des Implementierungscodes {#update}

Bevor Sie Code auf Ihrer Site bearbeiten, um Erstanbieter-Cookies zu verwenden, müssen folgende Voraussetzungen erfüllt sein:

* Fordern Sie ein SSL-Zertifikat an, indem Sie die oben im Abschnitt *Implementierung* des [Adobe Programms für verwaltete Zertifikate](#adobe-managed-certificate-program) beschriebenen Schritte befolgen.
* Erstellen Sie CNAME-Datensätze (siehe oben).
* Validieren Sie die Hostnamen (siehe oben).

Nachdem Sie geprüft haben, dass Ihr(e) Hostname(n) reagieren und die Weiterleitung an die Adobe-Datensammlungsserver funktioniert, können Sie Ihre Implementierung ändern, damit diese zu Ihren eigenen Cookie-Domains weist.

1. Öffnen Sie Ihre JavaScript-Kerndatei (`s_code.js/AppMeasurement.js`).
1. Wenn Sie Ihre Codeversion aktualisieren möchten, ersetzen Sie die gesamte `s_code.js/AppMeasurement.js`-Datei mit der neueren Version und ersetzen Sie alle Plugins oder Einstellungen (falls vorhanden). **Oder** wenn Sie den Code aktualisieren möchten, der nur für Erstanbieter-Cookies gilt, suchen Sie die Variablen s.trackingServer und s.trackingServerSecure (falls SSL verwendet wird) und verweisen Sie sie auf Ihre neuen Datenerfassungs-Hostnamen. Verwenden von mysite.com als Beispiel: `s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Laden Sie die aktualisierte JavaScript-Kerndatei auf Ihre Site.

1. Wenn Sie von einer älteren Implementierung zu Erstanbieter-Cookies wechseln oder zu einem anderen Hostnamen der Erstanbieter-Datensammlung wechseln, empfehlen wir, Besucher aus der vorherigen Domäne in die neue Domäne zu migrieren.

Siehe [Besuchermigration](https://docs.adobe.com/content/help/de-DE/analytics/components/metrics/unique-visitors.html) im Analytics-Implementierungshandbuch.

Nachdem Sie die JavaScript-Datei hochgeladen haben, ist die Konfiguration für die Erstanbieter-Cookie-Datensammlung abgeschlossen. Es wird empfohlen, Analytics-Berichte in den nächsten Stunden zu überwachen, um sicherzustellen, dass die Datenerfassung wie üblich erfolgt. Ist dies nicht der Fall, stellen Sie sicher, dass alle oben genannten Schritte ausgeführt wurden und veranlassen Sie, dass ein unterstützter Mitarbeiter Ihrer Organisation die Kundenunterstützung kontaktiert.
