---
description: Erfahren Sie mehr über die Anmeldung bei der Admin-Konsole, die Verwaltung der Experience Cloud-Benutzerberechtigungen und -Profil sowie die Browserunterstützung.
keywords: core services
seo-description: Erfahren Sie mehr über die Anmeldung bei der Admin-Konsole, die Verwaltung der Experience Cloud-Benutzerberechtigungen und -Profil sowie die Browserunterstützung.
seo-title: Verwalten von Experience Cloud-Benutzern und -produkten
solution: Experience Cloud
title: Verwalten von Experience Cloud-Benutzern und -produkten
uuid: aea4e4c3-f543-4e8d-b553-d838418477d6
translation-type: tm+mt
source-git-commit: fda58ef3a32af684482662ee462764b1b92f5cb2

---


# Verwalten von Experience Cloud-Benutzern und -produkten {#topic_3FCB4099640647E3B2411ADBFCE81909}

Erfahren Sie mehr über die Anmeldung bei der Admin-Konsole, die Verwaltung der Experience Cloud-Benutzerberechtigungen und -Profil sowie die Browserunterstützung.

>[!IMPORTANT]
>
>Durch die Verwaltung von Benutzern in der Admin Console werden neue Begriffe, Benutzeroberflächen und Navigationselemente eingeführt. Nachfolgend werden diese Änderungen beschrieben und Links zu weiteren Hilferessourcen angegeben. This help supplements the information in the [Enterprise Administration User Guide](https://helpx.adobe.com/enterprise/managing/user-guide.html) for all Adobe cloud products.

## Neue Funktionen für die Experience Cloud-Benutzerverwaltung {#concept_06A0A13362F644FB90F947238407637A}

Lernen Sie die neuesten Funktionen der Experience Cloud-Benutzerverwaltung kennen.

<!-- ### Business ID type

Adobe is now introducing a new identity type: **Business ID**. This identity type, improves the control of user and product management, and content, while increasing the flexibility of Experience Cloud and Creative Cloud storage usage among your team. With the introduction of this new identity type, Adobe is migrating all Adobe IDs (owned by the individual) used for business to the new Business IDs (owned by the organization).

If you're an existing Creative Cloud for enterprise or teams customer, Adobe will migrate all your users on the Admin Console with Adobe IDs to Business IDs. If you're a new enterprise or teams customer, you will add users to the Admin Console using one of the available identity types: Business ID, Enterprise ID, or Federated ID. 

Beginning May 89, 2020, enterprise admins cannot use the Adobe ID for new organizations created in the Admin Console. Latest: https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=engage&title=Type2e+DX+GTM

What to do

* Your users will need to accept Terms of Use (TOU) changes prior to accounts being migrated to Type2e. 
* Users that belong to multiple organizations might see a Profile Selection screen during the login workflow and need to select the correct one. This ensures that they are logging into the correct organization. (There might be multiple profiles to choose from if a users was a member of multiple organizations before the migration.) -->

### Admin-Tool

Administratoren können eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und deren Details im Admin Tool Ansicht haben. Siehe [Ansicht Experience Cloud-Benutzer im Admin Tool](admin-tool-experience-cloud.md).

## Bei der Admin Console anmelden {#section_705072FD4EBE4B70BC69EC81F2BB8669}

Administratoren verwalten Benutzer nicht mehr in Lösungen. Benutzer- und Produktverwaltung für Experience Cloud finden jetzt in der Admin-Konsole statt.

**So melden Sie sich bei der Admin-Konsole an**

1. Navigate to [https://adminconsole.adobe.com/enterprise/](https://adminconsole.adobe.com/enterprise/#).
1. Geben Sie Ihre [Adobe ID oder Enterprise ID](https://helpx.adobe.com/enterprise/help/identity.html) und Ihr Kennwort ein.

Alternatively, from the Experience Cloud menu ( ![](assets/menu-icon.png)), click **[!UICONTROL Administration]** > **[!UICONTROL Launch Admin Console]**.

**Verwandte Hilfe**

[Administrations-Benutzerhandbuch](https://helpx.adobe.com/enterprise/using/users.html) für Creative Cloud und Dokument Cloud. Einige Informationen sind für die Experience Cloud-Benutzerverwaltung relevant, z. B. für die [Verwaltung von Identitätstypen](https://helpx.adobe.com/enterprise/help/identity.html).

[Melden Sie sich an und verwalten Sie Ihre Profil-Einstellungen](../admin-getting-started/getting-started-experience-cloud.md#topic_AC564B6795334DE39359ADD87F52F2E0) , um Kennwörter, Organisationen und Benachrichtigungen zu verwalten.

## Produktprofile und Gruppen  {#section_AB50558124D541CF80A0D3D76D35A4BF}

Die Hinzufügung von Profilen stellt eine Veränderung gegenüber der bisherigen Gruppenverwaltung von Lösungsprodukten und -diensten dar. In der Admin-Konsole basieren die Berechtigungen auf Produktgruppen, d. h. Profilen und Diensten, die Sie Benutzern zuweisen können.

In Analytics können Sie beispielsweise eine Sammlung von Berichte-Tools wie Analyse Workspace und ReportBuilder sowie Report Suites, Metriken, Dimensionen usw. konfigurieren. Sie können Benutzern Berechtigungen für ein Profil erteilen, indem Sie sie zum Profil hinzufügen. See [Assign Analytics access permissions to a product profile](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391).

**Verwandte Hilfe**

[Eingeschränkte Administratorberechtigungen delegieren](../admin-getting-started/admin-getting-started.md#task_3A072C4AA9734BC59FFA7E015271BC7E)

## Analytics {#section_97DE101F92CD494AB073893680992F1A}

Verwalten Sie Benutzer- und Produktberechtigungen für Analytics in der Admin Console.

[Analytics-Zugriffsberechtigungen einem Produktprofil zuweisen](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) (auf dieser Seite).

**Migration von Benutzerkonten**

Analytics-Administratoren können Benutzerkonten mithilfe des verfügbaren Analytics-Migrationstools für Benutzer-IDs von der Analytics-Benutzerverwaltung in die [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/) / migrieren.

Die Kontomigration erfolgt für Kunden stufenweise. Adobe will notify and assist you when it is your time to migrate existing user accounts from **[!UICONTROL Admin Tools]** > **[!UICONTROL User Management]** to the Admin Console.

After the migration, users sign in using their Adobe ID (or Enterprise ID) and authenticate to their Experience Cloud solutions and services at [experiencecloud.adobe.com](https://experiencecloud.adobe.com). Benutzer, die versuchen, sich über die bisherigen Anmeldedaten anzumelden ([!DNL my.omniture.com] und [!DNL sc.omniture.com]), werden an [!DNL experiencecloud.adobe.com] weitergeleitet.

**Verwandte Hilfe**

[Analytics-Benutzer-ID-Migration](https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html)

## Target - Produktprofile im Vergleich zu Arbeitsbereichen {#section_3860AF177C9E4C7E9C390D36A414F353}

In Zielgruppe ist ein Arbeitsbereich ein Produkt-Profil. Damit kann eine Organisation einem bestimmten Satz von Benutzern bestimmte Eigenschaften zuweisen. Arbeitsbereiche ähneln auf vielerlei Weise den Report Suites in Adobe Analytics.

Siehe:
* [Berechtigungen für Unternehmensbenutzer](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html)
* [Produkte und Profil verwalten](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* Video: Konfigurieren von [Arbeitsbereichen in der Adobe Admin-Konsole](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Campaign - Produktprofile, Mandanten und Sicherheitsgruppen {#section_09CDF75366444CF5810CF321B7C712F3}

Ein *Mieter* in der Kampagne wird auf der Seite &quot;Produkte der Admin-Konsole&quot;als *Produkt* angezeigt.

*Die Sicherheitsgruppe* wird als Profil des Produkts angezeigt.

Informationen zu Sicherheitsgruppen und zum Zuweisen von Benutzern zu Sicherheitsgruppen finden Sie unter [Verwalten von Gruppen und Benutzern](https://helpx.adobe.com/campaign/standard/administration/using/managing-groups-and-users.html) .

## Experience Platform Launch {#section_F2DA6778DD2D48AA8F794041971EE6B1}

Der Start der Erlebnisplattform wird auf der Seite &quot;Produkte&quot;in der Admin-Konsole angezeigt. Sie können andere Lösungen und Dienste in ein Profil zum Starten von Produkten aufnehmen.

Informationen zu Benutzerberechtigungen in der Admin-Konsole finden Sie unter [Benutzerverwaltung](https://docs.adobelaunch.com/launch-reference/administration/user-permissions) und richten Sie startspezifische Optionen ein, einschließlich der Zuweisung von Berechtigungen zu Profilen.

## Dynamischer Tag-Manager {#section_3A41CF2BD5994B9891537D063571D4ED}

Laden Sie Benutzer zur Nutzung des Dynamic Tag Managements ein, weisen Sie Benutzerrollen zu und fügen Sie Benutzer Gruppen hinzu.

See [Users and Permissions](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) for information about how to invite users to Dynamic Tag Management and assign user roles and add users to groups.

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Erstellen Sie Audience Manager-Benutzer und weisen Sie sie Gruppen zu. Sie können auch Einschränkungen für Ansichten (Eigenschaften, Segmente, Ziele und AlgoModel) festlegen.

Siehe [Administration](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) in der Hilfe zu Audience Manager.

## Experience Cloud-Produkte verwalten {#task_16335111C52D40E9BAC73D0699584DBF}

Erstellen Sie ein Profil und weisen Sie es einer Berechtigungsgruppe zu.

Wenn Sie einen Benutzer zu einer Organisation einladen, können Sie dem Benutzer Zugriff auf Produkte und Profil gewähren. Sie können eingeschränkte Administratorberechtigungen auch an einen Benutzer delegieren. Auf ähnliche Weise können Sie Benutzergruppen erstellen und die Gruppe dann zu einem Profil hinzufügen, um den Zugriff zu aktivieren.

1. In the [Admin Console](https://adminconsole.adobe.com/enterprise/), click **[!UICONTROL Products]**.
1. Klicken Sie auf **[!UICONTROL Neues Profil]**.
1. Konfigurieren Sie die Profildetails und klicken Sie dann auf **[!UICONTROL Weiter]**.
1. Klicken Sie auf **[!UICONTROL Fertig]**.

Weitere Hilfe finden Sie unter:

* [Produkte und Profil verwalten](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* [Enterprise-Benutzerberechtigungen](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html) in der Hilfe zur Zielgruppe für weitere Informationen.
* Video: Konfigurieren von [Arbeitsbereichen in der Adobe Admin-Konsole](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Analytics-Zugriffsberechtigungen einem Produktprofil zuweisen {#task_040673FE3E3E429B9531FBCB8B6A4391}

Zugriffsberechtigungen für Analytics-Berichte (Report Suites, Metriken, Dimensionen usw.) einem Produktprofil zuweisen.

Sie können beispielsweise ein Produktprofil mit mehreren Analytics-Tools ([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics] und [!UICONTROL Report Builder]) erstellen, das Zugriff auf bestimmte Metriken und Dimensionen (einschließlich eVars) erhält und beispielswiese Segmente oder berechnete Metriken erstellen kann.

1. Sign in to the [Admin Console](https://adminconsole.adobe.com/enterprise), then click **[!UICONTROL Products]** (or click your product name).
1. Klicken Sie im Produktprofil dann auf **[!UICONTROL Berechtigungen]** (nur für Administratoren verfügbar).
1. Konfigurieren Sie die Profilberechtigungen:

| Element | Beschreibung |
|--- |--- |
| Report Suites | Aktivieren Sie Berechtigungen für bestimmte Report Suites. |
| Metriken | Gewähren Sie Zugriff auf Traffic, Konvertierung, benutzerdefinierte Ereignis, Lösungslösungen, Content-basierte Ereignis usw. |
| Dimensionen | Legen Sie Benutzerrechte auf einer granularen Ebene fest, einschließlich eVars, Traffic-Berichten, Lösungsberichten und Pfadsetzungsberichten. |
| Report Suite-Tools | Aktivieren Sie Benutzerberechtigungen für Web-Services, Report Suite-Verwaltung, Tools und Berichte sowie Dashboard-Elemente. |
| Analytics-Tools | Gewähren Sie Benutzern Zugriff auf allgemeine Elemente (Rechnungsstellung, Protokolle usw.), Unternehmensverwaltung, Werkzeuge, Web-Services, den Report Builder und die Data Connectors-Integration. Die Unternehmenseinstellungen aus der Kategorie „Anpassung der Admin Console“ sind nun in den Analytics-Tools zu finden. |

## Delegieren von administrativen Rollen an Benutzer {#task_3A072C4AA9734BC59FFA7E015271BC7E}

In der Admin-Konsole können Sie eingeschränkte Administratorrechte an andere Personen in Ihrem Unternehmen delegieren. Delegierte Rollen ermöglichen es Benutzern, den Softwarezugriff für Endbenutzer zu verwalten, Zugriffsbereitstellungsfunktionen bereitzustellen und als Supportdelegaten zu fungieren.

Sie können zum Beispiel:

* Erlauben Sie Ihrem Kreativdirektor, Zugriff auf die Creative Cloud zu gewähren.
* Erlauben Sie Ihrem Marketingdirektor, Zugriff auf die Experience Cloud zu gewähren.
* Halten Sie diese beiden Rollen getrennt, damit sie die Rollen der anderen nicht überspringen können.

Durch die Verwendung dieser Rollen können Sie die Verwaltung gleichzeitig an andere delegieren, ohne mehr Funktionen bereitzustellen, als sie benötigen.

1. Klicken Sie in der Admin Console auf **[!UICONTROL Benutzer]** und anschließend auf den entsprechenden Benutzernamen.
1. Klicken Sie auf **[!UICONTROL Administratorrechte bearbeiten]**.
1. Konfigurieren Sie die Administratorrechte des Benutzers.
1. Klicken Sie auf **[!UICONTROL Weiter]**, um die Einstellungen zu prüfen, und anschließend auf **[!UICONTROL Speichern]**.

## Unterstützte Browser und Systemanforderungen {#concept_CDC4371EB9BF433E9534F8716DC8A088}

Unterstützte Browser in der Experience Cloud.

Von Experience Cloud unterstützte Browser:

* [!DNL Microsoft Edge] (Microsoft hat die Unterstützung [für Internet Explorer 8, 9 und 10](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support) eingestellt. Daher behebt Adobe keine Probleme, die in Verbindung mit diesen bestimmten Versionen von Internet Explorer gemeldet wurden.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**Hinweis:** Obwohl die Experience Cloud-Oberfläche diese Browser unterstützt, unterstützen einzelne Lösungen möglicherweise nicht alle Browser. ([Analytics](https://docs.adobe.com/content/help/en/analytics/admin/sys-reqs.html) unterstützt beispielsweise nicht [!DNL Opera] und [Target](https://docs.adobe.com/help/en/target/using/implement-target/before-implement/supported-browsers.html) unterstützt nicht [!DNL Safari].)

**Anforderungen an Lösungen und Produkte**

* [Analytics](https://docs.adobe.com/content/help/en/analytics/admin/sys-reqs.html)
* [Report Builder ](https://docs.adobe.com/content/help/en/analytics/analyze/report-builder/report-builder-setup/system-requirements.html)
* [Adobe Target](https://docs.adobe.com/help/en/target/using/implement-target/before-implement/supported-browsers.html)
