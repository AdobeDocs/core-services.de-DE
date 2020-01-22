---
description: Erfahren Sie mehr über die Anmeldung bei der Admin-Konsole, die Verwaltung von Experience Cloud-Benutzerberechtigungen und -Produktprofilen und die Browserunterstützung.
keywords: core services
seo-description: Erfahren Sie mehr über die Anmeldung bei der Admin-Konsole, die Verwaltung von Experience Cloud-Benutzerberechtigungen und -Produktprofilen und die Browserunterstützung.
seo-title: Verwalten von Experience Cloud-Benutzern und -produkten
solution: Experience Cloud
title: Verwalten von Experience Cloud-Benutzern und -produkten
uuid: aea4e4c3-f543-4e8d-b553-d838418477d6
translation-type: tm+mt
source-git-commit: 6040c4d2f052c561958624296c8e62c8230ae820

---


# Verwalten von Experience Cloud-Benutzern und -produkten {#topic_3FCB4099640647E3B2411ADBFCE81909}

Erfahren Sie mehr über die Anmeldung bei der Admin-Konsole, die Verwaltung von Experience Cloud-Benutzerberechtigungen und -Produktprofilen und die Browserunterstützung.

>[!IMPORTANT]
>
>Durch die Verwaltung von Benutzern in der Admin Console werden neue Begriffe, Benutzeroberflächen und Navigationselemente eingeführt. Nachfolgend werden diese Änderungen beschrieben und Links zu weiteren Hilferessourcen angegeben. Diese Hilfestellungen ergänzen die im [Benutzerhandbuch für Administratoren für Enterprise](https://helpx.adobe.com/enterprise/managing/user-guide.html) enthaltenen Informationen für alle Adobe Cloud-Produkte.

## Neue Funktionen für die Experience Cloud-Benutzerverwaltung {#concept_06A0A13362F644FB90F947238407637A}

Lernen Sie die neuesten Funktionen der Experience Cloud-Benutzerverwaltung kennen.

## Bei der Admin Console anmelden {#section_705072FD4EBE4B70BC69EC81F2BB8669}

Administratoren verwalten Benutzer nicht mehr mithilfe von Lösungen. Die Benutzer- und Produktverwaltung für die Experience Cloud erfolgt nun in der Admin Console.

**So melden Sie sich in der Admin Console an:**

1. Navigate to [https://adminconsole.adobe.com/enterprise/](https://adminconsole.adobe.com/enterprise/#).
1. Geben Sie Ihre [Adobe ID oder Enterprise ID](https://helpx.adobe.com/enterprise/help/identity.html) und Ihr Kennwort ein.

Alternativ können Sie im Experience Cloud-Menü (![](assets/menu-icon.png)) auf **[!UICONTROL Administration]**>**[!UICONTROL  Admin Console starten]** klicken.

**Verwandte Hilfe**

[Benutzerhandbuch für Administratoren](https://helpx.adobe.com/enterprise/using/users.html) für die Creative Cloud und Document Cloud. Einige Informationen sind für die Experience Cloud-Benutzerverwaltung relevant, beispielsweise unter [Verwalten von Identitätstypen](https://helpx.adobe.com/enterprise/help/identity.html).

[Anmelden und Profileinstellungen verwalten](../admin-getting-started/getting-started-experience-cloud.md#topic_AC564B6795334DE39359ADD87F52F2E0) zur Verwaltung von Kennwörtern, Organisationen und Benachrichtigungen.

## Produktprofile und Gruppen  {#section_AB50558124D541CF80A0D3D76D35A4BF}

Durch das Hinzufügen von Produktprofilen wurde die Weise, wie Lösungsprodukte und Dienste bisher verwaltet wurden (mithilfe von Gruppen), verändert. In der Admin Console basieren Berechtigungen auf Produktprofilen, bei denen es sich um Gruppen von Produkten und Diensten handelt, die Sie Benutzern zuweisen können.

In Analytics können Sie beispielsweise eine Sammlung an Reportingtools (z. B. Analysis Workspace und Report Builder) mit Report Suites, Metriken, Dimensionen usw. konfigurieren. Sie können Benutzern eine Berechtigung für ein Produktprofil zuweisen, indem Sie die Benutzer den entsprechenden Profilen hinzufügen. Weitere Informationen finden Sie unter [Analytics-Zugriffsberechtigungen einem Produktprofil zuweisen](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391).

**Verwandte Hilfe**

[Eingeschränkte Administratorberechtigungen delegieren](../admin-getting-started/admin-getting-started.md#task_3A072C4AA9734BC59FFA7E015271BC7E)

## Analytics {#section_97DE101F92CD494AB073893680992F1A}

Verwalten Sie Benutzer- und Produktberechtigungen für Analytics in der Admin Console.

[Analytics-Zugriffsberechtigungen einem Produktprofil zuweisen](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) (auf dieser Seite).

**Migration von Benutzerkonten**

Analytics-Administratoren können Benutzerkonten mithilfe des verfügbaren Analytics-Migrationstools für Benutzer-IDs von der Analytics-Benutzerverwaltung in die [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/) / migrieren.

Die Kontomigration erfolgt für Kunden stufenweise. Adobe wird Sie benachrichtigen und unterstützen, wenn Sie an der Reihe sind, Ihre bestehenden Benutzerkonten von **[!UICONTROL Admin Tools]**>**[!UICONTROL  Benutzerverwaltung]** in die Admin Console zu migrieren.

After the migration, users sign in using their Adobe ID (or Enterprise ID) and authenticate to their Experience Cloud solutions and services at [experiencecloud.adobe.com](https://experiencecloud.adobe.com). Benutzer, die versuchen, sich über die bisherigen Anmeldedaten anzumelden ([!DNL my.omniture.com] und [!DNL sc.omniture.com]), werden an [!DNL experiencecloud.adobe.com] weitergeleitet.

**Verwandte Hilfe**

[Migration der Analytics-Benutzer-ID](https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html)

## Target - Produktprofile im Vergleich zu Arbeitsbereichen {#section_3860AF177C9E4C7E9C390D36A414F353}

In Target entspricht ein Arbeitsbereich einem Produktprofil. Mit seiner Hilfe können Organisationen Benutzergruppen bestimmten Eigenschaftsgruppen zuweisen. Arbeitsbereiche ähneln auf vielerlei Weise den Report Suites in Adobe Analytics.

Siehe:
* [Berechtigungen für Unternehmensbenutzer](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html)
* [Produkte und Profile verwalten](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* Video: [Target-Arbeitsbereiche in der Adobe Admin Console konfigurieren](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Campaign - Produktprofile, Mandanten und Sicherheitsgruppen {#section_09CDF75366444CF5810CF321B7C712F3}

Ein *Mandant* in Campaign wird auf der Produktseite der Admin Console als *Produkt* angezeigt.

Eine *Sicherheitsgruppe* wird als Produktprofil angezeigt.

Informationen zu Sicherheitsgruppen und zum Zuweisen von Benutzern zu Sicherheitsgruppen finden Sie unter [Verwalten von Gruppen und Benutzern](https://helpx.adobe.com/campaign/standard/administration/using/managing-groups-and-users.html) .

## Experience Platform Launch {#section_F2DA6778DD2D48AA8F794041971EE6B1}

Experience Platform Launch wird auf der Produktseite in der Admin Console angezeigt. Sie können weitere Lösungen und zentrale Dienste in ein Launch-Produktprofil integrieren.

See [User Management](https://docs.adobelaunch.com/launch-reference/administration/user-permissions) for information about user permissions in the Admin Console and set up Launch-specific options, including assigning rights to profiles.

## Dynamischer Tag-Manager {#section_3A41CF2BD5994B9891537D063571D4ED}

Laden Sie Benutzer zur Nutzung des Dynamic Tag Managements ein, weisen Sie Benutzerrollen zu und fügen Sie Benutzer Gruppen hinzu.

See [Users and Permissions](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) for information about how to invite users to Dynamic Tag Management and assign user roles and add users to groups.

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Erstellen Sie Audience Manager-Benutzer und weisen Sie diese Gruppen zu. Sie können außerdem Beschränkungen anzeigen (Eigenschaften, Segmente, Ziele und AlgoModel).

Siehe [Administration](https://docs.adobe.com/content/help/en/dtm/using/admin/users.html) in der Hilfe zu Audience Manager.

## Experience Cloud-Produkte verwalten {#task_16335111C52D40E9BAC73D0699584DBF}

Ein Produktprofil erstellen und einer Berechtigungsgruppe zuweisen.

Wenn Sie einen Benutzer einer Organisation zuweisen, können Sie dem Benutzer Zugriff auf Produkte und Produktprofile gewähren. Sie können außerdem eingeschränkte Administratorberechtigungen an einen Benutzer delegieren. Gleichermaßen können Sie Benutzergruppen erstellen und die Gruppe dann einem Produktprofil hinzufügen, um den Zugriff zu gewähren.

1. Klicken Sie in der [Admin Console](https://adminconsole.adobe.com/enterprise/) auf **[!UICONTROL Produkte]**.
1. Klicken Sie auf **[!UICONTROL Neues Profil]**.
1. Konfigurieren Sie die Profildetails und klicken Sie dann auf **[!UICONTROL Weiter]**.
1. Klicken Sie auf **[!UICONTROL Fertig]**.

Weitere Informationen finden Sie hier:

* [Produkte und Profile verwalten](https://helpx.adobe.com/enterprise/using/manage-products-and-profiles.html)
* [Enterprise-Benutzerrechte](https://docs.adobe.com/content/help/en/target/using/administer/manage-users/enterprise/property-channel.html) in der Target-Hilfe
* Video: [Target-Arbeitsbereiche in der Adobe Admin Console konfigurieren](https://helpx.adobe.com/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Analytics-Zugriffsberechtigungen einem Produktprofil zuweisen {#task_040673FE3E3E429B9531FBCB8B6A4391}

Zugriffsberechtigungen für Analytics-Berichte (Report Suites, Metriken, Dimensionen usw.) einem Produktprofil zuweisen.

Sie können beispielsweise ein Produktprofil mit mehreren Analytics-Tools ([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics] und [!UICONTROL Report Builder]) erstellen, das Zugriff auf bestimmte Metriken und Dimensionen (einschließlich eVars) erhält und beispielswiese Segmente oder berechnete Metriken erstellen kann.

1. Melden Sie sich in der [Admin Console](https://adminconsole.adobe.com/enterprise) an und klicken Sie dann auf **[!UICONTROL Produkte]**(oder auf Ihren Produktnamen).
1. Klicken Sie im Produktprofil dann auf **[!UICONTROL Berechtigungen]**(nur für Administratoren verfügbar).
1. Konfigurieren Sie die Profilberechtigungen:

| Element | Beschreibung |
|--- |--- |
| Report Suites | Gewähren Sie Zugriff auf bestimmte Report Suites. |
| Metriken | Gewähren Sie Zugriff auf Traffic, Konversion, benutzerdefinierte Ereignisse, Lösungsereignisse, Content-Unterstützung und mehr. |
| Dimensionen | Legen Sie Benutzerrechte granular fest, einschließlich eVars, Traffic-Berichten, Lösungsberichten und Pfadsetzungsberichten. |
| Report Suite-Tools | Gewähren Sie Benutzern Zugriff auf Webdiensten, Report Suite-Verwaltung, Tools und Berichte sowie Dashboard-Elemente. |
| Analytics-Tools | Gewähren Sie Benutzern Zugriff auf allgemeine Elemente (Rechnungsstellung, Protokolle usw.), Unternehmensverwaltung, Werkzeuge, Web-Services, den Report Builder und die Data Connectors-Integration. Die Unternehmenseinstellungen aus der Kategorie „Anpassung der Admin Console“ sind nun in den Analytics-Tools zu finden. |

## Delegieren von administrativen Rollen an Benutzer {#task_3A072C4AA9734BC59FFA7E015271BC7E}

In der Admin Console können Sie anderen Benutzern Ihrer Organisation eingeschränkte Administratorrechte zuweisen. Delegierte Rollen versetzen Benutzer in die Lage, den Software-Zugriff für Endbenutzer zu administrieren, andere zum Erteilen von Zugangsberechtigungen zu befähigen und als Supportbeauftragter zu fungieren.

Sie können zum Beispiel:

* Dem Kreativdirektor den Zugriff auf Creative Cloud gewähren.
* Dem Marketingdirektor den Zugriff auf die Experience Cloud gewähren.
* Halten Sie diese beiden Rollen auseinander, damit sie sich nicht überschneiden.

Durch die Verwendung dieser Rollen können Sie gleichzeitig die Verwaltung an andere delegieren, ohne mehr als die benötigten Berechtigungen zu erteilen.

1. Klicken Sie in der Admin Console auf **[!UICONTROL Benutzer]**und anschließend auf den entsprechenden Benutzernamen.
1. Klicken Sie auf **[!UICONTROL Administratorrechte bearbeiten]**.
1. Konfigurieren Sie die Administratorrechte des Benutzers.
1. Klicken Sie auf **[!UICONTROL Weiter]**, um die Einstellungen zu prüfen, und anschließend auf**[!UICONTROL  Speichern]**.

## Unterstützte Browser und Systemanforderungen {#concept_CDC4371EB9BF433E9534F8716DC8A088}

In Experience Cloud unterstützte Browser

Von Experience Cloud unterstützte Browser:

* [!DNL Microsoft Edge] (Microsoft hat den Support für Internet Explorer 8, 9 und 10 [eingestellt](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support). Aus diesem Grund werden von Adobe keine Probleme mehr behoben, die in Verbindung mit diesen speziellen Versionen von Internet Explorer gemeldet werden.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**** Hinweis: Obwohl die Experience Cloud-Oberfläche diese Browser unterstützt, unterstützen einzelne Lösungen möglicherweise nicht jeden Browser. ( [Analytics](https://docs.adobe.com/content/help/en/analytics/admin/sys-reqs.html) unterstützt beispielsweise nicht [!DNL Opera], [Target](https://docs.adobe.com/help/en/target/using/implement-target/before-implement/supported-browsers.html) nicht [!DNL Safari].)

**Anforderungen an Lösungen und Produkte**

* [Analytics](https://docs.adobe.com/content/help/en/analytics/admin/sys-reqs.html)
* [Report Builder ](https://docs.adobe.com/content/help/en/analytics/analyze/report-builder/report-builder-setup/system-requirements.html)
* [Adobe Target](https://docs.adobe.com/help/en/target/using/implement-target/before-implement/supported-browsers.html)
