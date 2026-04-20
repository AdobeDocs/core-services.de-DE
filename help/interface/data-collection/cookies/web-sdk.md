---
title: Cookies in Adobe Experience Platform Web SDK
description: Erfahren Sie, wie Web SDK Cookies verwendet, die für Ihre Implementierung gelten.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
TQID: https://experienceleague.adobe.com/jysQ5m7o0cI3ECKz2RWZB4Kt3own7XAPm04pr4yLh-k
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a42153ba5a885509e7735e7407e38586fcabb0ad
workflow-type: tm+mt
source-wordcount: 484
ht-degree: 1%

---

# Cookies in Adobe Experience Platform Web SDK

Adobe Experience Platform Web SDK verwendet Cookies, um implementierungsspezifische Werte zu speichern.

| Name | Maximales Alter | Größe | Beschreibung |
| --- | --- | --- | --- |
| **`AMCV_###@AdobeOrg`** | 34128000 (395 Tage) | 100-120 Byte (variabel) | Bei aktiviertem [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/idmigrationenabled) vorhanden. Dies ist hilfreich bei der Umstellung auf Web SDK, während einige Teile der Site weiterhin `visitor.js` verwenden. Die Web-SDK liest und schreibt während der Migration in dieses Cookie. |
| **`com.adobe.alloy.getTld`** | Keine (sofort gelöscht) | K. A. | Temporäres Helper-Cookie, das intern von Web SDK verwendet wird, um die Domain der aktuellen Site auf oberster Ebene zu ermitteln. Sobald die Domain auf oberster Ebene eingerichtet ist, wird das Cookie gelöscht. Es werden keine Verhaltens- oder Profildaten gespeichert. |
| **`demdex`** | 15552000 (180 Tage) | variiert | Vorhanden, wenn die Audience Manager ID-Synchronisierung aktiviert ist. Audience Manager setzt dieses Cookie, um eine eindeutige ID zuzuweisen und ID-Synchronisierung, Segmentierung, Modellierung und Reporting zu unterstützen. Siehe `demdex` in [Audience Manager-Cookies](audience-manager.md). |
| **`kndctr_<orgId>_identity`** | 34128000 (395 Tage) | 100-120 Byte (variabel) | Speichert die ECID und andere zugehörige Informationen für dieses Gerät. |
| **`kndctr_<orgId>_cluster`** | 1800 (30 Minuten) | 3-5 Byte | Speichert die Edge Network-Region (Standorthinweis), die die Anfragen des aktuellen Benutzers verarbeitet. Die Region wird im URL-Pfad verwendet, damit der Edge Network die Anfrage an die richtige Region weiterleiten kann. Wenn ein Benutzer innerhalb der Cookie-Lebensdauer eine Verbindung mit einer anderen IP-Adresse herstellt, wird die Anfrage erneut an die nächstgelegene Region weitergeleitet. |
| **`kndctr_<orgId>_consent`** | 15552000 (180 Tage) | 10-11 Byte | Speichert die Einverständniseinstellungen des Besuchers. Wird unabhängig vom Einverständnis immer festgelegt, da die Einverständnisvoreinstellungen selbst gespeichert werden. |
| **`kndctr_<orgId>_consent_check`** | 7200 (2 Stunden) | | Ein Helper im Sitzungsbereich, der Edge Network signalisiert, das Einverständnis Server-seitig nach Ablauf der TTL erneut zu überprüfen. Es erzwingt eine TTL bei zwischengespeicherter Zustimmung. |
| **`kndctr_<orgId>_personalization`** | 34128000 (395 Tage) | | Speichert Sitzungsinformationen, die Adobe Target zum Personalisieren von Inhalten verwendet. |
| **`mbox`** | 63072000 (2 Jahre) | | Bei aktiviertem [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) vorhanden. Dadurch kann das Target[Mbox-Cookie](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) von der Web-SDK festgelegt werden. |
| **`mboxEdgeCluster`** | 1800 (30 Minuten) | | Bei aktiviertem [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) vorhanden. Dadurch kann Web SDK dem `at.js` den richtigen Edge-Cluster übermitteln, damit die Zielprofile synchron bleiben, während Benutzende auf einer Site navigieren. |
| **`s_ecid`** | 63115200 (2 Jahre) | ~45 Byte | Enthält eine Kopie der CX Enterprise ID (ECID/MID) im `s_ecid=MCMID\|<ECID>`. Fungiert als First-Party-Backup der ECID, insbesondere für CNAME-Szenarien (First-Party-Szenarien). |

Edge Network setzt alle Cookies mit den Attributen `secure` und `sameSite="none"`. Wenn Sie derzeit sowohl sichere als auch nicht sichere Abschnitte auf Ihrer Website haben, kann die Benutzeridentifizierung ungenau sein. Wenn ein(e) Benutzende(r) von einem sicheren Abschnitt der Site zu einem nicht sicheren Abschnitt navigiert, generiert Edge Network mit der Anfrage einen neuen `ECID`.
