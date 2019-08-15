---
description: Analytics verwendet Cookies, um Informationen zu Variablen und Komponenten zu liefern, die nicht zwischen Bildanfragen und Browsersitzungen bestehen bleiben.
keywords: Cookies; Datenschutz
seo-description: Analytics verwendet Cookies, um Informationen zu Variablen und Komponenten zu liefern, die nicht zwischen Bildanfragen und Browsersitzungen bestehen bleiben.
seo-title: Erstanbieter-Cookies
solution: Experience Cloud, Analytics
title: Erstanbieter-Cookies
index: y
snippet: y
translation-type: tm+mt
source-git-commit: 345b1fda364d9f7e884e94f32807bb99cc0c3476

---


# Informationen zu Erstanbieter-Cookies

Analytics verwendet Cookies, um Informationen zu Variablen und Komponenten zu liefern, die nicht zwischen Bildanfragen und Browsersitzungen bestehen bleiben. Diese harmlosen Cookies stammen aus einer von Adobe gehosteten Domain und werden als Drittanbieter-Cookies bezeichnet.

Viele Browser und Anti-Spyware-Anwendungen dienen zum Ablehnen und Löschen von Drittanbieter-Cookies, einschließlich der in der Analytics-Datenerfassung verwendeten. Um Beschränkungen bei der Nachverfolgung durch Browser und Programme zu umgehen, können Sie Erstanbieter-Cookies implementieren.

Es stehen zwei Optionen zur Implementierung von Erstanbieter-Cookies zur Verfügung.

* Experience Platform ID-Dienst. Der ID-Dienst kann das Cookie im Erstanbieterkontext mit javascript festlegen.
* DNS-Einträge auf Ihrem Unternehmen DNS-Server.
* Wenn Ihre Site sichere Seiten über das `https:` Protokoll enthält und Sie nicht den Experience Platform ID-Dienst verwenden, können Sie mit Adobe arbeiten, um ein SSL-Zertifikat abzurufen, um Erstanbieter-Cookies zu implementieren.

Der SSL-Zertifikatsprozess kann häufig verwirrend und zeitraubend sein. Daher hat Adobe eine Partnerschaft mit digicert, einer branchenführenden Zertifizierungsstelle (CA) und einen integrierten Prozess entwickelt, mit dem der Kauf und die Verwaltung dieser Zertifikate automatisiert werden.

Mit Ihrer Berechtigung arbeiten wir mit unserem CA zusammen, um ein neues SHA -2 SSL-Zertifikat für Sie zu erstellen, bereitzustellen und zu verwalten. Adobe wird dieses Zertifikat weiterhin verwalten und sicherstellen, dass ein unerwartetes Ablaufdatum, ein unerwartetes Ablaufdatum oder ein Sicherheitsproblem nicht die Verfügbarkeit Ihrer Organisation sicher ist.

## Adobe Programm für verwaltete Zertifikate

Das Adobe Managed Certificate-Programm ist der empfohlene Prozess zur Implementierung eines neuen Erstanbieter-SSL-Zertifikats für Erstanbieter-Cookies.

Mit dem Programm "Adobe Managed Certificate" können Sie ohne zusätzliche Kosten ein neues Erstanbieter-SSL-Zertifikat für Erstanbieter-Cookies implementieren. Wenn Sie derzeit Ihr eigenes kundenverwaltetes SSL-Zertifikat haben, sprechen Sie mit dem Adobe-Kundendienst, um zum Adobe Managed Certificate-Programm zu migrieren.

### Implementierung

So implementieren Sie ein neues Erstanbieter-SSL-Zertifikat für Erstanbieter-Cookies:

1. Füllen Sie das Anforderungsformular aus und öffnen Sie ein Ticket mit dem Kundendienst, um Erstanbieter-Cookies im Adobe Managed Program einzurichten. Jedes Feld wird in dem Dokument anhand von Beispielen beschrieben.

1. Erstellen Sie CNAME-Datensätze (siehe Anweisungen unten). Beim Empfang des Tickets sollte Ihnen ein FPSSL-Spezialist ein Paar von CNAME-Aufzeichnungen bereitstellen. Diese Datensätze müssen auf dem DNS-Server Ihres Unternehmens konfiguriert werden, bevor Adobe das Zertifikat in Ihrem Namen erwerben kann. Die CNAMES ähneln dem folgenden.

* **Sicher** - Zum Beispiel verweist der Hostname `smetrics.example.com` auf: `example.com.ssl.d1.omtrdc.net`.
* **Nicht sicher** - zum Beispiel verweist der Hostname `metrics.example.com` auf: `example.com.d1.omtrdc.net`.

1. Wenn diese CNAMES vorhanden sind, arbeitet Adobe mit digicert zusammen, um ein Zertifikat auf den Produktionsservern von Adobe zu erwerben und zu installieren. Wenn Sie eine Implementierung haben, sollten Sie die Besuchermigration erwägen, um Ihre vorhandenen Besucher beizubehalten. Nachdem das Zertifikat live in die Produktionsumgebung von Adobe geschaltet wurde, können Sie Ihre Tracking-Server-Variablen auf die neuen Hostnamen aktualisieren. Wenn die Site nicht sicher (https) ist, aktualisieren Sie die `s.trackingServer`. Wenn die Site sicher ist (https), aktualisieren Sie beide `s.trackingServer` und `s.trackingServerSecure` Variablen.

1. Ping des Hostnamens (siehe unten).

1. Aktualisieren Sie den Implementierungscode (siehe unten).

### Wartung und Erneuerungen

SSL-Zertifikate laufen jedes Jahr ab, d. h. Adobe muss jedes Jahr ein neues Zertifikat für jede Implementierung erwerben. Alle unterstützten Benutzer in Ihrem Unternehmen erhalten bei jedem Ablauf einer Implementierung eine E-Mail-Benachrichtigung. Damit Adobe Ihren Hostnamen erneuert, muss ein unterstützter Benutzer auf die E-Email von Adobe antworten und angeben, dass Sie den ablaufbasierten Hostnamen für die Datenerfassung weiterhin verwenden möchten. An diesem Punkt wird automatisch ein neues Zertifikat gekauft und installiert.

### Häufig gestellte Fragen

| Frage | Antwort |
|---|---|
| **Ist dieser Prozess sicher?** | Ja |
| **Wie kann Adobe ein Zertifikat für unsere Domäne erwerben?** | Das Zertifikat kann nur gekauft werden, wenn Sie den angegebenen Hostnamen (z. B. smetrics.example.com) auf einen eigenen Hostnamen von Adobe verwiesen haben. Dadurch wird der Hostname an Adobe übermittelt und Adobe kann das Zertifikat in Ihrem Namen erwerben. |
| **Kann ich das Zertifikat sperren?** | Ja, als Eigentümer der Domäne haben Sie die Berechtigung, uns das Zertifikat zu sperren. Sie müssen nur ein Ticket mit der Kundenunterstützung öffnen, um dies abzuschließen. |
| **Verwendet dieses Zertifikat SHA -2-Verschlüsselung?** | Ja, Adobe arbeitet mit digicert zusammen, um ein SHA -2-Zertifikat zu erstellen. |
| **Kostet dies Mehrkosten?** | Nein, Adobe stellt diesen Dienst für alle aktuellen Analytics-Kunden kostenlos bereit. |

## Erstellen von CNAME-Aufzeichnungen

Das Netzwerkteam Ihres Unternehmens sollte Ihre DNS-Server konfigurieren, indem Sie neue CNAME-Einträge erstellen. Jeder Hostname leitet Daten an die Datenerfassungsserver von Adobe weiter.

Der FPC-Spezialist stellt Ihnen die konfigurierten Hostnamen und die cnames bereit, auf die sie verwiesen werden sollen. Beispiel:

* **SSL-Hostname**:`smetrics.mysite.com`
* **SSL-CNAME**:`mysite.com.ssl.d1.sc.omtrdc.net`
* **Nicht-SSL-Hostname**:`metrics.mysite.com`
* **Nicht-SSL-CNAME**:`mysite.com.d1.sc.omtrdc.net`

Solange der Implementierungscode nicht geändert wird, wirkt sich dieser Schritt nicht auf die Datenerfassung aus und kann jederzeit nach der Aktualisierung des Implementierungscodes durchgeführt werden.

>[!Note:] Der Experience Cloud Besucher-ID-Dienst bietet eine Alternative zum Konfigurieren eines CNAME, um Erstanbieter-Cookies zu aktivieren.

## Ping des Hostnamens

Ping des Hostnamens zur korrekten Weiterleitung. Alle Hostnamen müssen auf einen Ping reagieren, um Datenverlust zu verhindern.

Nachdem CNAME-Aufzeichnungen ordnungsgemäß konfiguriert wurden und Adobe die Installation des Zertifikats bestätigt hat, öffnen Sie eine Eingabeaufforderung und Ping Ihres Hostnamens (s). Using `mysite.com` as an example: `ping metrics.mysite.com`

Wenn alles erfolgreich eingerichtet wurde, it will return something similar to the following:

```Pinging mysite.com.112.2o7.net [66.235.132.232] with 32 bytes of data:
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246

Ping statistics for 66.235.132.232: Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds: Minimum = 19ms, Maximum = 19ms, Average = 19ms
```

Wenn die CNAME-Aufzeichnungen nicht korrekt eingerichtet werden oder nicht aktiv sind, erhalten Sie folgendes Ergebnis:

`Ping request could not find the host. Please check the name and try again.`

>[!Note:] Wenn Sie verwenden `https:// protocol`, reagiert Ping nur nach dem vom FPC-Spezialisten angegebenen Upload-Datum. Stellen Sie sicher, dass Sie den sicheren Hostnamen und den nicht sicheren Hostnamen ping, um sicherzustellen, dass beide korrekt funktionieren, bevor Sie Ihre Implementierung aktualisieren.

## Implementierungscode aktualisieren

Bevor Sie Code auf Ihrer Site bearbeiten, um Erstanbieter-Cookies zu verwenden, müssen Sie folgende Voraussetzungen erfüllen:

* Fordern Sie ein SSL-Zertifikat an, wie beschrieben in Implementierungsschritten für das Adobe Managed Certificate-Programm.
* Erstellen Sie CNAME-Einträge.
* Ping des Hostnamens.

Nachdem Sie überprüft haben, ob Ihre Hostnamen reagieren und an Adobe-Datenerfassungsserver weiterleiten, können Sie Ihre Implementierung ändern, um auf Ihre eigenen Datenerfassungshostnamen zu verweisen.

1. Open your core JavaScript file (`s_code.js/AppMeasurement.js`).
1. Wenn Sie Ihre Codeversion aktualisieren möchten, ersetzen Sie die gesamte `s_code.js/AppMeasurement.js` --Datei mit der neueren Version und ersetzen Sie alle Plugins oder Anpassungen (falls vorhanden). **Wenn** Sie den Code aktualisieren möchten, der nur für Erstanbieter-Cookies gilt, suchen Sie die Variablen s. trackingserver und s. trackingserversecure (falls SSL verwendet wird) und verweisen Sie auf Ihre neuen Datenerfassungshostnamen. Using mysite.com as an example:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Laden Sie die aktualisierte Kern-javascript-Datei auf Ihre Site hoch.
1. Wenn Sie von einer älteren Implementierung zu Erstanbieter-Cookies wechseln oder zu einem anderen Hostnamen der Erstanbieter-Sammlung wechseln, empfehlen wir, Besucher aus der vorherigen Domäne in die neue Domäne zu migrieren.

Siehe [Besuchermigration](https://docs.adobe.com/help/en/analytics/implementation/javascript-implementation/visitor-migration.html) im Analytics-Implementierungshandbuch.

Nachdem Sie die javascript-Datei hochgeladen haben, wird alles für die Erstanbieter-Cookie-Datenerfassung konfiguriert. Es wird empfohlen, Analytics-Berichte für die nächsten Stunden zu überwachen, um sicherzustellen, dass die Datenerfassung normal fortgesetzt wird. Falls dies nicht der Fall ist, vergewissern Sie sich, dass alle oben aufgeführten Schritte abgeschlossen sind, und bitten Sie einen der unterstützten Benutzer Ihres Unternehmens, sich an den Kundendienst zu wenden.
