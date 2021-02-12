---
description: Erfahren Sie, wie Sie Benutzerberechtigungen und Produktprofile in Adobe Experience Cloud verwalten. Erfahren Sie mehr über die Anmeldung bei Adobe Admin Console und die Browser-Unterstützung für Experience Cloud.
solution: Admin
title: 'Verwalten von Benutzern und Produkten '
index: true
translation-type: ht
source-git-commit: 119bbd98e78fe55ae30ef874e2125fa196221363
workflow-type: ht
source-wordcount: '1421'
ht-degree: 100%

---


# Verwalten von Experience Cloud-Benutzern und -produkten {#topic_3FCB4099640647E3B2411ADBFCE81909}

Erfahren Sie mehr über die Anmeldung bei der Admin Console, die Verwaltung von Benutzerberechtigungen und Produktprofilen für Experience Cloud und über die Browser-Unterstützung.

>[!IMPORTANT]
>
>Durch die Verwaltung von Benutzern in der Admin Console werden neue Begriffe, Benutzeroberflächen und Navigationselemente eingeführt. Nachfolgend werden diese Änderungen beschrieben und Links zu weiteren Hilferessourcen angegeben. Diese Hilfe ergänzt die im [Benutzerhandbuch für Enterprise-Administratoren](https://helpx.adobe.com/de/enterprise/managing/user-guide.html) enthaltenen Informationen für alle Adobe Cloud-Produkte.

## Neue Funktionen für die Experience Cloud-Benutzerverwaltung {#concept_06A0A13362F644FB90F947238407637A}

Lernen Sie die neuesten Funktionen der Benutzer- und Produktverwaltung in Experience Cloud kennen.

<!-- ### Business ID type

Adobe is introducing an identity type called Business ID. This identity type improves the control of user and product management. Adobe is migrating all Adobe IDs (owned by individuals) that are used for business to the new enterprise Business IDs owned by your organization.

If you are an existing Experience Cloud customer, Adobe will migrate all your users with Adobe IDs in the Admin Console to Business IDs. If you are a new enterprise or teams customer, you will add users to the Admin Console using one of the available identity types: Business ID, Enterprise ID, or Federated ID.

What to do

* Your users will need to accept Terms of Use (TOU) changes prior to accounts being migrated to Type2e. 
* Users that belong to multiple organizations might see a Profile Selection screen during the login workflow and need to select the correct one. This ensures that they are logging into the correct organization. (There might be multiple profiles to choose from if a user was a member of multiple organizations before the migration.)

Beginning May 2020, enterprise administrators cannot use the Adobe ID for new organizations created in the Admin Console. Latest: https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=engage&title=Type2e+DX+GTM-->

### Admin-Tool

Administratoren können im Admin-Tool eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und deren Details anzeigen. Siehe [Anzeigen von Experience Cloud-Benutzern im Admin-Tool](admin-tool-experience-cloud.md).

## Bei der Admin Console anmelden {#section_705072FD4EBE4B70BC69EC81F2BB8669}

Die Administratoren verwalten die Benutzer nicht mehr in bestimmten Produktlösungen. Die Benutzer- und Produktverwaltung für Experience Cloud erfolgt jetzt in der Admin Console.

Aktion zum Anmelden bei der Admin Console:

1. Gehen Sie zu [https://adminconsole.adobe.com/enterprise/](https://adminconsole.adobe.com/enterprise/#).
1. Geben Sie Ihre [Adobe ID oder Enterprise ID](https://helpx.adobe.com/de/enterprise/help/identity.html) und Ihr Kennwort ein.

Alternativ können Sie im Experience Cloud-Menü (![](assets/menu-icon.png)) auf **[!UICONTROL Administration]** > **[!UICONTROL Admin Console starten]** klicken.

**Verwandte Hilfe**

[Administrations-Benutzerhandbuch](https://helpx.adobe.com/de/enterprise/using/users.html) für die Creative Cloud und Document Cloud. Einige Informationen sind für die Experience Cloud-Benutzerverwaltung relevant, z. B. für die [Verwaltung von Identitätstypen](https://helpx.adobe.com/de/enterprise/help/identity.html).

[Anmelden und Profileinstellungen verwalten](../admin-getting-started/getting-started-experience-cloud.md#topic_AC564B6795334DE39359ADD87F52F2E0).

## Produktprofile und Gruppen {#section_AB50558124D541CF80A0D3D76D35A4BF}

Die Hinzufügung von Produktprofilen stellt eine Veränderung gegenüber der bisherigen Verwaltung von Lösungsprodukten und -diensten (mithilfe von Gruppen) dar. In der Admin Console basieren die Berechtigungen auf Produktprofilen. Dabei handelt es sich um Gruppen mit Produkten und Diensten, die Sie Benutzern zuweisen können.

In Analytics können Sie beispielsweise eine Sammlung von Reporting-Tools wie Analysis Workspace und Report Builder sowie Report Suites, Metriken, Dimensionen usw. konfigurieren. Sie können Benutzern Berechtigungen für ein Produktprofil erteilen, indem Sie sie dem Profil hinzufügen. Siehe [Analytics-Zugriffsberechtigungen einem Produktprofil zuweisen](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) auf dieser Seite.

**Übertragung von Verwaltungsrechten**

Siehe [Eingeschränkte Administratorrechte delegieren](../admin-getting-started/admin-getting-started.md#task_3A072C4AA9734BC59FFA7E015271BC7E) auf dieser Seite.

## Analytics {#section_97DE101F92CD494AB073893680992F1A}

Verwalten Sie Benutzer- und Produktberechtigungen für Analytics in der Admin Console.

[Analytics-Zugriffsberechtigungen einem Produktprofil zuweisen](../admin-getting-started/admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) (auf dieser Seite).

**Migration von Benutzerkonten**

Analytics-Administratoren können Benutzerkonten mithilfe des verfügbaren Analytics-Migrationstools für Benutzer-IDs von der Analytics-Benutzerverwaltung in die [Adobe Admin Console](https://adminconsole.adobe.com/enterprise/) migrieren.

Die Kontomigration erfolgt für Kunden stufenweise. Adobe wird Sie benachrichtigen und unterstützen, wenn Sie an der Reihe sind, Ihre bestehenden Benutzerkonten von **[!UICONTROL Admin Tools]** > **[!UICONTROL Benutzerverwaltung]** in die Admin Console zu migrieren.

Nach der Migration müssen sich Benutzer mithilfe ihrer Adobe ID (oder Enterprise ID) anmelden und sich unter [experiencecloud.adobe.com](https://experiencecloud.adobe.com) für ihre Experience Cloud-Lösungen und -Dienste authentifizieren. Benutzer, die versuchen, sich über die bisherigen Anmeldedaten anzumelden ([!DNL my.omniture.com] und [!DNL sc.omniture.com]), werden an [!DNL experiencecloud.adobe.com] weitergeleitet.

**Verwandte Hilfe**

[Migration der Analytics-Benutzer-ID](https://docs.adobe.com/content/help/de-DE/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html)

## Adobe Target – Produktprofile und Arbeitsbereiche im Vergleich {#section_3860AF177C9E4C7E9C390D36A414F353}

In Adobe Target ist ein Arbeitsbereich ein Produktprofil. Er ermöglicht einer Organisation das Zuweisen bestimmter Benutzergruppen zu bestimmten Eigenschaftsgruppen. Arbeitsbereiche ähneln auf vielerlei Weise den Report Suites in Adobe Analytics.

Siehe:

* [Berechtigungen für Unternehmensbenutzer](https://docs.adobe.com/content/help/de-DE/target/using/administer/manage-users/enterprise/property-channel.html)
* [Verwalten von Produkten und Profilen](https://helpx.adobe.com/de/enterprise/using/manage-products-and-profiles.html)
* Video: [Konfigurieren von Adobe Target-Arbeitsbereichen in der Adobe Admin Console](https://helpx.adobe.com/de/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Campaign – Produktprofile, Mandanten und Sicherheitsgruppen {#section_09CDF75366444CF5810CF321B7C712F3}

Ein *Mandant* wird in Campaign auf der Seite „Produkte der Admin Console“ als *Produkt* angezeigt.

Die *Sicherheitsgruppe* wird als Produktprofil angezeigt.

Informationen zu Sicherheitsgruppen und zum Zuweisen von Benutzern zu Sicherheitsgruppen finden Sie unter [Verwalten von Gruppen und Benutzern](https://docs.adobe.com/content/help/de-DE/campaign-standard/using/administrating/users-and-security/managing-groups-and-users.html).

## Experience Platform Launch {#section_F2DA6778DD2D48AA8F794041971EE6B1}

Experience Platform Launch wird auf der Seite „Produkt“ in der Admin Console angezeigt. Sie können weitere Lösungen und Dienste in ein Launch-Produktprofil aufnehmen.

Informationen zu Benutzerberechtigungen in der Admin Console und zum Einrichten Launch-spezifischer Optionen, einschließlich der Zuweisung von Rechten zu Profilen, finden Sie unter [Benutzerverwaltung](https://docs.adobe.com/content/help/de-DE/launch/using/reference/admin/user-permissions.html).

## Experience Manager as a Cloud Service

Adobe Enterprise-Kunden werden in der Adobe Admin Console als IMS-Organisationen angezeigt. Dies ist das Portal, das Adobe-Kunden verwenden, um ihre Produktberechtigungen für ihre Benutzer und Gruppen zu verwalten. AEM-Kunden können die Adobe Admin Console verwenden, um ihre Produktberechtigungen und die IMS-Authentifizierung für AEM as a Cloud Service zu verwalten.

Siehe [IMS-Unterstützung für AEM as a Cloud Service](https://docs.adobe.com/content/help/de-DE/experience-manager-cloud-service/security/ims-support.html#managing-products-and-user-access-in-admin-console).

## Experience Platform Launch {#section_3A41CF2BD5994B9891537D063571D4ED}

Laden Sie Benutzer zu [!UICONTROL Platform Launch] ein und weisen Sie ihnen Benutzerrollen und -rechte zu.

Siehe [Benutzerberechtigungen](https://experienceleague.adobe.com/docs/launch/using/admin/user-permissions.html?lang=de#admin).

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Erstellen Sie Audience Manager-Benutzer und weisen Sie sie Gruppen zu. Sie können auch Einschränkungen anzeigen (Eigenschaften, Segmente, Ziele und [!DNL AlgoModel]).

Siehe [Administration](https://docs.adobe.com/content/help/de-DE/dtm/using/admin/users.html) in der Hilfe zu Audience Manager.

## Experience Cloud-Produkte verwalten {#task_16335111C52D40E9BAC73D0699584DBF}

Erstellen Sie ein Produktprofil und weisen Sie es einer Berechtigungsgruppe zu.

Wenn Sie einen Benutzer in eine Organisation einladen, können Sie dem Benutzer Zugriff auf Produkte und Produktprofile gewähren. Sie können auch eingeschränkte Administratorberechtigungen an einen Benutzer delegieren. Gleichermaßen können Sie Benutzergruppen erstellen und die Gruppe dann einem Produktprofil hinzufügen, um den Zugriff zu aktivieren.

1. Klicken Sie in der [Admin Console](https://adminconsole.adobe.com/enterprise/) auf **[!UICONTROL Produkte]**.
1. Klicken Sie auf **[!UICONTROL Neues Profil]**.
1. Konfigurieren Sie die Profildetails und klicken Sie dann auf **[!UICONTROL Weiter]**.
1. Klicken Sie auf **[!UICONTROL Fertig]**.

Weitere Hilfe finden Sie unter:

* [Verwalten von Produkten und Profilen](https://helpx.adobe.com/de/enterprise/using/manage-products-and-profiles.html)
* [Enterprise-Benutzerberechtigungen](https://docs.adobe.com/content/help/de-DE/target/using/administer/manage-users/enterprise/property-channel.html) in der Hilfe zu Adobe Target.
* Video: [Konfigurieren von Adobe Target-Arbeitsbereichen in der Adobe Admin Console](https://helpx.adobe.com/de/target/kb/how-to-configure-target-workspaces-in-adobe-admin-console0.html)

## Analytics-Zugriffsberechtigungen einem Produktprofil zuweisen {#task_040673FE3E3E429B9531FBCB8B6A4391}

Zugriffsberechtigungen für Analytics-Berichte (Report Suites, Metriken, Dimensionen usw.) einem Produktprofil zuweisen.

Sie können beispielsweise ein Produktprofil mit mehreren Analytics-Tools ([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics] und [!UICONTROL Report Builder]) erstellen, das Zugriff auf bestimmte Metriken und Dimensionen (einschließlich eVars) erhält und beispielsweise Segmente oder berechnete Metriken erstellen kann.

1. Melden Sie sich bei der [Admin Console](https://adminconsole.adobe.com/enterprise) an und klicken Sie dann auf **[!UICONTROL Produkte]** (oder auf Ihren Produktnamen).
1. Klicken Sie im Produktprofil dann auf **[!UICONTROL Berechtigungen]** (nur für Administratoren verfügbar).
1. Konfigurieren Sie die Profilberechtigungen:

| Element | Beschreibung |
|--- |--- |
| Report Suites | Aktivieren Sie Berechtigungen für bestimmte Report Suites. |
| Metriken | Aktivieren Sie Berechtigungen für Traffic, Konversion, benutzerspezifische Ereignisse, Lösungsereignisse, Inhaltsbewahrung usw. |
| Dimensionen | Passen Sie den Benutzerzugriff auf einer granularen Ebene an, einschließlich eVars, Traffic-Berichten, Lösungsberichten und Pfadberichten. |
| Report Suite-Tools | Aktivieren Sie Benutzerberechtigungen für Webdienste, Report Suite-Verwaltung, Tools und Berichte sowie Dashboard-Elemente. |
| Analytics-Tools | Gewähren Sie Benutzern Zugriff auf allgemeine Elemente (Rechnungsstellung, Protokolle usw.), Unternehmensverwaltung, Werkzeuge, Web-Services, den Report Builder und die Data Connectors-Integration. Die Unternehmenseinstellungen aus der Kategorie „Anpassung der Admin Console“ sind nun in den Analytics-Tools zu finden. |

## Delegieren von administrativen Rollen an Benutzer {#task_3A072C4AA9734BC59FFA7E015271BC7E}

In der Admin Console können Sie eingeschränkte Administratorrechte an andere Personen in Ihrem Unternehmen delegieren. Delegierte Rollen ermöglichen es Benutzern, den Softwarezugriff für Endbenutzer zu verwalten, Zugriffsimplementierungsfunktionen bereitzustellen und als Stellvertreter des Supports zu fungieren.

Sie können zum Beispiel:

* Ihren Creative Director Zugriff auf die Creative Cloud gewähren lassen.
* Ihren Marketing Director Zugriff auf die Experience Cloud gewähren lassen.
* Halten Sie diese beiden Rollen getrennt, damit sie die jeweils andere Rolle nicht überschreiten können.

Mithilfe dieser Rollen können Sie die Verwaltung gleichzeitig an andere delegieren, ohne mehr Funktionen bereitzustellen, als benötigt werden.

1. Klicken Sie in der Admin Console auf **[!UICONTROL Benutzer]** und anschließend auf den entsprechenden Benutzernamen.
1. Klicken Sie auf **[!UICONTROL Administratorrechte bearbeiten]**.
1. Konfigurieren Sie die Administratorrechte des Benutzers.
1. Klicken Sie auf **[!UICONTROL Weiter]**, um die Einstellungen zu prüfen, und anschließend auf **[!UICONTROL Speichern]**.

## Unterstützte Browser und Systemanforderungen {#concept_CDC4371EB9BF433E9534F8716DC8A088}

Unterstützte Browser in der Experience Cloud.

* [!DNL Microsoft Edge] (Microsoft hat für Internet Explorer 8, 9 und 10 den [Support beendet](https://www.microsoft.com/de-de/WindowsForBusiness/End-of-IE-support). Aus diesem Grund werden von Adobe keine Probleme mehr behoben, die in Verbindung mit diesen speziellen Versionen von Internet Explorer gemeldet werden.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**Hinweis:** Obwohl die Experience Cloud-Oberfläche diese Browser unterstützt, unterstützen einzelne Lösungen möglicherweise nicht alle Browser. ([Analytics](https://docs.adobe.com/content/help/de-DE/analytics/admin/sys-reqs.html) unterstützt beispielsweise nicht [!DNL Opera] und [Adobe Target](https://docs.adobe.com/help/de-DE/target/using/implement-target/before-implement/supported-browsers.html) unterstützt nicht [!DNL Safari].)

### Anforderungen an Lösungen und Produkte

* [Analytics](https://docs.adobe.com/content/help/de-DE/analytics/admin/sys-reqs.html)
* [Report Builder ](https://docs.adobe.com/content/help/de-DE/analytics/analyze/report-builder/report-builder-setup/system-requirements.html)
* [Adobe Target](https://docs.adobe.com/help/de-DE/target/using/implement-target/before-implement/supported-browsers.html)
