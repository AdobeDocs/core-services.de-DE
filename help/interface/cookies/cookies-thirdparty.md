---
description: Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.
keywords: cookies;privacy
seo-description: Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.
seo-title: Wie sich veränderter Drittanbieter-Cookie-Support auf Kunden auswirkt
solution: Marketing Cloud,Analytics,Adobe Target,Adobe Social
title: Wie sich veränderter Drittanbieter-Cookie-Support auf Kunden auswirkt
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
translation-type: ht
source-git-commit: f65132e291ba925ded39d75e92b24cf707d520b5
workflow-type: ht
source-wordcount: '368'
ht-degree: 100%

---


# Auswirkungen der geänderten Unterstützung von Drittanbieter-Cookies auf Kunden {#how-changes-to-third-party-cookie-support-impacts-customers}

Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.

In der folgenden Liste wird erläutert, wie sich die Unterstützung von Drittanbieter-Cookies auf aktuelle Implementierungen der Adobe Experience Cloud-Lösungen auswirkt:

## Adobe Analytics und Adobe Target

* Kunden mit [Erstanbieter-Implementierung](/help/interface/cookies/cookies-first-party.md) sind größtenteils nicht betroffen.
* Kunden, die keine Erstanbieter-Implementierung verwenden, können den [Experience Platform-ID-Dienst](https://docs.adobe.com/content/help/de-DE/id-service/using/implementation/implementation-guides.html) implementieren, um das ID-Cookie als Erstanbieter-Cookie ohne Erstanbieter-Implementierung zu speichern.

## Adobe Experience Manager

* Da Adobe Experience Manager vollständig innerhalb der Kundendomäne ausgeführt wird, kommt es nur zu minimaler Interaktion mit Drittanbieter-Cookies und damit zu minimalen oder keinerlei Auswirkungen.

## Adobe Social

* Social ist nicht betroffen, solange der Kunde über die neueste Version des Codes verfügt.

## Adobe Advertising Cloud

* Suche:

   * Wenn die Suche auf der Grundlage von Adobe Analytics-Daten optimiert wird, wird sie auf dieselbe Weise wie Adobe Analytics beeinflusst.
   * Die Erfassung von Konversionsdaten sollte davon nicht betroffen sein.

* Anzeigen:

   * Die Remarketing-Anzeige hängt heute vollständig von der Verwendung von Drittanbieter-Cookies ab.
   * Die Anzeige ist auch stark von der Verfügbarkeit verschiedener Werbenetzwerk-Cookies für die Synchronisierung abhängig.
   * Die Gesamtauswirkung ist nicht bekannt. Die Anzeige wird jedoch vom ersten Punkt an stärker beeinflusst als andere Dienste.
   * Wir arbeiten intern und mit unseren Werbepartnern zusammen, um die vollständigen Auswirkungen auf das Senden von Werbeanzeigen zu bewerten.

* Social:

   * Es gibt keine Auswirkungen auf Facebook-Marktplatzierungen.
   * Facebook Exchange (FBX) ist genauso betroffen wie das Senden der Display-Anzeige.
