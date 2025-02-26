---
title: Verwalten von Benutzer- und Produktlizenzen
description: Verwalten Sie Benutzende und Produktlizenzen in Admin Console für Experience Cloud-Programme.
application: Experience Cloud
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: c82821c4-aa5d-48ae-8bef-5937fede8db2
source-git-commit: 9932f21e4aa4d4a5bf08d7f1617b4c25d4fb14bb
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 3%

---

# Benutzerverwaltung und Produktlizenzen

Auf dieser Seite finden Sie Informationen speziell für Experience Cloud-Administratoren sowie Links zur allgemeinen Dokumentation für Benutzer- und Produktverwaltung.

Eine allgemeine Hilfe zur Identitätsverwaltung, die für alle Adobe-Programme gilt, finden Sie im [Enterprise and Teams Admin Guide](https://helpx.adobe.com/de/enterprise/admin-guide.html).

In den folgenden Abschnitten finden Sie Links zu Ressourcen in der Hilfe zu Admin Console.

## Administratorrollen in Admin Console

Admin Console verfügt über drei primäre Administrationsrollen mit jeweils spezifischen Zugriffs- und Verantwortungsebenen:

**Systemadministrator:** Vollzugriff - Verwaltet alle Aspekte der Konsole.

Wichtigste Zuständigkeiten:

* Hinzufügen, Entfernen und Verwalten von Benutzern.
* Produktlizenzen zuweisen und widerrufen.
* Konfigurieren Sie Identitäts- und Authentifizierungseinstellungen.
* Rechnungsinformationen anzeigen und verwalten
* Richten Sie zusätzliche Administratoren ein und delegieren Sie Rollen.

  **Am besten geeignet für** IT-Administratoren oder Teamleiter, die die Adobe-Umgebung des gesamten Unternehmens überwachen.

**Produktadministrator** Produktspezifische Verwaltung: Steuert den Zugriff und die Berechtigungen für bestimmte Adobe-Produkte.

Wichtigste Zuständigkeiten:

* Zuweisen und Verwalten von Lizenzen für ein bestimmtes Produkt.
* Erstellen und Verwalten von Produktprofilen.
* Hinzufügen oder Entfernen von Benutzern in zugewiesenen Produkten.

  **Best for:** Teams/Benutzer, die bestimmte Software wie Marketo Engage oder Adobe Creative Cloud verwalten.

**Produktprofil-Administrator** Granulare Rollenverwaltung: konzentriert sich auf die Verwaltung von Benutzergruppen und Berechtigungen innerhalb eines Produkts.

* Hauptaufgaben:
* Erstellen und Verwalten von Produktprofilen.
* Weisen Sie Berechtigungen und Funktionszugriff innerhalb von Profilen zu.
* Hinzufügen oder Entfernen von Benutzern innerhalb von Profilen.

  **Am besten geeignet für:** Abteilungsleiter oder Teammanager, die kleinere Gruppen mit speziellen Anforderungen überwachen

  Admins können je nach den Anforderungen des Unternehmens Rollen kombinieren, um eine größere Flexibilität zu erzielen.

## Einrichten von Admin Console

Um Identitäts- und Produktlizenzen für Experience Cloud-Programme zu verwalten, navigieren Sie zu [Admin Console](https://adminconsole.adobe.com/enterprise/).

* [Einrichten von Identität und Single Sign-on](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html) - Erfahren Sie, wie Sie die Konten Ihrer Benutzer mit verschiedenen ID-Typen mit oder ohne Single Sign-on (SSO) einrichten. Richten Sie SSO für die Adobe-Software ein, konfigurieren Sie SAML-Einstellungen und gehen Sie die häufigsten Fragen und Fehler durch.

* [Organisation über Verzeichnisvertrauen einrichten](https://helpx.adobe.com/enterprise/using/directory-trust.html) - Verwenden Sie Verzeichnisvertrauen, um Ihre Benutzer gegenüber einer Domain zu authentifizieren, die bereits von einer anderen Organisation beansprucht wurde.

  Informationen [ Organisationen finden Sie unter ](organizations.md) in Experience Cloud .

* [Authentifizierungseinstellungen (Unternehmen)](https://helpx.adobe.com/enterprise/using/authentication-settings.html) - Admin Console unterstützt verschiedene Kennwortschutzstufen und -richtlinien, um Sicherheit zu gewährleisten. Sie können festlegen, dass eine Kennwortschutzstufe für alle Benutzer in Ihrem Unternehmen gelten soll. Die Adobe-Kundenunterstützung bietet drei Sicherheitsstufen.

* [Datenschutz und Sicherheitskontakte](https://helpx.adobe.com/enterprise/using/security-contacts.html) - Adobe legt Wert auf den Schutz der Daten Ihres Unternehmens und Ihrer Benutzer. Im Falle eines Sicherheitsvorfalls, der unsere Softwarelösungen betrifft, werden Benachrichtigungen an die entsprechenden Compliance-Beauftragten gesendet.

  Unternehmen verfügen über eigenes Personal, dessen Rolle speziell für Datenschutz, Integrität und andere Compliance-Angelegenheiten zuständig ist. Daher sind Kontaktinformationen für dieses Personal von entscheidender Bedeutung, um eine umgehende Benachrichtigung im Fall eines Sicherheitsvorfalls zu gewährleisten.

## Benutzerverwaltung

* [Mehrere Benutzer verwalten](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) CSV-Massen-Upload - Erfahren Sie, wie Sie mehrere Benutzer über den CSV-Massen-Upload auf der Adobe Admin Console verwalten.

* [Identitätstypen](https://helpx.adobe.com/de/enterprise/using/identity.html) - Identitätstypen ermöglichen der Organisation verschiedene Ebenen der Kontrolle über die Konten und Daten von Benutzenden. Die Auswahl des Identitätsmodells wirkt sich darauf aus, wie Ihr Unternehmen Assets speichert und freigibt. Während Federated ID- und Enterprise ID-Modelle vom Unternehmen erstellt und verwaltet werden, werden Adobe-IDs vom Kontakt erstellt und verwaltet.

* [User Sync Tool](https://helpx.adobe.com/enterprise/using/user-sync.html) (UST) - Das Adobe User Sync Tool ist ein Desktop-Programm, mit dem der Prozess der Synchronisierung von Benutzerdaten zwischen dem Identitätsverwaltungssystem eines Unternehmens (wie Active Directory) und Adobes Adobe Admin Console automatisiert wird. Mit dem Tool können Admins die Benutzerbereitstellung, Aktualisierungen und Deaktivierung über Adobe-Produkte hinweg optimieren.

  Mit dem Tool zur Benutzersynchronisierung können Unternehmen die Verwaltung von Benutzerkonten und Lizenzen vereinfachen, indem Benutzerdaten (z. B. Rollen, Gruppen und Zugriffsberechtigungen) automatisch zwischen ihrem Verzeichnis-Service und Adobe-Systemen synchronisiert werden. Dieses Tool ist besonders für Unternehmen mit großen Teams nützlich. Dies trägt dazu bei, die Konsistenz und Sicherheit zu wahren und gleichzeitig sicherzustellen, dass Benutzende nur Zugriff auf die Produkte und Services haben, auf die sie Anspruch haben.

* [Benutzerdetails anzeigen (Admin-Tool)](admin-tool-experience-cloud.md) - Administratoren können eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und -Richtlinien mit Details im [!UICONTROL Admin-Tool] anzeigen.

## Berichte und Protokolle

* [Auditprotokoll](https://helpx.adobe.com/enterprise/using/audit-logs.html) Zum Nachverfolgen aller in Admin Console vorgenommenen Änderungen.

Hilfe, die oben nicht beschrieben ist, finden Sie im [Enterprise- und Team-Administratorhandbuch](https://helpx.adobe.com/de/enterprise/admin-guide.html).

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