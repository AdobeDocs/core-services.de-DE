---
description: Target verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, die Relevanz von Online-Inhalten und -Angeboten für Besucher zu testen.
keywords: cookies;privacy
seo-description: Target verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, die Relevanz von Online-Inhalten und -Angeboten für Besucher zu testen.
seo-title: Cookies in Target
solution: Marketing Cloud,Analytics,Target,Social
title: Cookies in Target
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Adobe Zielgruppe Cookies{#target-cookies}

Adobe Zielgruppe verwendet Cookies, um Website-Betreibern die Möglichkeit zu geben, zu testen, welche Online-Inhalte und Angebot für Besucher relevanter sind.

Sie können diese Einstellungen bei Bedarf ändern, mit Ausnahme der Cookie-Dauer. Wenden Sie sich beim Ändern der Cookie-Einstellungen an Ihren Kundenbetreuer.

>[!NOTE]
>
>Adobe Zielgruppe-Benutzer können auch benutzerdefinierte Drittanbieter-Cookies erstellen.

<table id="table_54B402C6E19C4A70B1E27BC9DFF776EB"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Wenn </th> 
   <th colname="col2" class="entry"> Information </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Cookie-Name </p> </td> 
   <td colname="col2"> <p>mbox. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Cookie-Domäne </p> </td> 
   <td colname="col2"> <p>Die zweite und oberste Ebene der Domänen, von denen Sie die mbox beliefern. Da die Belieferung von der Domäne Ihres Unternehmens stattfindet, handelt es sich um ein Erstanbieter-Cookie. Beispiel: <span class="filepath">meinunternehmen.com</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Serverdomäne </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> clientcode.tt.omtrdc.net</span>, unter Verwendung des Clientcodes für Ihr Adobe-Zielgruppe-Konto. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Cookie-Dauer </p> </td> 
   <td colname="col2"> <p>Das Cookie bleibt zwei Jahre nach seiner letzten Anmeldung im Browser des Besuchers. Die Dauer des Cookies kann nicht geändert werden. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn einer Ihrer Domänennamen einen Ländercode enthält, wie beispielsweise [!DNL mycompany.co.uk], konfigurieren Sie gemeinsam mit Ihrem Kundenservice die [!DNL mbox.js], damit dieser Domänenname unterstützt wird.

Das Cookie enthält eine Reihe von Werten, mit denen verwaltet werden kann, wie Ihre Besucher Adobe Zielgruppe-Kampagnen erleben:

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
   <td colname="col2"> <p>Eine eindeutige ID für eine Benutzersitzung. Standardmäßig dauert dies 30 Minuten. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> pc ID</span> </p> </td> 
   <td colname="col2"> <p>Eine halbständige ID für den Browser eines Besuchers. Lässt sich so lange halten, bis Cookies manuell gelöscht werden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> check</span> </p> </td> 
   <td colname="col2"> <p>Ein einfacher Testwert, der bestimmt, ob ein Besucher Cookies unterstützt. Wird jedes Mal eingestellt, wenn ein Besucher eine Seite anfordert. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> disable</span> </p> </td> 
   <td colname="col2"> <p>Wird eingestellt, wenn die Ladezeit des Besuchers das in der Datei <span class="filepath">mbox.js</span> konfigurierte Time-out überschreitet. Standardmäßig ist dieser Wert eine Stunde gültig. </p> </td> 
  </tr> 
 </tbody> 
</table>

