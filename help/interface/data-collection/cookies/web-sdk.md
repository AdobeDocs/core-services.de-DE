---
title: Cookies in Adobe Experience Platform Web SDK
description: Erfahren Sie, wie Web SDK Cookies verwendet, die für Ihre Implementierung gelten.
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

# Cookies in Adobe Experience Platform Web SDK

Adobe Experience Platform Web SDK verwendet Cookies, um implementierungsspezifische Werte zu speichern.

| Name | Maximales Alter | Größe | Beschreibung |
|---|---|---|---|
| **kndctr_&lt;ORG_ID>_identity** | 34128000 (395 Tage) | 100-120 Byte (variabel) | Speichert die ECID sowie andere Informationen im Zusammenhang mit der ECID. |
| **kndctr_&lt;ORG_ID>_consent** | 15552000 (180 Tage) | 10-11 Byte | Speichert die Einverständnisvoreinstellungen des Benutzers für die Website. |
| **kndctr_&lt;ORG_ID>_cluster** | 1800 (30 Minuten) | 3-5 Byte | Speichert den Edge Network-Bereich, der den Anfragen des aktuellen Benutzers dient. Die Region wird im URL-Pfad verwendet, damit das Edge Network die Anfrage an die richtige Region weiterleiten kann. Wenn ein(e) Benutzende(r) eine Verbindung mit einer anderen IP-Adresse oder in einer anderen Sitzung herstellt, wird die Anfrage erneut an die nächstgelegene Region weitergeleitet. |
| **mbox** | 63072000 (2 Jahre) | | Dies ist vorhanden, wenn die Einstellung für die Zielmigration auf „true“ festgelegt ist. Dadurch kann das Target[Mbox-Cookie](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) von der Web-SDK festgelegt werden. |
| **mboxEdgeCluster** | 1800 (30 Minuten) | | Dies ist vorhanden, wenn die Einstellung für die Zielmigration auf „true“ festgelegt ist. Dadurch kann Web SDK dem `at.js` den richtigen Edge-Cluster übermitteln, damit die Zielprofile synchron bleiben, während Benutzende auf einer Site navigieren. |
| **AMCV_##@AdobeOrg** | 34128000 (395 Tage) | | Bei aktiviertem [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/idmigrationenabled) vorhanden. Dies ist hilfreich bei der Umstellung auf Web SDK, während einige Teile der Site noch `visitor.js` verwenden. |

Das Edge Network setzt alle Cookies mit den Attributen `secure` und `sameSite="none"`. Wenn Sie derzeit sowohl sichere als auch nicht sichere Abschnitte auf Ihrer Website haben, kann die Benutzeridentifizierung ungenau sein. Wenn ein(e) Benutzende(r) von einem sicheren Abschnitt der Site zu einem nicht sicheren Abschnitt navigiert, generiert das Edge Network mit der Anfrage einen neuen `ECID`.
