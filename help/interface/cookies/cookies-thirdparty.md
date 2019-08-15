---
description: Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.
keywords: Cookies; Datenschutz
seo-description: Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.
seo-title: Wie sich veränderter Drittanbieter-Cookie-Support auf Kunden auswirkt
solution: Marketing Cloud, Analytics, Target, Social
title: Wie sich veränderter Drittanbieter-Cookie-Support auf Kunden auswirkt
uuid: 27332 e 0 d -6932-4 a 6 e-b 97 b -0 adeced 0 b 050
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: f59badcd3423ada51a3fe0c605158a009d5b1d64

---


# Auswirkungen von Änderungen an der Unterstützung von Drittanbieter-Cookies{#how-changes-to-third-party-cookie-support-impacts-customers}

Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.

Die folgende Liste gibt Aufschluss darüber, wie sich die Unterstützung für Drittanbieter-Cookies auf aktuelle Implementierungen der Adobe Experience Cloud-Lösungen auswirkt:

## Adobe Analytics und Adobe Target

* Customers with a [first-party implementation](/help/interface/cookies/cookies-first-party.md) would remain largely unaffected.
* Customers that are not using first-party implementation can implement the [Experience Platform ID Service](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/implementation-guides.html) to store the ID cookie as a first-party cookie without a first-party implementation.

## Adobe Experience Manager

* Da Adobe Experience Manager vollständig innerhalb der Domäne des Kunden arbeitet, gibt es minimale Interaktionen mit Drittanbieter-Cookies und so wenig ohne Auswirkung auf keine Auswirkungen.

## Adobe Social

* Social ist nicht betroffen, solange der Kunde über die neueste Version des Codes verfügt.

## Adobe Advertising Cloud

* Durchsuchen:

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

