---
description: Hier erfahren Sie, wie Adobe Target Cookies verwendet, um Website-Betreibern die Möglichkeit zu geben, zu testen, welche Online-Inhalte und Angebote für Besucher am relevantesten sind.
keywords: Cookies, Datenschutz
solution: Experience Cloud,Analytics,Target,Social
title: 'Cookies in Adobe Target  '
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Administrator
level: Erfahren
translation-type: tm+mt
source-git-commit: 61d60273e933c637dfe4400da78257e1c80015b3
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 99%

---


# Cookies in Adobe Target {#target-cookies}

Adobe Target verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, die Relevanz von Online-Inhalten und -Angeboten für Besucher zu testen.

Mit Ausnahme der Cookie-Dauer können Sie diese Einstellungen bei Bedarf ändern. Wenden Sie sich beim Ändern der Cookie-Einstellungen an Ihren Kundenbetreuer.

>[!NOTE]
>
>Benutzer von Adobe Target können auch benutzerdefinierte Drittanbieter-Cookies erstellen.

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
   <td colname="col2"> <p>mbox. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Cookie-Domäne </p> </td> 
   <td colname="col2"> <p>Die zweite und oberste Ebene der Domänen, von denen Sie die mbox bedienen. Da die Belieferung von der Domäne Ihres Unternehmens stattfindet, handelt es sich um ein Erstanbieter-Cookie. Beispiel: <span class="filepath">meinunternehmen.com</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Serverdomäne </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> clientcode.tt.omtrdc.net</span>, unter Verwendung des Kundencodes für Ihr Adobe Target-Konto. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Cookie-Dauer </p> </td> 
   <td colname="col2"> <p>Das Cookie bleibt zwei Jahre nach der letzten Anmeldung des Besuchers in seinem Browser. Die Dauer des Cookies kann nicht geändert werden. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn einer Ihrer Domänennamen einen Ländercode enthält, wie beispielsweise [!DNL mycompany.co.uk], konfigurieren Sie gemeinsam mit Ihrem Kundenservice die [!DNL mbox.js], damit dieser Domänenname unterstützt wird.

Das Cookie enthält eine Reihe von Werten, mit denen verwaltet werden kann, wie Ihre Besucher Adobe Target-Kampagnen erleben:

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
   <td colname="col2"> <p>Eine eindeutige ID für eine Benutzersitzung. Standardmäßig ist dieser Wert 30 Minuten gültig. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> pc ID</span> </p> </td> 
   <td colname="col2"> <p>Eine semi-permanente ID für den Browser eines Besuchers. Sie ist gültig, bis Cookies manuell gelöscht werden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> check</span> </p> </td> 
   <td colname="col2"> <p>Ein einfacher Testwert zur Bestimmung, ob ein Besucher Cookies unterstützt. Wird jedes Mal festgelegt, wenn ein Besucher eine Seite anfordert. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> disable</span> </p> </td> 
   <td colname="col2"> <p>Wird eingestellt, wenn die Ladezeit des Besuchers das in der Datei <span class="filepath">mbox.js</span> konfigurierte Time-out überschreitet. Standardmäßig ist dieser Wert eine Stunde gültig. </p> </td> 
  </tr> 
 </tbody> 
</table>

