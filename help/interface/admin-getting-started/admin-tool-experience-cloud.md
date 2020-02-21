---
description: Erfahren Sie mehr über das Experience Cloud Admin Tool, um eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer anzuzeigen.
keywords: core services
seo-description: Erfahren Sie mehr über das Experience Cloud Admin Tool, um eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer anzuzeigen.
seo-title: Anzeigen von Experience Cloud-Benutzern und -Benutzerdetails
solution: Experience Cloud
title: 'Anzeigen von Experience Cloud-Benutzern und -Benutzerdetails '
translation-type: tm+mt
source-git-commit: 3595229c176bf4999ed149377adfeb55efc80071

---


# Experience Cloud Admin Tool

Das Experience Cloud-Admin-Tool ermöglicht es Administratoren, eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer anzuzeigen. Jede Seite mit Benutzerdetails enthält wichtige Details zum Produktzugriff, zu Rollen und zu zuletzt aufgerufenen Informationen.  

1. Log in to <https://experience.adobe.com/>.

   ![](assets/admin-tool.png)

1. Klicken Sie in der Experience Cloud-Startseite auf **[!UICONTROL Admin Tool.]** (Alternativ können Sie in der Startseiten-URL _Home_ durch _admin ersetzen._)

   Die Seite &quot; [!UICONTROL Benutzer] &quot;wird angezeigt.

## Benutzerseite

Auf dieser Seite wird eine vollständige Liste der Benutzer mit Zugriff auf Experience Cloud in Ihrer Organisation angezeigt. Es enthält Informationen zur Lösungsberechtigungen und zur letzten Anmeldung. Sie können nach benutzerdefinierten Ansichten der Benutzerliste suchen, sortieren und filtern.

![](assets/admin-tool-users.png)

| Element | Beschreibung |
|---|---|
| [!UICONTROL Name] | Der Vor- und Nachname des Benutzers. Sie können diese Spalte von A bis Z und Z bis A sortieren.  Klicken Sie auf den Namen eines Benutzers, um weitere Details zum Benutzer anzuzeigen. |
| [!UICONTROL E-Mail] | Die mit dem Benutzer verknüpfte E-Mail-Adresse. Die Spalte kann sortiert werden: A->Z, Z->A. |
| [!UICONTROL ID-Typ] | Der Identitätstyp für das Benutzerkonto. Filter können angewendet werden, um bestimmte ID-Typen anzuzeigen. Weitere Informationen finden Sie unter Identitätstypen [verwalten](https://helpx.adobe.com/enterprise/using/identity.html) . |
| [!UICONTROL Lösungen] | Zusammenfassung der Experience Cloud-Lösungen, auf die der Benutzer zugreifen kann. Sie können Filter anwenden, um eine Liste von Benutzern mit einem bestimmten Lösungszugriff einzuschränken. |
| [!UICONTROL Letzte Anmeldung] | Uhrzeit und Datum der letzten Benutzeranmeldung bei Experience Cloud. Diese Spalte kann nach auf- oder absteigenden Daten sortiert werden. <br> **** Wichtig: Die letzten Anmeldedaten werden nicht länger als 30 Tage vor dem Datumswert gespeichert, sodass die Benutzer möglicherweise keine Informationen zur letzten Anmeldung haben. [!UICONTROL Ab dem (Datum)] werden die letzten Anmeldedaten des Benutzers 365 Tage lang aufbewahrt. Sie können diese Informationen verwenden, um die aktuelle Anmeldeaktivität in der Experience Cloud anzuzeigen, jedoch nicht, um bei inaktiven Konten tätig zu werden. Außerdem haben kürzlich erstellte Benutzer möglicherweise keinen letzten Anmeldestatus. |

## Benutzerlistenansicht anpassen

Sie können die Spalten suchen, sortieren oder filtern, um die Benutzerliste anzupassen.

* Suchen Sie nach Benutzern nach Name oder E-Mail. Die Suchvorgänge entsprechen der eingegebenen Textzeichenfolge.
* Sortieren Sie die Spalte nach auf- oder absteigenden Werten. Dies gilt für Spalten [!UICONTROL Name,] [!UICONTROL E-Mail,] [!UICONTROL Letzte Anmeldung] .
* Klicken Sie auf das Symbol **[!UICONTROL Filtern nach]** , um mehrere Filter anzuwenden, um Benutzer mit bestimmten Kriterien aufzulisten. Wenn mehrere Filterkategorien angewendet werden, enthalten Suchvorgänge E-Mail-Domäne `AND` ID-Typ- `AND` Lösung.

| Element | Beschreibung |
|---------|----------|
| [!UICONTROL E-Mail-Domäne] -Filter | Suchen Sie in der Spalte &quot;E-Mail&quot;nach Zeichenfolgen, um die Ergebnisse auf eine oder mehrere Domänen zu beschränken. Fügen Sie mehrere Filter hinzu, indem Sie nach jedem Suchbegriff die Eingabetaste drücken |
| [!UICONTROL ID-Typ] -Filter | Wählen Sie aus den verfügbaren ID-Typen. Als Filter können mehrere ID-Typen verwendet werden. |
| [!UICONTROL Lösungsfilter] | Wählen Sie aus den verfügbaren Lösungen. Mehrere Lösungsfilter suchen nach Ergebnissen, die Lösung 1 `OR` Lösung 2 enthalten. |

## Benutzerdetails anzeigen

Klicken Sie auf der Seite &quot; [!UICONTROL Benutzer] &quot;auf die E-Mail-Adresse des Benutzers, um dessen Details anzuzeigen.

![](assets/admin-tool-user-details.png)

Eine detaillierte Ansicht der einzelnen Benutzer zeigt wichtige Details zum Lösungszugriff des Benutzers, zu Admin- und Produktrollen sowie zu den zuletzt aufgerufenen Informationen an.

## Info zu Abschnitt

In diesem Abschnitt wird eine Zusammenfassung des Benutzerkontos angezeigt, darunter:

* Benutzeravatar und Systemadmin-Badge (falls zutreffend)
* Name
* E-Mail
* Benutzername (bei Konten mit Federated ID können Benutzernamen von der E-Mail-Adresse abweichen)
* [ID-Typ](https://helpx.adobe.com/enterprise/using/identity.html)
* Land
* Letzte Anmeldung

## Lösungszusammenfassung

In diesem Abschnitt wird eine Zusammenfassung der Experience Cloud-Lösungen angezeigt, auf die der Benutzer zugreifen kann. Umfasst die Rolle der Produktverwaltung, sofern zutreffend

## Detaillierte Produktzugriffsliste

In diesem Abschnitt wird eine vollständige Liste aller Produktprofile angezeigt, die dem Benutzer zugehören.

| Element | Beschreibung |
|---------|----------|
| [!UICONTROL Produkt] | Name des Produkts, das mit dem Produktprofil verknüpft ist. |
| [!UICONTROL Instanz] | Name der Instanz (z. B. Anmelde- oder Mieter), die dem Produkt- und Produktprofil zugeordnet ist. |
| [!UICONTROL Produktprofil] | Eindeutiger Name des Produktprofils. |
| [!UICONTROL Nach Gruppe zugewiesen] | Name der Benutzergruppe, die den Benutzer mit einem Produktprofil verknüpft. Leere Ergebnisse zeigen an, dass der Benutzer dem Produktprofil direkt zugewiesen wurde, nicht über eine Gruppe. |
| [!UICONTROL Produktrollen] | Rollenzuweisung des Benutzers im Produktprofil. Diese Informationen gelten derzeit nur für Target-Produktprofile. |
