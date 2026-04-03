---
title: Agent-KI in Experience Cloud-Anwendungen
description: Erfahren Sie, wo in Experience Cloud-Programmen eine agentische KI verfügbar ist.
solution: Experience Cloud
landing-page-name: ai
landing-page-breadcrumb-title: AI Documentation
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
exl-id: c1a8f9a7-4752-4040-b5f0-dc775417f536
source-git-commit: 3ee209e2b49cf9ac3d26806519b8ece57d19a7dc
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 3%

---

# Agent AI in Adobe Experience Cloud

Aktualisiert: **3. April 2026**

Adobe Experience Platform Agents wird von [Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/de/docs/experience-cloud-ai/experience-cloud-ai/home) unterstützt, um agentische KI-Funktionen in Experience Cloud-Programmen zu aktivieren.

Diese Agenten helfen bei der Automatisierung von Aufgaben, liefern schneller Erkenntnisse und optimieren Workflows. Dadurch können Teams effizienter arbeiten und mehr Nutzen aus Experience Cloud ziehen.

Der Zugriff auf KI-Agenten in Experience Cloud ist verfügbar unter:

* [Bestehende Experience Cloud-Programme](#existing-apps)
* [AI-First-Experience Cloud-Anwendungen](#ai-first-apps)

In den folgenden Abschnitten werden diese beiden Methoden zum Aktivieren der agenten KI in Experience Cloud beschrieben.

## Bestehende Experience Cloud-Programme {#existing-apps}

In bestehenden Programmen können Sie natürliche Sprache verwenden, um Adobe Experience Platform-Agenten über die [KI-Assistent](https://experienceleague.adobe.com/de/docs/experience-cloud-ai/experience-cloud-ai/home) Konversationsoberfläche anzuweisen. Der KI-Assistent ist sowohl in der Vollbild- als auch in der Rechtsleistenansicht verfügbar.

Agenten können in bestehenden Experience Cloud-Programmen für Kunden in einer der folgenden Kategorien aktiviert werden:

* Sie haben eine Lizenz für Adobe Experience Platform Agents AI Credits erworben
* Sie werden in eine nutzungsgebundene Testversion eingeschlossen (eingeschränkte KI-Credits bereitgestellt)
* Sie haben die Agent Orchestrator Promo SKU (zeitgebundene Testlizenz) abgeschlossen.

Die Verwendung von KI-Agenten für _Agentenaufträge_ nutzt KI-Credits. Erfahren Sie mehr über Agentenaufträge und KI-Credits in _[Agentenaufträge und KI-](/help/interface/features/ai-credit-consumption.md)_).

KI-Agenten befolgen _Ihre_ Eingabe, Aufsicht und berücksichtigen die Zugriffskontrollen auf Produktebene. Sie können nur Aufträge ausführen oder auf Daten zugreifen, zu deren Nutzung Sie in der zugrunde liegenden Experience Cloud-Anwendung berechtigt sind.

### KI-Agenten in bestehenden Experience Cloud-Apps {#existing-apps-table}

In der folgenden Tabelle sind Experience Platform-Agenten aufgeführt, die in bestehenden Experience Cloud-Programmen verfügbar sind.

| Agent-Name | Funktionen | Unterstützte Anwendungen |
|---|----------|----------|
| [Brand Experience Agent](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/ai-in-aem/agents/brand-experience/overview) | <ul><li>Beschleunigt die Migration und Modernisierung digitaler Erlebnisse durch automatische Umstrukturierung, Anreicherung und Validierung vorhandener Sites, damit Teams schneller zu modernen, KI-fähigen Erlebnissen mit weniger Risiko und manuellem Aufwand wechseln können.</li><li>Übernimmt die Erstellung und Aktualisierung umfangreicher Erlebnisse und reduziert so den manuellen Aufwand und die Zykluszeit erheblich, sodass Teams schneller arbeiten können, ohne auf Qualität oder Konsistenz zu verzichten.</li><li>Beschleunigt die Erstellung optimierter, markeninterner Formulare, indem Formulare automatisch generiert, strukturiert und validiert werden. Dadurch können Teams schneller starten und mit minimalem manuellen Aufwand qualitativ hochwertigere Daten erfassen.</li><li>Hilft Entwicklern und technischen Administratoren von AEM CS bei der Fehlerbehebung bei Build-Schritt-Fehlern in der Cloud Manager-Pipeline, indem die Grundursache analysiert und Fehlerbehebungen vorgeschlagen werden.</li></ul> | <ul><li>Adobe Experience Manager Sites Cloud Services (Erlebnismodernisierung)</li></ul><ul><li>Adobe Experience Manager Sites (Experience Production)</li></ul><ul><li>Adobe Experience Manager Forms (Formularerstellung)</li></ul><ul><li>Alle Cloud-basierten Adobe Experience Manager-Anwendungen (Entwicklungsunterstützung)</li></ul> |
| [Brand Governance Agent](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/ai-in-aem/agents/governance/overview) | Schützen Sie die Markenintegrität und die Einhaltung automatisierter Markenrichtlinien, Prüfungen, Berechtigungen und Intelligenz zur Unterstützung von DRM durch Governance in Echtzeit. | <ul><li>Adobe Experience Manager Assets</li><li>Adobe Experience Manager Sites (Markenrichtlinie)</li></ul> |
| [Journey Agent](https://experienceleague.adobe.com/de/docs/experience-cloud-ai/experience-cloud-ai/agents/ajo-agent) | Ihre Teams können schnell skalierbare Multi-Touch-Journey für Kunden erstellen, analysieren und optimieren. | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> |
| [Produktsupport-Agent](https://experienceleague.adobe.com/de/docs/experience-cloud-ai/experience-cloud-ai/agents/product-support) | Beheben Sie Support-Probleme, ohne Ihre Workflows zu verlassen, erstellen Sie Support-Tickets und verfolgen Sie den Fallfortschritt mit dem KI-Assistenten. | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li><li>Customer Journey Analytics (B2B- und B2C-Editionen)</li><li>Adobe Experience Manager</li></ul> |
| [Adobe Marketing Agent for Microsoft 365 Copilot](https://experienceleague.adobe.com/de/docs/experience-cloud-ai/experience-cloud-ai/agents/ama-ms) | verbindet Experience Platform direkt mit Microsoft 365 Copilot. Sie können in Microsoft 365-Anwendungen wie Teams, Word, PowerPoint und Excel Fragen in natürlicher Sprache stellen, um sofort Marketing-Erkenntnisse aus Experience Platform abzurufen, ohne Ihren Workflow zu unterbrechen. | <ul><li> Adobe Agent Orchestrator mit Unterstützung für Audience Agent, Journey Agent, Customer Journey Analytics Data Insights, Experience Platform Operational Insights</li></ul> |

## AI-First-Experience Cloud-Anwendungen {#ai-first-apps}

KI-First-Anwendungen werden mit generativem oder agentem Al als Kern erstellt. Sie nutzen generative oder agentische AL für wichtige Aufgaben, und die agentischen Funktionen sind bereits in der AL-FIRST-Anwendungslizenz enthalten. Daher benötigen sie keine Experience Platform Agent Orchestrator-Lizenz.

In der folgenden Tabelle sind Experience Platform-Agenten aufgeführt, die als Al-First-Anwendungen verfügbar sind. Sie werden durch die Lizenzierung dieser Al-First-Anwendungen aktiviert:

| Agent-Name | Funktionen | Unterstützte Anwendungen |
|---|----------|----------|
| [Experimentation Agent](https://experienceleague.adobe.com/de/docs/journey-optimizer/using/content-management/content-experiment/experiment/experiment-accelerator-security) | Automatisieren, analysieren und synthetisieren Sie Einblicke, sodass Sie wirkungsvolle Experimente und Wachstumsmöglichkeiten schnell von einem zentralen Arbeitsbereich aus identifizieren können - und das bei gleichzeitiger Reduzierung manueller Prozesse. | <ul><li>AJO Experimentation Accelerator</li></ul> |
| [LLM-Optimierungsagent](https://experienceleague.adobe.com/de/docs/llm-optimizer/using/home) | Verbesserung der Sichtbarkeit, Genauigkeit und Einflussnahme in KI-gestützten Suchumgebungen, Bereitstellung von Einblicken in das Markenpräsenz in KI-generierte Antworten, Angebot präskriptiver Inhaltsempfehlungen und Automatisierung von Optimierungskorrekturen. | <ul><li>Adobe LLM Optimizer</li></ul> |
| [Site Optimization Agent](https://experienceleague.adobe.com/de/docs/experience-manager-sites-optimizer/content/home) | Maximieren Sie die geschäftliche Auswirkung, indem Sie Website-Verbesserungen automatisch erkennen und bereitstellen. Durch die Verwendung generativer KI und mehrerer Überwachungstechnologien können Sie die Erfassung und Interaktion von Website-Traffic steigern und vieles mehr | <ul><li>AEM Sites Optimizer</li></ul> |
| [Product Advisor Agent](https://experienceleague.adobe.com/de/docs/brand-concierge/content/documentation/overview) | Steigern Sie Ihre Konversionen und Interaktionen durch intelligente, kontextbezogene Produkterkennung, die auf individuelle Vorlieben und Verhaltensweisen zugeschnitten ist. | <ul><li>Adobe Brand Concierge</li></ul> |

## Weitere Hilfe zu diesem Thema

* [Agent-Vorgänge und KI-Kreditverbrauch](/help/interface/features/ai-credit-consumption.md)
* [KI in Experience Cloud](https://experienceleague.adobe.com/en/docs/ai) Dokumentations-Startseite
* [Übersicht über Agenten in AEM](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/ai-in-aem/agents/overview)

[!BADGE Weitere Informationen zu Adobe for Business]{type=Informative url="https://business.adobe.com/de/products/experience-platform/agent-orchestrator.html" tooltip="Navigieren Sie zu Business.adobe.com ."}
