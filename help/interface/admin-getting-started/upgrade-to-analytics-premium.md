---
description: Administratoren können mehr darüber erfahren, was sie bei einem Upgrade auf Analytics Premium erwartet, wie hoch die Anforderungen sind und wo sie als Experience Cloud-Administrator Hilfe finden.
keywords: upgrading
seo-description: Administratoren können mehr darüber erfahren, was sie bei einem Upgrade auf Analytics Premium erwartet, wie hoch die Anforderungen sind und wo sie als Experience Cloud-Administrator Hilfe finden.
seo-title: Upgrade auf Analytics Premium und die Experience Cloud
solution: Experience Cloud
title: Upgrade auf Analytics Premium und die Experience Cloud
topic: Premium
uuid: 450a601c-d199-4e90-b525-19bd9f9576d2
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 42%

---


# Upgrade auf Analytics Premium und die Experience Cloud

Administratoren können mehr darüber erfahren, was sie bei einem Upgrade auf Analytics Premium erwartet, wie hoch die Anforderungen sind und wo sie als Experience Cloud-Administrator Hilfe finden.

## Analytics Premium {#section_7F50AD7906544F899B844BE31D3BB507}

Durch die Aktualisierung auf Adobe Analytics Premium erhalten Sie alle verfügbaren Funktionen oder Produkte von Analytics Standard, einschließlich Data Warehouse, Ad-hoc-Analysen, ReportBuilder und Data Connectors. (Diese Produkte wurden mit SiteCatalyst, der Punktlösung, separat an Kunden verkauft.)

Analytics Premium bietet Ihnen:

* Zugriff auf 250 Konversionsvariablen (eVars)
* [Mobile App Analytics](https://docs.adobe.com/content/help/de-DE/mobile-services/using/home.html)
* Data Workbench (visuelle Datenabfrage, regelbasierte Zuordnung, kanalübergreifende Analyse)

>[!NOTE]
>
>Bei der Aktualisierung ist keine Migration erforderlich. Beachten Sie jedoch Folgendes:
>
>* Die eVars 76-250 (SiteCatalyst) und 100-250 (Standard) sind in den Admin Tools sichtbar, sind aber noch nicht aktiviert.>
>* Die Analyse der Beitragsleistung wird von Adobe aktiviert. Der Speicherort wird nicht geändert (er ist weiterhin auf der Seite &quot;Anomalieerkennung&quot;verfügbar), aber jetzt wird automatisch ein Beginn zur Analyse aller Datenpunkte ausgeführt.>


## Analytics Premium Complete {#section_BFAD815EDF364845A52B340B2FD5B64C}

In Analytics Premium Complete erhalten Sie alle Funktionen von [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507)sowie die folgenden Upgrades:

| Produkt | Upgrades |
|--- |--- |
| Reports and Analytics | <ul><li>[Beitragsanalyse](https://docs.adobe.com/content/help/de-DE/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html)</li><li>[Kundenattribute](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1) (bis zu 200)</li></ul> |
| Data Workbench | <ul><li>Algorithmische Zuordnung</li><li>Vordefinierte Arbeitsbereiche</li></ul> |
| Analytics Platform | [Live-Stream](https://helpx.adobe.com/analytics/kb/getting-started-with-livestream-api.html) (Rohdaten, Dashboards, Auslöser) |

## Predictive Intelligence {#section_B407932C07A7476F83FB0275C3FB63DC}

Die Aktualisierung auf Predictive Intelligence ermöglicht [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus:

| Produkt | Upgrades |
|---|---|
| Reports and Analytics | [Beitragsanalyse](https://docs.adobe.com/content/help/de-DE/analytics/analyze/analysis-workspace/virtual-analyst/contribution-analysis/ca-tokens.html) |
| Data Workbench | Vorgefertigte Arbeitsbereiche für die Qualifizierung von Audiencen und das prädiktive Marketing. |
| Analytics Platform | Live-Stream (Dashboards und Auslöser) |

## Customer 360 {#section_3B2AC245388248688067DC9A48957AFB}

Upgrade auf Customer 360 Angebots [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus:

| Produkt | Upgrades |
|--- |--- |
| [Kundenattribute](../attributes/attributes.md) | Kundenattribute (Analyse und Segmentfreigabe) |
| Data Workbench | <ul><li>Abgeleitete Kundenattribute</li><li>Vordefinierte Arbeitsbereiche für die Erkennung von Audiencen</li></ul> |
| Analytics Platform | [Kundenattribute](../attributes/attributes.md) |

## Advanced Attribution {#section_9E4986A8389946CCAA7D003268343296}

Advanced Attribution Angebots Zugriff auf [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507)plus Algorithmic Attribution in Data Workbench (25 % Server-Aufrufvolumen).

## Data Workbench-Anforderungen  {#section_D959CA68D6DB42C38707F8E0CA3654CC}

Die aktualisierten Benutzer können über eine E-Mail an `dwb@adobe.com` anfordern, dass alle Kundenlizenzen mit der Premium-Information aktualisiert werden. Dadurch werden Funktionen wie die algorithmische Zuordnung aktiviert.

TechOps überprüft Ihre vertragliche Verpflichtung und ermittelt die geeignete verwaltete Infrastruktur, erhöht oder verringert die Kapazität und koordiniert dann mit Ihnen über den Kundenbetreuer oder die Beratung die Implementierung von Änderungen.

Sämtliche Software, die am Kundenstandort ausgeführt wird, muss deaktiviert werden. Dies schließt Sensoren ein, d. h. Sie müssen eine ordnungsgemäße Verfolgung durch Analytics-Tags sicherstellen.

## Experience Cloud – Benutzer und Produkte verwalten {#section_6471C54454024301B2E0B687F79F6738}

Experience Cloud und Hauptdienste stehen Analytics Standard- und Premium-Benutzern zur Verfügung, vorausgesetzt, die Modernisierung der Implementierung wurde wie in [Erste Schritte - ermöglichen Sie Ihre Lösungen für Hauptdienste](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C) beschrieben durchgeführt. (Dieser Prozess unterstützt Sie beim Modernisieren Ihrer Implementierung und ermöglicht es Ihnen, ein Administrator in Experience Cloud zu werden.)

After you join the Experience Cloud, you can log in via the Experience Cloud at [!DNL experiencecloud.adobe.com] and begin using core services (including Customer Attributes, Audiences, and Mobile app analytics).

### Verwalten Sie Benutzer und Gruppen

Die Benutzerverwaltung erfolgt in der [Adobe Admin Console](https://helpx.adobe.com/enterprise/help/aedash.html) (Produktlink).

Sie können eine 1:1-Zuordnung zwischen einer in der Adobe Admin-Konsole erstellten Gruppe und einer Lösungsgruppe (z. B. Adobe Analytics) einrichten. Danach wird für einen neuen Benutzer, der der zugeordneten Admin-Konsolengruppe hinzugefügt wird, automatisch ein Analytics-Lösungskonto erstellt und mit der Adobe-ID des Benutzers verknüpft. (Vorhandene Benutzer müssen ihre Anmeldeinformationen für das Lösungskonto manuell verknüpfen, um über die Experience Cloud-Anmeldung auf Lösungen zuzugreifen.)

>[!NOTE]
>
>Sie können mehrere Lösungsgruppen einer Admin Console-Gruppe zuordnen. Adobe empfiehlt jedoch die 1:1-Zuordnung. Durch die vorzeitige Zuordnung der Gruppen können Sie mehrere Benutzer einladen, erstellen, berechtigen und hinzufügen, indem Sie eine CSV hochladen.
