---
title: Benutzer und Produkte verwalten
description: Erfahren Sie, wie Sie sich bei der Admin Console anmelden und Experience Cloud-Benutzerberechtigungen und -Produktprofile verwalten. Erfahren Sie mehr über die Zuweisung von Administratorrechten an Experience Cloud-Benutzer und über die Browserunterstützung für Experience Cloud.
solution: Admin
index: true
feature: Admin Console
topic: Administration
role: Administrator
level: Experienced
exl-id: af9eda5b-d984-44b7-a7b3-52dfc4e03d8f
source-git-commit: 0069c8b06cbacca6cd9fbdb898d4445931384ebb
workflow-type: tm+mt
source-wordcount: '1277'
ht-degree: 100%

---

# Verwalten von Experience Cloud-Benutzern und -produkten

Erfahren Sie mehr über die Anmeldung bei der Admin Console, die Verwaltung von Benutzerberechtigungen und Produktprofilen für Experience Cloud und über die Browser-Unterstützung.

>[!IMPORTANT]
>
>Die folgenden Informationen gelten speziell für Experience Cloud-Anwendungen. Diese Informationen ergänzen die im [Benutzerhandbuch für Enterprise-Administratoren](https://helpx.adobe.com/de/enterprise/admin-guide.html) enthaltenen allgemeinen Informationen für alle Adobe Cloud-Produkte.

Sie können im Admin-Tool eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und deren Details anzeigen. Siehe [Anzeigen von Experience Cloud-Benutzern im Admin-Tool](admin-tool-experience-cloud.md).

## Was ist ein Produktprofil? {#section_AB50558124D541CF80A0D3D76D35A4BF}

[!UICONTROL Produktprofile] sind Gruppen von Produkten und Diensten, die Sie Benutzern zuweisen können. In Experience Cloud basieren die Berechtigungen auf dem Produktprofil und nicht auf dem Benutzer. (Sie können jedoch bestimmten Benutzern Administratorrechte zuweisen.)

In Analytics können Sie beispielsweise eine Sammlung von Reporting-Tools wie Analysis Workspace und Report Builder sowie Report Suites, Metriken und Dimensionen konfigurieren. Sie können Berechtigungen für ein Produktprofil erteilen, indem Sie Benutzer zum Profil hinzufügen.

* Siehe [Analytics-Zugriffsberechtigungen einem Produktprofil zuweisen](admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) auf dieser Seite.
* Siehe [Delegieren von administrativen Rollen an Benutzer](#delegate-rights) auf dieser Seite

## Verwalten von Experience Cloud-Produktprofilen {#task_16335111C52D40E9BAC73D0699584DBF}

Sie können ein Produktprofil erstellen und es einer Berechtigungsgruppe zuweisen.

Wenn Sie einen Benutzer in eine Organisation einladen, können Sie dem Benutzer Zugriff auf Produkte und Produktprofile gewähren. Sie können auch eingeschränkte Administratorberechtigungen an einen Benutzer delegieren. Gleichermaßen können Sie Benutzergruppen erstellen und die Gruppe dann einem Produktprofil hinzufügen, um den Zugriff zu aktivieren.

1. Klicken Sie in der [Admin Console](https://adminconsole.adobe.com/enterprise/) auf **[!UICONTROL Produkte]**.
1. Klicken Sie auf den Namen Ihres Unternehmens.
1. Klicken Sie auf **[!UICONTROL Neues Profil]**.
1. Konfigurieren Sie die Profildetails und klicken Sie dann auf **[!UICONTROL Speichern]**.

Weitere Informationen (und Hilfe zur Produktverwaltung für Creative Cloud und Document Cloud) finden Sie unter [Identität](https://helpx.adobe.com/de/enterprise/admin-guide.html/de/enterprise/using/identity.ug.html) im [Administrations-Benutzerhandbuch](https://helpx.adobe.com/de/enterprise/admin-guide.html/de/enterprise/using/users.ug.html).

**Verwandte Hilfe.**

* [Produkte und Profile verwalten](https://helpx.adobe.com/de/enterprise/admin-guide.html/de/enterprise/using/manage-products.ug.html) im Administrations-Benutzerhandbuch.
* [Enterprise-Benutzerberechtigungen](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=de) in der Hilfe zu Adobe Target.
* Video: [Konfigurieren von Adobe Target-Arbeitsbereichen in der Adobe Admin Console](https://helpx.adobe.com/de/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

<!-- ## What's new in Experience Cloud user management {#concept_06A0A13362F644FB90F947238407637A}

Learn about the latest features in Experience Cloud user and product management.

### Business ID type

Adobe is introducing an identity type called Business ID. This identity type improves the control of user and product management. Adobe is migrating all Adobe IDs (owned by individuals) that are used for business to the new enterprise Business IDs owned by your organization.

If you are an existing Experience Cloud customer, Adobe will migrate all your users with Adobe IDs in the Admin Console to Business IDs. If you are a new enterprise or teams customer, you will add users to the Admin Console using one of the available identity types: Business ID, Enterprise ID, or Federated ID.

What to do

* Your users will need to accept Terms of Use (TOU) changes prior to accounts being migrated to Type2e. 
* Users that belong to multiple organizations might see a Profile Selection screen during the login workflow and need to select the correct one. This ensures that they are logging into the correct organization. (There might be multiple profiles to choose from if a user was a member of multiple organizations before the migration.)

Beginning May 2020, enterprise administrators cannot use the Adobe ID for new organizations created in the Admin Console. Latest: https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=engage&title=Type2e+DX+GTM-->

## Delegieren von administrativen Rollen an Benutzer {#delegate-rights}

In der Admin Console können Sie eingeschränkte Administratorrechte an andere Personen in Ihrem Unternehmen delegieren. Delegierte Rollen ermöglichen es Benutzern, den Softwarezugriff für Endbenutzer zu verwalten, Zugriffsimplementierungsfunktionen bereitzustellen und als Stellvertreter des Supports zu fungieren.

Sie können zum Beispiel:

* Ihren Creative Director Zugriff auf die Creative Cloud gewähren lassen.
* Ihren Marketing Director Zugriff auf die Experience Cloud gewähren lassen.
* Halten Sie diese beiden Rollen getrennt, damit sie die jeweils andere Rolle nicht überschreiten können.

Mithilfe dieser Rollen können Sie die Verwaltung gleichzeitig an andere delegieren, ohne mehr Funktionen bereitzustellen, als benötigt werden.

1. Klicken Sie in der Admin Console auf **[!UICONTROL Benutzer]** und anschließend auf den entsprechenden Benutzernamen.

   ![](assets/edit-admin-rights.png)

1. Klicken Sie auf **[!UICONTROL Administratorrechte bearbeiten]**.

   ![](assets/edit-admin-rights-page.png)

1. Legen Sie die Administratorrechte des Benutzers fest.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Analytics-Benutzer und -Produkte verwalten {#section_97DE101F92CD494AB073893680992F1A}

Sie können Zugriffsberechtigungen für Analytics-Berichte (Report Suites, Metriken, Dimensionen usw.) einem Produktprofil zuweisen.

Sie können beispielsweise ein Produktprofil erstellen, das mehrere Analytics-Tools enthält ([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics] und [!UICONTROL Report Builder]). Diese Profile enthalten Berechtigungen für bestimmte Metriken und Dimensionen (einschließlich eVars) sowie Funktionen wie Segmente oder die Erstellung berechneter Metriken.

1. Melden Sie sich bei [Admin Console](https://adminconsole.adobe.com/enterprise) an und klicken Sie dann auf **[!UICONTROL Produkte]**.
1. Klicken Sie auf der Seite [!UICONTROL Produkte] auf Ihr Produkt, klicken Sie dann auf **[!UICONTROL Berechtigungen]** (nur für Administratoren verfügbar).
1. Konfigurieren Sie die Profilberechtigungen:

| Element | Beschreibung |
|--- |--- |
| Report Suites | Aktivieren Sie Berechtigungen für bestimmte Report Suites. |
| Metriken | Aktivieren Sie Berechtigungen für Traffic, Konversion, benutzerspezifische Ereignisse, Lösungsereignisse, Inhaltsbewahrung usw. |
| Dimensionen | Passen Sie den Benutzerzugriff auf einer granularen Ebene an, einschließlich eVars, Traffic-Berichten, Lösungsberichten und Pfadberichten. |
| Report Suite-Tools | Aktivieren Sie Benutzerberechtigungen für Webdienste, Report Suite-Verwaltung, Tools und Berichte sowie Dashboard-Elemente. |
| Analytics-Tools | Gewähren Sie Benutzern Zugriff auf allgemeine Elemente (Abrechnung, Protokolle usw.), Unternehmensverwaltung, Tools, Web-Services, Report Builder und die Data Connectors-Integration. Die Unternehmenseinstellungen aus der Kategorie „Anpassung der Admin Console“ sind nun in den Analytics-Tools zu finden. |

**Migration von Benutzerkonten**

Analytics-Administratoren können Benutzerkonten mithilfe des verfügbaren Analytics-Migrationstools für Benutzer-IDs von der Analytics-Benutzerverwaltung in die [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/) migrieren.

Die Kontomigration erfolgt für Kunden stufenweise. Adobe wird Sie benachrichtigen und unterstützen, wenn Sie an der Reihe sind, Ihre bestehenden Benutzerkonten von **[!UICONTROL Admin Tools]** > **[!UICONTROL Benutzerverwaltung]** in die Admin Console zu migrieren.

Nach der Migration müssen sich Benutzer mithilfe ihrer Adobe ID (oder Enterprise ID) anmelden und sich unter [experience.adobe.com](https://experience.adobe.com) für ihre Experience Cloud-Lösungen und -Dienste authentifizieren. Benutzer, die versuchen, sich über die bisherigen Anmeldedaten anzumelden ([!DNL my.omniture.com], [!DNL sc.omniture.com] und [!DNL experiencecloud.adobe.com]), werden an [!DNL experience.adobe.com] weitergeleitet.

**Verwandte Hilfe.**

Weitere Informationen finden Sie unter [Migration der Analytics-Benutzer-ID](https://experienceleague.adobe.com/docs/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html?lang=de).

## Adobe Target verwalten – Produktprofile und Arbeitsbereiche im Vergleich {#section_3860AF177C9E4C7E9C390D36A414F353}

In Adobe Target ist ein Arbeitsbereich ein Produktprofil. Er ermöglicht einer Organisation das Zuweisen bestimmter Benutzergruppen zu bestimmten Eigenschaftsgruppen. Arbeitsbereiche ähneln auf vielerlei Weise den Report Suites in Adobe Analytics.

Siehe:

* [Berechtigungen für Unternehmensbenutzer](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=en)
* [Verwalten von Produkten und Profilen](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/manage-products.ug.html)
* Video: [Konfigurieren von Adobe Target-Arbeitsbereichen in der Adobe Admin Console](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Campaign – Produktprofile, Mandanten und Sicherheitsgruppen verwalten {#section_09CDF75366444CF5810CF321B7C712F3}

Ein *Mandant* wird in Campaign auf der Seite „Produkte der Admin Console“ als *Produkt* angezeigt.

Die *Sicherheitsgruppe* wird als Produktprofil angezeigt.

Informationen zu Sicherheitsgruppen und zum Zuweisen von Benutzern zu Sicherheitsgruppen finden Sie unter [Verwalten von Gruppen und Benutzern](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/users-and-security/managing-groups-and-users.html?lang=de).

## Verwalten der Experience Platform-Datenerfassung (Launch) {#section_F2DA6778DD2D48AA8F794041971EE6B1}

Experience Platform [!UICONTROL Datenerfassung] ([!UICONTROL Launch]) wird auf der Seite [!UICONTROL Produkte] in der [!UICONTROL Admin Console] angezeigt. Sie können weitere Lösungen und Dienste in ein Launch-Produktprofil aufnehmen.

Laden Sie Benutzer zu [!UICONTROL Platform Launch] ein und weisen Sie ihnen Benutzerrollen und -rechte zu.

Informationen zu Benutzerberechtigungen in der Admin Console und zum Einrichten Launch-spezifischer Optionen, einschließlich der Zuweisung von Rechten zu Profilen, finden Sie unter [Benutzerverwaltung](https://experienceleague.adobe.com/docs/launch/using/admin/user-permissions.html?lang=de#admin).

## Experience Manager as a Cloud Service

Adobe Enterprise-Kunden werden in der Adobe [!UICONTROL Admin Console] als Organisationen dargestellt. Experience Manager-Kunden können die Adobe [!UICONTROL Admin Console] verwenden, um ihre Produktberechtigungen und die IMS-Authentifizierung für Experience Manager als [!UICONTROL Cloud Service] zu verwalten.

Siehe [IMS-Unterstützung für Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/security/ims-support.html?lang=de).

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Erstellen Sie Audience Manager-Benutzer und weisen Sie sie Gruppen zu. Sie können auch Einschränkungen anzeigen (Eigenschaften, Segmente, Ziele und [!DNL AlgoModel]).

Siehe [Administration](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/administration/administration-overview.html?lang=de) in der Hilfe zu Audience Manager.

## Unterstützte Browser in der Experience Cloud

* [!DNL Microsoft® Edge] (Microsoft® hat für Internet Explorer 8, 9 und 10 den [Support beendet](https://www.microsoft.com/de-de/WindowsForBusiness/End-of-IE-support). Aus diesem Grund werden von Adobe keine Probleme mehr behoben, die in Verbindung mit diesen speziellen Versionen von Internet Explorer gemeldet werden.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**Hinweis:** Obwohl die Experience Cloud-Oberfläche diese Browser unterstützt, unterstützen einzelne Anwendungen nicht alle Browser. ([Analytics](https://experienceleague.adobe.com/docs/analytics/admin/sys-reqs.html?lang=de) unterstützt beispielsweise nicht [!DNL Opera] und [Adobe Target](https://experienceleague.adobe.com/docs/target/using/implement-target/before-implement/supported-browsers.html?lang=de) unterstützt nicht [!DNL Safari].)

### Anforderungen an Lösungen und Produkte

* [Analytics](https://experienceleague.adobe.com/docs/analytics/admin/sys-reqs.html?lang=en)
* [Report Builder ](https://experienceleague.adobe.com/docs/analytics/analyze/report-builder/report-builder-setup/system-requirements.html?lang=de)
* [Adobe Target](https://experienceleague.adobe.com/docs/target/using/implement-target/before-implement/supported-browsers.html?lang=en)
