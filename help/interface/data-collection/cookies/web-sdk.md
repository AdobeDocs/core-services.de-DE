---
title: Cookies im Adobe Experience Platform Web SDK
description: Erfahren Sie, wie das Web SDK Cookies verwendet, die für Ihre Implementierung gelten.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
source-git-commit: d69af76f6deff4f2b73e67ee7b69b9fee1ee3a2e
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 1%

---

# Adobe Experience Platform Web SDK-Cookies

Das Adobe Experience Platform Web SDK verwendet Cookies, um für Ihre Implementierung spezifische Werte zu speichern.

| Name | Max. Alter | Größe | Beschreibung |
|---|---|---|---|
| **kndctr_&lt;ORG_ID>_identity** | 34128000 (395 Tage) | 100-120 Byte (Variable) | Speichert die ECID sowie andere Informationen zur ECID. |
| **kndctr_&lt;ORG_ID>_consent** | 15552000 (180 Tage) | 10-11 Byte | Speichert die Zustimmungsvoreinstellung des Benutzers für die Website. |
| **kndctr_&lt;ORG_ID>_cluster** | 1800 (30 Minuten) | 3-5 Byte | Speichert den Edge Network-Bereich, der den Anforderungen des aktuellen Benutzers entspricht. Der Bereich wird im URL-Pfad verwendet, damit das Edge Network die Anfrage an den richtigen Bereich weiterleiten kann. Wenn ein Benutzer eine Verbindung mit einer anderen IP-Adresse oder in einer anderen Sitzung herstellt, wird die Anforderung erneut an den nächsten Bereich weitergeleitet. |
| **mbox** | 63072000 (2 Jahre) | | Vorhanden, wenn die Target-Migrationseinstellung auf &quot;true&quot;gesetzt ist. Dadurch kann das Target-[mbox-Cookie](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) vom Web SDK gesetzt werden. |
| **mboxEdgeCluster** | 1800 (30 Minuten) | | Vorhanden, wenn die Target-Migrationseinstellung auf &quot;true&quot;gesetzt ist. Dadurch kann das Web SDK den richtigen Edge-Cluster mit `at.js` kommunizieren, sodass Target-Profile synchronisiert bleiben können, wenn Benutzer auf einer Site navigieren. |
| **AMCV_###@AdobeOrg** | 34128000 (395 Tage) | | Vorhanden, wenn [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/idmigrationenabled) aktiviert ist. Dies ist beim Übergang zum Web SDK hilfreich, während einige Teile der Site weiterhin `visitor.js` verwenden. |

Das Edge Network setzt alle Cookies mit den Attributen `secure` und `sameSite="none"`. Wenn Ihre Website derzeit sowohl sichere als auch nicht sichere Abschnitte enthält, kann die Benutzeridentifizierung ungenau sein. Wenn ein Benutzer von einem sicheren Bereich der Site zu einem nicht sicheren Bereich navigiert, generiert das Edge Network eine neue `ECID` mit der Anforderung.
