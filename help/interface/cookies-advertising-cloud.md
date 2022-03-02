---
description: Hier erfahren Sie mehr über Adobe Ad Cloud-Cookies für das Zuordnen von Werbeinteraktions-Ereignissen zu Konversionsereignissen und möglicherweise zum Verwenden dieser Informationen zur Optimierung von Anzeigenangeboten.
title: 'Cookies in Advertising Cloud  '
uuid: 2eec48a3-3e81-488e-8e30-5fd62885de0b
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 6818edea-31b1-49fc-bca2-32828c7ca78d
source-git-commit: 854a2b298db4fab3339e2b2ea03701dc6511af8d
workflow-type: ht
source-wordcount: '569'
ht-degree: 100%

---

# Cookies in Advertising Cloud {#advertising-cloud-cookies}

Advertising Cloud verwendet Cookies, um Ereignisse von Anzeigeninteraktionen Konversionsereignissen zuzuordnen und diese Informationen ggf. zur Optimierung der Anzeigengebote zu verwenden.

>[!NOTE]
>
>Das JavaScript-Tag der Beta-Advertising-Cloud, das den [Adobe Experience Cloud ID (ECID) Service](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=de) verwendet, erstellt [Erstanbieter-Experience Cloud-s_ecid-Cookies](cookies-first-party.md) und nicht Advertising-Cloud-Cookies.

## Cookie-Name: _lcc

<table id="table_821F8EBE91F244CBA72B0975B961B908"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gespeicherte Informationen </p> </td> 
   <td colname="col2"> <p>IDs und Zeitstempel (im Format JJJJMMTT) von Anzeigenklicks</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Ablauf </p> </td> 
   <td colname="col2"> <p>15 Minuten</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Nutzung </p> </td> 
   <td colname="col2"> <p>Ein Drittanbieter-Cookie, mit dem festgestellt wird, ob ein Klick-Ereignis auf einer Display-Anzeige als Adobe Analytics-Treffer gewertet werden soll </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Position </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Größe </p> </td> 
   <td colname="col2"> <p>52 Byte </p> </td> 
  </tr> 
 </tbody> 
</table>

## Cookie-Name: _tmae

<table id="table_28C2B62595E240D5A3C3E0BE147748C1"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gespeicherte Informationen </p> </td> 
   <td colname="col2"> <p>Kodierte IDs und Zeitstempel für Anzeigeninteraktionen mit Advertising Cloud DSP-Tracking </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Ablauf </p> </td> 
   <td colname="col2"> <p>1 Jahr </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Nutzung </p> </td> 
   <td colname="col2"> <p>Ein Drittanbieter-Cookie, das Benutzerinteraktionen mit Anzeigen speichert, z. B. „Anzeige xyz123 wurde zuletzt am 30. Juni 2016 angesehen“ </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Position </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Größe </p> </td> 
   <td colname="col2"> <p>Variable; Daten sind kodiert und haben normalerweise weniger als 1 KB </p> </td> 
  </tr> 
 </tbody> 
</table>

## Cookie-Name: adcloud

<table id="table_D7CD238736BC4571883F92F47673F57C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gespeicherte Informationen </p> </td> 
   <td colname="col2"> <p>Die Zeitstempel des letzten Besuchs auf der Website des Werbetreibenden und der letzte Suchklick des Surfers sowie die ef_id, die erstellt wurde, als der Benutzer auf eine Anzeige geklickt hat</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Ablauf </p> </td> 
   <td colname="col2"> <p>Cookies, die am 24. Februar 2021 oder früher gesetzt wurden, laufen nach 730 Tagen ab. Cookies, die am 25. Februar 2021 oder später gesetzt werden, laufen nach 364 Tagen ab.</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Nutzung </p> </td> 
   <td colname="col2"> <p>Ein Erstanbieter-Cookie, das die Surfer-ID mit relevanten Zielgruppensegmenten und Konversionen verknüpft </p> <p> Informationen zum letzten Besuch werden zur Optimierung der Seitenladezeiten verwendet, indem unnötige Aufrufe von Adobe-Servern verhindert werden. </p> <p>Informationen zum letzten Suchklick helfen dabei festzustellen, ob ein Konversionsereignis durch einen Klick oder ein Viewthrough zustande gekommen ist (Konversion durch Impressionen, aber keine Klicks). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Position </p> </td> 
   <td colname="col2"> <p>Die oberste Domänenebene des Werbetreibenden (z. B. beispiel.com) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Größe </p> </td> 
   <td colname="col2"> <p>Variabel, normalerweise aber 50 bis 150 Byte </p> </td> 
  </tr> 
 </tbody> 
</table>

## Cookie-Name: ev_sync_*

(ev_sync_ax, ev_sync_bk, ev_sync_dd, ev_sync_fs, ev_sync_ix, ev_sync_nx, ev_sync_ox, ev_sync_pm, ev_sync_rc, ev_sync_tm, ev_sync_yh)

<table id="table_A05C02AB261946E0AABAD78259392D81"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gespeicherte Informationen </p> </td> 
   <td colname="col2"> <p>Das Datum, an dem die Synchronisierung im Format JJJJMMTT durchgeführt wird </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Ablauf </p> </td> 
   <td colname="col2"> <p>Das Datum, an dem die Synchronisierung im Format JJJJMMTT durchgeführt wird </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Nutzung </p> </td> 
   <td colname="col2"> <p>Ein Drittanbieter-Cookie speziell für Anzeigenbörsen, das die Surfer-ID in Advertising Cloud mit der Partner-Anzeigenbörse synchronisiert. Das Cookie wird für neue Surfer erstellt und sendet eine Synchronisierungsanforderung, wenn es abgelaufen ist. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Position </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Größe </p> </td> 
   <td colname="col2"> <p>8 Zeichen </p> </td> 
  </tr> 
 </tbody> 
</table>

## Cookie-Name: everest_g_v2

<table id="table_04043292A43B41B69EAF17AF4E217C69"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gespeicherte Informationen </p> </td> 
   <td colname="col2"> <p>Browser und Surfer-ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Ablauf </p> </td> 
   <td colname="col2"> <p>2 Jahre </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Nutzung </p> </td> 
   <td colname="col2"> <p>Erstellt, nachdem ein Benutzer anfänglich auf die Anzeige eines Kunden geklickt hat, und verwendet, um die aktuellen und nachfolgenden Klicks anderen Ereignissen auf der Kundenwebsite zuzuordnen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Position </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Größe </p> </td> 
   <td colname="col2"> <p>~27 Zeichen </p> </td> 
  </tr> 
 </tbody> 
</table>

## Cookie-Name: everest_session_v2

<table id="table_1A3AE4CA71304ADB943CB1F64BE695F5"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gespeicherte Informationen </p> </td> 
   <td colname="col2"> <p>Die Sitzungs-ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Ablauf </p> </td> 
   <td colname="col2"> <p>Wenn der Browser geschlossen wird </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Nutzung </p> </td> 
   <td colname="col2"> <p>Ein Drittanbieter-Sitzungs-Cookie; für alle Konten wird ein Cookie verwendet </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Position </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Größe </p> </td> 
   <td colname="col2"> <p>~16 Zeichen </p> </td> 
  </tr> 
 </tbody> 
</table>

## Cookie-Name: ev_tm

<table id="table_6C4D9DCFA4BF4FB2BD445E027550955F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gespeicherte Informationen </p> </td> 
   <td colname="col2"> <p>ID der Advertising Cloud DSP (Demand Side Platform) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Ablauf </p> </td> 
   <td colname="col2"> <p>2 Jahre </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Nutzung </p> </td> 
   <td colname="col2"> <p>Ein Drittanbieter-Cookie, das die DSP-ID speichert, die der Surfer-ID im Cookie everest_g_v2 entspricht </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Position </p> </td> 
   <td colname="col2"> <p>everesttech.net </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Größe </p> </td> 
   <td colname="col2"> <p>~20 Byte </p> </td> 
  </tr> 
 </tbody> 
</table>

## Cookie-Name: id_adcloud

<table> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gespeicherte Informationen </p> </td> 
   <td colname="col2"> <p>Die Surfer-ID </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Ablauf </p> </td> 
   <td colname="col2"> <p>91 Tage </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Nutzung </p> </td> 
   <td colname="col2"> <p>Das Cookie wird in der Erstanbieterdomäne gesetzt, wird aber noch nicht verwendet </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Position </p> </td> 
   <td colname="col2"> <p>Die oberste Domänenebene des Werbetreibenden (z. B. beispiel.com) </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Größe </p> </td> 
   <td colname="col2"> <p>16 Byte </p> </td> 
  </tr> 
 </tbody> 
</table>
