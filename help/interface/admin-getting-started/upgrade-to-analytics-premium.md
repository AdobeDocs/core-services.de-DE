---
description: Administratoren können mehr darüber erfahren, was sie bei einem Upgrade auf Analytics Premium erwartet, wie hoch die Anforderungen sind und wo sie als Experience Cloud-Administrator Hilfe finden.
keywords: Upgrade
seo-description: Administratoren können mehr darüber erfahren, was sie bei einem Upgrade auf Analytics Premium erwartet, wie hoch die Anforderungen sind und wo sie als Experience Cloud-Administrator Hilfe finden.
seo-title: Upgrade auf Analytics Premium und die Experience Cloud
solution: Experience Cloud
title: Upgrade auf Analytics Premium und die Experience Cloud
topic: Premium
uuid: 450a601c-d199-4e90-b525-19bd9f9576d2
translation-type: tm+mt
source-git-commit: 979b2202a70e2a5362aa86a65a17d7c4279b3a1a

---


# Upgrade auf Analytics Premium und die Experience Cloud

Administratoren können mehr darüber erfahren, was sie bei einem Upgrade auf Analytics Premium erwartet, wie hoch die Anforderungen sind und wo sie als Experience Cloud-Administrator Hilfe finden.


## Analytics Premium {#section_7F50AD7906544F899B844BE31D3BB507}

Ein Upgrade auf Adobe Analytics Premium bietet Ihnen alle Funktionen und Produkte, die in Analytics Standard verfügbar sind, darunter Data Warehouse, Ad Hoc Analysis, Report Builder und Data Connectors. (Diese Produkte werden Kunden, die die Punktlösung SiteCatalyst verwenden, separat angeboten.)

Analytics Premium bietet Ihnen Folgendes:

* Zugriff auf 250 Konversion-Variablen (eVars)
* [Analyse mobiler Apps](https://marketing.adobe.com/resources/help/en_US/mobile/)
* Data Workbench (visuelle Datenabfrage, regelbasierte Zuordnung, kanalübergreifende Analyse)



>[!NOTE]
>
>Bei einem Upgrade ist keine Migration erforderlich, jedoch sollten Sie folgende Punkte berücksichtigen:
>
>* eVars 76 bis 250 (SiteCatalyst) und 100 bis 250 (Standard) werden in Admin Tools angezeigt, sind jedoch nicht bereits aktiviert.&gt;
>* Die Beitragsanalyse wird von Adobe aktiviert. Der Standort wird nicht geändert (das Element ist nach wie vor auf der Seite „Anomalieerkennung“ verfügbar), jedoch beginnt die Analyse aller Datenpunkte nun automatisch.&gt;


In den folgenden Abschnitten wird beschrieben, wo Sie Hilfe zu den von Ihnen erworbenen Funktionen finden:

* [Analytics Premium Complete](../admin-getting-started/upgrade-to-analytics-premium.md#section_BFAD815EDF364845A52B340B2FD5B64C)
* [Predictive Intelligence](../admin-getting-started/upgrade-to-analytics-premium.md#section_B407932C07A7476F83FB0275C3FB63DC)
* [Customer 360](../admin-getting-started/upgrade-to-analytics-premium.md#section_3B2AC245388248688067DC9A48957AFB)
* [Advanced Attribution](../admin-getting-started/upgrade-to-analytics-premium.md#section_9E4986A8389946CCAA7D003268343296)
* [Data Workbench-Anforderungen ](../admin-getting-started/upgrade-to-analytics-premium.md#section_D959CA68D6DB42C38707F8E0CA3654CC)
* [Experience Cloud](../admin-getting-started/upgrade-to-analytics-premium.md#section_6471C54454024301B2E0B687F79F6738)



## Analytics Premium Complete {#section_BFAD815EDF364845A52B340B2FD5B64C}

In Analytics Premium Complete erhalten Sie alle Funktionen von [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) sowie folgende Upgrades:

| Produkt | Upgrades |
|--- |--- |
| Reports and Analytics | <ul><li>[Beitragsanalyse](https://marketing.adobe.com/resources/help/en_US/analytics/contribution/)</li><li>[Kundenattribute](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1) (bis zu 200)</li></ul> |
| Data Workbench | <ul><li>Algorithmische Zuordnung</li><li>Vordefinierte Arbeitsbereiche</li></ul> |
| Analytics-Plattform | [Livestream](https://marketing.adobe.com/developer/documentation/analytics-live-stream/overview-1) (Rohdaten, Dashboards, Trigger) |


## Predictive Intelligence {#section_B407932C07A7476F83FB0275C3FB63DC}

Ein Upgrade auf Predictive Intelligence bietet [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus:

| Produkt | Upgrades |
|---|---|
| Reports and Analytics | [Beitragsanalyse](https://marketing.adobe.com/resources/help/en_US/analytics/contribution/) |
| Data Workbench | Vordefinierte Arbeitsbereiche für Zielgruppenqualifikationen und vorausschauendes Marketing |
| Analytics-Plattform | Livestream (Dashboards und Trigger) |


## Customer 360 {#section_3B2AC245388248688067DC9A48957AFB}

Ein Upgrade auf Customer 360 bietet Ihnen [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) plus:

| Produkt | Upgrades |
|--- |--- |
| [Kundenattribute](../attributes/attributes.md) | Kundenattribute (Analyse und Segmentfreigabe) |
| Data Workbench | <ul><li>Abgeleitete Kundenattribute</li><li>Vordefinierte Arbeitsbereiche für Zielgruppenerkennung</li></ul> |
| Analytics-Plattform | [Kundenattribute](../attributes/attributes.md) |


## Advanced Attribution {#section_9E4986A8389946CCAA7D003268343296}

Advanced Attribution bietet Zugriff auf [Analytics Premium](../admin-getting-started/upgrade-to-analytics-premium.md#section_7F50AD7906544F899B844BE31D3BB507) sowie die algorithmische Zuordnung in Data Workbench (25 % Server-Aufrufvolumen).

## Data Workbench-Anforderungen  {#section_D959CA68D6DB42C38707F8E0CA3654CC}

Die aktualisierten Benutzer können über eine E-Mail an `dwb@adobe.com` anfordern, dass alle Kundenlizenzen mit der Premium-Information aktualisiert werden. Dies aktiviert Funktionen wie die algorithmische Zuordnung.

TechOps überprüfen Ihre Vertragsverpflichtungen und bestimmen die angemessene verwaltete Infrastruktur, erhöhen oder reduzieren die Kapazität und koordinieren über den Account Manager oder über eine Beratung die Durchführung jeglicher Änderungen.

Sämtliche Software, die am Kundenstandort ausgeführt wird, muss deaktiviert werden. Dies umfasst auch Sensoren, Sie müssen also eine ordnungsgemäße Verfolgung über Analytics-Tags sicherstellen.

**Premium Complete** und **Advanced Attribution**

Informationen zur regelbasierten Zuordnung in vordefinierten Vorlagen finden Sie unter [Regelbasierte Zuordnung](https://marketing.adobe.com/resources/help/en_US/insight/client/?f=c_rules_attrib).

Informationen zur algorithmischen Zuordnung finden Sie im Dokument zum [Finden der geeignetsten Zuordnung](https://marketing.adobe.com/resources/help/en_US/insight/client/?f=c_attrib_algorithmic).

**Predictive Intelligence**

Predictive Intelligence in Data Workbench beinhaltet die folgenden Visualisierungen:

* [Tendenzauswertung der Zielgruppe](https://marketing.adobe.com/resources/help/en_US/insight/client/?f=c_visitor_propensity)
* [Besucheraufteilung](https://marketing.adobe.com/resources/help/en_US/insight/client/?f=c_visitor_cluster)
* [Korrelationsanalyse](https://marketing.adobe.com/resources/help/en_US/insight/client/?f=c_correlation_analysis)


**Customer 360** und **Advanced Attribution**

Siehe Informationen zu regelbasierter Analytics-Zuordnung in vordefinierten Vorlagen unter [Regelbasierte Zuordnung](https://marketing.adobe.com/resources/help/en_US/insight/client/?f=c_rules_attrib).

Siehe Informationen zu Vorlagen der algorithmischen Zuordnung im Dokument zum [Finden der geeignetsten Zuordnung](https://marketing.adobe.com/resources/help/en_US/insight/client/?f=c_attrib_algorithmic)..

## Experience Cloud – Benutzer und Produkte verwalten {#section_6471C54454024301B2E0B687F79F6738}

Experience Cloud und Hauptdienste stehen Analytics Standard- und Premium-Benutzern zur Verfügung, vorausgesetzt, die Modernisierung der Implementierung wurde wie in [Erste Schritte - ermöglichen Sie Ihre Lösungen für Hauptdienste](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C) beschrieben durchgeführt. (Dieser Prozess unterstützt Sie beim Modernisieren Ihrer Implementierung und ermöglicht es Ihnen, ein Administrator in Experience Cloud zu werden.)

Nachdem Sie Mitglied der Experience Cloud geworden sind, können Sie sich über [!DNL marketing.adobe.com] bei der Experience Cloud anmelden und damit beginnen, die Hauptdienste zu verwenden (einschließlich Kundenattributen, Zielgruppen und Analysen mobiler Apps).

**Verwalten Sie Benutzer und Gruppen**

Die Benutzerverwaltung geschieht über die [Adobe Admin Console](https://helpx.adobe.com/enterprise/help/aedash.html) (Produktlink).

Sie können eine 1-zu-1-Zuordnung zwischen einer Gruppe, die in der Adobe Admin Console erstellt wurde, und einer Lösungsgruppe (wie z. B. Adobe Analytics) festlegen. Daraufhin wird für einen neuen Benutzer, der zur zugeordneten Admin Console-Gruppe hinzugefügt wird, automatisch ein Analytics-Lösungskonto erstellt und mit der Adobe ID des Benutzers verknüpft. (Vorhandene Benutzer müssen die Anmeldeinformationen Ihres Lösungskontos manuell verknüpfen, wenn sie über die Anmeldung bei der Experience Cloud auf Lösungen zugreifen möchten.)


>[!NOTE]
>
>Sie können mehrere Lösungsgruppen einer Admin Console-Gruppe zuordnen. Adobe empfiehlt jedoch eine 1-zu-1-Zuordnung. Die frühzeitige Zuordnung der Gruppen ermöglicht es Ihnen, mehrere Benutzer gleichzeitig hinzuzufügen, einzuladen, zu erstellen und ihnen Berechtigungen zuzuweisen, indem Sie eine CSV-Datei hochladen.

