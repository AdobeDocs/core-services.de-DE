---
description: 'Audience Manager nutzt einige einfache Cookies für verschiedene Funktionen. Hierzu zählt Folgendes: Das Zuweisen von IDs, das Aufzeichnen von Datenaufrufen, das Nachverfolgen von Fehlern sowie das Durchführen von Tests. (Mit diesen Tests wird ermittelt, ob Cookies gesetzt werden können.) Im vorliegenden Abschnitt werden die verschiedenen von Audience Manager gesetzten Cookies aufgeführt und beschrieben.'
keywords: Cookies
seo-description: 'Audience Manager nutzt einige einfache Cookies für verschiedene Funktionen. Hierzu zählt Folgendes: Das Zuweisen von IDs, das Aufzeichnen von Datenaufrufen, das Nachverfolgen von Fehlern sowie das Durchführen von Tests. (Mit diesen Tests wird ermittelt, ob Cookies gesetzt werden können.) Im vorliegenden Abschnitt werden die verschiedenen von Audience Manager gesetzten Cookies aufgeführt und beschrieben.'
seo-title: Cookies in Audience Manager
solution: Marketing Cloud, Audience Manager
title: Cookies in Audience Manager
uuid: 8 b 384 c 38-b 85 a -4 e 93-b 00 e -41 a 9 d 3 ae 2 b 21
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 426c1fecf16e1cf83cd28971e4de6fdb66b0e10d

---


# Cookies in Audience Manager{#audience-manager-cookies}

Audience Manager nutzt einige einfache Cookies für verschiedene Funktionen. Hierzu zählt Folgendes: Das Zuweisen von IDs, das Aufzeichnen von Datenaufrufen, das Nachverfolgen von Fehlern sowie das Durchführen von Tests. (Mit diesen Tests wird ermittelt, ob Cookies gesetzt werden können.) Im vorliegenden Abschnitt werden die verschiedenen von Audience Manager gesetzten Cookies aufgeführt und beschrieben.

Inhalt:

<ul class="simplelist"> 
 <li> <a href="../cookies-overview/cookies-am.md#section-089407f3e2fe4f489b97164df3cd036c" format="dita" scope="local"> demdex-Cookie </a> </li> 
 <li> <a href="../cookies-overview/cookies-am.md#section-a71050d788d54350adc6b3f6ebf32398" format="dita" scope="local"> dextp-Cookie </a> </li> 
 <li> <a href="../cookies-overview/cookies-am.md#section-670ae9e671874576b528b46e8a1d24ac" format="dita" scope="local"> dstjs-Cookie </a> </li> 
 <li> <a href="../cookies-overview/cookies-am.md#section-0d1fea09c83249dfa944cc028a8ef840" format="dita" scope="local"> _dp-Cookie </a> </li> 
</ul>

## demdex-Cookie {#section-089407f3e2fe4f489b97164df3cd036c}

<table id="table_1CCF7EA2BC9E421F8DEECA5F611E33F6"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Zielsetzung</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager</span> setzt dieses Cookie, um Websitebesuchern eine individuelle ID zuzuweisen. Das <span class="wintitle">demdex</span>-Cookie hilft <span class="keyword">Audience Manager</span> bei der Ausführung grundlegender Funktionen wie Besucheridentifikation, ID-Synchronisierung, Segmentierung, Modellierung, Berichterstellung usw. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Inhalt</b> </p> </td> 
   <td colname="col2"> <p>Das <span class="wintitle">demdex</span>-Cookie umfasst eine Unique User-ID (UUID), wie im unten stehenden Beispiel zu sehen ist: </p> <p> <span class="codeph"> 06151304227769720433039235178204449977 </span> </p> <p>Weitere Informationen finden Sie unter <a href="https://marketing.adobe.com/resources/help/en_US/aam/ids-in-aam.html" format="https" scope="external">Index of IDs in Audience Manager </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Weitere Attribute</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_11291DA87C5045E880034E06C863BCDA"> 
      <li id="li_40C30A06A12449A4A8748621223CA71B">Lebensdauer: Das <span class="wintitle">demdex</span>-Cookie verfügt über eine Gültigkeitsdauer (TTL-Intervall) von 180 Tagen. Das TTL-Intervall wird bei jeder Benutzerinteraktion mit einer Partnerwebsite auf 180 Tage zurückgesetzt. Das Cookie läuft ab, wenn ein Benutzer innerhalb des TTL-Intervalls Ihre Site nicht erneut aufruft. </li> 
      <li id="li_A589EDA2198249829207A183872EF1FF">Opt-out-Möglichkeit: <span class="keyword">Audience Manager</span> setzt das Cookie mit einer <span class="codeph">Do Not Target</span>-Zeichenfolge zurück, wenn ein Benutzer sich gegen die Erfassung von Daten ausgesprochen hat. In diesem Fall ist das TTL-Intervall für das Cookie auf 10 Jahre festgelegt. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

## dextp-Cookie {#section-a71050d788d54350adc6b3f6ebf32398}

<table id="table_7343C9C9ADD24D3FA693ECC76E4A4045"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Zielsetzung</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager</span> setzt dieses Cookie, um den Zeitpunkt des letzten Aufrufs zur Datensynchronisierung aufzuzeichnen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Inhalt</b> </p> </td> 
   <td colname="col2"> <p>Das <span class="wintitle">dextp</span>-Cookie umfasst einen Datenanbieternamen bzw. eine Datenanbieter-ID sowie einen UNIX-UTC-Zeitstempel. Der Zeitstempel ist als mit senkrechtem Strich (Pipe) getrennte Zeichenfolge formatiert. In den Beispielen stehen die <i>kursiv</i> dargestellten Inhalte für Variablenplatzhalter. </p> <p> 
     <ul id="ul_80D0BC3FCF06470991E12712401D784A"> 
      <li id="li_03747A433CEB4756A26CD866E716B89D">Alter Stil: <span class="codeph"> <span class="varname"> Name des Datenanbieters hier </span>-1490307822097| <span class="varname"> Name des Datenanbieters hier </span>-1490307822038 </span> </li> 
      <li id="li_79E7000E82DB4ADA9E9887B017343B2D">Neuer Stil: <span class="codeph">21-1-1490307821616|544-1-1490307821793|3-1-1490307821852|420-1-1490307822038| </span> </li> 
     </ul> </p> <p>Sehen Sie sich auch den unten stehenden Abschnitt zur Datensyntax des dextp-Cookies an. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Weitere Attribute</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_4922AC2CD55D4C888A6FBEB22F8B889B"> 
      <li id="li_91A68C44E53840379C2ACDED25468735">Lebensdauer: Das <span class="wintitle">dextp</span>-Cookie verfügt über eine Gültigkeitsdauer (TTL-Intervall) von 180 Tagen. </li> 
      <li id="li_6B8C674EFAAC4DABA0A640CF29247F99">Opt-out-Möglichkeit: <span class="keyword">Audience Manager</span> setzt das Cookie mit einer <span class="codeph">Do Not Target</span>-Zeichenfolge zurück, wenn ein Benutzer sich gegen die Erfassung von Daten ausgesprochen hat. In diesem Fall ist das TTL-Intervall für das Cookie auf 10 Jahre festgelegt. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Datensyntax des dextp-Cookies**

In der folgenden Tabelle werden die in einem [!DNL dextp]-Cookie enthaltenen Elemente anhand ihrer Position in der Datenzeichenfolge aufgeführt und definiert.

<table id="table_BE00604B97F24F5A94AA4F566063D785"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Position der Variablen </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Erste oder zweite Position</b> </p> </td> 
   <td colname="col2"> <p>Die Position des Namens bzw. der ID des Datenanbieters variiert. Dies hängt davon ab, welche Formatierung das Cookie verwendet (Formatierung im neuen oder alten Stil). </p> <p> <b>Formatierung im alten Stil:</b> </p> <p> 
     <ul id="ul_5BFBF40E3FE849CA859030F2D070FDF6"> 
      <li id="li_E8F4DC0CB15B472ABE9892B3A61D7F77">Syntax: <span class="codeph"> <span class="varname"> Name des Datenanbieters </span> - <span class="varname"> UNIX UTC-Zeitstempel </span></span> </li> 
      <li id="li_7CD8B101156140F49EA97B18E9591402">Example: <span class="codeph"> dataProvider1 - 1490307822038 </span> </li> 
     </ul> </p> <p>In dem im alten Stil formatierten Cookie wird der Datenanbieter mit einem lesbaren Namen identifiziert. </p> <p> <b>Formatierung im neuen Stil:</b> </p> <p> 
     <ul id="ul_AC6225CA781746148C125F21DFED1ED9"> 
      <li id="li_29C4B52E398B4EA28944980A15B05A57">Syntax: <span class="codeph"> <span class="varname"> Datenanbieter-ID </span> -1|2 - <span class="varname"> UNIX UTC Timestamp </span></span> </li> 
      <li id="li_3BF30CA5FED242DF96E0B54AFC64B06F">Beispiel: <span class="codeph"> 123345 - 1 - 1490307822038 </span> </li> 
     </ul> </p> <p>Im neuen Stil formatiertes Cookie: </p> <p> 
     <ul id="ul_F05A91A455FA44C7A71186C0C9E31630"> 
      <li id="li_A8C9638173684359BABC4207845A4F48">Der lesbare Name des Datenanbieters wird durch eine numerische ID ersetzt. </li> 
      <li id="li_28F1E2DB24904E53BE9718AD788CE61E">Der Aufruftyp wird mit ID 1 oder ID 2 identifiziert. ID 1 steht für einen Aufruf zur Datensynchronisierung. ID 2 steht für einen veralteten Aufruf, der nicht mehr verwendet wird. Sie sollten nicht viele (oder gar keine) dextp-Cookies mit ID 2 erhalten. </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Letztes</b> </p> </td> 
   <td colname="col2"> <p>An letzter Position befindet sich ein UNIX-UTC-Zeitstempel. </p> </td> 
  </tr> 
 </tbody> 
</table>

## dst-Cookie {#section-670ae9e671874576b528b46e8a1d24ac}

<table id="table_83AE9B6350C6408BAECD9FCF33022B98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <b>Zielsetzung</b> </p> </td> 
   <td colname="col2"> <p> <span class="keyword"> Audience Manager</span> setzt dieses Cookie, wenn bei der Übermittlung von Daten an ein <a href="https://marketing.adobe.com/resources/help/en_US/aam/c_destinations.html" format="https" scope="external">Ziel</a> ein Fehler auftritt . </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Inhalt</b> </p> </td> 
   <td colname="col2"> <p> Das <span class="wintitle">DST</span>-Cookie umfasst Sätze von Ziel-IDs und UNIX-Zeitstempeln, die als mit senkrechtem Strich (Pipe) getrennte Zeichenfolgen formatiert sind. In den Beispielen stehen die <i>kursiv</i> dargestellten Inhalte für Variablenplatzhalter. </p> <p> 
     <ul id="ul_CE98076A02DA413486C1D341E9806889"> 
      <li id="li_850209D956644749B98C7A208C825C15">Syntax: <span class="codeph"><span class="varname"> Ziel-ID </span> - <span class="varname"> UNIX UTC-Zeitstempel </span></span> </li> 
      <li id="li_4A22152C70844733982230EBF7B9EB78">Beispiel: <span class="codeph">067797-1490349684|1010788-1490349692|1067797-1490349692 </span> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>Weitere Attribute</b> </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_5D13DD701B484B51BF2808A69A919106"> 
      <li id="li_4E665114C63246FBA32A4E19984D2693">Lebensdauer: Das <span class="wintitle">dst</span>-Cookie verfügt über eine Gültigkeitsdauer (TTL-Intervall) von 180 Tagen. </li> 
      <li id="li_A682B566704F43D2AB72487EFF212474">Opt-out-Möglichkeit: <span class="keyword">Audience Manager</span> setzt das Cookie mit einer <span class="codeph">Do Not Target</span>-Zeichenfolge zurück, wenn ein Benutzer sich gegen die Erfassung von Daten ausgesprochen hat. </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

## _dp-Cookie {#section-0d1fea09c83249dfa944cc028a8ef840}

Dies ist ein temporäres Cookie. [!DNL Audience Manager] versucht, das [!DNL _dp] Cookie festzulegen, um festzustellen, ob andere Cookies in der demdex. net-Domäne in einem Drittanbieterkontext gesetzt werden können. When [!DNL _dp] is set it contains a value of 1. [!DNL Audience Manager] liest diesen Wert und entfernt den Cookie sofort. If the [!DNL _dp] cookie is not present, [!DNL Audience Manager] knows it cannot set cookies.

>[!MORE_LIKE_THIS]
>
>* [Aufrufe an die Domäne „demdex.net“ ](https://marketing.adobe.com/resources/help/en_US/aam/demdex-calls.html)
>* [Adobe Datenschutzcenter](http://www.adobe.com/privacy.html)
>* [Audience Manager – Datensicherheit und Datenschutz](https://marketing.adobe.com/resources/help/en_US/aam/c_data_security_and_privacy.html)
>* [Audience Manager – Datenschutz und Data Retention FAQ](https://marketing.adobe.com/resources/help/en_US/aam/faq_privacy.html)

