---
description: Erfahren Sie mehr über das Experience Cloud Admin Tool, um eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer Ansicht.
keywords: core services
seo-description: Erfahren Sie mehr über das Experience Cloud Admin Tool, um eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer Ansicht.
seo-title: Ansicht Experience Cloud-Benutzer und -Benutzerdetails
solution: Experience Cloud
title: 'Ansicht Experience Cloud-Benutzer und -Benutzerdetails '
index: true
translation-type: tm+mt
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e

---


# Ansicht Experience Cloud-Benutzer im Admin Tool

Administratoren können eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und deren Details im Admin Tool Ansicht haben. Zu den Benutzerdetails zählen der Produktzugriff, die Rollen und die zuletzt aufgerufenen Informationen. (**Hinweis:** Benutzer- und Produktverwaltung werden in der [Admin-Konsole](admin-getting-started.md)konfiguriert.)

1. Log in to `https://experience.adobe.com/.`

   ![](assets/admin-tool.png)

1. Klicken Sie in der Experience Cloud-Startseite auf **[!UICONTROL Admin Tool.]**

   (Alternativ können Sie in der Startseiten-URL _home_ durch _admin ersetzen._)

   Die Seite &quot; [!UICONTROL Benutzer] &quot;wird angezeigt.

## Benutzerseite

Auf dieser Seite wird die vollständige Liste der Benutzer mit Zugriff auf Experience Cloud in Ihrem Unternehmen angezeigt. Es enthält Informationen zur Lösungsberechtigungen und zur letzten Anmeldung. Sie können nach benutzerdefinierten Ansichten der Liste suchen, sortieren und filtern.

![](assets/admin-tool-users.png)

| Element | Beschreibung |
|---|---|
| [!UICONTROL Name] | Der Vor- und Nachname des Benutzers. Sie können diese Spalte von A bis Z und Z bis A sortieren.  Klicken Sie auf den Namen eines Benutzers, um weitere Details zum Benutzer anzuzeigen. |
| [!UICONTROL E-Mail ] | Die mit dem Benutzer verknüpfte E-Mail-Adresse. Die Spalte kann sortiert werden: A->Z, Z->A. |
| [!UICONTROL ID-Typ] | Der Identitätstyp für das Konto des Benutzers. Filter können auf Ansichten-spezifische ID-Typen angewendet werden. Weitere Informationen finden Sie unter Identitätstypen [verwalten](https://helpx.adobe.com/enterprise/using/identity.html) . |
| [!UICONTROL Lösungen] | Zusammenfassung der Experience Cloud-Lösungen, auf die der Benutzer zugreifen kann. Sie können Filter anwenden, um die Liste von Benutzern mit einem bestimmten Lösungszugriff einzuschränken. |
| [!UICONTROL Letzte Anmeldung] | Uhrzeit und Datum der letzten Benutzeranmeldung bei Experience Cloud. Diese Spalte kann nach auf- oder absteigenden Daten sortiert werden. <br> **Wichtig:** Ab dem 13. Januar 2020 werden die letzten Anmeldedaten eines Benutzers 365 Tage lang aufbewahrt. Diese Informationen sollen die aktuelle Aktivität bei der Anmeldung in der Experience Cloud anzeigen und nicht empfehlen, vor dem 13. Januar 2020 Maßnahmen für inaktive Konten zu ergreifen. |

## Benutzerdefinierte Liste-Ansicht

Sie können die Spalten suchen, sortieren oder filtern, um die Liste des Benutzers anzupassen.

* Suchen Sie nach Benutzern nach Name oder E-Mail. Die Suchvorgänge entsprechen der von Ihnen eingegebenen Textzeichenfolge.
* Sortieren Sie die Spalte nach auf- oder absteigenden Werten. Dies gilt für Spalten [!UICONTROL Name,] [!UICONTROL E-Mail,] [!UICONTROL Letzte Anmeldung] .
* Klicken Sie auf das Symbol **[!UICONTROL Filtern nach]** , um mehrere Filter auf Listen mit bestimmten Kriterien anzuwenden. Wenn mehrere Filter-Kategorien angewendet werden, enthalten Suchvorgänge E-Mail-Domäne `AND` ID- `AND` Typ-Lösung.

| Element | Beschreibung |
|---------|----------|
| [!UICONTROL E-Mail-Domäne] -Filter | Suchen Sie in der Spalte &quot;E-Mail&quot;nach Zeichenfolgen, um die Ergebnisse auf eine oder mehrere Domänen zu beschränken. Hinzufügen mehrerer Filter durch Drücken der Eingabetaste nach jedem Suchbegriff |
| [!UICONTROL ID-Typ] -Filter | Wählen Sie aus den verfügbaren ID-Typen. Als Filter können mehrere ID-Typen verwendet werden. |
| [!UICONTROL Lösungsfilter] | Wählen Sie aus den verfügbaren Lösungen. Mehrere Lösungs-Filter suchen nach Ergebnissen, die Lösung 1 `OR` Lösung 2 enthalten. |

## Benutzerdetails der Ansicht

Klicken Sie auf der Seite &quot; [!UICONTROL Benutzer] &quot;auf die E-Mail-Adresse des Benutzers, um die Benutzerdetails Ansicht.

![](assets/admin-tool-user-details.png)

Eine detaillierte Ansicht der einzelnen Benutzer enthält wichtige Informationen zum Lösungszugriff, zu den Admin- und Produktrollen sowie zu den zuletzt aufgerufenen Informationen.

## Info zu Abschnitt

In diesem Abschnitt wird eine Zusammenfassung des Benutzerkontos angezeigt, darunter:

* Benutzeravatar und Systemadmin-Badge (falls zutreffend)
* Name
* E-Mail 
* Benutzername (bei Konten mit Federated ID können Benutzernamen von der E-Mail-Adresse abweichen)
* [ID-Typ](https://helpx.adobe.com/enterprise/using/identity.html)
* Country
* Letzte Anmeldung

## Lösungszusammenfassung

In diesem Abschnitt wird eine Zusammenfassung der Experience Cloud-Lösungen angezeigt, auf die der Benutzer zugreifen kann. Umfasst die Rolle der Produktverwaltung, sofern zutreffend.

## Detaillierte Liste des Produktzugriffs

In diesem Abschnitt wird eine vollständige Liste aller Produktbenutzermitgliedschaften für Profil angezeigt.

| Element | Beschreibung |
|---------|----------|
| [!UICONTROL Produkt] | Name des Produkts, das mit dem Profil verknüpft ist. |
| [!UICONTROL Instanz] | Name der Instanz (z. B. Anmelde- oder Mieter-Firma), die mit dem Produkt- und Produkt-Profil verknüpft ist. |
| [!UICONTROL Produkt-Profil] | Eindeutiger Name des Profils. |
| [!UICONTROL Nach Gruppe zugewiesen] | Name der Benutzergruppe, die den Benutzer mit einem Profil verknüpft. Leere Ergebnisse zeigen an, dass der Benutzer dem Profil direkt zugewiesen wurde, nicht über eine Gruppe. |
| [!UICONTROL Produktrollen] | Rollenzuweisung des Benutzers im Profil des Produkts. Diese Informationen gelten derzeit nur für Adobe Zielgruppe-Profil. |
