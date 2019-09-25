---
description: Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.
keywords: Cookies, Datenschutz
seo-description: Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.
seo-title: Wie sich veränderter Drittanbieter-Cookie-Support auf Kunden auswirkt
solution: Experience Cloud,Analytics,Target,Social
title: Wie sich veränderter Drittanbieter-Cookie-Support auf Kunden auswirkt
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
index: y
internal: n
snippet: y
translation-type: ht
source-git-commit: f59badcd3423ada51a3fe0c605158a009d5b1d64

---


# Auswirkungen der geänderten Unterstützung von Drittanbieter-Cookies{#how-changes-to-third-party-cookie-support-impacts-customers}

Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.

Die folgende Liste gibt Aufschluss darüber, wie sich die Unterstützung für Drittanbieter-Cookies auf aktuelle Implementierungen der Adobe Experience Cloud-Lösungen auswirkt:

## Adobe Analytics und Adobe Target

* Kunden mit [Erstanbieter-Implementierung](/help/interface/cookies/cookies-first-party.md) sind größtenteils nicht betroffen.
* Kunden, die keine Erstanbieter-Implementierung verwenden, können den [Experience Platform-ID-Dienst](https://docs.adobe.com/content/help/de-DE/id-service/using/implementation-guides/implementation-guides.html) implementieren, um das ID-Cookie als Erstanbieter-Cookie ohne Erstanbieter-Implementierung zu speichern.

## Adobe Experience Manager

* Da Adobe Experience Manager vollständig innerhalb der Kundendomäne ausgeführt wird, kommt es nur zu minimaler Interaktion mit Drittanbieter-Cookies und damit zu minimalen oder keinerlei Auswirkungen.

## Adobe Social

* Social ist nicht betroffen, solange der Kunde über die neueste Version des Codes verfügt.

## Adobe Advertising Cloud

* Suche:

   * Bei mit Adobe Analytics-Daten optimierter Suchfunktion wäre die Suche genau wie Adobe Analytics betroffen.
   * Die Erfassung von Konversionsdaten wäre nicht betroffen.

* Anzeigen:

   * Das Display-Remarketing ist derzeit vollständig von der Verwendung von Drittanbieter-Cookies abhängig.
   * Display ist auch stark von der Verfügbarkeit verschiedener Werbenetzwerkcookies für die Synchronisierung abhängig.
   * Die Gesamtwirkung ist unbekannt. Doch schon jetzt kann konstatiert werden, dass Display stärker als andere Services betroffen ist.
   * Wir arbeiten derzeit intern und in Kooperation mit unseren Werbepartnern daran, das volle Ausmaß der Auswirkungen auf die Anzeigenzustellung zu evaluieren.

* Social:

   * Es gibt keinerlei Auswirkungen auf Anzeigen auf dem Facebook-Marktplatz.
   * Facebook Exchange (FBX) wird genau so wie die Display-Anzeigenzustellung betroffen sein.

