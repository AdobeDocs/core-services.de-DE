---
description: Scene7 verwendet Cookies, um nützliche Informationen zu speichern, die zur Bereitstellung dynamischer Medien an den Browser genutzt werden können.
keywords: Cookies, Datenschutz
seo-description: Scene7 verwendet Cookies, um nützliche Informationen zu speichern, die zur Bereitstellung dynamischer Medien an den Browser genutzt werden können.
seo-title: Cookies in Scene7
solution: Experience Cloud,Analytics,Target,Social
title: Cookies in Scene7
uuid: f9b9d13a-17e5-4139-8c84-6fe5d22c4196
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 7137e608ddece5bf2a3983b3b18909ba89d607a6

---


# Cookies in Scene7{#scene-cookies}

Scene7 verwendet Cookies, um nützliche Informationen zu speichern, die zur Bereitstellung dynamischer Medien an den Browser genutzt werden können.

Scene7 speichert für einige ältere AS2 Flash-basierte Viewer Informationen lokal.

Für AS2-Viewer gilt Folgendes:

* Cookies verfolgen den Sitzungsstatus eines Benutzers, z. B. aktuell angezeigte Seite, aktuell angezeigtes Bild, aktueller Zoomfaktor usw.
* Cookies ermitteln, wie viel Zeit seit der letzten Sitzung des Benutzers vergangen ist. Der Benutzer kann diese Informationen nutzen und sich entscheiden, ob er eine vorherige Sitzung weiterführen oder eine neue Sitzung starten möchte. Die Informationen werden auch an die Scene7-Server gesendet, aber nicht verwendet.

Für E-Katalog-Viewer mit AS2 Flash gilt Folgendes:

* Cookies speichern benutzergenerierte Inhalte (in erster Linie Inhalte, die vom Benutzer im E-Katalog-Viewer in der „Klebezettel“-Funktion eingegeben werden). Diese Inhalte werden wiederhergestellt, wenn der Benutzer eine Sitzung wiederaufnimmt.
* Wenn der Benutzer eine E-Mail initiiert, um den E-Katalog mit einem anderen Benutzer zu teilen, werden die Inhalte der „Klebezettel“-Funktion aus dem zweiten AS2-Viewer-Bullet auf unsere Server kopiert, um sie dem Empfänger bereitzustellen. Wenn der Empfänger die Viewer-Sitzung initiiert, werden die Inhalte aus der „Klebezettel“-Funktion vom Server abgerufen und in ein Cookie kopiert. Diese Funktion wird nur selten verwendet, sodass sie nicht abläuft und veraltete Inhalte nicht entfernt werden. Derzeit bleibt sie auf den Servern zeitlich unbegrenzt bestehen.

Bei den neueren AS3-Viewern wird auf Sitzungspersistenz verzichtet.

**Cookie-Name: VatLogin.jsp**

| Attribut | Beschreibung |
|---|---|
| Gespeicherte Informationen | Stellt das Sitzungs-Cookie ein. Der in IPS ImageServer eingebettete AuthFilter (IS, IR und auch die SWFs/Skins und Videokontexte) verwendet das Cookie zur Zugriffsautorisierung. Sofern vorhanden, gestattet es den Durchlauf von HTTP-Anforderungen. Andernfalls werden Anforderungen als nicht autorisiert zurückgegeben. |
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
   <td colname="col2"> <p>&lt;assetId&gt; ist der Name des Assets, mit dem die Anzeige arbeitet. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Ablauf </td> 
   <td colname="col2"> Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird. </td> 
  </tr> 
 </tbody> 
</table>

**Cookie-Name: s7js.flyout.InfoMessage.displayed`assetId`_idx`id`.ant**

Browser-Cookies werden von älteren DHTML-Anzeigen zur Speicherung von Statusinformationen und Anmerkungsdaten genutzt. Sie werden auch vom Multiscreen-DHTML-Flyout genutzt, um die  Meldungsanzeige sitzungsspezifisch zu machen.

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
   <td colname="col2"> <p> </p> <p> &lt;assetId&gt; ist der Name des Assets, mit dem die Anzeige arbeitet, und &lt;id&gt; ist der 0-basierte Anmerkungsindex. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Ablauf </td> 
   <td colname="col2"> Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird. </td> 
  </tr> 
 </tbody> 
</table>

