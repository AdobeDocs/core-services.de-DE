---
title: Adobe Experience Platform Web SDK-Cookies
description: Erfahren Sie, wie das Web SDK Cookies verwendet, die für Ihre Implementierung gelten.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
source-git-commit: 66f78a04674a82335f5df20c4c15d983b6ebdc66
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# Adobe Experience Platform Web SDK-Cookies

Das Adobe Experience Platform Web SDK verwendet Cookies, um für Ihre Implementierung spezifische Werte zu speichern.

| Name | Max. Alter | Beschreibung |
|---|---|---|
| **kndct_orgid_identity** | 34128000 (395 Tage) | Speichert die ECID sowie andere Informationen zur ECID. |
| **kndctr_orgid_consent_check** | 7200 (2 Stunden) | Signalisiert den Server, die Zustimmungsvoreinstellungen serverseitig zu suchen. |
| **kndctr_orgid_consent** | 15552000 (180 Tage) | Speichert die Zustimmungsvoreinstellung des Benutzers für die Website. |
| **kndctr_orgid_cluster** | 1800 (30 Minuten) | Speichert den Edge Network-Bereich, der den Anforderungen des aktuellen Benutzers entspricht. Der Bereich wird im URL-Pfad verwendet, damit das Edge Network die Anfrage an den richtigen Bereich weiterleiten kann. Wenn ein Benutzer eine Verbindung mit einer anderen IP-Adresse oder in einer anderen Sitzung herstellt, wird die Anforderung erneut an den nächsten Bereich weitergeleitet. |
| **Mbox** | 63072000 (2 Jahre) | Vorhanden, wenn die Target-Migrationseinstellung auf &quot;true&quot;gesetzt ist. Dadurch wird Target ermöglicht [Mbox-Cookie](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) vom Web SDK festgelegt werden. |
| **mboxEdgeCluster** | 1800 (30 Minuten) | Vorhanden, wenn die Target-Migrationseinstellung auf &quot;true&quot;gesetzt ist. Dadurch kann das Web SDK den richtigen Edge-Cluster mit dem `at.js` damit Target-Profile synchronisiert bleiben können, wenn Benutzer auf einer Site navigieren. |
| **AMCV_###@AdobeOrg** | 34128000 (395 Tage) | Vorhanden, wenn [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/idmigrationenabled) aktiviert ist. Dies ist beim Übergang zum Web SDK hilfreich, während einige Teile der Site weiterhin verwenden `visitor.js`. |

Das Edge Network setzt alle Cookies mit dem `secure` und `sameSite="none"` -Attribute. Wenn Ihre Website derzeit sowohl sichere als auch nicht sichere Abschnitte enthält, kann die Benutzeridentifizierung ungenau sein. Wenn ein Benutzer von einem sicheren Bereich der Site zu einem nicht sicheren Bereich navigiert, generiert das Edge Network eine neue `ECID` mit der Anfrage.
