---
title: Agent-Vorgänge und KI-Kreditverbrauch
description: Erfahren Sie mehr über Agentenaufträge und KI-Kreditverbrauchsraten in Experience Cloud-Programmen.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
source-git-commit: 7eb6c6e463102ca445093c69797619202202b35e
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 10%

---

# Agent-Vorgänge und KI-Kreditverbrauch

Erfahren Sie mehr über die Verwendung von agenten KI-Aufträgen und die Verwendung von KI-Krediten in Experience Cloud-Programmen. Informationen zur Aktivierung der Funktionen der agenten KI in bestehenden Experience Cloud-Programmen finden Sie unter [Agentische KI in Experience Cloud](agentic-ai.md#existing-apps).

## Agentenaufträge

Ein _Agentenauftrag_ ist eine Reihe von Aufgaben und Aktionen, die ein Agent ausführt, um ein bestimmtes Ergebnis zu erzielen, wie durch Kundeneingaben angewiesen.

Mithilfe natürlicher Eingabeaufforderungen über den KI-Assistenten können Sie Agenten bitten, bestimmte Aufträge auszuführen. Basierend auf diesen Eingaben koordiniert Agent Orchestrator die entsprechenden Agenten, um jeden Schritt in den entsprechenden Experience Cloud-Programmen auszuführen.

## KI-Credits

Ein _KI-_) ist eine nutzungsbasierte Metrik, die die Ausführung von Agentenvorgängen quantifiziert. KI-Credits gelten nicht für [KI-First-Anwendungen](/help/interface/features/agentic-ai.md).

## KI-Kreditnutzung

Die Verwendung von KI-Guthaben kann je nach Komplexität und Wert des ausgeführten Auftrags variieren:

* Einfache (oft einstufige) Aufgaben verbrauchen weniger Guthaben
* Komplexe (oft mehrstufige) Aufgaben verbrauchen mehr Guthaben
* Aufgaben mit erweitertem Argumentieren, Validierung, Koordination mit mehreren Agenten oder Integration verbrauchen mehr Credits

### Geschätzte KI-Kreditverbrauchsraten

| Agent | Job | Unterstützte Anwendungen | Geschätzte KI-Guthaben |
|------|-----|------------------------|----------------------|
| Audience Agent | Zielgruppen-/Konto-Idee | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 50 |
| Audience Agent | Wissensbasierte Zielgruppen-/Kontoerstellung | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 150 |
| Audience Agent | Zielgruppen-/Kontoverwaltung | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 25 |
| Audience Agent | Zielgruppen-/Kontoanalyse | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 25 |
| Audience Agent | Einkaufsgruppenidee | <ul><li>Adobe Journey Optimizer (B2B)</li></ul> | 25 |
| Data Insights Agent | Datenanalyse und -visualisierung | <ul><li>Customer Journey Analytics</li></ul> | 25 |
| Journey Agent | Journey | <ul><li>Adobe Journey Optimizer (B2B)</li></ul> | 25 |
| Journey Agent | Journey-Erstellung | <ul><li>Adobe Journey Optimizer (B2B, B2C)</li></ul> | 30 |
| Journey Agent | Journey-Analyse | <ul><li>Adobe Journey Optimizer (B2B, B2C)</li></ul> | 50 |
| Journey Agent | Journey-Verwaltung | <ul><li>Adobe Journey Optimizer (B2B, B2C)</li></ul> | 25 |
| Produktsupport-Agent | Knowledge-based Troubleshooting | <ul><li>Mehrere Experience Cloud-Anwendungen</li></ul> | 0 |
| Produktsupport-Agent | Erstellung und Nachverfolgung von Support-Fällen | <ul><li>Mehrere Experience Cloud-Anwendungen</li></ul> | 10 |
| Inhaltsratgeber-Agent | Inhaltserkennung | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 5 |
| Inhaltsratgeber-Agent | Inhaltsaktualisierung und -optimierung | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 10 |
| Brand Experience Agent | Bereitstellungs-Support | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 5 |
| Brand Experience Agent | Site-Modernisierung | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 100 |

>[!NOTE]
>
>Der tatsächliche KI-Kreditverbrauch kann je nach der Anzahl der ausgeführten Schritte und Iterationen pro Schritt variieren.

## Weitere Hilfe zu diesem Thema

* [Agent AI in Experience Cloud](/help/interface/features/agentic-ai.md)
* [Nutzungsgebundene Testversion für Adobe Experience Platform-Agenten](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)