---
description: Erfahren Sie, inwiefern die Unterstützung für Drittanbieter-Cookies in Browsern immer mehr eingeschränkt wird.
keywords: Cookies, Datenschutz
solution: Experience Cloud,Analytics,Target
title: 'Auswirkungen von Änderungen an der Unterstützung von Drittanbieter-Cookies auf Kunden '
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
feature: Cookies
topic: Administration
role: Administrator
level: Experienced
exl-id: 3d12a1b1-c952-4b42-815d-f64b31429cec
source-git-commit: ef6196c3096ac7b26633eb4b1b9b2db26237732a
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 84%

---

# Auswirkungen der geänderten Unterstützung von Drittanbieter-Cookies auf Kunden {#how-changes-to-third-party-cookie-support-impacts-customers}

Die Unterstützung für Drittanbieter-Cookies in Browsern ist mehr und mehr zurückgegangen. Aus diesem Grund hat Adobe an neuen Lösungen gearbeitet, die sowohl den Anforderungen der Kunden als auch dem Recht der Verbraucher auf Privatsphäre in den Adobe Experience Cloud-Lösungen in ausgewogenem Maße Rechnung tragen.

In der folgenden Liste wird erläutert, wie sich die Unterstützung von Drittanbieter-Cookies auf aktuelle Implementierungen der Adobe Experience Cloud-Lösungen auswirkt:

## Adobe Analytics und Adobe Target

* Analytics und Target sind größtenteils nicht betroffen, da dieselbe Site-Aktivität nur auf Erstanbieter-Cookies angewiesen ist. Zur domänenübergreifenden Erläuterung der Benutzeraktivität sind Drittanbieter-Cookies erforderlich. Bei Browsern, in denen Drittanbieter-Cookies blockiert werden, ist ein domänenübergreifendes Tracking mit Cookies nicht möglich.

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
