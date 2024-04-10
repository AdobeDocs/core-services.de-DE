---
description: Erfahren Sie mehr über die Anforderungen und Möglichkeiten bei der Aktualisierung auf Analytics Premium.
solution: Experience Cloud
title: Upgrade auf Analytics Premium und Experience Cloud
topic: Administration
uuid: 450a601c-d199-4e90-b525-19bd9f9576d2
feature: Admin Console
role: Admin
level: Experienced
exl-id: 746d396d-9629-42db-8c55-07d2d24e4611
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 90%

---

# Aktualisieren auf Analytics Premium und Experience Cloud

Administratoren können mehr darüber erfahren, was sie bei einem Upgrade auf Analytics Premium erwartet, wie hoch die Anforderungen sind und wo sie als Experience Cloud-Administrator Hilfe finden.

## Analytics Premium {#section_7F50AD7906544F899B844BE31D3BB507}

Durch die Aktualisierung auf Adobe Analytics Premium erhalten Sie alle verfügbaren Funktionen oder Produkte von Analytics Standard, einschließlich Data Warehouse, Ad Hoc Analysis, Report Builder und Data Connectors.

Analytics Premium bietet Ihnen:

* Zugriff auf 250 Konversionsvariablen (eVars)
* [Mobile App Analytics](https://experienceleague.adobe.com/docs/mobile-services/using/home.html?lang=de)
* Data Workbench (visuelle Datenabfrage, regelbasierte Zuordnung, kanalübergreifende Analyse)

>[!NOTE]
>
>Bei der Aktualisierung ist keine Migration erforderlich. Beachten Sie jedoch Folgendes:
>
>* Die eVars 76-250 und 100-250 (Standard) sind in den Admin Tools sichtbar, sind jedoch nicht aktiviert.
>* Die Beitragsanalyse wird von Adobe aktiviert. Der Speicherort wird nicht geändert (er ist weiterhin auf der Seite „Anomalieerkennung“ verfügbar), aber die Analyse aller Datenpunkte wird automatisch gestartet.

## Analytics Premium Complete {#section_BFAD815EDF364845A52B340B2FD5B64C}

In Analytics Premium Complete erhalten Sie alle Funktionen von [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) sowie die folgenden Upgrades:

| Produkt | Upgrades |
|--- |--- |
| Reports &amp; Analytics | <ul><li>[Beitragsanalyse](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html?lang=de)</li><li>[Kundenattribute](attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1) (bis zu 200)</li></ul> |
| Data Workbench | <ul><li>Algorithmische Zuordnung</li><li>Vordefinierte Arbeitsbereiche</li></ul> |
| Analytics Platform | [Live-Stream](https://github.com/AdobeDocs/analytics-1.4-apis/blob/master/docs/live-stream-api/index.md) (Rohdaten, Dashboards, Auslöser) |

{style="table-layout:auto"}

## Predictive Intelligence {#section_B407932C07A7476F83FB0275C3FB63DC}

Die Aktualisierung auf Predictive Intelligence ermöglicht [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus:

| Produkt | Upgrades |
|---|---|
| Reports &amp; Analytics | [Beitragsanalyse](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html?lang=de) |
| Data Workbench | Vorgefertigte Arbeitsbereiche für die Qualifizierung von Zielgruppen und das prädiktive Marketing |
| Analytics Platform | Live-Stream (Dashboards und Auslöser) |

{style="table-layout:auto"}

## Customer 360 {#section_3B2AC245388248688067DC9A48957AFB}

Ein Upgrade auf Customer 360 beinhaltet [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus:

| Produkt | Upgrades |
|--- |--- |
| [Kundenattribute](attributes.md) | Kundenattribute (Analyse und Segmentfreigabe) |
| Data Workbench | <ul><li>Abgeleitete Kundenattribute</li><li>Vordefinierte Arbeitsbereiche für die Erkennung von Zielgruppen</li></ul> |
| Analytics Platform | [Kundenattribute](attributes.md) |

{style="table-layout:auto"}

## Advanced Attribution {#section_9E4986A8389946CCAA7D003268343296}

Advanced Attribution bietet Zugriff auf [Analytics Premium](upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507), plus Algorithmic Attribution in Data Workbench (25 % Server-Aufrufvolumen).

## Data Workbench-Anforderungen {#section_D959CA68D6DB42C38707F8E0CA3654CC}

Die aktualisierten Benutzer können über eine E-Mail an `dwb@adobe.com` anfordern, dass alle Kundenlizenzen mit der Premium-Information aktualisiert werden. Durch diese Aktualisierung werden Funktionen wie Algorithmic Attribution ermöglicht.

TechOps überprüft Ihre vertragliche Verpflichtung und ermittelt die geeignete verwaltete Infrastruktur, erhöht oder verringert die Kapazität und koordiniert dann mit Ihnen über den Account Manager oder die Beratung, um Änderungen bereitzustellen.

Sämtliche Software, die am Kundenstandort ausgeführt wird, muss deaktiviert werden. Diese Software enthält Sensoren, d. h. Sie müssen eine ordnungsgemäße Verfolgung durch [!DNL Analytics]-Tags sicherstellen.

## Experience Cloud – Benutzer und Produkte verwalten {#section_6471C54454024301B2E0B687F79F6738}

Experience Cloud und zentrale Services stehen Analytics Standard- und Premium-Benutzern zur Verfügung, vorausgesetzt, die Modernisierung der Implementierung wurde so durchgeführt wie in [Erste Schritte – Aktivieren Ihrer Programme für zentrale Services](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C) beschrieben. (Dieser Prozess hilft Ihnen, Ihre Implementierung zu modernisieren, und ermöglicht es Ihnen, Administrator beim Experience Cloud zu werden.)

Nachdem Sie Experience Cloud beigetreten sind, können Sie sich unter folgender Adresse über Experience Cloud anmelden [!DNL experience.adobe.com] und beginnen Sie mit der Verwendung von zentralen Services (einschließlich Kundenattributen, Zielgruppen und Analysen für Mobile Apps).

### Verwalten Sie Benutzer und Gruppen

Die Benutzerverwaltung erfolgt in der [Adobe Admin Console](https://helpx.adobe.com/de/enterprise/using/admin-console.html) (Produktlink).

Sie können eine 1:1-Zuordnung zwischen einer in der Adobe Admin Console erstellten Gruppe und einer Lösungsgruppe (z. B. Adobe Analytics) einrichten. Danach wird für einen neuen Benutzer, der zur zugeordneten Admin Console-Gruppe hinzugefügt wird, automatisch ein Analytics-Programmkonto erstellt und mit der Adobe ID des Benutzers verknüpft. (Vorhandene Benutzer müssen ihre Anmeldeinformationen für das Programmkonto manuell verknüpfen, um über die Experience Cloud-Anmeldung auf Programme zuzugreifen.)

>[!NOTE]
>
>Sie können einer Admin Console-Gruppe mehrere Programmgruppen zuordnen. Adobe empfiehlt jedoch die 1:1-Zuordnung. Durch die vorzeitige Zuordnung der Gruppen können Sie mehrere Benutzer einladen, erstellen, berechtigen und hinzufügen, indem Sie eine CSV-Datei hochladen.
