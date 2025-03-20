---
title: Verwalten von Benutzer- und Produktlizenzen
description: Verwalten Sie Benutzende und Produktlizenzen in der Admin Console für Experience Cloud-Anwendungen.
application: Experience Cloud
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: c82821c4-aa5d-48ae-8bef-5937fede8db2
source-git-commit: ce65c5292caaa4a24945e2119e78fd97a7d84109
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 7%

---

# Benutzerverwaltung und Produktlizenzen

Sie können Benutzende und Produktlizenzen in der Adobe [Admin Console](https://adminconsole.adobe.com/enterprise/) verwalten. Eine allgemeine Hilfe zur Identitätsverwaltung, die für alle Adobe-Programme gilt, finden Sie im [Enterprise and Teams Admin Guide](https://helpx.adobe.com/de/enterprise/admin-guide.html).

Diese Seite enthält Informationen, die speziell für Experience Cloud-Administratoren nützlich sind, definiert Rollen und enthält Links zu allgemeinen Themen zur Benutzer- und Produktverwaltung im Enterprise-Handbuch.

## Administratorrollen in Admin Console

Admin Console verfügt über drei primäre Administrationsrollen mit jeweils spezifischen Zugriffs- und Verantwortungsebenen:

| Rolle | Beschreibung |
| ------- | ------- |
| Systemadministrator | Vollständiger Zugriff : Verwaltet alle Aspekte der Konsole. <br>Wichtigste Zuständigkeiten: <br><ul><li>Hinzufügen, Entfernen und Verwalten von Benutzern.</li><li>Produktlizenzen zuweisen und widerrufen.</li><li>Konfigurieren von Identitäts- und Authentifizierungseinstellungen</li><li>Rechnungsinformationen anzeigen und verwalten</li><li>Richten Sie zusätzliche Administratoren ein und delegieren Sie Rollen.</li></ul> **Am besten geeignet für** IT-Administratoren oder Teamleiter, die die Adobe-Umgebung des gesamten Unternehmens überwachen. |
| Produkt-Administrator | Produktspezifische Verwaltung - Steuert den Zugriff und die Berechtigungen für bestimmte Adobe-Produkte.<br>Wichtigste Zuständigkeiten:<ul><li>Zuweisen und Verwalten von Lizenzen für ein bestimmtes Produkt.</li><li>Erstellen und Verwalten von Produktprofilen.</li><li>Hinzufügen oder Entfernen von Benutzern in zugewiesenen Produkten.</li></ul>   **Best for:** Teams/Benutzer, die bestimmte Software wie Marketo Engage oder Adobe Creative Cloud verwalten. |
| Produktprofil-Administrator | Granulare Rollenverwaltung: Mit Augenmerk auf die Verwaltung von Benutzergruppen und Berechtigungen innerhalb eines Produkts.<br>Hauptaufgaben:<ul><li>Erstellen und Verwalten von Produktprofilen.</li><li>Weisen Sie Berechtigungen und Funktionszugriff innerhalb von Profilen zu.</li><li>Hinzufügen oder Entfernen von Benutzern innerhalb von Profilen.</li></ul> **Am besten geeignet für:** Abteilungsleiter oder Teamleiter, die kleinere Gruppen mit speziellen Anforderungen überwachen. <br> können je nach den Anforderungen des Unternehmens Rollen kombinieren, um eine größere Flexibilität zu erzielen. |

## Admin Console für Experience Cloud

Um Identitäts- und Produktlizenzen für Experience Cloud-Programme zu verwalten, navigieren Sie zu [Admin Console](https://adminconsole.adobe.com/enterprise/).

Hier finden Sie Ressourcen, die Sie möglicherweise benötigen, wenn Sie als Administrator in Admin Console beginnen möchten:

### Einrichten von Ressourcen

| Hilfe-Link | Beschreibung |
| ------- | ------ |
| [Einrichten von Identität und Single Sign-on](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html) | **[!UICONTROL Admin Console]** > **[!UICONTROL Einstellungen]** <br> Erfahren Sie, wie Sie Benutzerkonten mit verschiedenen ID-Typen einrichten können, mit oder ohne Single Sign-on (SSO). Richten Sie SSO für die Adobe-Software ein, konfigurieren Sie SAML-Einstellungen und gehen Sie die häufigsten Fragen und Fehler durch. |
| [Einrichten der Organisation über Verzeichnisvertrauen](https://helpx.adobe.com/enterprise/using/directory-trust.html) | Authentifizieren Sie Ihre Benutzer gegenüber einer Domain, die bereits von einer anderen Organisation beansprucht wurde. Informationen zum Suchen und Wechseln von Organisationen finden Sie unter [Organisationen in Experience Cloud](organizations.md). |
| [Authentifizierungseinstellungen (Unternehmen)](https://helpx.adobe.com/enterprise/using/authentication-settings.html) | Admin Console unterstützt verschiedene Kennwortschutzstufen und -richtlinien, um Sicherheit und Schutz zu gewährleisten. Sie können festlegen, dass eine Kennwortschutzstufe für alle Benutzer in Ihrem Unternehmen gelten soll. |
| [Datenschutz und Sicherheitskontakte](https://helpx.adobe.com/enterprise/using/security-contacts.html) | Schützen Sie die Daten Ihrer Organisation und Benutzer. Wenn ein Sicherheitsvorfall im Zusammenhang mit unseren Softwarelösungen auftritt, werden Benachrichtigungen an die entsprechenden Compliance-Beauftragten gesendet. Unternehmen verfügen über Mitarbeiter, deren Rolle speziell auf Datenschutz, Integrität und andere Compliance-Aspekte ausgerichtet ist. Daher sind Kontaktinformationen für dieses Personal von entscheidender Bedeutung, um eine umgehende Benachrichtigung im Fall eines Sicherheitsvorfalls zu gewährleisten. |

### Benutzerverwaltung

| Hilfe-Link | Beschreibung |
| ------- | ------- |
| [Verwalten mehrerer Benutzer](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) | **[!UICONTROL Admin Console]** > **[!UICONTROL Benutzer]** <br>Erfahren Sie, wie Sie mehrere Benutzer über den CSV-Massen-Upload in die Admin Console verwalten. |
| [Identitätstypen](https://helpx.adobe.com/de/enterprise/using/identity.html) | Identitätstypen ermöglichen dem Unternehmen verschiedene Ebenen der Kontrolle über die Konten und Daten der Benutzer. Die Auswahl des Identitätsmodells wirkt sich darauf aus, wie Ihr Unternehmen Assets speichert und freigibt. Während Federated ID- und Enterprise ID-Modelle vom Unternehmen erstellt und verwaltet werden, werden Adobe-IDs vom Kontakt erstellt und verwaltet. |
| [User Sync Tool](https://helpx.adobe.com/enterprise/using/user-sync.html) (UST) | Das Adobe User Sync Tool ist ein Desktop-Programm, mit dem die Synchronisierung von Benutzerdaten zwischen dem Identitätsverwaltungssystem eines Unternehmens (z. B. Active Directory) und Adobe Admin Console automatisiert wird. Mit dem Tool können Admins die Benutzerbereitstellung, Aktualisierungen und Deaktivierung über Adobe-Produkte hinweg optimieren. |
| [Anzeigen von Benutzerdetails (Admin-Tool)](admin-tool-experience-cloud.md) | Eine sortierbare und filterbare Liste aller Experience Cloud-Benutzenden und -Richtlinien mit Details im [!UICONTROL Admin-Tool] anzeigen. |

### Berichte und Protokolle

| Hilfe-Link | Beschreibung |
| ------- |------- |
| [Auditprotokoll](https://helpx.adobe.com/enterprise/using/audit-logs.html) | **[!UICONTROL Insights]** > **[!UICONTROL Protokolle]** > **[!UICONTROL Auditprotokoll]** <br> alle in Admin Console vorgenommenen Änderungen verfolgen. |


## Anwendungsspezifische Ressourcen

Über diese Links finden Sie Administrationsinformationen zu bestimmten Experience Cloud-Programmen.

<!-- | Application | Link to resource|
| ------- | ------- |
|  [!DNL Analytics] <p>Customer Journey Analytics| [Analytics in the Adobe Admin Console overview](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-console/home) <p>[Administration requirements](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/frequently-asked-questions-analysis-workspace) |
| [!DNL Audience Manager] | [Audience Manager user migration to Admin Console](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/administration/admin-console-migration) |
| [!DNL Campaign] v8 |  [Get started with permissions](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions) |
| [!DNL Campaign Standard] to [!DNL Campaign v8] | [User access management from Campaign Standard to Campaign V8](https://experienceleague.adobe.com/en/docs/campaign-web/acs-to-ac/user-management-acs) |
| [!DNL Commerce] | [Configure the Commerce Admin Integration with Adobe ID](https://experienceleague.adobe.com/en/docs/commerce-admin/start/admin/ims/adobe-ims-config) |
| [!DNL Dynamic Media Classic] | [Administration setup](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/setup/administration-setup#user_administration) |
| [!DNL Experience Manager as a Cloud Service] |  [Accessing the Admin Console](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console) |
| [!DNL Experience Platform] <p>[!DNL Data Collection] | [Access control UI overview](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/overview) <p>[Permission management for data collection in Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/collection/permissions)|
| [!DNL GenStudio for Performance Marketing] | [Provision Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/product-provisioning) |
| [!DNL Journey Optimizer] | [Manage users and roles](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions) |
| [!DNL Journey Optimizer B2B Edition] | [User management](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/admin/user-management) |
|[!DNL  Journey Orchestration] | [Access management](https://experienceleague.adobe.com/en/docs/journeys/using/starting-with-journeys/access-management) |
| [!DNL Marketo Engage] | [Understanding Marketo Subscription and User Migration to the Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console) |
| [!DNL Marketo Measure] | [Adobe Admin Console Setup](https://experienceleague.adobe.com/en/docs/marketo-measure/using/configuration-and-setup/getting-started-with-marketo-measure/adobe-admin-console-setup) |
| [!DNL Mix Modeler] | [Access controls](https://experienceleague.adobe.com/en/docs/mix-modeler/using/data-governance/access-controls) |
| [!DNL Pass] | [Get started with Account IQ](https://experienceleague.adobe.com/en/docs/pass/aiq-help/get-started) |
| [!DNL Target] | [Administrator first steps](https://experienceleague.adobe.com/en/docs/target/using/administer/start-target) <p> [User management](https://experienceleague.adobe.com/en/docs/target/using/administer/manage-users/user-management) |
| [!DNL Workfront] | [Manage users in the Adobe Admin Console](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/add-users/create-manage-users/admin-console) |

 -->

* [Analytics](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-console/home)
* [Customer Journey Analytics](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/frequently-asked-questions-analysis-workspace)
* [Audience Manager](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/administration/admin-console-migration)
* [Campaign v8](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/admin/permissions/gs-permissions)
* [Campaign Standard](https://experienceleague.adobe.com/en/docs/campaign-web/acs-to-ac/user-management-acs)
* [Commerce](https://experienceleague.adobe.com/en/docs/commerce-admin/start/admin/ims/adobe-ims-config)
* [Dynamic Media Classic](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/setup/administration-setup#user_administration)
* [Experience Manager as a Cloud Service](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console)
* [Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/overview) und [Datenerfassung](https://experienceleague.adobe.com/en/docs/experience-platform/collection/permissions)
* [GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/product-provisioning)
* [Journey Optimizer](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions)
* [Journey Optimizer B2B edition](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/admin/user-management)
* [Journey Orchestration](https://experienceleague.adobe.com/en/docs/journeys/using/starting-with-journeys/access-management)
* [Marketo Engage](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console)
* [Marketo Measure](https://experienceleague.adobe.com/en/docs/marketo-measure/using/configuration-and-setup/getting-started-with-marketo-measure/adobe-admin-console-setup)
* [Mix Modeler](https://experienceleague.adobe.com/en/docs/mix-modeler/using/data-governance/access-controls)
* [Adobe Pass](https://experienceleague.adobe.com/en/docs/pass/aiq-help/get-started)
* [Zielgruppe](https://experienceleague.adobe.com/en/docs/target/using/administer/start-target)
* [Workfront](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/add-users/create-manage-users/admin-console)

Der Großteil der Admin Console-Hilfe für alle Adobe-Programme ist im [Enterprise- und Team-Administratorhandbuch“ ](https://helpx.adobe.com/de/enterprise/admin-guide.html).
