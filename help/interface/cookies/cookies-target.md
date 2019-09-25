---
description: Target verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, die Relevanz von Online-Inhalten und -Angeboten für Besucher zu testen.
keywords: Cookies, Datenschutz
seo-description: Target verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, die Relevanz von Online-Inhalten und -Angeboten für Besucher zu testen.
seo-title: Cookies in Target
solution: Experience Cloud,Analytics,Target,Social
title: Cookies in Target
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
index: y
internal: n
snippet: y
translation-type: ht
source-git-commit: 426c1fecf16e1cf83cd28971e4de6fdb66b0e10d

---


# Cookies in Target{#target-cookies}

Target verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, die Relevanz von Online-Inhalten und -Angeboten für Besucher zu testen.

Sie können diese Einstellungen bei Bedarf ändern, außer die Cookie-Dauer. Wenden Sie sich an Ihren Kundenbetreuer, wenn Sie Cookie-Einstellungen ändern möchten.

>[!NOTE]
>
>Benutzer von Target können auch benutzerdefinierte Drittanbieter-Cookies erstellen.

<table id="table_54B402C6E19C4A70B1E27BC9DFF776EB"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Einstellung </th> 
   <th colname="col2" class="entry"> Information </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Cookie-Name </p> </td> 
   <td colname="col2"> <p>mbox </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Cookie-Domäne </p> </td> 
   <td colname="col2"> <p>Die obersten und die darunter liegenden Ebenen der Domänen, von denen die mbox beliefert wird. Da die Belieferung von der Domäne Ihres Unternehmens stattfindet, handelt es sich um ein Erstanbieter-Cookie. Beispiel: <span class="filepath">meinunternehmen.com</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Serverdomäne </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> clientcode.tt.omtrdc.net</span>, unter Verwendung des Kundencodes für Ihr Target-Konto. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Cookie-Dauer </p> </td> 
   <td colname="col2"> <p>Das Cookie verbleibt ab der letzten Anmeldung des Benutzers zwei Jahre im Browser. Sie können die Cookie-Dauer nicht ändern. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn einer Ihrer Domänennamen einen Ländercode enthält, wie beispielsweise [!DNL mycompany.co.uk], konfigurieren Sie gemeinsam mit Ihrem Kundenservice die [!DNL mbox.js], damit dieser Domänenname unterstützt wird.

Das Cookie enthält verschiedene Werte, mit denen verwaltet werden kann, wie die Besucher die Target-Kampagnen erleben:

<table id="table_5245F72A2D5A4322B40ABB10B7DFB338"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Wert </th> 
   <th colname="col2" class="entry"> Definition </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> session ID</span> </p> </td> 
   <td colname="col2"> <p>Eine eindeutige Kennung für eine Benutzersitzung. Standardmäßig ist diese 30 Minuten gültig. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> pc ID</span> </p> </td> 
   <td colname="col2"> <p>Eine eingeschränkt dauerhafte Kennung für den Browser eines Besuchers. Bleibt bestehen, bis das Cookie manuell gelöscht wird. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> check</span> </p> </td> 
   <td colname="col2"> <p>Ein einfacher Testwert, mit dem bestimmt wird, ob ein Besucher Cookies unterstützt. Wird immer dann eingestellt, wenn ein Besucher eine Seite anfordert. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> disable</span> </p> </td> 
   <td colname="col2"> <p>Wird eingestellt, wenn die Ladezeit des Besuchers das in der Datei <span class="filepath">mbox.js</span> konfigurierte Time-out überschreitet. Standardmäßig ist dieser Wert eine Stunde gültig. </p> </td> 
  </tr> 
 </tbody> 
</table>

