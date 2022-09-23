---
description: Erfahren Sie, wie das ID-Service in allen Experience Cloud-Programmen gespeichert und verwendet wird.
solution: Experience Cloud,Analytics,Target
title: Cookies in Experience Cloud
uuid: a4788c1c-0402-4fc8-b894-cd24fa794f4f
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bd9bea58-9987-40d6-84e0-da185388bbbb
source-git-commit: eb2ad8a8255915be47b6002a78cc810b522170d2
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 100%

---

# Cookies in Experience Cloud{#experience-cloud-cookies}

Adobe Experience Cloud verwendet Cookies, um eine Besucher-ID zu speichern, die für alle Experience Cloud-Programme genutzt wird.

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
   <td colname="col2"> <p>Dieses Cookie wird durch die Domain des Kunden festgelegt, nachdem das AMCV-Cookie vom Client festgelegt wurde. Dieses Cookie ermöglicht das durchgängige ID-Tracking als Erstanbieter und wird als Referenz-ID verwendet, wenn das AMCV-Cookie abgelaufen ist. Weitere Details zum AMCV-Cookie finden Sie hier. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Position </p> </td> 
   <td colname="col2"> <p>Nur CNAME-Kunden. Gilt nicht für Drittanbieter-Szenarien. Cookie wird in Ihrer Domain gespeichert; dieselbe Domain wie die von CNAME und Ihrer Analytics-Bildanforderung verwendete. </p> </td> 
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

Der [Experience Platform-ID-Dienst](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=de) verwendet JavaScript, um eine Unique-Visitor-ID in einem `AMCV_###@AdobeOrg`-Cookie in der Domain der aktuellen Website zu speichern, wobei `###` eine zufällige Zeichenfolge wie `AMCV_1FD6776A524453CC0A490D44%40AdobeOrg.` darstellt.

Siehe auch [Cookies und der ID-Dienst](https://experienceleague.adobe.com/docs/id-service/using/intro/cookies.html?lang=de).

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
   <td colname="col2"> <p> Unique-Visitor-IDs, die von Experience Cloud-Lösungen verwendet werden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Ablauf </p> </td> 
   <td colname="col2"> <p> 2 Jahre </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Nutzung </p> </td> 
   <td colname="col2"> <p> Dieses Cookie wird zur Identifizierung eines Unique Visitor verwendet. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Position </p> </td> 
   <td colname="col2"> <p> Dieses Cookie wird in der Domain der Website gespeichert (nicht in der Domain der Bildanforderung). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Größe </p> </td> 
   <td colname="col2"> <p> Variiert. Die meisten Kunden können davon ausgehen, dass dieses Cookie etwa 200 Byte lang ist. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Kein Wert hinzugefügt. Chrome ist standardmäßig auf Lax eingestellt. </p> </td> 
   <td colname="col2"> <p> Cookies mit dieser Einstellung werden nur gesendet, wenn die in der URL des Browsers angezeigte Domain mit der Domain des Cookies übereinstimmt. Dies ist die neue Standardeinstellung für Cookies in Chrome. </p> </td> 
  </tr> 
 </tbody> 
</table>
