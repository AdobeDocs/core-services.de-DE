---
title: Anzeigen von Benutzern und Benutzerdetails
description: Erfahren Sie mehr über das Admin-Tool in Experience Cloud. Eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und -Richtlinien anzeigen.
application: Experience Cloud
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 127eecdd-3862-48ba-8cf6-a8082d2b7bae
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 83%

---

# Anzeigen von Experience Cloud-Benutzern und -Richtlinien in der [!UICONTROL Admin-Tool]

Administratoren können eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und -Richtlinien mit Details in der Datei anzeigen. [!UICONTROL Admin-Tool]. Zu den Benutzerdetails zählen der Produktzugriff und die Rollen der Benutzer sowie die zuletzt aufgerufenen Informationen. Zu den Richtliniendetails gehören die Benutzenden-, Gruppen-, Entwickler-, Integrations- und Admin-Liste einer Richtlinie (Produktprofil) sowie detaillierte Berechtigungen und Ressourceninformationen für die Richtlinie.

>[!NOTE]
>
>Benutzer- und Produktverwaltung werden in der [Admin Console](admin-getting-started.md) konfiguriert.

1. Melden Sie sich bei `https://experience.adobe.com/.` an.

   ![Zugriff auf Admin Console](assets/admin-tool.png)

1. Unter [!UICONTROL Schnellzugriff], klicken Sie auf **[!UICONTROL Admin-Tool]**.

   (Alternativ können Sie in der Startseiten-URL _home_ durch _admin_ ersetzen.)

   Die Seite [!UICONTROL Benutzer] wird angezeigt.

## Seite „Benutzer“

Auf dieser Seite wird die vollständige Liste der Benutzer mit Zugriff auf Experience Cloud in Ihrer Organisation angezeigt. Sie enthält Informationen zu Programmberechtigungen und zur letzten Anmeldung. Sie können nach benutzerdefinierten Ansichten der Benutzerliste suchen, sortieren und filtern.

![Admin Console-Benutzerseite](assets/admin-tool-users.png)

| Element | Beschreibung |
|---|---|
| [!UICONTROL Name] | Der Vor- und Nachname des Benutzers. Sie können diese Spalte von A bis Z und von Z bis A sortieren. Wählen Sie den Namen eines Benutzers aus, um weitere Details zu ihm anzuzeigen. |
| [!UICONTROL E-Mail] | Die mit dem Benutzer verknüpfte E-Mail-Adresse. Die Spalte kann von A bis Z und von Z bis A sortiert werden. |
| [!UICONTROL ID-Typ] | Der Identitätstyp für das Konto des Benutzers. Es können Filter angewendet werden, um spezielle ID-Typen anzuzeigen. Weitere Informationen finden Sie unter [Verwalten von Identitätstypen](https://helpx.adobe.com/de/enterprise/using/identity.html). |
| [!UICONTROL Lösungen] | Zusammenfassung der Experience Cloud-Programme, auf die der Benutzer zugreifen kann. Sie können Filter anwenden, um die Liste auf Benutzer mit Zugriff auf bestimmte Programme einzuschränken. |
| [!UICONTROL Letzte Anmeldung] | Uhrzeit und Datum der letzten Benutzeranmeldung beim Experience Cloud. Diese Spalte kann nach auf- oder absteigenden Datumsangaben sortiert werden. <br> **Wichtig:** Ab dem 13. Januar 2020 werden die letzten Anmeldedaten eines Benutzers 365 Tage lang aufbewahrt. Diese Informationen sollen die aktuelle Anmeldeaktivität in Experience Cloud anzeigen und keine Empfehlung für Maßnahmen bei inaktiven Konten vor dem 13. Januar 2020 sein. |

## Anpassen der Benutzerlistenansicht

Sie können die Spalten suchen, sortieren oder filtern, um die Benutzerliste anzupassen.

* Suchen Sie Benutzer nach Name oder E-Mail-Adresse. Die Suchvorgänge entsprechen der von Ihnen eingegebenen Textzeichenfolge.
* Sortieren Sie die Spalte nach auf- oder absteigenden Werten. Dies Sortierung gilt für die Spalten [!UICONTROL Name], [!UICONTROL E-Mail], und [!UICONTROL Letzte Anmeldung].
* Um mehrere Filter anzuwenden und Benutzer mit bestimmten Kriterien aufzulisten, klicken Sie auf das Symbol **[!UICONTROL Filtern nach]**. Wenn mehrere Filterkategorien angewendet werden, enthalten Suchvorgänge die E-Mail-Domäne `AND` ID-Typ `AND` Lösung.

| Element | Beschreibung |
|---------|----------|
| Filter [!UICONTROL E-Mail-Domäne] | Suchen Sie in der Spalte „E-Mail“ nach Zeichenfolgen, um die Ergebnisse auf eine oder mehrere Domänen zu beschränken. Hinzufügen mehrerer Filter durch Drücken der Eingabetaste nach jedem Suchbegriff. |
| Filter [!UICONTROL ID-Typ] | Wählen Sie aus den verfügbaren ID-Typen aus. Als Filter können mehrere ID-Typen verwendet werden. |
| Filter [!UICONTROL Lösung] | Wählen Sie aus den verfügbaren Programmen. Mehrfache Programmfilter suchen nach Ergebnissen, die Lösung 1 `OR` Lösung 2 enthalten. |

## Anzeigen der Benutzerdetails

Wählen Sie auf der Seite [!UICONTROL Benutzer] die E-Mail-Adresse eines Benutzers aus, um seine Details anzuzeigen.

![Anzeigen von Benutzerdetails in Admin Console](assets/admin-tool-user-details.png)

Eine detaillierte Ansicht jedes Benutzers zeigt wichtige Details zum Programmzugriff, zu den Admin- und Produktrollen sowie zu den zuletzt aufgerufenen Informationen des Benutzers an.

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

In diesem Abschnitt wird eine Zusammenfassung der Experience Cloud-Programme angezeigt, auf die der Benutzer zugreifen kann. Umfasst die Rolle der Produktverwaltung, sofern anwendbar.

## Detaillierte Liste des Produktzugriffs

In diesem Abschnitt wird eine vollständige Liste aller Produktprofilmitgliedschaften für den Benutzer angezeigt.

| Element | Beschreibung |
|---------|----------|
| [!UICONTROL Produkt] | Name des Produkts, das mit dem Profil verknüpft ist. |
| [!UICONTROL Instanz] | Name der Instanz (z. B. Unternehmensanmeldung oder Mandant), die mit dem Produkt und Produktprofil verknüpft ist. |
| [!UICONTROL Produktprofil] | Eindeutiger Name des Produktprofils. |
| [!UICONTROL Nach Gruppe zugewiesen] | Name der Benutzergruppe, die den Benutzer mit einem Produktprofil verknüpft. Leere Ergebnisse geben an, dass der Benutzer dem Produktprofil direkt und nicht über eine Gruppe zugewiesen wurde. |
| [!UICONTROL Produktrollen] | Rollenzuweisung des Benutzers im Produktprofil. Diese Informationen gelten derzeit nur für Adobe Target-Produktprofile. |

## Seite „Richtlinien“

Auf dieser Seite finden Sie eine vollständige Liste der Experience Cloud-Richtlinien in Ihrem Unternehmen. Sie enthält Informationen zu Produkten, Instanzen, Benutzern und Entwicklern. Sie können nach benutzerdefinierten Ansichten der Richtlinienliste suchen, sortieren und filtern.

![Richtlinienseite in Admin Console](assets/admin-tool-policies.png)

| Element | Beschreibung |
|---|---|
| [!UICONTROL Produktprofil] | Der Name des Produktprofils. Die Spalte kann A->Z oder Z->A sortiert werden. Um weitere Details zur Richtlinie anzuzeigen, wählen Sie den Namen eines Produktprofils aus. |
| [!UICONTROL Produkt] | Das Produkt, das mit dem Produktprofil verknüpft ist. Die Spalte kann von A bis Z und von Z bis A sortiert werden. |
| [!UICONTROL Instanz] | Die Instanz (z. B. Mandant oder angemeldetes Unternehmen), die mit dem Produktprofil verknüpft ist. Produkte ohne eindeutige Instanzen oder Mandanten haben als Wert „-“. Die Spalte kann von A bis Z und von Z bis A sortiert werden. |
| [!UICONTROL Anzahl der Benutzer] | Eindeutige Anzahl der mit dem Produktprofil verknüpften Benutzer, einschließlich direkter Zuweisung und Gruppenzuweisung. Die Spalte kann vom Kleinsten bis zum Größten oder vom Größten bis zum Kleinsten sortiert werden. |
| [!UICONTROL Anzahl der Entwickler] | Anzahl der mit dem Produktprofil verbundenen Entwicklerrollen. Die Spalte kann vom Kleinsten bis zum Größten oder vom Größten bis zum Kleinsten sortiert werden. |

## Anpassen der Richtlinienlistenansicht

Sie können die Spalten suchen, sortieren oder filtern, um die Richtlinienliste anzupassen.

* Suchen Sie nach Produktprofilen mit dem Namen. Die Suchvorgänge entsprechen der von Ihnen eingegebenen Textzeichenfolge.
* Sortieren Sie die Spalte nach auf- oder absteigenden Werten. Diese Sortierung gilt für [!UICONTROL Produktprofil,] [!UICONTROL Produkt,] [!UICONTROL Instance,] [!UICONTROL Anzahl der Benutzer,] und [!UICONTROL Anzahl der Entwickler,] Spalten.
* Wählenn Sie das Symbol **[!UICONTROL Filtern nach]** aus, um mehrere Filter anzuwenden und Produktprofile mit bestimmten Kriterien aufzulisten. Wenn mehrere Filterkategorien angewendet werden, enthalten Suchvorgänge Gruppen, die mit der `AND` Instanzlösung `AND` verknüpft sind.

| Element | Beschreibung |
|---------|----------|
| [!UICONTROL Instanzfilter] | Suchen Sie in der Spalte „Instanz“ nach Zeichenfolgen, um die Ergebnisse auf eine oder mehrere Instanzen zu beschränken. Sie können mehrerer Filter durch Drücken der Eingabetaste nach jedem Suchbegriff hinzufügen. |
| Filter [!UICONTROL Lösung] | Wählen Sie aus den verfügbaren Programmen. Mehrfache Programmfilter suchen nach Ergebnissen, die Lösung 1 `OR` Lösung 2 enthalten. |

## Ansicht der Richtliniendetails

Wählen Sie auf der Seite [!UICONTROL Richtlinien] den Produktprofilnamen aus, um die Details einer Richtlinie anzuzeigen.

![Richtliniendetails in Admin Console anzeigen](assets/admin-tool-policy-detail.png)

Eine detaillierte Ansicht der einzelnen Produktprofile enthält wichtige Details zu den Themen des Produktprofils (Benutzer, Gruppen usw.). Außerdem werden Zugriffsberechtigungen und Ressourcen angezeigt, die vom Produktprofil aktiviert wurden.

Details des Produktprofils können in CSV-Dateien exportiert werden. Bei der Option [!UICONTROL CSV exportieren] werden zwei CSV-Dateien erzeugt:

* Personendetails (Benutzer, Benutzergruppen, Entwickler, Integrationen, Administratoren)
* Informationen zu Berechtigungen und Ressourcen

## Zusammenfassung

In diesem Abschnitt wird eine Zusammenfassung des Produktprofils angezeigt, einschließlich Folgendem:

* Name des Produktprofils
* Anzahl der Benutzer
* Anzahl der Entwickler
* Anzahl der Integrationen
* Zugehörige Produkte
* Instanz

## Detaillierte Personenliste

Dieser Abschnitt enthält eine vollständige Liste aller Benutzer, Benutzergruppen, Entwickler, Integrationen und Administratoren, die dem Profil zugewiesen sind.

| Tab | Beschreibung |
|---------|----------|
| [!UICONTROL Benutzer] | Die Liste der im Produktprofil enthaltenen Benutzer. Die Benutzergruppenzuordnung wird in der Spalte [!UICONTROL Nach Gruppe zugewiesen] angezeigt. |
| [!UICONTROL Benutzergruppen] | Die Liste der mit dem Produktprofil verknüpften Benutzergruppen. |
| [!UICONTROL Entwickler] | Die Liste der mit dem Produktprofil verbundenen Entwickler. |
| [!UICONTROL Integrationen] | Die Liste der mit dem Produktprofil verbundenen Integrationen. |
| [!UICONTROL Administratoren] | Die Liste der mit dem Produktprofil verknüpften Administratoren. |

## Detaillierte Listen zu Berechtigungen und Ressourcen

Dieser Abschnitt enthält eine vollständige Liste der Berechtigungen und Ressourcen, die für das Produktprofil verfügbar sind. Berechtigungen und Ressourcen, die im Produktprofil enthalten sind, sind mit einem ✔ gekennzeichnet. Die Listen der Berechtigungen und Ressourcen wurden zur einfacheren Anzeige in Registerkarten und Spalten geordnet. Registerkarten und Spalten zeigen die Liste der Abschnitte an, die für das aktuelle Produkt gelten.

## Ergänzende Informationen

* [Verwalten von Benutzern](https://helpx.adobe.com/de/enterprise/using/users.html) in der [!DNL Admin Console]