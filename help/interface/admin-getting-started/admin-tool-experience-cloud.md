---
description: Erfahren Sie mehr über das Experience Cloud Admin Tool, um eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und -Richtlinien Ansicht.
keywords: core services
seo-description: Erfahren Sie mehr über das Experience Cloud Admin Tool, um eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und -Richtlinien Ansicht.
seo-title: Anzeigen von Experience Cloud-Benutzern und -Benutzerdetails
solution: Experience Cloud
title: 'Anzeigen von Experience Cloud-Benutzern und -Benutzerdetails '
index: true
translation-type: tm+mt
source-git-commit: fa03e384d1dc878d45ef4b8d1f6fe269734ea891
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 52%

---


# Ansicht Experience Cloud-Benutzer und -Richtlinien im Admin Tool

Administratoren können eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und -Richtlinien mit Details im Admin Tool Ansicht. Zu den Benutzerdetails zählen der Produktzugriff, die Rollen und die zuletzt aufgerufenen Informationen. Zu den Richtliniendetails gehören der Benutzer, die Gruppe, der Entwickler, die Integration und die Admin-Liste einer Richtlinie (Profil) sowie detaillierte Informationen zu Berechtigungen und Ressourcen für die Richtlinie.

>[!NOTE]
>
>User and product management is configured in the [Admin Console](admin-getting-started.md).

1. Bei anmelden.`https://experience.adobe.com/.`

   ![](assets/admin-tool.png)

1. Klicken Sie unter [!UICONTROL Schnellzugriff]auf **[!UICONTROL Admin Tool.]**

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

## Info zu Abschnitt

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

## Seite &quot;Richtlinien&quot;

Auf dieser Seite finden Sie eine vollständige Liste der Experience Cloud-Richtlinien in Ihrem Unternehmen. Es enthält Informationen zu Produkten, Instanzen, Benutzern und Entwicklern. Sie können nach benutzerdefinierten Ansichten der Liste suchen, sortieren und filtern.

![](assets/admin-tool-policies.png)

| Element | Beschreibung |
|---|---|
| [!UICONTROL Produktprofil] | Der Name des Profils. Die Spalte kann sortiert werden: A->Z, Z->A. Klicken Sie auf den Profil eines Produkts, um weitere Details zur Richtlinie anzuzeigen. |
| [!UICONTROL Produkt] | Das Produkt, das mit dem Profil verknüpft ist. Die Spalte kann von A bis Z und von Z bis A sortiert werden. |
| [!UICONTROL Instanz] | Die Instanz (z. B. Mieter- oder Anmelde-Firma), die mit dem Profil des Produkts verknüpft ist. Produkte ohne eindeutige Instanzen oder Mandanten zeigen ein &quot;-&quot;für den Wert an. Die Spalte kann von A bis Z und von Z bis A sortiert werden. |
| [!UICONTROL Anzahl der Benutzer] | Eindeutige Anzahl der mit dem Profil verknüpften Benutzer, einschließlich direkter Zuweisung und Gruppenzuweisung. Die Spalte kann vom kleinsten bis zum größten oder vom größten bis zum kleinsten sortiert werden. |
| [!UICONTROL Anzahl Entwickler] | Anzahl der mit dem Produkt-Profil verbundenen Entwicklerrollen. Die Spalte kann vom kleinsten bis zum größten oder vom größten bis zum kleinsten sortiert werden. |

## Richtlinien anpassen - Liste Ansicht

Sie können die Spalten suchen, sortieren oder filtern, um die Richtlinien-Liste anzupassen.

* Suchen Sie anhand des Namens nach Produkt-Profilen. Die Suchvorgänge entsprechen der von Ihnen eingegebenen Textzeichenfolge.
* Sortieren Sie die Spalte nach auf- oder absteigenden Werten. Dies gilt für [!UICONTROL Product Profil,] [!UICONTROL Product,] [!UICONTROL Instance,] [!UICONTROL Anzahl der Benutzer und] Anzahl der Entwickler,  Spalten.
* Click the **[!UICONTROL Filter By]** icon to apply multiple filters to list product profiles with specific criteria. Wenn mehrere Filter-Kategorien angewendet werden, enthalten Suchvorgänge Gruppen, die mit der `AND` Instanzlösung `AND` verknüpft sind.

| Element | Beschreibung |
|---------|----------|
| [!UICONTROL Instanzfilter] | Suchen Sie in der Spalte &quot;Instanz&quot;nach Zeichenfolgen, um die Ergebnisse auf eine oder mehrere Instanzen zu beschränken. hinzufügen mehrere Filter durch Drücken der Eingabetaste nach jedem Suchbegriff. |
| Filter [!UICONTROL Lösung] | Wählen Sie aus den verfügbaren Lösungen aus. Mehrere Lösungsfilter suchen nach Ergebnissen, die Lösung 1 `OR` Lösung 2 enthalten. |

## Details zur Ansicht

Klicken Sie auf der Seite &quot; [!UICONTROL Richtlinien] &quot;auf den Produktnamen, um die Details einer Richtlinie Ansicht.

![](assets/admin-tool-policy-detail.png)

Eine detaillierte Ansicht der einzelnen Profil zeigt wichtige Details zu den Themen des Profils (Benutzer, Gruppen usw.) an. Außerdem werden Berechtigungen und Ressourcen angezeigt, die vom Profil des Produkts aktiviert wurden.

Details des Profils können in CSV-Dateien exportiert werden. Bei der Option &quot;CSV  exportieren&quot;werden zwei CSV-Dateien erzeugt:

* Themendetails (Benutzer, Benutzergruppen, Entwickler, Integrationen, Administratoren)
* Elemente zu Berechtigungen und Ressourcen

## Übersichtsabschnitt

In diesem Abschnitt wird eine Zusammenfassung des Profils des Produkts angezeigt, darunter:

* Produktname Profil
* Anzahl der Benutzer
* Anzahl der Entwickler
* Anzahl der Integrationen
* Zugehörige Produkte
* Instanz

## Detaillierte Liste

Dieser Abschnitt enthält eine vollständige Liste aller Benutzer, Benutzergruppen, Entwickler, Integrationen und Administratoren, die dem Profil zugewiesen sind.

| Tab | Beschreibung |
|---------|----------|
| [!UICONTROL Benutzer] | Liste der im Produkt-Profil enthaltenen Benutzer. Die Benutzergruppenzuordnung wird in der Spalte [!UICONTROL Zugewiesen nach Gruppe] angezeigt. |
| [!UICONTROL Benutzergruppen] | Liste der mit dem Produkt-Profil verknüpften Benutzergruppen. |
| [!UICONTROL Entwickler] | Liste der mit dem Produkt-Profil verbundenen Entwickler. |
| [!UICONTROL Integrationen] | Liste von Integrationen, die mit dem Produkt-Profil verbunden sind. |
| [!UICONTROL Administratoren] | Liste von Administratoren, die mit dem Produkt-Profil verknüpft sind. |

## Detaillierte Listen zu Berechtigungen und Ressourcen

Dieser Abschnitt enthält eine vollständige Liste der Berechtigungen und Ressourcen, die für das Profil verfügbar sind. Berechtigungen und Ressourcen, die im Profil des Produkts enthalten sind, wurden mit einem ✔ gekennzeichnet. Die Listen der Berechtigungen und Ressourcen wurden zur einfacheren Anzeige in Registerkarten und Spalten kategorisiert. Registerkarten und Spalten zeigen die Liste der Abschnitte an, die für das aktuelle Produkt gelten.
