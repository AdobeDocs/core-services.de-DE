---
description: Erfahren Sie, wie der Besucher-ID-Service in allen CX Enterprise-Anwendungen gespeichert und verwendet wird.
solution: Experience Cloud,Analytics,Target
title: Cookies in Experience Cloud
uuid: a4788c1c-0402-4fc8-b894-cd24fa794f4f
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bd9bea58-9987-40d6-84e0-da185388bbbb
TQID: https://experienceleague.adobe.com/2i8AyRTW37TGYTpcLBh-ZMTyET0NvpRweTnUuk8Nnis
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
  - id: e43347a8-f2c5-4aa4-8623-6f13875d7e3a
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 7bfc22e90d727d1743c2b6b7bc645033d5d38f1b
workflow-type: tm+mt
source-wordcount: 371
ht-degree: 67%

---

# Cookies in CX Enterprise

Adobe CX Enterprise verwendet Cookies, um eine Besucher-ID zu speichern, die in allen CX Enterprise-Anwendungen verwendet wird. Diese Cookies gelten speziell für den Zugriff auf Adobe CX Enterprise-Anwendungen unter [experience.adobe.com](https://experience.adobe.com).

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
   <td colname="col2"> <p> Enthält eine Kopie der CX Enterprise ID (ECID) oder MID. Die MID ist in einem Schlüssel-Wert-Paar gespeichert, das dieser Syntax folgt: s_ecid=MCMID|&lt;ECID&gt; </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Ablauf </p> </td> 
   <td colname="col2"> <p>2 Jahre, obwohl die meisten modernen Browser auf 13 Monate verkürzt</p> </td> 
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

Der [Besucher-ID](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=de)Dienst verwendet JavaScript, um eine Unique-Visitor-ID in einem `AMCV_###@AdobeOrg`-Cookie in der Domain der aktuellen Website zu speichern, wobei `###` eine zufällige Zeichenfolge wie `AMCV_1FD6776A524453CC0A490D44%40AdobeOrg.` darstellt

Siehe auch [Cookies und der Besucher-ID-Dienst](https://experienceleague.adobe.com/docs/id-service/using/intro/cookies.html?lang=de).

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
   <td colname="col2"> <p> Unique Visitor IDs, die von CX Enterprise Solutions verwendet werden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Ablauf </p> </td> 
   <td colname="col2"> <p> 13 Monate </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Nutzung </p> </td> 
   <td colname="col2"> <p> Dieses Cookie wird zur Identifizierung eines Unique Visitor verwendet. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Standort </p> </td> 
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

