---
description: Hier erfahren Sie mehr über Audience Manager-Cookies in Adobe Experience Cloud.
keywords: 'Cookies in '
solution: Experience Cloud, Audience Manager
title: 'Cookies in Audience Manager '
uuid: 8b384c38-b85a-4e93-b00e-41a9d3ae2b21
feature: Cookies
topic: Administration
role: Administrator
level: Erfahren
translation-type: ht
source-git-commit: 61d60273e933c637dfe4400da78257e1c80015b3
workflow-type: ht
source-wordcount: '613'
ht-degree: 100%

---


# Cookies in Audience Manager {#audience-manager-cookies}

Audience Manager vertraut bei der Ausführung verschiedener Funktionen auf ein einige einfache Cookies. Dazu gehören die Zuweisung von IDs, die Aufzeichnung von Datenaufrufen, die Fehlerverfolgung und Tests, um zu prüfen, ob Cookies gesetzt werden können. In diesem Abschnitt werden die verschiedenen Cookies aufgelistet und beschrieben, die von Audience Manager gesetzt werden.

**demdex-Cookie**

<table id="table_1CCF7EA2BC9E421F8DEECA5F611E33F6"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Zweck</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager</span> setzt dieses Cookie, um Site-Besuchern eine eindeutige ID zuzuweisen. Das <span class="wintitle">demdex</span>-Cookie hilft <span class="keyword">Audience Manager</span> bei der Ausführung grundlegender Funktionen wie Besucheridentifikation, ID-Synchronisierung, Segmentierung, Modellierung, Berichterstellung usw. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Inhalt</b> </p> </td> 
   <td colname="col2"> <p>Das <span class="wintitle">demdex</span>-Cookie umfasst eine eindeutige Benutzer-ID (UUID), wie im unten stehenden Beispiel zu sehen ist: </p> <p> <span class="codeph"> 06151304227769720433039235178204449977 </span> </p> <p>Weitere Informationen finden Sie unter <a href="https://docs.adobe.com/content/help/de-DE/audience-manager/user-guide/reference/ids-in-aam.html" format="https" scope="external">Index of IDs in Audience Manager</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Weitere Attribute</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_11291DA87C5045E880034E06C863BCDA"> 
      <li id="li_40C30A06A12449A4A8748621223CA71B">Lebensdauer: Das <span class="wintitle">demdex</span>-Cookie verfügt über eine Gültigkeitsdauer (TTL-Intervall) von 180 Tagen. Der TTL-Wert wird bei jeder Benutzerinteraktion mit einer Partner-Website auf 180 Tage zurückgesetzt. Das Cookie läuft ab, wenn ein Benutzer nicht innerhalb des TTL-Intervalls zu Ihrer Site zurückkehrt. </li> 
      <li id="li_A589EDA2198249829207A183872EF1FF">Abwahl: <span class="keyword">Audience Manager</span> setzt das Cookie mit einer <span class="codeph">Do Not Adobe Target</span>-Zeichenfolge zurück, wenn ein Benutzer die Datenerfassung abwählt. In diesem Fall ist das TTL-Intervall für das Cookie auf 10 Jahre festgelegt. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

**dextp-Cookie**

<table id="table_7343C9C9ADD24D3FA693ECC76E4A4045"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Zweck</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager</span> setzt dieses Cookie, um den Zeitpunkt des letzten Aufrufs zur Datensynchronisierung aufzuzeichnen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Inhalt</b> </p> </td> 
   <td colname="col2"> <p>Das <span class="wintitle">dextp</span>-Cookie umfasst einen Datenanbieternamen bzw. eine Datenanbieter-ID sowie einen UNIX-UTC-Zeitstempel. Der Zeitstempel ist als mit senkrechtem Strich (Pipe) getrennte Zeichenfolge formatiert. In den Beispielen stehen die <i>kursiv</i> dargestellten Inhalte für Variablenplatzhalter. </p> <p> 
     <ul id="ul_80D0BC3FCF06470991E12712401D784A"> 
      <li id="li_03747A433CEB4756A26CD866E716B89D">Alter Stil: <span class="codeph"> <span class="varname"> Name des Datenanbieters hier </span>-1490307822097| <span class="varname"> Name des Datenanbieters hier </span>-1490307822038 </span> </li> 
      <li id="li_79E7000E82DB4ADA9E9887B017343B2D">Neuer Stil: <span class="codeph">21-1-1490307821616|544-1-1490307821793|3-1-1490307821852|420-1-1490307822038| </span> </li> 
     </ul> </p> <p>Siehe auch den Abschnitt unten zur Syntax von dextp-Daten. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Weitere Attribute</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_4922AC2CD55D4C888A6FBEB22F8B889B"> 
      <li id="li_91A68C44E53840379C2ACDED25468735">Lebensdauer: Das <span class="wintitle">dextp</span>-Cookie verfügt über eine Gültigkeitsdauer (TTL-Intervall) von 180 Tagen. </li> 
      <li id="li_6B8C674EFAAC4DABA0A640CF29247F99">Abwahl: <span class="keyword">Audience Manager</span> setzt das Cookie mit einer <span class="codeph">Do Not Adobe Target</span>-Zeichenfolge zurück, wenn ein Benutzer die Datenerfassung abwählt. In diesem Fall ist das TTL-Intervall für das Cookie auf 10 Jahre festgelegt. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

Datensyntax des dextp-Cookies:

In der folgenden Tabelle werden die in einem [!DNL dextp]-Cookie enthaltenen Elemente anhand ihrer Position in der Datenzeichenfolge aufgeführt und definiert.

<table id="table_BE00604B97F24F5A94AA4F566063D785"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Variablenposition </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Erste oder zweite</b> </p> </td> 
   <td colname="col2"> <p>Die Position des Namens oder der ID des Datenanbieters hängt davon ab, ob das Cookie die Formatierung im alten oder neuen Stil verwendet. </p> <p> <b>Formatierung im alten Stil:</b> </p> <p> 
     <ul id="ul_5BFBF40E3FE849CA859030F2D070FDF6"> 
      <li id="li_E8F4DC0CB15B472ABE9892B3A61D7F77">Syntax: <span class="codeph"> <span class="varname"> Name des Datenanbieters</span> - <span class="varname"> UNIX UTC-Zeitstempel </span> </span> </li> 
      <li id="li_7CD8B101156140F49EA97B18E9591402">Beispiel: <span class="codeph">dataProvider1 – 1490307822038 </span> </li> 
     </ul> </p> <p>Das Cookie im alten Stil identifiziert den Datenanbieter mit einem lesbaren Namen. </p> <p> <b>Formatierung im neuen Stil:</b> </p> <p> 
     <ul id="ul_AC6225CA781746148C125F21DFED1ED9"> 
      <li id="li_29C4B52E398B4EA28944980A15B05A57">Syntax: <span class="codeph"> <span class="varname"> ID des Datenanbieters </span> - 1|2 - <span class="varname"> UNIX UTC-Zeitstempel </span> </span> </li> 
      <li id="li_3BF30CA5FED242DF96E0B54AFC64B06F">Beispiel: <span class="codeph"> 123345 - 1 - 1490307822038 </span> </li> 
     </ul> </p> <p>Das Cookie im neuen Stil: </p> <p> 
     <ul id="ul_F05A91A455FA44C7A71186C0C9E31630"> 
      <li id="li_A8C9638173684359BABC4207845A4F48">Ersetzt den lesbaren Namen des Datenanbieters durch eine numerische ID. </li> 
      <li id="li_28F1E2DB24904E53BE9718AD788CE61E">Identifiziert den Aufruftyp mit ID 1 oder ID 2. ID 1 steht für einen ID-Synchronisierungsaufruf. ID 2 steht für einen nicht mehr unterstützten Aufruf, der nicht mehr verwendet wird. Es sollten nicht viele (bzw. keine) dextp-Cookies mit ID 2 angezeigt werden. </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Letzte</b> </p> </td> 
   <td colname="col2"> <p>Die letzte Position enthält einen UNIX UTC-Zeitstempel. </p> </td> 
  </tr> 
 </tbody> 
</table>

**dst-Cookie**

<table id="table_83AE9B6350C6408BAECD9FCF33022B98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Zweck</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager</span> setzt dieses Cookie, wenn bei der Übermittlung von Daten an ein <a href="https://docs.adobe.com/content/help/de-DE/audience-manager/user-guide/features/destinations/destinations.html#purposes" format="https" scope="external">Ziel</a> ein Fehler auftritt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Inhalt</b> </p> </td> 
   <td colname="col2"> <p> Das <span class="wintitle">DST</span>-Cookie umfasst Sätze von Ziel-IDs und UNIX-Zeitstempeln, die als mit senkrechtem Strich (Pipe) getrennte Zeichenfolgen formatiert sind. In den Beispielen stehen die <i>kursiv</i> dargestellten Inhalte für Variablenplatzhalter. </p> <p> 
     <ul id="ul_CE98076A02DA413486C1D341E9806889"> 
      <li id="li_850209D956644749B98C7A208C825C15">Syntax: <span class="codeph"> <span class="varname"> Ziel-ID </span> - <span class="varname"> UNIX-UTC-Zeitstempel </span> </span> </li> 
      <li id="li_4A22152C70844733982230EBF7B9EB78">Beispiel: <span class="codeph">067797-1490349684|1010788-1490349692|1067797-1490349692 </span> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Weitere Attribute</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_5D13DD701B484B51BF2808A69A919106"> 
      <li id="li_4E665114C63246FBA32A4E19984D2693">Lebensdauer: Das <span class="wintitle">dst</span>-Cookie verfügt über eine Gültigkeitsdauer (TTL-Intervall) von 180 Tagen. </li> 
      <li id="li_A682B566704F43D2AB72487EFF212474">Abwahl: <span class="keyword">Audience Manager</span> setzt das Cookie mit einer <span class="codeph">Do Not Adobe Target</span>-Zeichenfolge zurück, wenn ein Benutzer die Datenerfassung abwählt. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

**_dp-Cookie**

Dies ist ein temporäres Cookie. [!DNL Audience Manager] versucht, das [!DNL _dp]-Cookie zu setzen, um zu ermitteln, ob in der Domäne „demdex.net“ andere Cookies in einem Drittanbieter-Kontext gesetzt werden können. Wenn [!DNL _dp] gesetzt ist, enthält es den Wert 1. [!DNL Audience Manager] liest diesen Wert und entfernt das Cookie dann sofort. Wenn das [!DNL _dp]-Cookie nicht vorhanden ist, weiß [!DNL Audience Manager], dass keinerlei Cookies gesetzt werden können.