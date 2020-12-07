---
description: Adobe Experience Cloud verwendet Cookies, um eine Besucher-ID zu speichern, die für alle Experience Cloud-Lösungen genutzt wird.
keywords: cookies;privacy
solution: Experience Cloud,Analytics,Target
title: Experience Cloud-Cookies | Adobe Experience Cloud
uuid: a4788c1c-0402-4fc8-b894-cd24fa794f4f
translation-type: tm+mt
source-git-commit: 4bea0c29afa580dc63b21535ce5c275cd649c9a5
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 98%

---


# Experience Cloud-Cookies {#experience-cloud-cookies}

Adobe Experience Cloud verwendet Cookies, um eine Besucher-ID zu speichern, die für alle Experience Cloud-Lösungen genutzt wird.

**Cookie-Name: s_ecid**

<table id="table_FF4C70D3D4CC425BA65162D5A9504F7D"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>Attribut </p> </th> 
   <th colname="col2" class="entry"> <p>Beschreibung </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gespeicherte Informationen </p> </td> 
   <td colname="col2"> <p> Enthält eine Kopie der Experience Cloud ID (ECID) oder der MID. Die MID ist in einem Schlüssel-Wert-Paar gespeichert, das dieser Syntax folgt: s_ecid=MCMID|&lt;ECID&gt; </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Ablauf </p> </td> 
   <td colname="col2"> <p>2 Jahre </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Nutzung </p> </td> 
   <td colname="col2"> <p>Dieses Cookie wird durch die Domäne des Kunden festgelegt, nachdem das AMCV-Cookie vom Client festgelegt wurde. Dieses Cookie ermöglicht das durchgängige ID-Tracking als Erstanbieter und wird als Referenz-ID verwendet, wenn das AMCV-Cookie abgelaufen ist. Weitere Details zum AMCV-Cookie finden Sie hier. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Position </p> </td> 
   <td colname="col2"> <p>Nur CNAME-Kunden. Gilt nicht für Drittanbieter-Szenarien. Cookie wird in Ihrer Domäne gespeichert; dieselbe Domäne wie die von CNAME und Ihrer Analytics-Bildanforderung verwendete. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Größe </p> </td> 
   <td colname="col2"> <p>45 Byte </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> SameSite=Lax </p> </td> 
   <td colname="col2"> <p>Cookies mit dieser Einstellung werden nur gesendet, wenn die in der URL des Browsers angezeigte Domain mit der Domain des Cookies übereinstimmt. Dies ist die neue Standardeinstellung für Cookies in Chrome.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Cookie-Name: AMCV_###@AdobeOrg**

Der [Experience Platform-ID-Dienst](https://docs.adobe.com/content/help/de-DE/id-service/using/home.html) verwendet JavaScript, um eine Unique Visitor-ID in einem `AMCV_###@AdobeOrg`-Cookie in der Domäne der aktuellen Website zu speichern, wobei `###` eine zufällige Zeichenfolge wie `AMCV_1FD6776A524453CC0A490D44%40AdobeOrg.` darstellt.

Siehe auch [Cookies und der ID-Dienst](https://docs.adobe.com/content/help/de-DE/id-service/using/intro/cookies.html).

<table id="table_1883C0836C1E4AF5A262FBF5000C1B11"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>Attribut </p> </th> 
   <th colname="col2" class="entry"> <p>Beschreibung </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gespeicherte Informationen </p> </td> 
   <td colname="col2"> <p> Unique Visitor-IDs, die von Experience Cloud-Lösungen verwendet werden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Ablauf </p> </td> 
   <td colname="col2"> <p> 2 Jahre </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Nutzung </p> </td> 
   <td colname="col2"> <p> Dieses Cookie wird zur Identifizierung eines Unique Visitor verwendet </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Position </p> </td> 
   <td colname="col2"> <p> Dieses Cookie wird in der Domäne der Website gespeichert (nicht in der Domäne der Bildanforderung). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Größe </p> </td> 
   <td colname="col2"> <p> Variiert. Die meisten Kunden können davon ausgehen, dass dieses Cookie etwa 200 Byte lang ist. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Kein Wert hinzugefügt. Chrome wird standardmäßig auf Lax eingestellt. </p> </td> 
   <td colname="col2"> <p> Cookies mit dieser Einstellung werden nur gesendet, wenn die in der URL des Browsers angezeigte Domain mit der Domain des Cookies übereinstimmt. Dies ist die neue Standardeinstellung für Cookies in Chrome. </p> </td> 
  </tr> 
 </tbody> 
</table>
