---
description: Analytics verwendet Cookies, um Informationen zu Variablen und Komponenten zu liefern, die nicht zwischen Bildanfragen und Browsersitzungen bestehen bleiben.
keywords: Cookies, Datenschutz
seo-description: Analytics verwendet Cookies, um Informationen zu Variablen und Komponenten zu liefern, die nicht zwischen Bildanfragen und Browsersitzungen bestehen bleiben.
seo-title: Erstanbieter-Cookies
solution: Experience Cloud,Analytics
title: Erstanbieter-Cookies
index: y
snippet: y
translation-type: tm+mt
source-git-commit: 90123ac9194d180a6a8ae59a273a6a6154ea8d96

---


# Informationen zu Erstanbieter-Cookies

Analytics verwendet Cookies, um Informationen zu Variablen und Komponenten zu liefern, die nicht zwischen Bildanfragen und Browsersitzungen bestehen bleiben. Diese harmlosen Cookies stammen aus einer von Adobe gehosteten Domain und werden als Drittanbieter-Cookies bezeichnet.

Viele Browser und Anti-Spyware-Anwendungen sind dafür ausgelegt, Cookies von Drittanbietern abzuweisen und zu löschen, einschließlich der bei der Analytics-Datensammlung verwendeten Cookies. Um diese Einschränkungen beim Tracking durch Browser und Programme zu umgehen, können Sie Erstanbieter-Cookies implementieren.

Es stehen zwei Optionen zur Implementierung von Erstanbieter-Cookies zur Verfügung.

* Der ID-Dienst von Experience Platform. Der ID-Dienst kann das Cookie im Erstanbieterkontext mit JavaScript setzen.
* DNS-Einträge im DNS-Server Ihres Unternehmens.
* Wenn Ihre Site sichere Seiten mit dem `https:`-Protokoll enthält und Sie den Experience Platform ID-Dienst nicht verwenden, können Sie von Adobe ein SSL-Zertifikat anfordern, mit dem Sie Erstanbieter-Cookies implementieren können.

Der Bereitstellungsprozess von SSL-Zertifikaten kann verwirrend und zeitraubend sein. Daher ist Adobe eine Partnerschaft mit DigiCert, einer branchenführenden Zertifizierungsstelle (CA), eingegangen und hat einen integrierten Prozess entwickelt, durch den der Kauf und die Verwaltung dieser Zertifikate automatisiert werden.

Mit Ihrer Einwilligung übernehmen wir gemeinsam mit unserer CA die Erstellung, Bereitstellung und Verwaltung eines neuen SHA-2-SSL-Zertifikats. Adobe verwaltet dieses Zertifikat und gewährleistet, dass die sichere Datenerfassung durch Ihr Unternehmen nicht durch ein unerwartetes Ablaufen der Gültigkeit, die Aberkennung oder ein Sicherheitsproblem gefährdet wird.

## Adobe Managed Certificate Program

Das Adobe Managed Certificate Program (Adobe-Programm für verwaltete Zertifikate) ist das empfohlene Verfahren zur Implementierung eines neuen Erstanbieter-SSL-Zertifikats für Erstanbieter-Cookies.

Mit diesem Programm können Sie ohne zusätzliche Kosten ein neues Erstanbieter-SSL-Zertifikat für Erstanbieter-Cookies implementieren. Wenn Sie derzeit Ihr eigenes kundenverwaltetes SSL-Zertifikat haben, sprechen Sie mit der Adobe-Kundenunterstützung über den Umstieg zum Adobe Managed Certificate Program.

### Implementierung

So implementieren Sie ein neues Erstanbieter-SSL-Zertifikat für Erstanbieter-Cookies:

1. Füllen Sie das [Anforderungsformular für Erstanbieter-Cookies](/help/interface/cookies/assets/FPC_Request_Form.xlsx) aus und erstellen Sie ein Ticket für die Kundenunterstützung, um Erstanbieter-Cookies im Adobe Managed Program einzurichten. Bei jedem Feld finden Sie eine Beschreibung anhand von Beispielen.

1. Erstellen Sie CNAME-Datensätze (siehe Anweisungen unten). Nach Erhalt des Tickets sollte ein Kundenbetreuer Ihnen ein Paar CNAME-Einträge zur Verfügung stellen. Diese Datensätze müssen auf dem DNS-Server Ihres Unternehmens konfiguriert werden, bevor Adobe das Zertifikat in Ihrem Namen erwerben kann. Die CNAMEs sehen in etwa folgendermaßen aus: **Sicher** – Zum Beispiel verweist der Hostname `smetrics.example.com` auf: `example.com.ssl.d1.omtrdc.net`. **Nicht sicher** – Zum Beispiel verweist der Hostname `metrics.example.com` auf `example.com.d1.omtrdc.net`.

1. Wenn diese CNAMEs eingerichtet sind, kauft und installiert Adobe gemeinsam mit DigiCert ein Zertifikat auf den Produktionsservern von Adobe. Wenn Sie bereits ein Zertifikat implementiert haben, sollten Sie eine Besuchermigration erwägen, um Ihre vorhandenen Besucher zu behalten. Nachdem das Zertifikat live in die Produktionsumgebung von Adobe übermittelt wurde, können Sie Ihre Tracking-Server-Variablen gemäß den neuen Hostnamen aktualisieren. Wenn die Site nicht sicher (http) ist, aktualisieren Sie `s.trackingServer`. Wenn die Site sicher ist (https), aktualisieren Sie beide Variablen, `s.trackingServer` und `s.trackingServerSecure`.

1. Führen Sie einen Ping auf den Hostnamen durch (siehe unten).

1. Aktualisieren Sie den Implementierungscode (siehe unten).

### Wartung und Verlängerung

SSL-Zertifikate laufen jedes Jahr ab, d. h. Adobe muss jedes Jahr ein neues Zertifikat für jede Implementierung erwerben. Alle unterstützten Benutzer in Ihrem Unternehmen erhalten kurz von jedem Ablauf einer Implementierung eine E-Mail-Benachrichtigung. Damit Adobe Ihren Hostnamen verlängert, muss ein unterstützter Benutzer auf die E-Mail von Adobe antworten und angeben, dass der ablaufende Hostname weiterhin für die Datenerfassung verwendet werden soll. Adobe kauft dann automatisch ein neues Zertifikat und installiert es.

### Häufig gestellte Fragen

| Frage | Antwort |
|---|---|
| **Ist dieser Prozess sicher?** | Ja, das Adobe Managed-Programm ist sicherer als unsere frühere Methode, da weder Zertifikate noch private Schlüssel außerhalb von Adobe und der Zertifizierungsstelle ausgetauscht werden. |
| **Wie kann Adobe ein Zertifikat für unsere Domäne erwerben?** | Das Zertifikat kann nur gekauft werden, wenn Sie mit dem jeweiligen Hostnamen (z. B. smetrics.beispiel.com) auf Hostnamen von Adobe verweisen. Dadurch wird dieser Hostname an Adobe übertragen und Adobe kann das Zertifikat in Ihrem Namen erwerben. |
| **Kann ich verlangen, dass das Zertifikat entzogen wird?** | Ja, als Eigentümer der Domäne können Sie verlangen, dass uns das Zertifikat entzogen wird. Sie müssen dazu nur ein Ticket bei der Kundenunterstützung erstellen. |
| **Verwendet dieses Zertifikat SHA-2-Verschlüsselung?** | Ja, Adobe gibt in Zusammenarbeit mit DigiCert ein SHA-2-Zertifikat heraus. |
| **Verursacht dies Mehrkosten?** | Nein, Adobe stellt diesen Dienst allen aktuellen Analytics-Kunden kostenlos zur Verfügung. |

## Erstellen von CNAME-Datensätzen

Das Netzwerkteam Ihres Unternehmens sollte Ihre DNS-Server konfigurieren, indem es neue CNAME-Datensätze erstellt. Jeder Hostname leitet Daten an die Datenerfassungsserver von Adobe weiter.

Der FPC-Spezialist stellt Ihnen die konfigurierten Hostnamen bereit und gibt an, auf welche CNAMEs sie verweisen sollen. Beispiel:

* **SSL-Hostname**:`smetrics.mysite.com`
* **SSL-CNAME**:`mysite.com.ssl.sc.omtrdc.net`
* **Nicht-SSL-Hostname**:`metrics.mysite.com`
* **Nicht-SSL-CNAME**:`mysite.com.sc.omtrdc.net`

Solange der Implementierungscode nicht verändert wird, beeinflusst dieser Schritt nicht die Datensammlung und kann zu einem beliebigen Zeitpunkt nach der Aktualisierung des Implementierungscodes vorgenommen werden.

>[!NHinweis:] Der Experience Cloud-Besucher-ID-Dienst bietet eine Alternative zum Konfigurieren eines CNAME, um Erstanbieter-Cookies zu ermöglichen.

## Ping an den Hostnamen durchführen

Führen Sie einen Ping an den Hostnamen durch, um eine korrekte Weiterleitung zu garantieren. Alle Hostnamen müssen auf einen Ping reagieren, um Datenverlust zu verhindern.

Nachdem CNAME-Datensätze ordnungsgemäß konfiguriert wurden und Adobe die Installation des Zertifikats bestätigt hat, öffnen Sie eine Eingabeaufforderung und führen Sie einen Ping an Ihre Hostnamen durch. Verwenden von `mysite.com` als Beispiel: `ping metrics.mysite.com`

Wenn alles erfolgreich eingerichtet wurde, wird in etwa Folgendes zurückgegeben:

```Pinging mysite.com.112.2o7.net [66.235.132.232] with 32 bytes of data:
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246
Reply from 66.235.132.232: bytes=32 time=19ms TTL=246

Ping statistics for 66.235.132.232: Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),
Approximate round trip times in milli-seconds: Minimum = 19ms, Maximum = 19ms, Average = 19ms
```

Wenn die CNAME-Datensätze nicht korrekt eingerichtet oder nicht aktiv sind, erhalten Sie folgendes Ergebnis:

`Ping request could not find the host. Please check the name and try again.`

>[!NHinweis:] Wenn Sie `https:// protocol` verwenden, reagiert der Ping erst nach dem durch den FPC-Spezialisten festgelegten Upload-Datum. Stellen Sie auch sicher, dass ein Ping des sicheren und des nicht sicheren Hostnamens durchgeführt wird, sodass gewährleistet ist, dass beide korrekt funktionieren, bevor Sie Ihre Implementierung aktualisieren..

## Aktualisierung des Implementierungscodes

Bevor Sie Code auf Ihrer Site bearbeiten, um Erstanbieter-Cookies zu verwenden, müssen folgende Voraussetzungen erfüllt sein:

* Fordern Sie ein SSL-Zertifikat an, wie oben in den Implementierungsschritten für das Adobe Managed Certificate Program beschrieben.
* Erstellen Sie CNAME-Datensätze (siehe oben).
* Führen Sie einen Ping auf den Hostnamen durch (siehe oben).

Nachdem Sie geprüft haben, dass Ihr(e) Hostname(n) reagieren und die Weiterleitung an die Adobe-Datensammlungsserver funktioniert, können Sie Ihre Implementierung ändern, damit diese zu Ihren eigenen Cookie-Domains weist.

1. Öffnen Sie Ihre JavaScript-Kerndatei (`s_code.js/AppMeasurement.js`).
1. Wenn Sie Ihre Codeversion aktualisieren möchten, ersetzen Sie die gesamte `s_code.js/AppMeasurement.js`-Datei mit der neueren Version und ersetzen Sie alle Plugins oder Einstellungen (falls vorhanden). **Oder** wenn Sie den Code aktualisieren möchten, der nur für Erstanbieter-Cookies gilt, suchen Sie die Variablen s.trackingServer und s.trackingServerSecure (falls SSL verwendet wird) und verweisen Sie sie auf Ihre neuen Datenerfassungs-Hostnamen. Verwenden von mysite.com als Beispiel:`s.trackingServer = "metrics.mysite.com"` `s.trackingServerSecure = "smetrics.mysite.com"`

1. Laden Sie die aktualisierte JavaScript-Kerndatei auf Ihre Site.

1. Wenn Sie von einer älteren Implementierung zu Erstanbieter-Cookies wechseln oder zu einem anderen Hostnamen der Erstanbieter-Datensammlung wechseln, empfehlen wir, Besucher aus der vorherigen Domäne in die neue Domäne zu migrieren.

Siehe [Besuchermigration](https://docs.adobe.com/help/en/analytics/implementation/javascript-implementation/visitor-migration.html) im Analytics-Implementierungshandbuch.

Nachdem Sie die JavaScript-Datei hochgeladen haben, ist die Konfiguration für die Erstanbieter-Cookie-Datensammlung abgeschlossen. Es wird empfohlen, Analytics-Berichte in den nächsten Stunden zu überwachen, um sicherzustellen, dass die Datenerfassung wie üblich erfolgt. Ist dies nicht der Fall, stellen Sie sicher, dass alle oben genannten Schritte ausgeführt wurden und veranlassen Sie, dass ein unterstützter Mitarbeiter Ihrer Organisation die Kundenunterstützung kontaktiert.
