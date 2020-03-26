---
description: Scene7 verwendet Cookies, um nützliche Informationen zu speichern, die zur Bereitstellung dynamischer Medien an den Browser genutzt werden können.
keywords: cookies;privacy
seo-description: Scene7 verwendet Cookies, um nützliche Informationen zu speichern, die zur Bereitstellung dynamischer Medien an den Browser genutzt werden können.
seo-title: Cookies in Scene7
solution: Marketing Cloud,Analytics,Adobe Target,Adobe Social
title: Cookies in Scene7
uuid: f9b9d13a-17e5-4139-8c84-6fe5d22c4196
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Cookies in Scene7{#scene-cookies}

Scene7 verwendet Cookies, um nützliche Informationen zu speichern, die zur Bereitstellung dynamischer Medien an den Browser genutzt werden können.

Scene7 speichert Informationen für einige ältere AS2 Flash-basierte Viewer lokal.

Für AS2-Viewer Cookies:

* Verfolgen Sie den Sitzungsstatus eines Benutzers, z. B. die aktuelle angezeigte Seite und das angezeigte Bild, den aktuellen Zoomgrad usw.
* Bestimmen Sie, wie lange es seit der vorherigen Sitzung des Benutzers ist. Der Viewer verwendet diese Informationen, um zu entscheiden, ob eine vorherige Sitzung oder eine neue Beginn-Sitzung fortgesetzt werden soll. Diese Informationen werden auch an die Scene7-Server gesendet, jedoch nicht verwendet.

Für AS2 Flash-E-Katalog-Viewer Cookies:

* Cookies speichern benutzergenerierte Inhalte (in erster Linie Inhalte, die vom Benutzer im E-Katalog-Viewer in der „Klebezettel“-Funktion eingegeben werden). Dieser Inhalt wird wiederhergestellt, wenn der Benutzer eine Sitzung wiederaufnimmt.
* Wenn der Benutzer eine E-Mail zum Freigeben des E-Mail-Katalogs für einen anderen Benutzer aufruft, wird der Inhalt der Klebezettel des zweiten AS2-Viewers auf unsere Server kopiert, um ihn dem Empfänger bereitzustellen. Wenn der Empfänger die Viewer-Sitzung initiiert, wird der Inhalt der Klebezettel vom Server abgerufen und in ein Cookie kopiert. Diese Funktion wird nur wenig genutzt, sodass sie nicht abläuft und statische Inhalte nicht entfernt werden. Zu diesem Zeitpunkt bleibt es auf den Servern unbegrenzt.

Die neueren AS3-Viewer implementieren keine Sitzungspersistenz.

**Cookie-Name: VatLogin.jsp**

| Attribut | Beschreibung |
|---|---|
| Gespeicherte Informationen | Stellt das Sitzungs-Cookie ein. Der in IPS ImageServer eingebettete AuthFilter (IS, IR und auch die SWFs/Skins und Videokontexte) verwendet das Cookie zur Zugriffsautorisierung. Sofern vorhanden, gestattet es den Durchlauf von HTTP-Anforderungen. Andernfalls werden nicht autorisierte Daten zurückgegeben. |
| Ablauf | Dieses Cookie ist ein Sitzungs-Cookie. Derzeit ist der Sitzungsablaufzeitraum in der [!DNL web.xml] der Scene7-IPS auf 45 Minuten eingestellt. |

**Cookie-Name: s7js.flyout.InfoMessage.displayed`assetId`.state**

<table id="table_6835D64C5D464A049F576621F2BE3FAD"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Gespeicherte Informationen </td> 
   <td colname="col2"> <p>&lt;assetId&gt; ist der Name des Assets, mit dem der Viewer arbeitet. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Ablauf </td> 
   <td colname="col2"> Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird. </td> 
  </tr> 
 </tbody> 
</table>

**Cookie-Name: s7js.flyout.InfoMessage.displayed`assetId`_idx`id`.ant**

Browser-Cookies werden von älteren DHTML-Viewern zum Speichern von Statusinformationen und Anmerkungsdaten verwendet. Sie werden auch vom Multiscreen DHTML Flyout verwendet, um die Meldungsanzeige sitzungsspezifisch zu machen.

<table id="table_8F6CC83D32D54BEE99884318AD126C98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Attribut </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Gespeicherte Informationen </td> 
   <td colname="col2"> <p> </p> <p> &lt;assetId&gt; ist der Name des Assets, mit dem der Viewer arbeitet, und &lt;id&gt; ist der 0-basierte Anmerkungsindex. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Ablauf </td> 
   <td colname="col2"> Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird. </td> 
  </tr> 
 </tbody> 
</table>

