---
description: Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.
keywords: cookies;privacy
seo-description: Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.
seo-title: Wie sich veränderter Drittanbieter-Cookie-Support auf Kunden auswirkt
solution: Marketing Cloud,Analytics,Adobe Target,Adobe Social
title: Wie sich veränderter Drittanbieter-Cookie-Support auf Kunden auswirkt
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# How changes to third-party cookie support impact customers{#how-changes-to-third-party-cookie-support-impacts-customers}

Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.

In der folgenden Liste wird erläutert, wie sich die Unterstützung von Drittanbieter-Cookies auf aktuelle Implementierungen der Adobe Experience Cloud-Lösungen auswirkt:

## Adobe Analytics und Adobe Target

* Kunden mit [Erstanbieter-Implementierung](/help/interface/cookies/cookies-first-party.md) sind größtenteils nicht betroffen.
* Customers that are not using first-party implementation can implement the [Experience Platform ID Service](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/implementation-guides.html) to store the ID cookie as a first-party cookie without a first-party implementation.

## Adobe Experience Manager

* Da Adobe Experience Manager vollständig innerhalb der Kundendomäne ausgeführt wird, kommt es nur zu minimaler Interaktion mit Drittanbieter-Cookies und damit zu minimalen oder keinerlei Auswirkungen.

## Adobe Social

* Social ist nicht betroffen, solange der Kunde über die neueste Version des Codes verfügt.

## Adobe Advertising Cloud

* Suche:

   * Wird die Suche auf der Grundlage von Adobe Analytics-Daten optimiert, wird die Suche auf dieselbe Weise wie Adobe Analytics beeinflusst.
   * Die Erfassung von Konversionsdaten sollte davon nicht betroffen sein.

* Anzeigen:

   * Display-Remarketing heute hängt vollständig von der Verwendung von Drittanbieter-Cookies ab.
   * Die Anzeige ist auch stark von der Verfügbarkeit verschiedener Werbe-Netzwerk-Cookies für die Synchronisierung abhängig.
   * Die Gesamtwirkung ist nicht bekannt. Die Anzeige wird jedoch vom ersten Punkt an stärker beeinflusst als andere Dienste.
   * Wir arbeiten intern und mit unseren Werbepartnern zusammen, um die Auswirkungen auf den Versand von Werbeanzeigen in vollem Umfang zu bewerten.

* Social:

   * Es gibt keine Auswirkungen auf Facebook-Marktplatzierungen.
   * Facebook Exchange (FBX) wird genauso betroffen sein wie der Versand der Anzeige.
