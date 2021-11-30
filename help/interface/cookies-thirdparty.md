---
description: Erfahren Sie, inwiefern die Unterstützung für Drittanbieter-Cookies in Browsern immer mehr eingeschränkt wird.
keywords: Cookies;Datenschutz
solution: Experience Cloud,Analytics,Target
title: 'Auswirkungen der geänderten Unterstützung von Drittanbieter-Cookies auf Kunden '
uuid: 27332e0d-6932-4a6e-b97b-0adeced0b050
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 3d12a1b1-c952-4b42-815d-f64b31429cec
source-git-commit: ae14748aa7b0f0d803d48fe980a6743f53d996ab
workflow-type: ht
source-wordcount: '265'
ht-degree: 100%

---

# Auswirkungen der geänderten Unterstützung von Drittanbieter-Cookies auf Kunden {#how-changes-to-third-party-cookie-support-impacts-customers}

Der Support für Drittanbieter-Cookies wurde Browser-übergreifend stärker eingeschränkt. Daher hat Adobe an neuen Programmen gearbeitet, die die Kundenanforderungen sorgfältig mit dem Recht der Verbraucher auf Datenschutz in allen Experience Cloud-Programmen in Einklang bringen.

In der folgenden Liste wird erläutert, wie sich der Support von Drittanbieter-Cookies auf aktuelle Implementierungen von Adobe Experience Cloud-Anwendungen auswirkt:

## Adobe Analytics und Adobe Target

* Analytics und Target sind größtenteils nicht betroffen, da dieselbe Website-Aktivität nur auf First-Party-Cookies angewiesen ist. Zum domainübergreifenden Nachvollziehen der Benutzeraktivität sind Drittanbieter-Cookies erforderlich. Bei Browsern, in denen Cookies von Drittanbietern blockiert sind, ist ein domainübergreifendes Tracking mit Cookies nicht möglich.

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
   * Adobe arbeitet intern und mit seinen Werbepartnern zusammen, um die vollständigen Auswirkungen auf das Senden von Werbeanzeigen zu bewerten.
