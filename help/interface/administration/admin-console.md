---
title: Verwalten von Benutzer- und Produktlizenzen
description: Verwalten Sie Benutzende und Produktlizenzen in Admin Console für CX Enterprise-Anwendungen.
application: Experience Cloud
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: c82821c4-aa5d-48ae-8bef-5937fede8db2
autotag-review: '2026-05-12T21:16:07.250Z'
TQID: 'https://experienceleague.adobe.com/tONTr5mo5qLUxNS-q-uHGMCc5jKkURApIR-2RW0aV3w'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: eb7e29b9-c5e9-4ed0-8e4b-6465dabb3cb1
  - id: f1299f18-ec4b-4531-b2a2-df3b94ff9a68
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: d00e9f03-e50b-4162-b143-0c0817c937c2
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 9c2010694b8bb32c3922dd65f846375e43b2caac
workflow-type: tm+mt
source-wordcount: 1073
ht-degree: 8%

---

# Benutzer- und Produktverwaltung

Sie können Benutzende und Produktlizenzen in der Adobe [Admin Console](https://adminconsole.adobe.com/enterprise/) verwalten. Eine allgemeine Hilfe zur Identitätsverwaltung, die für alle Adobe-Programme gilt, finden Sie im [Enterprise and Teams Admin Guide](https://helpx.adobe.com/de/enterprise/admin-guide.html).

Diese Seite enthält Informationen, die speziell für CX Enterprise-Administratoren nützlich sind, definiert Rollen und enthält Links zu allgemeinen Themen des Benutzer- und Produktmanagements im Enterprise-Handbuch.

## Administratorrollen in Admin Console

Admin Console verfügt über drei primäre Administrationsrollen mit jeweils spezifischen Zugriffs- und Verantwortungsebenen:

| Rolle | Beschreibung |
| ------- | ------- |
| Systemadministrator | Vollständiger Zugriff : Verwaltet alle Aspekte der Konsole. <br>Wichtigste Zuständigkeiten: <br><ul><li>Hinzufügen, Entfernen und Verwalten von Benutzern.</li><li>Produktlizenzen zuweisen und widerrufen.</li><li>Konfigurieren von Identitäts- und Authentifizierungseinstellungen</li><li>Rechnungsinformationen anzeigen und verwalten</li><li>Richten Sie zusätzliche Administratoren ein und delegieren Sie Rollen.</li></ul> **Am besten geeignet für** IT-Administratoren oder Teamleiter, die die Adobe-Umgebung des gesamten Unternehmens überwachen. |
| Produkt-Administrator | Produktspezifische Verwaltung - Steuert den Zugriff und die Berechtigungen für bestimmte Adobe-Produkte.<br>Wichtigste Zuständigkeiten:<ul><li>Zuweisen und Verwalten von Lizenzen für ein bestimmtes Produkt.</li><li>Erstellen und Verwalten von Produktprofilen.</li><li>Hinzufügen oder Entfernen von Benutzern in zugewiesenen Produkten.</li></ul>   **Best for:** Teams/Benutzer, die bestimmte Software wie Marketo Engage oder Adobe Creative Cloud verwalten. |
| Produktprofil-Administrator | Granulare Rollenverwaltung: Mit Augenmerk auf die Verwaltung von Benutzergruppen und Berechtigungen innerhalb eines Produkts.<br>Hauptaufgaben:<ul><li>Erstellen und Verwalten von Produktprofilen.</li><li>Weisen Sie Berechtigungen und Funktionszugriff innerhalb von Profilen zu.</li><li>Hinzufügen oder Entfernen von Benutzern innerhalb von Profilen.</li></ul> **Am besten geeignet für:** Abteilungsleiter oder Teamleiter, die kleinere Gruppen mit speziellen Anforderungen überwachen. <br> Admins können je nach den Anforderungen des Unternehmens Rollen kombinieren, um eine größere Flexibilität zu erzielen. |

## Admin Console für CX Enterprise

Um Identitäts- und Produktlizenzen für CX Enterprise-Anwendungen zu verwalten, navigieren Sie zur [Admin Console](https://adminconsole.adobe.com/enterprise/).

Hier finden Sie Ressourcen, die Sie möglicherweise benötigen, wenn Sie als Administrator in Admin Console beginnen möchten:

### Einrichten von Ressourcen

| Hilfe-Link | Beschreibung |
| ------- | ------ |
| [Einrichten von Identität und Single Sign-on](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html) | **[!UICONTROL Admin Console]** > **[!UICONTROL Einstellungen]** <br> Erfahren Sie, wie Sie Benutzerkonten mit verschiedenen ID-Typen einrichten können, mit oder ohne Single Sign-on (SSO). Richten Sie SSO für die Adobe-Software ein, konfigurieren Sie SAML-Einstellungen und gehen Sie die häufigsten Fragen und Fehler durch. |
| [Einrichten der Organisation über Verzeichnisvertrauen](https://helpx.adobe.com/enterprise/using/directory-trust.html) | Authentifizieren Sie Ihre Benutzer gegenüber einer Domain, die bereits von einer anderen Organisation beansprucht wurde. Informationen zum Suchen und Wechseln von Organisationen finden Sie unter [Organisationen in CX Enterprise](organizations.md). |
| [Authentifizierungseinstellungen (Unternehmen)](https://helpx.adobe.com/enterprise/using/authentication-settings.html) | Admin Console unterstützt verschiedene Kennwortschutzstufen und -richtlinien, um Sicherheit und Schutz zu gewährleisten. Sie können festlegen, dass eine Kennwortschutzstufe für alle Benutzer in Ihrem Unternehmen gelten soll. |
| [Datenschutz und Sicherheitskontakte](https://helpx.adobe.com/enterprise/using/security-contacts.html) | Schützen Sie die Daten Ihrer Organisation und Benutzer. Wenn ein Sicherheitsvorfall im Zusammenhang mit unseren Softwarelösungen auftritt, werden Benachrichtigungen an die entsprechenden Compliance-Beauftragten gesendet. Unternehmen verfügen über Mitarbeiter, deren Rolle speziell auf Datenschutz, Integrität und andere Compliance-Aspekte ausgerichtet ist. Daher sind Kontaktinformationen für dieses Personal von entscheidender Bedeutung, um eine umgehende Benachrichtigung im Fall eines Sicherheitsvorfalls zu gewährleisten. |

### Benutzerverwaltung

| Hilfe-Link | Beschreibung |
| ------- | ------- |
| [Adobe ID zurücksetzen](https://helpx.adobe.com/account/individual/sign-in-and-security/security-and-recovery/cant-sign-in-to-adobe-account.html) | Melden Sie sich ab und klicken Sie dann auf **[!UICONTROL Hilfe bei der Anmeldung]** > **[!UICONTROL Kennwort zurücksetzen]**. |
| [Verwalten mehrerer Benutzer](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) | **[!UICONTROL Admin Console]** > **[!UICONTROL Benutzer]** <br>Erfahren Sie, wie Sie mehrere Benutzer über den CSV-Massen-Upload in die Admin Console verwalten. |
| [Identitätstypen](https://helpx.adobe.com/de/enterprise/using/identity.html) | Identitätstypen ermöglichen dem Unternehmen verschiedene Ebenen der Kontrolle über die Konten und Daten der Benutzer. Die Auswahl des Identitätsmodells wirkt sich darauf aus, wie Ihr Unternehmen Assets speichert und freigibt. Während Federated ID- und Enterprise ID-Modelle vom Unternehmen erstellt und verwaltet werden, werden Adobe-IDs vom Kontakt erstellt und verwaltet. |
| [User Sync Tool](https://helpx.adobe.com/enterprise/using/user-sync.html) (UST) | Das Adobe User Sync Tool ist ein Desktop-Programm, mit dem die Synchronisierung von Benutzerdaten zwischen dem Identitätsverwaltungssystem eines Unternehmens (z. B. Active Directory) und Adobe Admin Console automatisiert wird. Mit dem Tool können Admins die Benutzerbereitstellung, Aktualisierungen und Deaktivierung über Adobe-Produkte hinweg optimieren. |
| [Anzeigen von Benutzerdetails (Admin-Tool)](admin-tool-experience-cloud.md) | Eine sortierbare und filterbare Liste aller CX Enterprise-Benutzer und -Richtlinien mit Details im [!UICONTROL Admin-Tool] anzeigen. |

### Berichte und Protokolle

| Hilfe-Link | Beschreibung |
| ------- | ------- |
| [Auditprotokoll](https://helpx.adobe.com/enterprise/using/audit-logs.html) | **[!UICONTROL Insights]** > **[!UICONTROL Protokolle]** > **[!UICONTROL Auditprotokoll]** <br> alle in Admin Console vorgenommenen Änderungen verfolgen. |


## Anwendungsspezifische Ressourcen

Über diese Links finden Sie Administrationsinformationen zu bestimmten CX Enterprise-Anwendungen.

<!--
| Application | Link to resource|
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

* [Advertising Search, Social und Commerce](https://experienceleague.adobe.com/en/docs/advertising/search-social-commerce/target/user-administration)
* [Analytics](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-console/home)
* [Customer Journey Analytics](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/frequently-asked-questions-analysis-workspace)
* [Audience Manager](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/administration/admin-console-migration)
* [Campaign v8](https://experienceleague.adobe.com/de/docs/campaign/campaign-v8/permissions/gs-permissions)
* [Campaign Standard](https://experienceleague.adobe.com/en/docs/campaign-web/acs-to-ac/user-management-acs)
* [Commerce](https://experienceleague.adobe.com/en/docs/commerce-admin/start/admin/ims/adobe-ims-config)
* [Dynamic Media Classic](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/setup/administration-setup#user_administration)
* [Experience Manager as a Cloud Service](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console)
* [Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/overview) und [Datenerfassung](https://experienceleague.adobe.com/en/docs/experience-platform/collection/permissions)
* [GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/product-provisioning)
* [Journey Optimizer](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions)
* [Journey Optimizer B2B edition](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/admin/user-management)
* [Journey Orchestration](https://experienceleague.adobe.com/en/docs/journeys/using/starting-with-journeys/access-management)
* [Marketo Engage](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console)
* [Marketo Measure](https://experienceleague.adobe.com/en/docs/marketo-measure/using/configuration-and-setup/getting-started-with-marketo-measure/adobe-admin-console-setup)
* [Mix Modeler](https://experienceleague.adobe.com/en/docs/mix-modeler/using/data-governance/access-controls)
* [Target](https://experienceleague.adobe.com/en/docs/target/using/administer/start-target)
* [Workfront](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/add-users/create-manage-users/admin-console)

Der Großteil der Admin Console-Hilfe für alle Adobe-Programme ist im [Enterprise- und Team-Administratorhandbuch“ &#x200B;](https://helpx.adobe.com/de/enterprise/admin-guide.html).

