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
TQID: https://experienceleague.adobe.com/pjC1VIudoJcKjT26T9WpdWEGESQi-1QLc4KlyAqewq8
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: f84b2906-3ce9-4ef0-86f6-cda249273937id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: b75843fa-0a67-4a44-a6b1-cc627b0481dcid: cda95149-19e1-4cfa-a57e-751283a32378id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: bbbea26f-9621-49eb-9ab8-e06fb3bbce8cid: bcc5edb5-84c3-4940-9f84-ed88b6c16274id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1id: d00e9f03-e50b-4162-b143-0c0817c937c2id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 27da689e214c6c2408be2cb004c8791990513780
workflow-type: tm+mt
source-wordcount: 1063
ht-degree: 6%

---

# Agent AI in Adobe Experience Cloud

Aktualisiert: **13. März 2026**

Adobe Experience Platform Agents wird von [Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/home) unterstützt, um agentische KI-Funktionen in Experience Cloud-Programmen zu aktivieren.

Diese Agenten helfen bei der Automatisierung von Aufgaben, liefern schneller Erkenntnisse und optimieren Workflows. Dadurch können Teams effizienter arbeiten und mehr Nutzen aus Experience Cloud ziehen.

Der Zugriff auf KI-Agenten in Experience Cloud ist verfügbar unter:

* [Bestehende Experience Cloud-Programme](#existing-apps)
* [AI-First-Experience Cloud-Anwendungen](#ai-first-apps)

In den folgenden Abschnitten werden diese beiden Methoden zum Aktivieren der agenten KI in Experience Cloud beschrieben.

## Bestehende Experience Cloud-Programme {#existing-apps}

In bestehenden Programmen können Sie natürliche Sprache verwenden, um Adobe Experience Platform-Agenten über die [KI-Assistent](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/home) Konversationsoberfläche anzuweisen. Der KI-Assistent ist sowohl in der Vollbild- als auch in der Rechtsleistenansicht verfügbar.

Agenten können in bestehenden Experience Cloud-Programmen für Kunden in einer der folgenden Kategorien aktiviert werden:

* Sie haben eine Lizenz für Adobe Experience Platform Agents AI Credits erworben
* Sie werden in eine nutzungsgebundene Testversion eingeschlossen (eingeschränkte KI-Credits bereitgestellt)
* Sie haben die Agent Orchestrator Promo SKU (zeitgebundene Testlizenz) abgeschlossen.

Die Verwendung von KI-Agenten für _Agentenaufträge_ nutzt KI-Credits. Erfahren Sie mehr über Agentenaufträge und KI-Credits in [Agentenaufträge und KI-](https://experienceleague.adobe.com/en/docs/core-services/interface/features/ai-credit-consumption)).

KI-Agenten befolgen _Ihre_ Eingabe, Aufsicht und berücksichtigen die Zugriffskontrollen auf Produktebene. Sie können nur Aufträge ausführen oder auf Daten zugreifen, zu deren Nutzung Sie in der zugrunde liegenden Experience Cloud-Anwendung berechtigt sind.

### KI-Agenten in bestehenden Experience Cloud-Apps {#existing-apps-table}

In der folgenden Tabelle sind Experience Platform-Agenten aufgeführt, die in bestehenden Experience Cloud-Programmen verfügbar sind.

| Agent-Name | Funktionen | Unterstützte Anwendungen |
| --- | ---------- | ---------- |
| [Audience Agent](https://experienceleague.adobe.com/de/docs/experience-cloud-ai/experience-cloud-ai/agents/audience) | Ihre Teams in die Lage versetzen, Zielgruppen mithilfe von Aufforderungen zur Veröffentlichung in natürlicher Sprache zu erstellen, zu verwalten und zu optimieren, um die Markteinführung zu vereinfachen und zu beschleunigen. | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> |
| [Content Advisor Agent](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/content-advisor/overview) | <ul><li>Hilft Teams dabei, die relevantesten Inhalte im gesamten Unternehmen schnell in natürlicher Sprache zu finden, wodurch die für die Suche aufgewendete Zeit verkürzt und Entscheidungen und die Ausführung beschleunigt werden können.</li><li>Vereinfachen Sie die Erstellung visueller Inhaltsvarianten aus Quell-Assets mithilfe natürlicher Eingabeaufforderungen.</li></ul> | <ul><li>Adobe Experience Manager Assets</li></ul><ul><li>Dynamic Media (Cloud Services)</li></ul> |
| [Data Insights Agent](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai) | Beantwortet schnell Fragen zu Ihren Daten. Er erstellt relevante Visualisierungen in Analysis Workspace mithilfe von Komponenten aus Ihrer Datenansicht und unter Verwendung Ihrer tatsächlichen Daten. | <ul><li>Customer Journey Analytics (B2B- und B2C-Editionen)</li></ul> |
| [Brand Experience Agent](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/brand-experience/overview) | <ul><li>Beschleunigt die Migration und Modernisierung digitaler Erlebnisse durch automatische Restrukturierung, Anreicherung und Validierung vorhandener Sites, sodass Teams schneller zu modernen, KI-fähigen Erlebnissen mit weniger Risiko und manuellem Aufwand wechseln können.</li><li>Erstellt und aktualisiert umfangreiche Erlebnisse, was den manuellen Aufwand und die Zykluszeit erheblich reduziert, sodass Teams schneller agieren können, ohne auf Qualität oder Konsistenz zu verzichten.</li><li>Beschleunigt die Erstellung optimierter, markenkonformer Formulare, indem Erlebnisse automatisch generiert, strukturiert und validiert werden. So können Teams schneller starten und mit minimalem manuellen Aufwand qualitativ hochwertigere Daten erfassen.</li><li>Unterstützt AEM CS-Entwickler und technische Administratoren bei der Fehlerbehebung bei Buildschrittfehlern in der Cloud Manager-Pipeline, indem die Ursache analysiert und Korrekturen vorgeschlagen werden.</li></ul> | <ul><li>Adobe Experience Manager Sites Cloud Service (Modernisierung der Customer Experience)</li></ul><ul><li>Adobe Experience Manager Sites (Experience Production)</li></ul><ul><li>Adobe Experience Manager Forms (Formularerstellung)</li></ul><ul><li>Alle Cloud-basierten Adobe Experience Manager-Anwendungen (Entwicklungsunterstützung)</li></ul> |
| [Brand Governance Agent](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/governance/overview) | <ul><li>Schützt die Markenintegrität und Compliance mit automatisierten Markenrichtlinien, Zugriffsrechten und intelligenter Unterstützung von DRM durch Governance in Echtzeit.</li> | <ul><li>Adobe Experience Manager Assets</li><li>Adobe Experience Manager Sites (Markenrichtlinien)</li></ul> |
| [Journey Agent](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/ajo-agent) | Ermöglicht euren Teams die schnelle Erstellung, Analyse und Optimierung von Customer Journeys mit mehreren Touchscreens. | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> |
| [Product Support Agent](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/product-support) | Beheben Sie Support-Probleme, ohne Ihre Workflows zu verlassen, erstellen Sie Support-Tickets für Kunden und verfolgen Sie den Fortschritt von Fällen mit AI Assistant. | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li><li>Customer Journey Analytics (B2B- und B2C-Editionen)</li><li>Adobe Experience Manager</li></ul> |

## KI-gestützte Experience Cloud-Programme. {#ai-first-apps}

KI-gestützte Anwendungen werden im Kern mit generativem oder agentem Al entwickelt. Sie verwenden generative oder agentische Al für wichtige Aufgaben, und die agentischen Funktionen sind bereits in der Al-first-Anwendungslizenz enthalten. Daher benötigen sie nicht die Experience Platform Agent Orchestrator-Lizenz.

In der folgenden Tabelle sind Experience Platform-Agents aufgelistet, die als All-First-Anwendungen verfügbar sind. Sie werden durch die Lizenzierung dieser Al-First-Anwendungen aktiviert:

| Agent-Name | Funktionen | Unterstützte Anwendungen |
| --- | ---------- | ---------- |
| [Experimentation Agent](https://experienceleague.adobe.com/en/docs/experimentation-accelerator/using/get-started/experiment-accelerator-security) | Automatisieren, analysieren und synthetisieren Sie Einblicke, sodass Sie wirkungsvolle Experimente und Wachstumsmöglichkeiten schnell von einem zentralen Arbeitsbereich aus identifizieren können - und das bei gleichzeitiger Reduzierung manueller Prozesse. | <ul><li>AJO Experimentation Accelerator</li></ul> |
| [LLM-Optimierungsagent](https://experienceleague.adobe.com/de/docs/llm-optimizer/using/home) | Verbesserung der Sichtbarkeit, Genauigkeit und Einflussnahme in KI-gestützten Suchumgebungen, Bereitstellung von Einblicken in das Markenpräsenz in KI-generierte Antworten, Angebot präskriptiver Inhaltsempfehlungen und Automatisierung von Optimierungskorrekturen. | <ul><li>Adobe LLM Optimizer</li></ul> |
| [Site Optimization Agent](https://experienceleague.adobe.com/de/docs/experience-manager-sites-optimizer/content/home) | Maximieren Sie die geschäftliche Auswirkung, indem Sie Website-Verbesserungen automatisch erkennen und bereitstellen. Durch die Verwendung generativer KI und mehrerer Überwachungstechnologien können Sie die Erfassung und Interaktion von Website-Traffic steigern und vieles mehr | <ul><li>AEM Sites Optimizer</li></ul> |
| [Product Advisor Agent](https://experienceleague.adobe.com/en/docs/brand-concierge/content/documentation/overview) | Steigern Sie Ihre Konversionen und Interaktionen durch intelligente, kontextbezogene Produkterkennung, die auf individuelle Vorlieben und Verhaltensweisen zugeschnitten ist. | <ul><li>Adobe Brand Concierge</li></ul> |

## Weitere Hilfe zu diesem Thema

* [Agent-Vorgänge und KI-Kreditverbrauch](/help/interface/features/ai-credit-consumption.md)
* [KI in Experience Cloud](https://experienceleague.adobe.com/en/docs/ai) Dokumentations-Startseite
* [Übersicht über Agenten in AEM](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/overview)

[!BADGE Weitere Informationen zu Adobe for Business]{type=Informative url="https://business.adobe.com/products/experience-platform/agent-orchestrator.html" tooltip="Navigieren Sie zu Business.adobe.com ."}

