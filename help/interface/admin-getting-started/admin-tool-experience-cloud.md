---
description: Lernen Sie das Experience Cloud Admin-Tool kennen, um eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer anzuzeigen.
keywords: core services
seo-description: Lernen Sie das Experience Cloud Admin-Tool kennen, um eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer anzuzeigen.
seo-title: Anzeigen von Experience Cloud-Benutzern und -Benutzerdetails
solution: Experience Cloud
title: 'Anzeigen von Experience Cloud-Benutzern und -Benutzerdetails '
index: true
translation-type: ht
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e
workflow-type: ht
source-wordcount: '693'
ht-degree: 100%

---


# Anzeigen von Experience Cloud-Benutzern im Admin-Tool

Administratoren können im Admin-Tool eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und deren Details anzeigen. Zu den Benutzerdetails zählen der Produktzugriff, die Rollen und die zuletzt aufgerufenen Informationen. (**Hinweis:** Benutzer- und Produktverwaltung werden in der [Admin Console](admin-getting-started.md) konfiguriert.)

1. Bei anmelden.`https://experience.adobe.com/.`

   ![](assets/admin-tool.png)

1. Klicken Sie auf der Experience Cloud-Startseite auf **[!UICONTROL Admin Tool.]**

   (Alternativ können Sie in der Startseiten-URL _home_ durch _admin_ ersetzen.)

   Die Seite [!UICONTROL Benutzer] wird angezeigt.

## Seite „Benutzer“

Auf dieser Seite wird die vollständige Liste der Benutzer mit Zugriff auf Experience Cloud in Ihrer Organisation angezeigt. Sie enthält Informationen zur Lösungsberechtigungen und zur letzten Anmeldung. Sie können nach benutzerdefinierten Ansichten der Benutzerliste suchen, sortieren und filtern.

![](assets/admin-tool-users.png)

| Element | Beschreibung |
|---|---|
| [!UICONTROL Name] | Der Vor- und Nachname des Benutzers. Sie können diese Spalte von A bis Z und Z bis A sortieren. Klicken Sie auf den Namen eines Benutzers, um weitere Details zu ihm anzuzeigen. |
| [!UICONTROL E-Mail] | Die mit dem Benutzer verknüpfte E-Mail-Adresse. Die Spalte kann von A bis Z und von Z bis A sortiert werden. |
| [!UICONTROL ID-Typ] | Der Identitätstyp für das Konto des Benutzers. Es können Filter angewendet werden, um spezielle ID-Typen anzuzeigen. Weitere Informationen finden Sie unter [Verwalten von Identitätstypen](https://helpx.adobe.com/de/enterprise/using/identity.html). |
| [!UICONTROL Lösungen] | Zusammenfassung der Experience Cloud-Lösungen, auf die der Benutzer zugreifen kann. Sie können Filter anwenden, um die Liste der Benutzer mit einem bestimmten Lösungszugriff einzuschränken. |
| [!UICONTROL Letzte Anmeldung] | Uhrzeit und Datum der letzten Benutzeranmeldung bei der Experience Cloud. Diese Spalte kann nach auf- oder absteigenden Datumsangaben sortiert werden. <br> **Wichtig:** Ab dem 13. Januar 2020 werden die letzten Anmeldedaten eines Benutzers 365 Tage lang aufbewahrt. Diese Informationen sollen die aktuelle Aktivität bei der Anmeldung in der Experience Cloud anzeigen und sie dienen nicht als Empfehlung, vor dem 13. Januar 2020 Maßnahmen für inaktive Konten zu ergreifen. |

## Anpassen der Benutzerlistenansicht

Sie können die Spalten suchen, sortieren oder filtern, um die Benutzerliste anzupassen.

* Suchen Sie Benutzer nach Name oder E-Mail-Adresse. Die Suchvorgänge entsprechen der von Ihnen eingegebenen Textzeichenfolge.
* Sortieren Sie die Spalte nach auf- oder absteigenden Werten. Dies gilt für die Spalten [!UICONTROL Name], [!UICONTROL E-Mail] und [!UICONTROL Letzte Anmeldung].
* Klicken Sie auf das Symbol **[!UICONTROL Filtern nach]**, um mehrere Filter anzuwenden und Benutzer mit bestimmten Kriterien aufzulisten. Wenn mehrere Filterkategorien angewendet werden, enthalten Suchvorgänge die E-Mail-Domäne `AND`ID-Typ `AND` Lösung.

| Element | Beschreibung |
|---------|----------|
| Filter [!UICONTROL E-Mail-Domäne] | Suchen Sie in der Spalte „E-Mail“ nach Zeichenfolgen, um die Ergebnisse auf eine oder mehrere Domänen zu beschränken. Hinzufügen mehrerer Filter durch Drücken der Eingabetaste nach jedem Suchbegriff. |
| Filter [!UICONTROL ID-Typ] | Wählen Sie aus den verfügbaren ID-Typen aus. Als Filter können mehrere ID-Typen verwendet werden. |
| Filter [!UICONTROL Lösung] | Wählen Sie aus den verfügbaren Lösungen aus. Mehrere Lösungsfilter suchen nach Ergebnissen, die Lösung 1 `OR` Lösung 2 enthalten. |

## Anzeigen der Benutzerdetails

Klicken Sie auf der Seite [!UICONTROL Benutzer] auf die E-Mail-Adresse des Benutzers, um die Details des jeweiligen Benutzers anzuzeigen.

![](assets/admin-tool-user-details.png)

Eine detaillierte Ansicht der einzelnen Benutzer enthält wichtige Einzelheiten zum Lösungszugriff, zu den Admin- und Produktrollen sowie zu den zuletzt aufgerufenen Informationen.

## Abschnitt „Info“

In diesem Abschnitt wird eine Zusammenfassung des Benutzerkontos angezeigt, einschließlich Folgendem:

* Benutzeravatar und Systemadmin-Zeichen (falls zutreffend)
* Name
* E-Mail
* Benutzername (bei Konten mit Federated ID können Benutzernamen von der E-Mail-Adresse abweichen)
* [ID-Typ](https://helpx.adobe.com/de/enterprise/using/identity.html)
* Land
* Letzte Anmeldung

## Lösungszusammenfassung

In diesem Abschnitt wird eine Zusammenfassung der Experience Cloud-Lösungen angezeigt, auf die der Benutzer zugreifen kann. Umfasst die Rolle der Produktverwaltung, sofern zutreffend.

## Detaillierte Liste des Produktzugriffs

In diesem Abschnitt wird eine vollständige Liste aller Produktprofilmitgliedschaften für den Benutzer angezeigt.

| Element | Beschreibung |
|---------|----------|
| [!UICONTROL Produkt] | Name des Produkts, das mit dem Profil verknüpft ist. |
| [!UICONTROL Instanz] | Name der Instanz (z. B. Unternehmensanmeldung oder Mandant), die mit dem Produkt und Produktprofil verknüpft ist. |
| [!UICONTROL Produktprofil] | Eindeutiger Name des Produktprofils. |
| [!UICONTROL Nach Gruppe zugewiesen] | Name der Benutzergruppe, die den Benutzer mit einem Produktprofil verknüpft. Leere Ergebnisse geben an, dass der Benutzer dem Produktprofil direkt und nicht über eine Gruppe zugewiesen wurde. |
| [!UICONTROL Produktrollen] | Rollenzuweisung des Benutzers im Produktprofil. Diese Informationen gelten derzeit nur für Adobe Target-Produktprofile. |
