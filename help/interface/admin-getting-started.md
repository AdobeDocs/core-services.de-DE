---
title: Verwalten von Benutzern und Produkten
description: Melden Sie sich bei der Admin Console an und verwalten Sie Experience Cloud-Benutzerberechtigungen und -Produkte (Produktprofile). Erfahren Sie mehr über die Zuweisung von Administratorrechten an Experience Cloud-Benutzer und über die Browser-Unterstützung für Experience Cloud.
solution: Admin
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: af9eda5b-d984-44b7-a7b3-52dfc4e03d8f
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '1582'
ht-degree: 74%

---

# Verwalten von Benutzern und Produkten in [!DNL Experience Cloud]

Erfahren Sie mehr über die Anmeldung bei der Admin Console, die Verwaltung von Benutzerberechtigungen und Produktprofilen für Experience Cloud und über die Browser-Unterstützung.

>[!IMPORTANT]
>
>Die folgenden Informationen gelten speziell für Experience Cloud-Anwendungen. Diese Informationen ergänzen die im [Benutzerhandbuch für Enterprise-Administratoren](https://helpx.adobe.com/de/enterprise/admin-guide.html) enthaltenen allgemeinen Informationen für alle Adobe Cloud-Produkte.

Sie können im Admin-Tool eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und deren Details anzeigen. Siehe [Anzeigen von Experience Cloud-Benutzern im Admin-Tool](admin-tool-experience-cloud.md).

## Aktualisierungshinweis zur Bereitstellung{#provisioning}

Aktualisiert am **20. Juli 2022**

>[!IMPORTANT]
>
>Beachten Sie die folgende Benachrichtigung bezüglich der Bereitstellung von Experience Cloud.

Adobe aktualisiert seine Bereitstellung, um allen Experience Cloud-Kundinnen und -Kunden Zugang zu grundlegenden Funktionen zu bieten, die die Interoperabilität zwischen einigen Experience Cloud-Produkten unterstützen. Adobe Experience Platform wird als neue Berechtigung den Experience Cloud-Organisationen der Benutzenden hinzugefügt, wobei [!UICONTROL Datenerfassung] als Service enthalten ist.

Die [!UICONTROL Datenerfassung] von Adobe Experience Platform umfasst [Tags](https://experienceleague.adobe.com/en/docs/tags) für ein vereinfachtes universelles Tag-Management und bietet eine zuverlässige, robuste und vollständige Infrastruktur für Streaming-Daten. Tags vereinfachen die Erfassung von Kundenerlebnisdaten und optimieren die Bereitstellung von Erlebnissen.

**Änderungen in der[!DNL Admin Console]**

Admins können Änderungen oder Ergänzungen der Datei sehen. [!DNL Admin Console] wie folgt:

* Die Adobe Experience Platform-Produktkarte in der Admin Console umfasst:

   * Places
   * Assurance
   * Identity-Namespace
   * Sandboxes
   * Experience-Datenmodell
   * Schemata
   * Datenströme
   * Besucher-ID

  Für Organisationen, die derzeit kein Experience Platform verwenden, sehen Sie jetzt die _Adobe Experience Platform_ Produkt in der [!DNL Admin Console], einschließlich der oben aufgeführten Funktionen.

  Für Organisationen, die derzeit Experience Platform verwenden, werden _Places_ jetzt in die Experience Platform-Karte integriert.

* Adobe Experience Platform-Datenerfassung (früher Launch) und Datenschutz werden weiterhin als separate Produktkarten neben den anderen Experience Platform-Funktionen angezeigt.

Weitere Informationen zu den neuen Funktionen finden Sie auf den entsprechenden Seiten in der Experience League:

* [Datenerfassung](https://experienceleague.adobe.com/docs/discontinued/using/reports-and-analytics.html?lang=de)
* [Places](https://experienceleague.adobe.com/en/docs/places/using/home)
* [Assurance](https://experienceleague.adobe.com/docs/platform-learn/implement-mobile-sdk/app-implementation/assurance.html?lang=de)
* [Identity-Namespace](https://experienceleague.adobe.com/docs/experience-platform/identity/home.html?lang=de)
* [Sandboxes](https://experienceleague.adobe.com/docs/experience-platform/sandbox/home.html?lang=de)
* [Experience-Datenmodell](https://experienceleague.adobe.com/docs/experience-platform/xdm/home.html?lang=de)
* [Schemata](https://experienceleague.adobe.com/docs/experience-platform/xdm/schema/composition.html?lang=de)
* [Datenströme](https://experienceleague.adobe.com/docs/experience-platform/edge/datastreams/overview.html?lang=de)
* [Besucher-ID](https://experienceleague.adobe.com/docs/core-services/interface/services/core-services.html?lang=de#section_3C9F6DF37C654D939625BB4D485E4354)
* [Datenschutz](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=de)

## Experience Cloud-Benutzerauthentifizierung (geplante Migration){#migration}

Ab Februar 2022 aktualisiert Adobe sein Profilverwaltungssystem, damit Unternehmen ihre Unternehmensberechtigungen für einzelne Profile besser verwalten können. Daher werden alle Benutzer mit einem persönlichen Profil, das einer einzelnen Adobe ID (Type1) entspricht, in ein neues Unternehmensprofil migriert. Dieses Profil entspricht einer _Business ID_ (Type2e).

Siehe [Identitätstypen auf Adobe [!DNL Admin Console]](https://helpx.adobe.com/de/enterprise/using/identity.html) für Informationen zu Identitätstypen.

### Migrationsprozess

Wenn Ihre Migration ansteht, erhalten Ihre Organisationsadministratoren 30 Tage vor der Migration eine Benachrichtigungs-E-Mail.

* Die Migration wird für entweder den Zeitraum zwischen 22 Uhr und 6 Uhr Ortszeit basierend auf der Hauptzeitzone Ihres Unternehmens oder für einen Zeitraum am Wochenende geplant.
* Während der Migration kann der Zugriff auf die Experience Cloud-Anwendung für ca. 15 Minuten unterbrochen sein. [!DNL Admin Console] kann bis zu 30 Minuten nicht zugänglich sein. Abgesehen davon verläuft die Migration nahtlos.

### Änderungen nach der Migration

[!DNL Admin Console]

* Administratoren mit mehreren Konten sehen möglicherweise eine Profilauswahl, wenn sie sich bei anmelden [!DNL Admin Console].
* Einzelne Adobe ID-Benutzende werden auf Business ID aktualisiert.
* Das Business ID-Verzeichnis wird hinzugefügt in **[!UICONTROL Einstellungen]** > **[!UICONTROL Identität]** > **[!UICONTROL Verzeichnisse]**.

  ![[!DNL Admin Console] Identität - Business ID](assets/identity-home.png)

### Anmeldung nach der Migration

Ihr Anmeldeerlebnis ändert sich mit diesem Update nicht:

1. Melden Sie sich mit denselben Anmeldeinformationen bei `experience.adobe.com` an.

1. Es wird ein neues Profil erstellt, das mit der Business ID verknüpft ist. Ihnen wird eine Meldung angezeigt, bei der Sie wählen können zwischen **[!UICONTROL Jetzt Mitglied werden]** und **[!UICONTROL Überspringen]**.

1. Wenn Sie eine dieser Optionen wählen, gelangen Sie zu einem bereits vorhandenen Landingpage-Erlebnis.

1. Jedem Geschäftsplan ist ein Adobe-Profil zugeordnet, das die Möglichkeit bietet, Assets zu organisieren, die aus zusätzlichen Adobe-Cloud-Angeboten (Creative Cloud und Document Cloud) erstellt wurden.

Weitere Informationen finden Sie unter [Einführung in Adobe-Profile](https://helpx.adobe.com/de/enterprise/kb/introducing-adobe-profiles.html).

## Was ist ein Produktprofil? {#section_AB50558124D541CF80A0D3D76D35A4BF}

_[!UICONTROL Produktprofile]_ sind Gruppen von Produkten und Diensten, die Sie Benutzern zuweisen können. In Experience Cloud basieren die Berechtigungen auf dem Produktprofil und nicht auf dem Benutzer. (Sie können jedoch bestimmten Benutzern Administratorrechte zuweisen.)

In Analytics können Sie beispielsweise eine Sammlung von Reporting-Tools wie Analysis Workspace und Report Builder sowie Report Suites, Metriken und Dimensionen konfigurieren. Sie können Berechtigungen für ein Produktprofil erteilen, indem Sie Benutzer zum Profil hinzufügen.

* Siehe [Analytics-Zugriffsberechtigungen einem Produktprofil zuweisen](admin-getting-started.md#task_040673FE3E3E429B9531FBCB8B6A4391) auf dieser Seite.
* Siehe [Delegieren von administrativen Rollen an Benutzer](#delegate-rights) auf dieser Seite.

## Verwalten von Experience Cloud-Produktprofilen {#task_16335111C52D40E9BAC73D0699584DBF}

Sie können ein Produktprofil erstellen und es einer Berechtigungsgruppe zuweisen.

Wenn Sie einen Benutzer in eine Organisation einladen, können Sie dem Benutzer Zugriff auf Produkte und Produktprofile gewähren. Sie können auch eingeschränkte Administratorberechtigungen an einen Benutzer delegieren. Gleichermaßen können Sie Benutzergruppen erstellen und die Gruppe dann einem Produktprofil hinzufügen, um den Zugriff zu aktivieren.

1. In der [[!DNL Admin Console]](https://adminconsole.adobe.com/enterprise/), auswählen **[!UICONTROL Produkte]**.
1. Wählen Sie den Namen Ihres Unternehmens aus.
1. Wählen Sie **[!UICONTROL Neues Profil]** aus.
1. Konfigurieren Sie die Profildetails und klicken Sie dann auf **[!UICONTROL Speichern]**.

Weitere Informationen (und Hilfe zur Produktverwaltung für Creative Cloud und Document Cloud) finden Sie unter [Identität](https://helpx.adobe.com/de/enterprise/using/identity.html) im [Administrations-Benutzerhandbuch](https://helpx.adobe.com/de/enterprise/using/users.html).

**Verwandte Hilfe.**

* [Verwalten von Benutzern](https://helpx.adobe.com/de/enterprise/using/users.html) in [!DNL Admin Console]
* [Produkte und Profile verwalten](https://helpx.adobe.com/de/enterprise/using/manage-products.html) in [!DNL Admin Console].
* [Enterprise-Benutzerberechtigungen](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=de) in der Hilfe zu Adobe Target.
* Video: [Konfigurieren von Adobe Target-Arbeitsbereichen in Adobe [!DNL Admin Console]](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-17521.html?lang=de)

## Delegieren von administrativen Rollen an Benutzer {#delegate-rights}

in [!DNL Admin Console]Alternativ können Sie eingeschränkte Administratorrechte an andere Personen in Ihrer Organisation delegieren. Delegierte Rollen ermöglichen es Benutzern, den Softwarezugriff für Endbenutzer zu verwalten, Zugriffsbereitstellungsfunktionen bereitzustellen und als Stellvertreter des Supports zu fungieren.

Sie können zum Beispiel:

* Ihren Creative Director Zugriff auf die Creative Cloud gewähren lassen.
* Erlauben Sie Ihrem Marketing-Leiter, Zugriff auf Experience Cloud zu gewähren.
* Halten Sie diese beiden Rollen getrennt, damit sie die jeweils andere Rolle nicht überschreiten können.

Mithilfe dieser Rollen können Sie die Verwaltung gleichzeitig an andere delegieren, ohne mehr Funktionen bereitzustellen, als benötigt werden.

1. In der [!DNL Admin Console], auswählen **[!UICONTROL Benutzer]** und wählen Sie dann den Namen des Benutzers aus.

   ![Administratorrechte in [!DNL Admin Console]](assets/edit-admin-rights.png)

1. Klicken Sie auf **[!UICONTROL Administratorrechte bearbeiten]**.

   ![Administratorrechte in bearbeiten [!DNL Admin Console]](assets/edit-admin-rights-page.png)

1. Legen Sie die Administratorrechte des Benutzers fest.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

## Verwalten von Analytics-Benutzern und -Produkten {#section_97DE101F92CD494AB073893680992F1A}

Sie können Zugriffsberechtigungen für Analytics-Berichte (Report Suites, Metriken, Dimensionen usw.) einem Produktprofil zuweisen.

Sie können beispielsweise ein Produktprofil erstellen, das mehrere Analytics-Tools enthält ([!UICONTROL Analysis Workspace], [!UICONTROL Reports &amp; Analytics] und [!UICONTROL Report Builder]). Diese Profile enthalten Berechtigungen für bestimmte Metriken und Dimensionen (einschließlich eVars) sowie Funktionen wie Segmente oder die Erstellung berechneter Metriken.

1. Beim anmelden [[!DNL Admin Console]](https://adminconsole.adobe.com/enterprise)und wählen Sie dann **[!UICONTROL Produkte]**.
1. Klicken Sie auf der Seite [!UICONTROL Produkte] auf Ihr Produkt und danach auf **[!UICONTROL Berechtigungen]** (nur für Administratoren verfügbar).
1. Konfigurieren Sie die Profilberechtigungen:

| Element | Beschreibung |
|--- |--- |
| Report Suites | Aktivieren Sie Berechtigungen für bestimmte Report Suites. |
| Metriken | Aktivieren Sie Berechtigungen für Traffic, Konversion, benutzerspezifische Ereignisse, Programmereignisse, Inhaltsbewahrung usw. |
| Dimensionen | Passen Sie den Benutzerzugriff auf einer granularen Ebene an, einschließlich eVars, Traffic-Berichte, Programmberichte und Pfadberichte. |
| Report Suite-Tools | Aktivieren Sie Benutzerberechtigungen für Webdienste, Report Suite-Verwaltung, Tools und Berichte sowie Dashboard-Elemente. |
| Analytics-Tools | Gewähren Sie Benutzern Zugriff auf allgemeine Elemente (Abrechnung, Protokolle usw.), Unternehmensverwaltung, Tools, Web-Services, Report Builder und die Data Connectors-Integration. Unternehmenseinstellungen in der Datei Anpassen [!DNL Admin Console] -Kategorien wurden in die Analytics-Tools verschoben. |

**Migration von Benutzerkonten**

Ein Migrationswerkzeug für Analytics-Benutzer-IDs ist verfügbar, mit dem Analytics-Admins Benutzerkonten von Analytics User Management in das migrieren können [Adobe [!DNL Admin Console]](https://adminconsole.adobe.com/enterprise/).

Die Kontomigration erfolgt für Kunden stufenweise. Adobe wird Sie benachrichtigen und unterstützen, wenn es an der Zeit ist, bestehende Benutzerkonten von zu migrieren. **[!UICONTROL Admin Tools]** > **[!UICONTROL Benutzerverwaltung]** in die [!DNL Admin Console].

Nach der Migration müssen sich Benutzer mithilfe ihrer Adobe ID (oder Enterprise ID) anmelden und sich unter [experience.adobe.com](https://experience.adobe.com) für ihre Experience Cloud-Programme und -Services authentifizieren. Benutzer, die versuchen, sich über die bisherigen Anmeldedaten anzumelden ([!DNL my.omniture.com], [!DNL sc.omniture.com] und [!DNL experiencecloud.adobe.com]), werden an [!DNL experience.adobe.com] weitergeleitet.

**Verwandte Hilfe.**

* [Analytics in der [!DNL Admin Console]](https://experienceleague.adobe.com/docs/analytics/admin/admin-console/home.html?lang=de)
* [Migration der Analytics-Benutzer-ID](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/user-product-management/migrate-users/c-migration-tool.html?lang=de)

## Adobe Target verwalten - Produktprofile und Arbeitsbereiche im Vergleich {#section_3860AF177C9E4C7E9C390D36A414F353}

In Adobe Target ist ein Arbeitsbereich ein Produktprofil. Er ermöglicht einer Organisation das Zuweisen bestimmter Benutzergruppen zu bestimmten Eigenschaftsgruppen. Arbeitsbereiche ähneln auf vielerlei Weise den Report Suites in Adobe Analytics.

Siehe:

* [Berechtigungen für Unternehmensbenutzer](https://experienceleague.adobe.com/docs/target/using/administer/manage-users/enterprise/property-channel.html?lang=de)
* [Verwalten von Produkten und Profilen](https://helpx.adobe.com/de/enterprise/using/manage-products.html)
* Video: [Konfigurieren von Adobe Target-Arbeitsbereichen in Adobe [!DNL Admin Console]](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-17521.html?lang=de)

## Campaign – Produktprofile, Mandanten und Sicherheitsgruppen verwalten {#section_09CDF75366444CF5810CF321B7C712F3}

Ein *Mandant* wird in Campaign auf der Seite „Produkte der Admin Console“ als *Produkt* angezeigt.

Die *Sicherheitsgruppe* wird als Produktprofil angezeigt.

Informationen zu Sicherheitsgruppen und zum Zuweisen von Benutzern zu Sicherheitsgruppen finden Sie unter [Verwalten von Gruppen und Benutzern](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/users-and-security/managing-groups-and-users.html?lang=de).

## Verwalten der Experience Platform-Datenerfassung {#section_F2DA6778DD2D48AA8F794041971EE6B1}

Die Experience Platform-[!UICONTROL Datenerfassung] wird auf der Seite [!UICONTROL Produkte] in der [!UICONTROL Admin Console] angezeigt. Sie können weitere Programme und Services in ein Datenerfassungs-Produktprofil aufnehmen.

Laden Sie Benutzende zur [!UICONTROL Platform-Datenerfassung] ein und weisen Sie ihnen Benutzerrollen und -rechte zu.

Siehe [Benutzerberechtigungen](https://experienceleague.adobe.com/docs/experience-platform/tags/admin/user-permissions.html?lang=de) Informationen zu Benutzerberechtigungen finden Sie in der [!DNL Admin Console] und über das Einrichten von Profilberechtigungen.

## Experience Manager as a Cloud Service

Adobe Enterprise-Kunden werden in der Adobe als Organisationen dargestellt. [!DNL Admin Console]. Experience Manager-Kunden können die Adobe verwenden [!DNL Admin Console] Verwalten von Produktberechtigungen und IMS-Authentifizierung für Experience Manager as a [!UICONTROL Cloud Service].

Siehe [IMS-Unterstützung für Experience Manager as a Cloud Service](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/security/ims-support.html?lang=de).

## Audience Manager {#section_C31E3FA8A1E14463B1B3E07235F1983C}

Erstellen Sie Audience Manager-Benutzer und weisen Sie sie Gruppen zu. Sie können auch Einschränkungen anzeigen (Merkmale, Segmente, Ziele und [!DNL AlgoModel]).

Siehe [Administration](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/administration/administration-overview.html?lang=de) in der Hilfe zu Audience Manager.

## Unterstützte Browser in Experience Cloud

* [!DNL Microsoft® Edge] (Microsoft® hat für Internet Explorer 8, 9 und 10 den [Support beendet](https://www.microsoft.com/de-de/WindowsForBusiness/End-of-IE-support). Aus diesem Grund werden von Adobe keine Probleme mehr behoben, die in Verbindung mit diesen speziellen Versionen von Internet Explorer gemeldet werden.)
* [!DNL Google Chrome]
* [!DNL Firefox]
* [!DNL Safari]
* [!DNL Opera]

**Hinweis:** Obwohl die Experience Cloud-Oberfläche diese Browser unterstützt, unterstützen einzelne Anwendungen nicht alle Browser. ([Analytics](https://experienceleague.adobe.com/docs/analytics/admin/admin-overview/sys-reqs.html?lang=de) unterstützt beispielsweise nicht [!DNL Opera] und [!DNL Adobe Target] unterstützt nicht [!DNL Safari].)

### Anforderungen an Lösungen und Produkte

* [Analytics](https://experienceleague.adobe.com/docs/analytics/admin/admin-overview/sys-reqs.html?lang=de)
* [Report Builder ](https://experienceleague.adobe.com/docs/analytics/analyze/report-builder/report-builder-setup/system-requirements.html?lang=de)
