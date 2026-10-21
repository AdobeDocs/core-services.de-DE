---
title: Cookies in Adobe Experience Platform Web SDK
description: Erfahren Sie, wie Web SDK Cookies verwendet, die für Ihre Implementierung gelten.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
TQID: 'https://experienceleague.adobe.com/jysQ5m7o0cI3ECKz2RWZB4Kt3own7XAPm04pr4yLh-k'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
    internal-label: Administration
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
    internal-label: Support
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
    internal-label: Getting started
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 7b12d5debfccd62ab7b416e9a6fe278d251a4ca5
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 0%
---
# Cookies in Adobe Experience Platform Web SDK

Adobe Experience Platform Web SDK verwendet Cookies, um implementierungsspezifische Werte zu speichern.

| Name | Maximales Alter | Größe | Beschreibung |
| --- | --- | --- | --- |
| **`AMCV_###@AdobeOrg`** | 33696000 (390 Tage), wenn von der Web-SDK geschrieben | 44 Byte beim Schreiben durch den Web SDK (`MCMID\|<ECID>`); größer beim Schreiben durch `VisitorAPI.js` | Vorhanden, wenn [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/idmigrationenabled) aktiviert ist. Dies ist die Standardeinstellung. Dies ist hilfreich bei der Umstellung auf Web SDK, während einige Teile der Site weiterhin `VisitorAPI.js` verwenden. Web SDK liest dieses Cookie, um eine vorhandene ECID wiederzuverwenden. Nachdem Edge Network eine ECID zurückgegeben hat, schreibt die Web-SDK sie in dieses Cookie, wenn das Cookie fehlt oder eine andere ECID enthält. |
| **`com.adobe.alloy.getTld`** | Keine (Sitzungs-Cookie, sofort gelöscht) | 22 Bytes | Temporäres Helper-Cookie, das intern von Web SDK verwendet wird, um die Domain der aktuellen Site auf oberster Ebene zu ermitteln. Die Web-SDK schreibt und löscht dieses Cookie, wenn die Bibliothek geladen wird, bevor der `configure` ausgeführt wird und bevor das Einverständnis ausgewertet wird, sodass Cookie-Scanner es als vor dem Einverständnis festgelegt melden können. Das Cookie enthält nur einen eigenen Namen und speichert keine Verhaltens- oder Profildaten. |
| **`demdex`** | 15552000 (180 Tage) | variiert | Drittanbieter-Cookie in der `demdex.net` Domain. Vorhanden, wenn [`thirdPartyCookiesEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/thirdpartycookiesenabled) aktiviert ist (Standard) und der Browser standardmäßig Drittanbieter-Cookies zulässt, z. B. Chrome oder Edge. In diesem Fall sendet die Web-SDK Identitätsanfragen an `adobedc.demdex.net`, wodurch dieses Cookie gesetzt wird. Audience Manager verwendet dieses Cookie, um eine eindeutige ID zuzuweisen und ID-Synchronisierung, Segmentierung, Modellierung und Reporting zu unterstützen. Siehe `demdex` in [Audience Manager-Cookies](audience-manager.md). |
| **`kndctr_<orgId>_identity`** | 34128000 (395 Tage) | 100-120 Byte (variabel) | Speichert die ECID und andere zugehörige Informationen für dieses Gerät. |
| **`kndctr_<orgId>_cluster`** | 1800 (30 Minuten) | 3-5 Byte | Speichert die Edge Network-Region (Standorthinweis), die die Anfragen des aktuellen Benutzers verarbeitet. Die Region wird im URL-Pfad verwendet, damit der Edge Network die Anfrage an die richtige Region weiterleiten kann. Wenn ein Benutzer innerhalb der Cookie-Lebensdauer eine Verbindung mit einer anderen IP-Adresse herstellt, wird die Anfrage erneut an die nächstgelegene Region weitergeleitet. |
| **`kndctr_<orgId>_consent`** | 15552000 (180 Tage) | 10-11 Byte | Speichert die Einverständniseinstellungen des Besuchers. Wird unabhängig vom Einverständnis immer festgelegt, da die Einverständnisvoreinstellungen selbst gespeichert werden. |
| **`kndctr_<orgId>_consent_check`** | 7200 (2 Stunden) | | Ein Helper im Sitzungsbereich, der Edge Network signalisiert, das Einverständnis Server-seitig nach Ablauf der TTL erneut zu überprüfen. Es erzwingt eine TTL bei zwischengespeicherter Zustimmung. |
| **`kndctr_<orgId>_personalization`** | 34128000 (395 Tage) | | Speichert Sitzungsinformationen, die Adobe Target zum Personalisieren von Inhalten verwendet. |
| **`kndctr_<orgId>_advertising`** | 31622400 (366 Tage), wird jedes Mal erneuert, wenn das Cookie aktualisiert wird | 80 Byte bis 1 KB (variabel) | Vorhanden, wenn die Adobe Advertising-Komponente (Beta) in Ihrem Web-SDK-Build enthalten ist und das Einverständnis des Besuchers `in` wird. Der Web-SDK schreibt dieses Cookie, wenn die Seiten-URL Adobe Advertising-Klickparameter enthält (`s_kwcid` oder `ef_id`) oder wenn [Adobe Advertising DSP](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/configure/advertising)-Advertiser konfiguriert sind. Es speichert URL-kodierte JSON-Dateien, die Such-Klickdaten (`_les_lsc`), eine Hash-IP-Adresse, einen LiveRampID-Umschlag (wenn ein RampID-JavaScript-Pfad konfiguriert ist) und Konversionszeitstempel enthalten können, die zum Drosselen doppelter Konversionen verwendet werden. In Browsern, die standardmäßig Drittanbieter-Cookies zulassen, werden auch die Adobe Advertising-Surfer-ID und die Anzeigeklickdaten gespeichert (`ev_lcc`). Dieses Cookie wird nur für den aktuellen Host-Namen gesetzt. Die Komponente lädt auch Ressourcen aus `pixel.everesttech.net`, `www.everestjs.net` (wenn eine ID5-Partner-ID konfiguriert ist) und Ihrem RampID-`ats.js`. Diese Ressourcen können ihre eigenen Cookies setzen, die auf dieser Seite nicht aufgeführt sind. |
| **`kndctr_<orgId>_bc_session_id`** | Keine (Sitzungs-Cookie) | | Vorhanden, wenn die Brand Concierge-Komponente (Betaversion) verwendet wird. Speichert die Sitzungs-ID des Brand Concierge-Chats. Web SDK liest dieses Cookie nur, wenn [`stickyConversationSession`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/conversation) aktiviert ist, sodass Chat-Sitzungen über Seitenladevorgänge hinweg bestehen bleiben. |
| **`mbox`** | 63072000 (2 Jahre) | | Bei aktiviertem [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) vorhanden. Dadurch kann das Target[Mbox-Cookie](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) von der Web-SDK festgelegt werden. |
| **`mboxEdgeCluster`** | 1800 (30 Minuten) | | Bei aktiviertem [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) vorhanden. Dadurch kann Web SDK dem `at.js` den richtigen Edge-Cluster übermitteln, damit die Zielprofile synchron bleiben, während Benutzende auf einer Site navigieren. Wenn das `kndctr_<orgId>_cluster` Cookie nicht vorhanden ist, liest die Web-SDK dieses Cookie auch, um Anfragen an die entsprechende Edge Network-Region weiterzuleiten. |
| **`s_ecid`** | 63115200 (2 Jahre) | ~45 Byte | Enthält eine Kopie der CX Enterprise ID (ECID/MID) im `s_ecid=MCMID\|<ECID>`. Fungiert als First-Party-Backup der ECID, insbesondere für CNAME-Szenarien (First-Party-Szenarien). Wenn [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/idmigrationenabled) aktiviert ist, liest die Web-SDK dieses Cookie, um eine vorhandene ECID wiederzuverwenden. |
| **Audience Manager-Cookie-Ziele** (Name variiert) | 864000 (10 Tage), es sei denn, das Ziel gibt eine andere Lebensdauer an | variiert | Vorhanden, wenn die Edge Network ein Audience Manager-[Cookie-Ziel](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/destinations/custom-destinations/create-cookie-destination) für den Besucher zurückgibt. Web SDK schreibt ein Erstanbieter-Cookie unter Verwendung des Cookie-Namens, des -Werts und der Domain, die im Ziel definiert sind. Die Werte sind URL-kodiert, entsprechend der Audience Manager Data Integration Library (DIL). |

Edge Network setzt alle zugehörigen Cookies mit den Attributen `secure` und `sameSite="none"` . Wenn Sie derzeit sowohl sichere als auch nicht sichere Abschnitte auf Ihrer Website haben, kann die Benutzeridentifizierung ungenau sein. Wenn ein(e) Benutzende(r) von einem sicheren Abschnitt der Site zu einem nicht sicheren Abschnitt navigiert, generiert Edge Network mit der Anfrage einen neuen `ECID`.

Cookies, die von der Web-SDK eigenständig und nicht auf Anweisung der Edge Network erstellt werden, verwenden verschiedene Attribute. Die `AMCV_###@AdobeOrg`-Cookie- und Audience Manager-Cookie-Ziele enthalten die Attribute `secure` und `sameSite="none"` nur auf HTTPS-Seiten. Die `com.adobe.alloy.getTld`- und `kndctr_<orgId>_advertising`-Cookies verwenden die Standardattribute des Browsers.
