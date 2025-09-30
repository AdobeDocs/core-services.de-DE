---
description: Erfahren Sie mehr über die neuesten Funktionen, Versionshinweise und bekannte Probleme bei Experience Cloud-Services wie Kundenattribute, Zielgruppen und Benutzerverwaltung.
solution: Experience Cloud
title: Gesammelte Versionshinweise für die Experience Cloud-Benutzeroberfläche
uuid: fcff8cc6-e587-4bf2-9a75-261d4eabc7d4
feature-set: Experience Cloud
feature: Release Notes
topic: Administration
role: Admin
level: Experienced
exl-id: b71d144c-a097-4cdb-9721-671519d38aff
source-git-commit: 66e8f4fe4ef0d0f2c00a875f13f0b8cd73ea1232
workflow-type: tm+mt
source-wordcount: '1291'
ht-degree: 84%

---

# Gesammelte Versionshinweise

Funktionen, Versionshinweise und bekannte Probleme in Verbindung mit der Experience Cloud-Schnittstelle.

Eine Liste der Aktualisierungen der Dokumentation finden Sie unter [Aktualisierungen der Dokumentation](doc-updates.md).

Versionshinweise zu allen Programmen finden Sie unter [Experience Cloud-Versionshinweise](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=de).

## September 2025

| Datum | Update | Beschreibung |
| -----------| -----------| ---------- |
| **Freitag, 25. September 2025** | Unterstützung für IP-Zugriffslisten | Für Organisationen, die IP-Zugriffslisten in Admin Console verfügbar und aktiviert haben, berücksichtigt Experience Cloud diese IP-Einschränkungen für den Zugriff auf Anwendungen auf der `https://experience.adobe.com` Domain. Diese Aktualisierung betrifft alle Web-Anwendungen, auf die über diese Domain zugegriffen wird, und Prüfungen werden bei der Anmeldung und beim Laden neuer Seiten in dieser Organisation durchgeführt. |

## März 2025

| Datum | Update | Beschreibung |
| -----------| -----------| ---------- |
| &#x200B;6. März 2025 | Korrektur der Rechtsklick-Menüoption | Navigationsregisterkarten in der Experience Cloud-Kopfzeile ermöglichen jetzt im Browser Dropdown-Menüfunktionen mit Rechtsklick. Damit wurde ein Problem behoben, das in der Version von Februar des Spectrum 2-Designsystems eingeführt wurde. |

## Februar 2025

| Datum | Funktion | Beschreibung |
| -----------| -----------| ---------- |
| Februar 13 | Spectrum 2 | Der Experience Cloud-Anwendungsrahmen, der die Kopfzeilenleiste und die von der Kopfzeilenleiste aus zugänglichen Komponenten sowie die linke Navigationsleiste für bestimmte Anwendungen enthält, wird auf Spectrum 2 aktualisiert, Adobes neuestes Design-System. Dieses überarbeitete Design enthält aktualisierte Symbolbilder, aber die gleiche Funktionalität. Einige Elemente in der Kopfzeile werden jedoch neu positioniert, um sie an andere Adobe-Sites und -Programme anzupassen. |

## Januar 2025

| Datum | Funktion | Beschreibung |
| -----------| -----------| ---------- |
| &#x200B;9. Januar | Produktnutzungsdaten | Um die Kontrolle der Voreinstellungen für Experience Cloud-Produktverwendungsdaten zu vereinfachen, haben wir unsere Seite [Voreinstellungen](../features/account-preferences.md#product-usage-data) von Experience Cloud optimiert, um doppelte Optionen zu entfernen. Mit dieser Vereinfachung haben wir die aktuellen Benutzereinstellungen beibehalten, und Sie können Ihre Voreinstellungen jederzeit auf [Experience Cloud-Voreinstellungen aktualisieren](https://experience.adobe.com/preferences). |

## &#x200B;2. Oktober 2024

| Funktion | Beschreibung |
| -----------| ---------- |
| Anpassbare Startseite | Klicken Sie auf der Experience Cloud-Landingpage auf **[!UICONTROL Bearbeiten]**. Der Modus [!UICONTROL Bearbeiten] ermöglicht es Ihnen, Ihre Experience Cloud-Startseite mit Zugriff auf eine Widget-Bibliothek und benutzerdefinierte Hintergründe zu personalisieren. [!UICONTROL Bearbeiten]-Modus bietet nahtlose, intuitive Steuerelemente zum Verschieben, Ändern der Größe und Verwalten von Widgets, einschließlich Massenaktionen und Layout-Anpassungen, die ein ästhetischeres und maßgeschneidertes Erlebnis bieten. |

## &#x200B;10. September 2024

| Funktion | Beschreibung |
| -----------| ---------- |
| Slack-Benachrichtigungen | Sie können Ihre Kontovoreinstellungen so konfigurieren, dass Experience Cloud-Benachrichtigungen an Slack gesendet werden. Detaillierte Informationen finden Sie unter {0 _Slack_ Benachrichtigungen in der [-Hilfe.](../features/account-preferences.md) |

<!-- ## July - August 2023

NA - released July 2022

Release: **July 20 - August 31, 2023**

Adobe is updating its provisioning to provide all [!DNL Experience Cloud] customers access to foundational capabilities that aid interoperability between some [!DNL Experience Cloud] products. Users will have [!DNL Experience Platform] as a new entitlement added to their [!DNL Experience Cloud] organizations, with [Data Collection](https://experienceleague.adobe.com/docs/analytics/analyze/reports-analytics/reporting-interface/overview-data-collection.html) as an included service. [!DNL Experience Platform] [!UICONTROL Data Collection] includes tags for simplified universal tag management and offers a trusted, robust, and complete streaming data infrastructure. This update simplifies your experience data collection and streamlines experience delivery. 

With this update, administrators may see changes or additions to the Admin Console:

* The Adobe [!DNL Experience Platform] product card in the Admin Console will include: [Places](https://experienceleague.adobe.com/docs/places/using/home.html), [Assurance](https://experienceleague.adobe.com/docs/platform-learn/implement-mobile-sdk/app-implementation/assurance.html), [Identity Namespace](https://experienceleague.adobe.com/docs/experience-platform/identity/home.html), [Sandboxes](https://experienceleague.adobe.com/docs/experience-platform/sandbox/home.html), [Experience Data Model](https://experienceleague.adobe.com/docs/experience-platform/xdm/home.html), [Schemas](https://experienceleague.adobe.com/docs/experience-platform/xdm/schema/composition.html), [Datastreams](https://experienceleague.adobe.com/docs/experience-platform/edge/datastreams/overview.html), and [Experience Cloud ID](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html).

  * For organizations who are not currently using [!DNL Experience Platform], you will now see the [!DNL Experience Platform] product in the [!UICONTROL Admin Console], including the capabilities listed above.

  * For organizations currently using [!DNL Experience Platform], [!UICONTROL Places] will be consolidated into the [!DNL Experience Platform] card.

* Adobe [!DNL Experience Platform] [Data Collection](https://experienceleague.adobe.com/docs/analytics/analyze/reports-analytics/reporting-interface/overview-data-collection.html) (formerly [!DNL Launch]) and [Privacy](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html) will continue to appear as their own product cards, separate from the other [!DNL Experience Platform] capabilities -->

## Mai 2023

* Im **[!UICONTROL Hilfe]**-Menü von [!DNL Experience Cloud] wurde die Inhaltssuche aktualisiert, um in den [Experience League](https://experienceleague.adobe.com/?lang=de#home)-Suchergebnissen nach Anwendung zu filtern.

## Juli 2022

| Funktion | Beschreibung |
| ------- | ------- |
| Einheitliche Startseite – Widget für Schnellzugriff | **Schnellere Navigation:** Sie können jetzt Ihre Startseite weiter personalisieren und entscheiden, welche Anwendungen immer griffbereit sein sollen. Verwenden Sie die neue Anheft-Funktion, um festzulegen, welche Anwendungen beim [!UICONTROL Schnellzugriff] im Vordergrund angezeigt werden sollen. <br>**Bleiben Sie mit der intelligenten Anheft-Funktion auf dem Laufenden:** Ihre neuen Anwendungen sind jetzt einfacher zu finden. Neu zugewiesene Anwendungen erhalten die Kennzeichnung _Neu_ und werden automatisch im [!UICONTROL Schnellzugriff] angeheftet. |

{style="table-layout:auto"}

## April 2022

| Funktion | Beschreibung |
| ------- |-------|
| Suche in natürlicher Sprache | Erhalten Sie sofort Antworten auf all Ihre Fragen zu Hilfe – durch die einheitliche Suche über eine einzige Oberfläche. Diese Funktion steht Ihnen auf jeder Seite von [!DNL Experience Platform] und [!DNL Journey Optimizer] immer zur Verfügung. |

{style="table-layout:auto"}

## März 2022

| Funktion | Beschreibung |
| ------- |-------|
| Auf [!UICONTROL Zuletzt verwendet] in Experience Platform und Journey Optimizer über die Suchleiste zugreifen | Benutzer können nun über die einheitliche Suchleiste von jeder Seite von AEP und AJO aus auf zuletzt aufgerufene Objekte zugreifen. |

{style="table-layout:auto"}

## Februar 2022

| Funktion | Beschreibung |
| ------- |-------|
| Tastaturbefehle (**[!UICONTROL Zuletzt verwendet]**) zur [Experience Cloud](https://experience.adobe.com/home?lang=de)-Startseite hinzugefügt | Unter der neuen Rubrik _Zuletzt verwendet_ auf der Landingpage können Sie auf Verknüpfungen zu Ihren letzten Arbeiten mit Journey Optimizer und Experience Platform zugreifen. Diese Aktualisierung beinhaltet auch allgemeine Verbesserungen hinsichtlich Layout und Reaktionsfähigkeit. |
| **[!UICONTROL Sandboxes]** in die Kopfzeilenleiste verschoben | Der Sandbox-Indikator ist jetzt für alle Programme der Experience Platform-Benutzeroberfläche in die Kopfzeile integriert. Siehe [Sandboxes](https://experienceleague.adobe.com/docs/experience-platform/sandbox/ui/user-guide.html?lang=de) in Experience Platform für weitere Informationen. |

{style="table-layout:auto"}

## November 2021

| Funktion | Beschreibung |
| ------- | ------- |
| Startseite | Die Fußzeilen-Informationen von Experience Cloud, einschließlich der rechtlichen Hinweise und der Sprachauswahl in den Voreinstellungen, wurden in die Benutzerprofilkarte verschoben. |
| AEP-Dashboards | [!DNL Helios Lite] empfiehlt während des Erstellungs-Wokflows von Experience Platform-Widgets Diagramme. [!DNL Helios] empfiehlt auf der Grundlage der ausgewählten Daten eine geeignete Visualisierung. |
| AEP-Dashboards | [!DNL Instory] bietet auf ML basierende Erklärungen und Beschriftungen für Diagramme. Auf der AEP-Dashboards-Seite werden Diagramme mit relevanten Aufzählungspunkten versehen, die wichtige Veränderungen und Ereignisse in den Diagrammdaten kennzeichnen. |

{style="table-layout:auto"}

## Oktober 2021

| Funktion | Beschreibung |
| ------- | ------- |
| Einheitliche Suche | Unified Search fügt dem Suchindex weiterhin Objekttypen hinzu. In diesem Update durchsucht die globale Suche jetzt Experience League-Inhalte und die folgenden Journey Optimizer-Objekttypen: <ul><li>Datensätze</li><li>Ziele</li><li>Abfragen</li><li>Schemata</li><li>Segmente</li><li>Quellen</li><li>Angebote</li><li>Komponenten</li><li>Nachrichten</li><li>Journeys</li></ul> |
| Zustimmung zu den Produktverwendungsdaten | Nach der ersten Anmeldung werden Sie aufgefordert, Voreinstellungen einzureichen, um zu erfahren, wie Adobe Sie mithilfe von hilfreichen, personalisierten Inhalten wie Tutorials, Handbücher, Quick Tipps, Empfehlungen, Lernvideos und mehr versorgen kann. Diese basieren auf den Nutzungsdaten Ihres Experience Cloud-Produkts. Diese Anfrage enthält auch eine Aktualisierung Ihrer Voreinstellungen für die Erfassung und Verwendung dieser Daten unter <https://experience.adobe.com/preferences>. |

{style="table-layout:auto"}

## August 2021

| Funktion | Beschreibung |
| ------- | -------|
| [!UICONTROL Unified Recents] – Erweiterte Unterstützung für kürzlich aufgerufene Geschäftsobjekte | [!UICONTROL Unified Recents] wurde auf zusätzliche Geschäftsobjekte in Journey Optimizer und Experience Platform erweitert. Journey Optimizer-Kunden können ihre kürzlich aufgerufenen Objekte (Nachrichten, Journeys, Segmente, Schemata, Datensätze, Datenquellen, Ereignisse, Aktionen, Quellen und Ziele) über die Startseite von Adobe Journey Optimizer finden. |

{style="table-layout:auto"}

## Juli 2021

Die einheitliche Suche wird aktualisiert und ist nun für Journey Optimizer, Angebote und Experience League verfügbar. Zuvor war diese Funktion nur für Experience Platform-Benutzer verfügbar.

## Juni 2021

| Funktion | Datum | Beschreibung |
| ------- | ------- | ------- |
| Single-Sign-On-Unterstützung für Adobe Federated IDs | 17. Juni 2021 | Wenn Sie Federated IDs verwenden, können Sie sich bei Experience Cloud anmelden, ohne eine E-Mail-Adresse oder ein Passwort eingeben zu müssen. Um diese Funktion zu verwenden, fügen Sie `#/sso:@domain` zur Experience Cloud-URL hinzu. <br>Nehmen wir beispielsweise an, Sie sind der Eigentümer der Domain `adobecustomer.com` und möchten sich bei Adobe Analytics anmelden. Die URL lautet: `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`. |
| Experience League Search | 1. Juni 2021 | Die Suche in der Dokumentation zu Experience Leaguen wurde verbessert. Navigieren Sie zu [Experience League](https://experienceleague.adobe.com/docs/?lang=de) und verwenden Sie das Feld **[!UICONTROL Suchen]**, um Tutorials, Dokumentationen, Kurse und mehr zu finden. |

{style="table-layout:auto"}

## Mai 2021

| Funktion | Beschreibung |
| ------- | ------- |
| Experience Cloud-Kopfzeile und -Navigation | Adobe Experience Cloud-Aktualisierungen beinhalten eine Änderung des hellen Designs für die Kopfzeile. Sie können einfach wieder zu einem dunklem Design wechseln und erhalten einen Link zur Steuerung zusätzlicher Voreinstellungen von Ihrem Benutzeravatar in der Kopfzeile von Experience Cloud. Obwohl nicht alle Anwendungen in Experience Cloud das Design unterstützen, wird durch diese Funktion die Unterstützung künftiger Designs freigeschaltet. |
| Experience Cloud Global Search | Mit dieser Version können Sie mit der globalen Experience Cloud-Suche nach allen [Experience League](https://experienceleague.adobe.com/?lang=de#home)-Dokumentationen, -Kursen und -Tutorials suchen. (Derzeit steht die globale Suche nur Benutzern von Experience Platform zur Verfügung. Die globale Suchfunktion für die [!UICONTROL Platform] ermöglicht es Ihnen, in Experience Cloud nach beliebigen Geschäftsobjekten zu suchen, z. B. nach Segmenten, Datensätzen, Schemata und mehr.) |
| Experience Cloud-Spracheinstellungen | Dieses Update bietet die Möglichkeit, Ihre bevorzugten Sprachen in den Experience Cloud-[Voreinstellungen](https://experience.adobe.com/preferences) festzulegen. |

{style="table-layout:auto"}

## August 2020

| Funktion | Beschreibung |
| -----------| ---------- |
| Admin-Tool – Richtlinien | Auf dieser Seite finden Sie eine vollständige Liste der Experience Cloud-Richtlinien in Ihrem Unternehmen. Sie enthält Informationen zu Produkten, Instanzen, Benutzern und Entwicklern. Sie können nach benutzerdefinierten Ansichten der Richtlinienliste suchen, sortieren und filtern. Weitere Informationen finden Sie in der Hilfe zum [Experience Cloud-Admin-Tool](../administration/admin-tool-experience-cloud.md). |

{style="table-layout:auto"}

## April 2020

* Die Seite „Experience Cloud- [!UICONTROL Feed]“ wurde entfernt. (EXC-8505)
* Die Experience Cloud-Anmeldeseite wurde aktualisiert und enthält jetzt neue Branding-Elemente. (EXC-10747)

## Februar 2020

| Funktion | Beschreibung |
| -----------| ---------- |
| Admin-Tool – Benutzerdetails anzeigen | Administratoren können im neuen Admin-Tool eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und deren Details anzeigen. Zu den Benutzerdetails zählen der Produktzugriff und die Rollen der Benutzer sowie die zuletzt aufgerufenen Informationen. Weitere Informationen finden Sie in der Hilfe zum [Experience Cloud-Admin-Tool](../administration/admin-tool-experience-cloud.md). |

{style="table-layout:auto"}

**Fehlerbehebungen**

* **Kundenattribute:** Benutzeroberfläche „Kundenattribute“ zeigt jetzt zusätzliche Status von Profilen an, die in Target synchronisiert wurden. (MCUI-10231)
* **Triggers Hauptdienst:** Aufgrund der mangelnden Verwendung wurde der Tendenzwert „Wahrscheinlichkeit einer Rückkehr in 30 Tagen“ beim Erstellen eines Auslösers vom Typ „Abbruch“ entfernt. (MCUI-10056)

## Januar 2020

* Die Feed-Seite wird seit Dezember 2019 nicht mehr unterstützt. Innerhalb des Produkts finden Sie eine Benachrichtigung zur Einstellung. (MCUI-10039)

<!-- ## August 2019

* Fixed a critical issue in Experience Cloud login that led to session logout for some users. (MCUI-6908)
* Updated Experience Cloud login to improve performance and reduce latency. (MCUI-6854, MCUI-6869, MCUI-6883)
* Updated interface cosmetically. (MCUI-6861, MCUI-6911, MCUI-6862)
* Fixed an issue with Experience Cloud [!UICONTROL Triggers] that led to incorrect interpretation of _Like_ clause in the [!UICONTROL Trigger] definition. (MCUI-6611)

## April 2019

* Updated the app switcher to include Marketo in Experience Cloud application suite, and branding updates to Experience Platform. (MCUI-6529)
* Updated Experience Cloud Home to include navigation links to the Feed and Administration pages. (MCUI-6682)
* Fixed an issue in the [!UICONTROL Trigger] definition for correct usage of "like" clause. (MCUI-6611)
* Improvements to Customer attributes for better logging in the Subscription service. (MCUI-6519)

## January 2019

**Note:** In March 2019, The Experience Cloud interface will not support Internet Explorer 11.

* Fixed an issue preventing the help search from returning results. (MCUI-1670)
* Fixed and improved eVar management in Triggers. (MCUI-6400)

## August 2018

* Made improvements on assets comment sync across Creative Cloud and Experience Cloud. (CORE-15971)
* Added feature flag to control Experience Cloud-Creative Cloud asset sync. (CORE-15938)
* Made improvements to Audience segments creation, including better search and listing experience. (CORE-5833, CORE-14278)
* Fixed a high priority issue that blocked folder sharing from Experience Cloud to Creative Cloud. (CORE-16677)

## July 2018

* Deployed a back-end capability to control asset sharing between Marketing Cloud-to-AEM and Marketing Cloud-to-Creative Cloud. (CORE-14386)
* Fixed an issue that blocked provisioning of new tenants on some environments. (CORE-15509)
* Fixed an issue that redirected users to `experiencecloud.adobe.com` using `http` instead of `https`. (CORE-15587)
* Fixed an issue that blocked notifications for some new tenants. (CORE-15240)

## June 2018

* Enabled a link to GDPR access for Administrators. (CORE-11731)
* Updated Beta Feedback feature to restrict file types that can be attached to feedback. (CORE-10474)
* Fixed an issue with deleting audiences from Audience Library. (CORE-12792)
* Fixed an issue that resulted in a blank screen while accessing Workspace links using Federated IDs. (CORE-11620)

## May 2018

| Feature | Description |
|--- |--- |
|New administration landing page|When you sign in to Experience Cloud and navigate to the Administration page, a new intuitive interface is available to help you quickly access your Experience Cloud applications and Core Services.|

{style="table-layout:auto"}

**Fixes** 

* Fixed an issue where the image upload failed due to a Scene7 update. (CORE-12746)
* Made updates to drop support for TLS 1.0 protocol, as mandated by PCI to eliminate security vulnerability. (CORE-7695)

## October 2017

**Known Issue**: Many of the maintenance notifications around scheduled maintenance / product updates are missing from the notifications email digest. We are working to ensure that all maintenance notifications are included in the email digest. 

## August 2017

| Feature | Description |
|--- |--- |
|Notifications - Granular settings|You can enable notifications for product and application events and activities, including notifications about [customer attributes](../services/customer-attributes/attributes.md) upload activity.|
|Notifications - Maintenance notifications|In Notification settings, you can enable maintenance notifications for products and applications.|
|Admin Console for Experience Cloud Solutions|New Experience Cloud customers can begin using the Admin Console, a central location for managing your Adobe entitlements across your entire organization.<br>The migration to the Admin Console for user management will proceed in waves. Adobe contacts you (system administrators) when it is time to migrate.<br>Analytics administrators, see  [Analytics Migration](https://experienceleague.adobe.com/docs/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html).|

{style="table-layout:auto"}

## May 2017

| Feature | Description |
|--- |--- |
|Bulk Report Suite Mapping|In Administration > Report Suite Mapping, you can now select multiple report suites, then map them to an organization. (Previously, you had to map them individually.)  <br>Mapping report suites to a single organization helps enable cross-application features and services in Experience Cloud.|
|Updates to Experience Cloud Audiences|**Applying Report Suites**<br>You can now apply a report suite to all your [audience rules](../services/audiences/create.md). (Previously, you had to specify a report suite in each rule definition.) <br>**Props and Variables**<br>You can now include Analytics props and default variables (in addition to eVars and events) in real-time audiences.|

{style="table-layout:auto"}

## November 2016

| Feature | Description |
|--- |--- |
|Update to Profile & Passwords|Users can no longer edit IMS user profile information under  Personal Details In  Edit Profile >  Profile & Passwords. Instead users are redirected to `accounts.adobe.com`. This update applies to all identity types (Adobe ID, Enterprise, and Federated).|

{style="table-layout:auto"}

**Fixes** 

* Fixed an issue with technical passwords that caused an error in folder sharing between Creative Cloud and Experience Cloud. (MAC-31067, MAC-32014)
* Fixed an issue with the upload of certain file types, including PDF, that was found after the October release in Assets Core Service. (MAC-32517)

## May 2016

<table id="table_ABBCE1A66F534059BD728BC2B9AEFA80"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Pre-configured product configurations in the Admin Console </p> </td> 
   <td colname="col2"> <p>Experience Cloud customer administrators can use product configurations that are pre-created and mapped to default permission groups for Analytics and Dynamic Tag Management. </p> <p>This optimization is available for newly provisioned organizations, and it reduces the amount of time required by organizations to manage users in the Admin Console. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Feed improvement </p> </td> 
   <td colname="col2"> <p> When creating a post in the Experience Cloud Feed, the To line now uses the currently active topic instead using the organization by default.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes**

* Fixed an issue preventing thumbnails from showing for assets shared from Assets on Demand to the Experience Cloud Feed. (MAC-29955) 

## February 2016

<table id="table_C9B288CF42034F329C3C72D95D22E515"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Experience Cloud Assets improvements </p> </td> 
   <td colname="col2"> <p>In Experience Cloud Assets, you can store, share, and synchronize your digital assets from one central location. Experience Cloud Assets uses some of the features available in <span class="keyword"> Adobe Experience Manager</span> (AEM). </p> <p>See <a href="../services/assets/experience-cloud-assets.md" format="dita" scope="local"> Experience Cloud</a></p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Account linking improvements </p> </td> 
   <td colname="col2"> <p>Improved the interface workflow for linking application accounts with the Experience Cloud (Adobe ID). This new workflow locates all the user's accounts associated with an organization, and lets you choose which account to link. We also streamlined the account linking experience, so that you no longer must access the Manage Organizations page to manually link accounts. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes** 

* Fixed an issue preventing linking and SSO for Analytics. This issue displayed the "Notice: The error message: ERROR IMS SSO Failed: Unable to find linked company."

## January 2016

<table id="table_4223658257DA41C999AC710A10D26771"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Audience Library messages </td> 
   <td colname="col2"> <p> We improved Audience Library to include helpful messages when building audiences or when a time-out occurs. </p> <p>For example, when adding more than five rules, a message displays indicating you exceeded maximum allowable rules. (MAC-27376, MAC-27375) </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Microsoft&reg; is [ending support](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support) for Internet Explorer 8, 9, and 10. As such, Adobe does not plan to fix issues reported against these specific versions of Internet Explorer. 

## October 2015

**Known Issues** 

* Customers are not able to log into Report Builder if they SSO into Analytics via Experience Cloud. This issue does not impact customers using legacy Analytics credentials.
* Known issue with the "Link to Report" function in Analytics. Customers logging into Analytics via Experience Cloud are directed to a non-SSO login page for Analytics when trying to share a report.

## September 2015

* Fixed an Audience Manager API performance issue causing intermittent timeouts when uploading customer attributes data. (MAC-26305)
* Fixed an issue that prevented users from adding up to 200 customer attributes to a subscription. (MAC-26188)
* Fixed an Audience Library issue that prevented audience sharing from Analytics segmentation. This issue caused "Collecting Data" (0 audiences) to display. To prevent this issue, Adobe recommends keeping the segment sizes under 50k audience members per segment. (MAC-25788)
* Fixed a previous known issue on the customer attributes - Edit Schema page that was causing a Content Aware error that was issued when changing a display name. (MAC-25589, AN-103834)

## July 2015

* Fixed an issue that prevented attribute descriptions specified on the View/Edit Schema page (in customer attributes) from being updated in Analytics reports. (MAC-25985)
* Fixed an issue preventing the thumbnails from rendering for uploaded assets. (MAC-25863)
* Fixed an issue that prevented new segments created in reports & analytics from being available in Experience Cloud Audiences. (MAC-25817)
* Fixed an issue that prevented audience sharing from Analytics, when using the visitor ID service. (MAC-25788, MAC-25747)
* Added support for multibyte characters in customer attributes. (MAC-25552)

**Known Issue**: A known issue is causing duplicate auto-generated accounts to be created in Audience Manager, and automatically linking them to a user's Experience Cloud identity. This issue occurs if you attempt to navigate to Audience Manager before linking your accounts. Adobe recommends that you link your Audience Manager accounts to Experience Cloud before navigating to Audience Manager. (MAC-25640) 

## May 2015

<table id="table_14E7B35E06C84A258A21D09691B58354"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>The left navigation menus have been updated and arranged to provide access to all the core services and applications. Notable changes include: </p> 
    <ul id="ul_5BEBAB86B9234A239C4E2DAF8826D8E3"> 
     <li id="li_7FA9F64CE69144B8A8A92746BF40E5A1">The <span class="term"> Audience Library</span> and <span class="term"> customer attributes</span> menu selections are now located under <span class="term"> Audiences</span>. </li> 
     <li id="li_95D62A43AE6243DBB2A65EDB830D05C4">The <span class="term"> Exchange</span> menu selection was moved from the Help drop-down menu to the left navigation rail. </li> 
     <li id="li_0443FD50C78446CD8AA27A4F272CAD31"> <span class="term"> Solutions</span> has been removed. You can launch all applications from the bottom half of the navigation rail. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

* Fixed an issue preventing customer attributes from syncing for some customers.
* Fixed an issue preventing [Adobe Target Product Documentation](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html) page from displaying in Japanese.
* Fixed an issue preventing the use of Japanese text in comments between [!DNL Creative Cloud] and [!DNL Experience Cloud].

## April 2015

<table id="table_3A6FBAE36558425A803B078150862C92"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Administration improvements: </p> 
    <ul id="ul_7D5FCBEFA262435D865CA1018BFB792E"> 
     <li id="li_6E98974CCB094ABBAB57C51ED56C3F00"> <span class="wintitle"> Admin Console</span> </li> 
     <li id="li_8CDAB6301FD44C3999EE4EEB1A0A2FD6">Enterprise and Federated ID support </li> 
    </ul> </td> 
   <td colname="col2"> <p>User and group management functionality has been moved to the Admin Console. The new navigation path is: </p> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol"> Administration</span> &gt; <span class="uicontrol"> Launch Admin Console</span></p> <p> Also, support for enterprise and federated IDs has been added. You can use enterprise IDs, federated IDs, and Adobe IDs in the same enterprise deployment. For example, use Adobe IDs for users who may use other Adobe product and services. Use enterprise or federated IDs for users where you want to strictly manage their accounts. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes** 

* Fixed an issue preventing single sign-on between [!DNL Experience Cloud] and [!DNL Advertising Cloud].

**Known Issues** 

* Linking and unlinking your dynamic tag management organization with Experience Cloud is not working for newly created Experience Cloud organizations. Adobe is working to fix this and restore normal functionality with the May release. If you experience problems when trying to single-sign on into dynamic tag management via Experience Cloud, use the legacy login at `dtm.adobe.com`.
* A known issue is preventing audience sharing from report suites which are not owned by the linked Analytics account. Remedial efforts are underway

## March 2015

<table id="table_54025DBE2D094FF1BE837BA60816C6DF"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Customer attributes </p> </td> 
   <td colname="col2"> <p>If you capture enterprise customer data in a customer relationship management (CRM) database, you can upload the data into a customer attribute data source in Experience Cloud. After the data is uploaded, you can run <span class="uicontrol"> Visitor Profile</span> &gt; <span class="uicontrol"> customer attributes</span> reports in Analytics. </p> <p>You can also use the uploaded data as an audience segment in <span class="keyword"> Adobe Target</span>. </p> <p>See <a href="../services/customer-attributes/attributes.md" format="dita" scope="local"> customer attributes</a> product documentation. </p> </td> 
  </tr> 
 </tbody> 
</table>

## March 2015

<table id="table_EB3FFBA2DF904546A5185EC9A63BBA98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Group Mapping </p> </td> 
   <td colname="col2"> <p>The Group Management page has been redesigned as an administrative interface that lets you create groups, add users to groups, and apply permissions across Experience Cloud applications. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>One-to-many mapping </p> </td> 
   <td colname="col2"> <p>When linking application accounts in Experience Cloud, if you have multiple applications and organizations, you can now map multiple products and services to a single organization. </p> </td> 
  </tr>
 </tbody> 
</table>

## February 2015

**Fixes**

* Improved the user email invitation workflow for account provisioning.
* Fixed an asset folder issue preventing [!DNL Experience Cloud] and [!DNL Adobe Campaign] assets from displaying identical folder hierarchies.
* Fixed an issue preventing the deletion of audiences that were part of deactivated [!DNL Target] activities.
* Fixed an issue preventing the Add (plus) icon from displaying under [!UICONTROL Rules] on the [!UICONTROL Create New Audience] page.
* Improved Experience Cloud interface support for Internet Explorer 9.

## January 2015

<table id="table_AD0A8CA760E64227BB04BA6B0E425E80"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Read-only access. </p> </td> 
   <td colname="col2"> <p>Administrators can now grant non-administrative users read-only access. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes** 

* Fixed an issue in which PNG files could not be rendered on a card.
* Fixed an issue with uploading files to Experience Cloud Assets via drag and drop.

**Known Issues** 

* Users are not able to share PowerPoint files on boards.
* Group and entitlement changes made in User Management take effect only after a new login.
* Some users might have issues uploading large file-types to Experience Cloud Assets.
* Users might be missing links on their Experience Cloud cards from Advertising Cloud.
* Some administrative users might experience issues linking their accounts after accepting an invitation to join Experience Cloud.
* Experience Cloud interface can reduce in performance when in parallel use by multiple users.
* Some users are able to delete an out-of-date asset instead of receiving an error notification.
* Some users might experience issues when logging into two browsers with the same Adobe ID simultaneously.
* Some users might be unable to re-add a Creative Cloud user to a shared folder after the Creative Cloud user has been deleted.
* Some users might experience a delay in the notification that occurs when a folder is shared from Experience Cloud to Creative Cloud.
* Some users might experience an issue sharing a folder between Experience Cloud and Creative Cloud.
* Some users may have trouble creating an audience within an Analytics report suite after shared audiences have been enabled.
* Some users may have trouble uploading assets to a board.

## November 2014

**Known issues**

* Some users are able to delete an out-of-date asset instead of receiving an error notification.
* Some `.png` files cannot be rendered on a card.
* Some users may have trouble uploading assets to a board.
* Group and entitlement changes made in user management only take effect after a new login.
* Admins must log out and back in to see changes made in Account Settings.
* Users are not able to share PowerPoint files on boards.
* Experience Cloud interface can reduce in performance when in parallel use by many users.
* Adobe Experience Manager to Creative Cloud synchronization is not working.

## October 2014

<table id="table_7C1ACE8108D54782AE128ACD35069DF5"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Edit User Permissions </p> </td> 
   <td colname="col2"> <p>Owners of a board can now edit user permissions on the particular board. </p> <p> 
     <ol id="ol_B12251C510744538AF9BCE60ACB04016"> 
      <li id="li_87B3EDE9542B47CEBE0BE7F2D1DE844D">On the board, select <span class="uicontrol"> Settings</span>. </li> 
      <li id="li_0F4786B0E1E743069D082E7DC488A031">Next to each owner, specify <span class="uicontrol"> Owner</span>, <span class="uicontrol"> Viewer</span>, or <span class="uicontrol"> Editor</span>. </li> 
     </ol> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes** 

* Creating a card from a PDF and sharing it to the board was returning an error message.

**Known Issues** 

* Some users may have trouble uploading assets to a board.
* Some `.png` files cannot be rendered on a card.
* Group and entitlement changes made in user management only take effect after a new login.
* Some users may not be able to create a card from a PDF and share it to a board.
* Some users are able to delete an out-of-date asset instead of receiving an error notification.
* Users are not able to share PowerPoint files on boards.
* Experience Cloud interface can reduce in performance when in parallel use by many users.
* The [!DNL Search&Promote] linking is not available from the [!UICONTROL Organizations & Product Access] page.

## September 2014

**Fixes and Improvements** 

* When you navigate to `experience.adobe.com`, the login experience is now consistent with Adobe's Creative Cloud login.
* On the Manage Organizations page, the linking experience (after an invite is received) is now consistent for each application.

**Known Issues** 

* Group and entitlement changes made in user management only take effect after a new login.
* Some users cannot create a card from a PDF and share it to a board.
* Some users may have trouble uploading assets to a board.
* Some users are able to delete an out-of-date asset instead of receiving an error notification.
* Users are not able to share PowerPoint files on boards.
* Some [!DNL .png] files cannot be rendered on a card.
* [!DNL Experience Cloud] interface can reduce in performance when in parallel use by many users.
* The [!DNL Search&Promote] linking is not available from the [!UICONTROL Organizations & Product Access] page.
* Some users may experience their [!DNL Creative Cloud] contents being removed from their folder, if the content is unshared in [!DNL Experience Cloud].

## August 2014

<table id="table_1E7DBEB5E83B4E4285B6FD1D718CD16D"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>You can now access <span class="keyword"> Adobe Mobile Services</span> from the left-hand navigation. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Known Issues** 

* Group and entitlement changes made in user management only take effect after a new login.
* Some users may not be able to create a card from a PDF and share it to a board.
* Some users may have trouble uploading assets to a board.
* Some users may not be able to log in from [!DNL Target] to [!DNL Experience Cloud].
* Some Audience Manager users cannot log into [!DNL Experience Cloud].
* Some users are able to delete an out-of-date asset instead of receiving an error notification.
* Files deleted from [!DNL Experience Cloud] are not being deleted from [!DNL Digital Asset Management].
* Users are not able to share PowerPoint files on boards.
* Some [!DNL .png] files cannot be rendered on a card.
* [!DNL Experience Cloud] interface can reduce in performance when in parallel use by many users.
* The [!DNL Search&Promote] linking is not available from the [!UICONTROL Organizations & Product Access] page.
* Some users may experience their [!DNL Creative Cloud] contents being removed from their folder, if the content is unshared in [!DNL Experience Cloud].

## July 2014

**Known Issues** 

* Files deleted from [!DNL Experience Cloud] are not being deleted from [!DNL Digital Asset Management].
* Some [!UICONTROL Exchange] users may find their names in the comments to be a long string ID instead of their names
* Some [!DNL .png] files cannot be rendered on a card
* Uploading files allows more file types than the drag-and-drop method. For best results, upload using [!UICONTROL Assets].
* The [!DNL Search&Promote] linking is not available from the [!UICONTROL Organizations & Product Access] page.
* [!DNL Exchange] users must clear their cookies to improve their experience.
* [!DNL Experience Cloud] interface can slow down when in parallel use by many users.
* Some users may experience their [!DNL Creative Cloud] contents being removed from their folder if the content is unshared in [!DNL Experience Cloud].
* You will be logged out after 15 minutes of inactivity. Also, logging out in one location logs you out of [!DNL Experience Cloud].
* Some users may not be able to link their Audience Manager accounts to [!DNL Experience Cloud].
* [!UICONTROL Exchange] users can only see English in language selector.

## June 2014

<table id="table_C9BD63436BF0414B97B8D07387D1993B"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="wintitle"> Save</span> button in Audiences </p> </td> 
   <td colname="col2"> <p>When you create an audience, the <span class="wintitle"> Save</span> button on the <span class="wintitle"> Create New Audience</span> page is now disabled until all the required fields are completed. 
     </p> </td> 
  </tr> 
 </tbody> 
</table>

**Known Issues** 

* Files deleted from [!DNL Experience Cloud] are not being deleted from [!DNL Digital Asset Management].
* Uploading files allows more file types than the drag-and-drop method. For best results, upload using Assets.
* The [!DNL Search&Promote] linking is not available from the [!UICONTROL Organizations & Product Access] page.
* Filters applied to trended reports from [!DNL Analytics] are not applied to cards in [!DNL Experience Cloud].
* Some users are not able to link their audience management account with their [!DNL Experience Cloud] account.
* You will be logged out after 15 minutes of inactivity. Also, logging out in one location logs you out of Experience Cloud.
* Some Exchange users may find their names in the comments to be a long string ID instead of their names

**Fixes** 

* Fixed an issue preventing video upload to apps.

## May 2014

<table id="table_4E4B34EEE3D94D78BA1A1FBC62950559"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Experience Cloud Exchange </p> </td> 
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol"> Help</span> &gt; <span class="uicontrol"> Exchange</span></p> <p>The <span class="keyword"> Experience Cloud</span><span class="wintitle"> Exchange</span> is a single destination where you can search, browse, select, pay, and download digital marketing extensions via apps. </p> <p>Apps include data connectors, custom configurations to Adobe's core product, third-party applications, reports, and <span class="keyword"> Experience Cloud</span> cards. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Experience Cloud Audiences </p> </td> 
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol"> Audiences</span></p> <p> <span class="wintitle"> Audiences</span> is where you create, edit, and manage audiences, similar to how you work with segments. For example, you can create a segment in Reports & Analytics, then share it to <span class="wintitle"> Experience Cloud</span><span class="wintitle"> Audiences</span>. Once shared, the audience is available in <span class="keyword"> Adobe Target</span> for campaign activities, and in Adobe Audience Manager for segmentation. </p> <p> <p>Note: To request enablement in Target, visit <a href="https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=X8SVES" format="http" scope="external"> https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=X8SVES</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Users who are mentioned on <span class="keyword"> Experience Cloud</span> cards now have permissions to that card. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>New Adobe users can link their Scene7 accounts to Adobe ID and their team members. Administrators can unlink users from Scene7 accounts as well. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Asset synchronization. </p> </td> 
   <td colname="col2"> <p> You can share assets within Experience Manager Assets with Experience Cloud and Creative Cloud. Any changes to these assets are reflected in the shared copies of the assets in Experience Cloud and Creative Cloud. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes** 

* [!DNL Experience Cloud] was not linking to [!DNL Adobe Target]. This issue occurred if the [!DNL Adobe Target] login can be used on multiple [!DNL Target] servers.
* [!DNL Adobe Advertising Cloud] was not creating users automatically when the user has been created in [!DNL Experience Cloud].
* Options in combo boxes used for adding new users temporarily disappeared while typing.
* The Comments link on asset card view was not selectable.
* After adding a custom tag to an asset, no other metadata changes were not persisting.
* Deleting an image, Assets does not warn if the image is used in Adobe Target Essentials.
* Slow [!UICONTROL Experience Cloud] interface performance when in parallel use by many users.
* Deleting an image in [!UICONTROL Experience Cloud Assets] was not issuing a warning if the image was used in [!DNL Adobe Target Essentials].
* When **[!UICONTROL remember me]** was not selected during login, the user was logged out after 15 minutes.
* Users were having to log out and back in for all permission and entitlement changes to take effect.
* Logging in to [!DNL Experience Cloud] was taking longer than a second.
* For certain users, deleting files from [!DNL Experience Cloud] did not synchronizing with [!DNL Digital Asset Management].
* Users were being logged out after only 15 minutes of browser inactivity.
* User were not able to share PowerPoint files on boards.
* Some users were experiencing poor visual layout in Internet Explorer 10.

## April 2014

<table id="table_D95C0DC64F2A4B47BAC83E504CFD6825"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Create cards from help topics </p> </td> 
   <td colname="col2"> <p>After you enable the Share to Adobe Experience Cloud feature in your browser's Bookmark toolbar, you can now share help pages from the microsite URL. </p> <p> <b>To share a help topic</b> </p> 
    <ol id="ol_F94B816121494B0FA16CC07B0E96AED8"> 
     <li id="li_F47187D4B5FE46D3A51D257DD569B4D6"> <p>In the <span class="keyword"> Experience Cloud</span>, select <span class="uicontrol"> Administration</span>. </p> </li> 
     <li id="li_94EF58E7A4974B63951E14F72A710183"> <p>Drag the <span class="uicontrol"> Share to Adobe Experience Cloud</span> button to your Bookmark toolbar. </p> </li> 
     <li id="li_69EEC4F25D8F4AD7AA106A10B7F50FF6"> <p>Navigate to a help page (or remain on this one), then select <span class="uicontrol"> Share to Adobe Experience Cloud</span> in your browser's Bookmarks toolbar. </p> <p>This step creates a card, which you can view in the <span class="wintitle"> Experience Cloud</span>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes**

* After adding a custom tag to an asset, no other metadata changes can be persisted.
* Users have to refresh the board to make the deleted cards disappear from view.
* When **[!UICONTROL Remember me]** is not selected during login, the user is logged out after 15 minutes
* [!DNL Analytics] application landing page shows formatting errors.
* Users must log out and log back in for all permission and entitlement changes to take effect.
* Deleting an image, [!UICONTROL Assets] does not warn if the image is used in [!DNL Adobe Target Essentials].
* Comments link on asset card view is not selectable.
* Options in combo boxes for adding new users temporarily disappear while typing.
* Logging in to [!DNL Experience Cloud] takes longer than a second.
* Data shared from [!DNL Advertising Cloud] is misrepresented in [!DNL Experience Cloud].
* Adobe [!DNL Advertising Cloud] does not create users automatically when user has been created in [!DNL Experience Cloud].
* [!DNL Experience Cloud] cannot be linked to [!DNL Adobe Target], if the [!DNL Adobe Target] login can be used on multiple [!DNL Target] servers.
* [!DNL Experience Cloud] interface can slow down when in parallel use by many users.
* [!DNL Search&Promote] linking is not available from the [!UICONTROL Organizations & Product Access] page.
* [!DNL Adobe Advertising Cloud] simulation cards are not rendering correctly.
* Filters applied to trended reports from [!DNL Analytics] are not applied to cards in [!DNL Experience Cloud].
* Filters applied to trended reports from Analytics are not applied to cards in Experience Cloud.
* Some Excel or CSV files cannot be uploaded to a board.
* Some users may not be able to link their audience management account with their [!DNL Experience Cloud].
* Some users may experience error when sharing [!DNL Analytics] segments in [!DNL Experience Cloud].
* Some users may not be able to drill down to subfolders in [!UICONTROL Asset Selector].
* Some users are not able to share AdLens gadgets in [!DNL Experience Cloud].

## March 2014

**Fixes** 

* Added the ability to remove your avatar image.
* Fixed an issue preventing you from unlinking your [!DNL Adobe Advertising Cloud] accounts.

**Known Issues** 

* Deleting an image in Experience Cloud Assets does not warn if the image is used in Adobe Target Essentials.
* Refreshing a card from [!DNL Analytics] can sometimes lead to an empty chart in the expanded card.
* Users must log out and log back in for all permission and entitlement changes to take effect.
* When *`Remember me`* is not selected during login, the user will be logged out after 15 minutes.
* [!DNL Analytics] application landing page shows formatting errors.
* The Comments link on asset card view is not selectable.
* Experience Cloud interface can slow down when in parallel use by many users
* Experience Cloud cannot be linked to [!DNL Adobe Target], if the [!DNL Adobe Target] login can be used on multiple Target servers.
* Logging in to Experience Cloud takes longer than a second.
* After adding a custom tag to an asset, no other metadata changes can be persisted.
* [!DNL Adobe Advertising Cloud] does not create users automatically when user has been created in Experience Cloud.
* Options in combo boxes for adding new users temporarily disappear while typing.
* Data shared from [!DNL Advertising Cloud] is mis-represented in Experience Cloud.
* Sharing Flickr images fails.
* Filters applied to trended reports from [!DNL Analytics] are not applied to cards in Experience Cloud.
* Group and entitlement changes made in user management only take effect after a new login.
* [!DNL Search&Promote] linking is not available from [!UICONTROL Organizations & Product Access].
* Users have to refresh the board to make the deleted cards disappear from view.
* Some Excel or CSV files cannot be uploaded to a board.
* [!DNL Adobe Advertising Cloud] simulation cards are not rendering correctly.
* Some PNG files cannot be rendered on a card.
* Beta feedback cannot be submitted.

## February 2014

<table id="table_DFAB002358C94A17A7F91DAB323A488F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Feature </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>OEmbed </p> </td> 
   <td colname="col2"> <p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Refresh Data </p> </td> 
   <td colname="col2"> <p> 
     The <span class="uicontrol"> Refresh Data</span> icon for a graph on a card is now hidden if the application does not allow a data refresh. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fixes** 

* Fixed an issue that prevented shared [!DNL Analytics] reports from applying segment filters.
* Fixed an issue causing applications to display on the [!UICONTROL Experience Cloud Solutions] page as linked, even if the applications accounts were not linked.
* Fixed an issue that prevented [!DNL Adobe Target] customers in Asia from being able to select the **[!UICONTROL Continue to Experience Cloud]** button on the linking page.
* Fixed an issue that prevented the sharing of YouTube videos.
 -->