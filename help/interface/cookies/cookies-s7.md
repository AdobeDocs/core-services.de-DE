---
description: Einsatz von Cookies durch Adobe Scene7 zum Speichern hilfreicher Informationen, die zur Bereitstellung von Dynamic Media an den Browser verwendet werden können.
keywords: cookies;privacy
solution: Experience Cloud,Analytics,Target
title: 'Cookies in Scene7 '
uuid: f9b9d13a-17e5-4139-8c84-6fe5d22c4196
translation-type: tm+mt
source-git-commit: 3f26c1af19a0838913eec2b4135304f5f3fcf0b4
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 100%

---


# Cookies in Scene7 {#scene-cookies}

Scene7 verwendet Cookies, um nützliche Informationen zu speichern, die zur Bereitstellung dynamischer Medien an den Browser genutzt werden können.

Scene7 speichert Informationen für einige ältere AS2 Flash-basierte Viewer lokal.

Für AS2-Viewer, -Cookies:

* Verfolgen Sie den Sitzungsstatus eines Benutzers, z. B. die aktuelle Seite und das angezeigte Bild, den aktuellen Zoomfaktor usw.
* Bestimmen Sie, wie viel Zeit seit der vorherigen Sitzung des Benutzers vergangen ist. Der Viewer verwendet diese Informationen, um zu entscheiden, ob eine vorherige Sitzung fortgesetzt oder eine neue Sitzung gestartet werden soll. Diese Informationen werden auch an die Scene7-Server gesendet, jedoch nicht verwendet.

Für AS2 Flash eCatalog-Viewer, -Cookies:

* Cookies speichern benutzergenerierte Inhalte (in erster Linie Inhalte, die vom Benutzer im E-Katalog-Viewer in der „Kurznotiz“-Funktion eingegeben werden). Dieser Inhalt wird wiederhergestellt, wenn der Benutzer eine Sitzung wieder aufnimmt.
* Wenn der Benutzer eine E-Mail zur eCatalog-Freigabe für einen anderen Benutzer initiiert, wird der Inhalt der Kurznotizen des zweiten AS2-Viewers auf unsere Server kopiert, um ihn dem Empfänger bereitzustellen. Wenn der Empfänger die Viewer-Sitzung initiiert, wird der Inhalt der Kurznotizen vom Server abgerufen und in ein Cookie kopiert. Diese Funktion wird nur wenig genutzt, sodass sie nicht abläuft und alte Inhalte nicht entfernt werden. Derzeit bleiben sie auf den Servern auf unbestimmte Zeit gespeichert.

Die neueren AS3-Viewer implementieren keine Sitzungspersistenz.

**Cookie-Name: VatLogin.jsp**

| Attribut | Beschreibung |
|---|---|
| Gespeicherte Informationen | Stellt das Sitzungs-Cookie ein. Der in IPS ImageServer eingebettete AuthFilter (IS, IR und auch die SWFs/Skins und Videokontexte) verwendet das Cookie zur Zugriffsautorisierung. Sofern vorhanden, gestattet es den Durchlauf von HTTP-Anforderungen. Andernfalls werden nicht autorisierte Daten zurückgegeben. |
| Ablauf | Dieses Cookie ist ein Sitzungs-Cookie. Derzeit ist der Sitzungsablaufzeitraum in der [!DNL web.xml] der Scene7-IPS auf 45 Minuten eingestellt. |

**Cookie-Name: s7js.flyout.InfoMessage.displayed `assetId`.state**

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

Browser-Cookies werden von älteren DHTML-Viewern zum Speichern von Statusinformationen und Daten von Kurznotizen verwendet. Sie werden auch vom Multiscreen DHTML Flyout verwendet, um die Meldungsanzeige sitzungsspezifisch zu machen.

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
   <td colname="col2"> <p> </p> <p> &lt;assetId&gt; ist der Name des Assets, mit dem der Viewer arbeitet und &lt;id&gt; ist der 0-basierte Index der Kurznotiz. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Ablauf </td> 
   <td colname="col2"> Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird. </td> 
  </tr> 
 </tbody> 
</table>

