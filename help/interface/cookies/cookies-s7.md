---
description: Scene7 verwendet Cookies, um nützliche Informationen zu speichern, die zur Bereitstellung dynamischer Medien an den Browser genutzt werden können.
keywords: Cookies; Datenschutz
seo-description: Scene7 verwendet Cookies, um nützliche Informationen zu speichern, die zur Bereitstellung dynamischer Medien an den Browser genutzt werden können.
seo-title: Cookies in Scene7
solution: Marketing Cloud, Analytics, Target, Social
title: Cookies in Scene7
uuid: f 9 b 9 d 13 a -17 e 5-4139-8 c 84-6 fe 5 d 22 c 4196
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: c24b266eda9aae1e86a58ac473fa339f7eb26efe

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

* [Cookie-Name: VatLogin.jsp](../cookies/cookies-s7.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [Cookie-Name: s 7 js. flyout. infomessage. displayed. state](../cookies/cookies-s7.md#section-14ad50dfcd7342f9ac80283b1f0d3400)
* [Cookie-Name: s 7 js. flyout. infomessage. displayed_ idx. ant](../cookies/cookies-s7.md#section-05d1c52c478541609f4a18a9c1eb032f)

## Cookie-Name: VatLogin.jsp {#section-03aa90aa7e36427b8cb12dc4a0f0291e}

| Attribut | Beschreibung |
|---|---|
| Gespeicherte Informationen | Stellt das Sitzungs-Cookie ein. Der in IPS ImageServer eingebettete AuthFilter (IS, IR und auch die SWFs/Skins und Videokontexte) verwendet das Cookie zur Zugriffsautorisierung. Sofern vorhanden, gestattet es den Durchlauf von HTTP-Anforderungen. Andernfalls werden Anforderungen als nicht autorisiert zurückgegeben. |
| Ablauf | Dieses Cookie ist ein Sitzungs-Cookie. Derzeit ist der Sitzungsablaufzeitraum in der [!DNL web.xml] der Scene7-IPS auf 45 Minuten eingestellt. |

## Cookie-Name: s 7 js. flyout. infomessage. displayed<assetId>.state {#section-14ad50dfcd7342f9ac80283b1f0d3400}

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

## Cookie-Name: s 7 js. flyout. infomessage. displayed<assetId>_ idx<id>. ant {#section-05d1c52c478541609f4a18a9c1eb032f}

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

