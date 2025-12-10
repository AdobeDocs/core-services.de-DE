---
title: Cookies in Adobe Experience Platform Web SDK
description: Erfahren Sie, wie Web SDK Cookies verwendet, die für Ihre Implementierung gelten.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
source-git-commit: 97b3db58a9bf25ec0a6dd18c7b62117063e58407
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 1%

---

# Cookies in Adobe Experience Platform Web SDK

Adobe Experience Platform Web SDK verwendet Cookies, um implementierungsspezifische Werte zu speichern.

| Name | Maximales Alter | Größe | Beschreibung |
|---|---|---|---|
| **`AMCV_###@AdobeOrg`** | 34128000 (395 Tage) | 100-120 Byte (variabel) | Bei aktiviertem [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/idmigrationenabled) vorhanden. Dies ist hilfreich bei der Umstellung auf Web SDK, während einige Teile der Site weiterhin `visitor.js` verwenden. Die Web-SDK liest und schreibt während der Migration in dieses Cookie. |
| **`demdex`** | 15552000 (180 Tage) | variiert | Vorhanden, wenn die Audience Manager ID-Synchronisierung aktiviert ist. Audience Manager setzt dieses Cookie, um eine eindeutige ID zuzuweisen und ID-Synchronisierung, Segmentierung, Modellierung und Reporting zu unterstützen. Siehe `demdex` in [Audience Manager-Cookies](audience-manager.md). |
| **`kndctr_<orgId>_identity`** | 34128000 (395 Tage) | 100-120 Byte (variabel) | Speichert die ECID und andere zugehörige Informationen für dieses Gerät. |
| **`kndctr_<orgId>_cluster`** | 1800 (30 Minuten) | 3-5 Byte | Speichert die Edge Network-Region (Standorthinweis), die die Anfragen des aktuellen Benutzers verarbeitet. Die Region wird im URL-Pfad verwendet, damit der Edge Network die Anfrage an die richtige Region weiterleiten kann. Wenn ein Benutzer innerhalb der Cookie-Lebensdauer eine Verbindung mit einer anderen IP-Adresse herstellt, wird die Anfrage erneut an die nächstgelegene Region weitergeleitet. |
| **`kndctr_<orgId>_consent`** | 15552000 (180 Tage) | 10-11 Byte | Speichert die Einverständniseinstellungen des Besuchers. Wird unabhängig vom Einverständnis immer festgelegt, da die Einverständnisvoreinstellungen selbst gespeichert werden. |
| **`kndctr_<orgId>_consent_check`** | 7200 (2 Stunden) | | Ein Helper im Sitzungsbereich, der Edge Network signalisiert, das Einverständnis Server-seitig nach Ablauf der TTL erneut zu überprüfen. Es erzwingt eine TTL bei zwischengespeicherter Zustimmung. |
| **`kndctr_<orgId>_personalization`** | 34128000 (395 Tage) | | Speichert Sitzungsinformationen, die Adobe Target zum Personalisieren von Inhalten verwendet. |
| **`mbox`** | 63072000 (2 Jahre) | | Bei aktiviertem [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) vorhanden. Dadurch kann das Target[Mbox-Cookie](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) von der Web-SDK festgelegt werden. |
| **`mboxEdgeCluster`** | 1800 (30 Minuten) | | Bei aktiviertem [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) vorhanden. Dadurch kann Web SDK dem `at.js` den richtigen Edge-Cluster übermitteln, damit die Zielprofile synchron bleiben, während Benutzende auf einer Site navigieren. |
| **`s_ecid`** | 63115200 (2 Jahre) | ~45 Byte | Enthält eine Kopie der Experience Cloud ID (ECID/MID) im `s_ecid=MCMID\|<ECID>`. Fungiert als First-Party-Backup der ECID, insbesondere für CNAME-Szenarien (First-Party-Szenarien). |

Edge Network setzt alle Cookies mit den Attributen `secure` und `sameSite="none"`. Wenn Sie derzeit sowohl sichere als auch nicht sichere Abschnitte auf Ihrer Website haben, kann die Benutzeridentifizierung ungenau sein. Wenn ein(e) Benutzende(r) von einem sicheren Abschnitt der Site zu einem nicht sicheren Abschnitt navigiert, generiert Edge Network mit der Anfrage einen neuen `ECID`.
