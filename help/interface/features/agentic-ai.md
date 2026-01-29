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
source-git-commit: 3ed72cfa1fd7a6559ac7dd7b31007798c228d53e
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 3%

---

# Agent AI in Adobe Experience Cloud

Aktualisiert: **29. Januar 2026**

Adobe Experience Platform-Agenten verwenden die Experience Platform [Agent Orchestrator](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/home), um den Experience Cloud-Programmen agentenbasierte Funktionen hinzuzufügen.

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

Die Verwendung von KI-Agenten für _Agentenaufträge_ nutzt KI-Credits. Erfahren Sie mehr über Agentenaufträge und KI-Credits in _[Agentenaufträge und KI-](/help/interface/features/ai-credit-consumption.md)_).

KI-Agenten befolgen _Ihre_ Eingabe, Aufsicht und berücksichtigen die Zugriffskontrollen auf Produktebene. Sie können nur Aufträge ausführen oder auf Daten zugreifen, die Sie für die Verwendung im zugrunde liegenden Experience Cloud-Produkt autorisiert haben.

### KI-Agenten in bestehenden Experience Cloud-Apps {#existing-apps-table}

In der folgenden Tabelle sind Experience Platform-Agenten aufgeführt, die in bestehenden Experience Cloud-Programmen verfügbar sind.

| Agent-Name | Funktionen | Unterstützte Anwendungen |
|---|----------|----------|
| [Audience Agent](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/audience) | Ihre Teams in die Lage versetzen, Zielgruppen mithilfe von Aufforderungen zur Veröffentlichung in natürlicher Sprache zu erstellen, zu verwalten und zu optimieren, um die Markteinführung zu vereinfachen und zu beschleunigen. | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> |
| **Content Advisor Agent** | <ul><li>[Inhaltserkennung](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/discovery/overview): Beschleunigen Sie das Authoring und die Erkennung durch vereinfachte Eingabeaufforderungen in natürlicher Sprache, um Experience Manager-Inhalte sofort in Bildern, Videos, textbasierten Dokumenten, Inhaltsfragmenten und Formularen zu finden und bereitzustellen.</li><li>[Inhaltsoptimierung](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/content-optimization/overview): Vereinfachen Sie die Erstellung visueller Inhaltsvarianten aus Quell-Assets mithilfe natürlicher Sprachaufforderungen.</li><li>[Erlebnisproduktion](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/production/overview): Automatisiert aufwändige und umfangreiche Aufgaben in der CMS. Dieser Agent wandelt manuelle, langwierige Prozesse in schnelle, KI-gestützte Workflows um, die jedes Erlebnis aktuell und konsistent halten und Ihrem Unternehmen helfen, Ihre Ziele zu erreichen.</li></ul> | <ul><li>Adobe Experience Manager (Content Discovery)</li></ul><ul><li>Adobe Experience Manager mit Dynamic Media mit OpenAPI (Inhaltsoptimierung)</li></ul><ul><li>Adobe Experience Manager Cloud Services und Edge Delivery Services (Erlebnisproduktion) </li></ul> |
| [Data Insights Agent](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai) | Beantwortet schnell Fragen zu Ihren Daten. Er erstellt relevante Visualisierungen in Analysis Workspace mithilfe von Komponenten aus Ihrer Datenansicht und unter Verwendung Ihrer tatsächlichen Daten. | <ul><li>Customer Journey Analytics (B2B- und B2C-Editionen)</li></ul> |
| **Brand Experience Agent** | [Bereitstellungsunterstützung](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/development/overview): Unterstützt Entwickler und technische Administratoren von AEM CS bei der Fehlerbehebung bei Build-Schritt-Fehlern in der Cloud Manager-Pipeline, indem die Grundursache analysiert und Fehlerbehebungen vorgeschlagen werden. | <ul><li>KI-Assistent in AEM Cloud Service und Adobe Managed Services</li></ul> |
| **Brand Governance Agent*** | [Brand Governance](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/governance/overview): Schützen Sie die Markenintegrität und die Compliance, indem Sie Sicherheits-, Regulierungs- und Markenrichtlinien in Experience Manager durchsetzen. Dieser Agent wendet die Markenverwaltung an, um visuelle und Messaging-Standards zu gewährleisten. Sie verwendet granulare Berechtigungen zum Verwalten von Zugriff und Inhaltsänderungen und integriert DRM, um Lizenzierungs- und Nutzungsbeschränkungen aufrechtzuerhalten. | <ul><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Assets</li><li>Adobe Experience Manager Forms</li></ul> |
| [Journey Agent](https://experienceleague.adobe.com/de/docs/experience-cloud-ai/experience-cloud-ai/agents/ajo-agent-analyze) | Ihre Teams können schnell skalierbare Multi-Touch-Journey für Kunden erstellen, analysieren und optimieren. | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> |
| [Produktsupport-Agent](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/new-features/customer-support) | Beheben Sie Support-Probleme, ohne Ihre Workflows zu verlassen, erstellen Sie Support-Tickets und verfolgen Sie den Fallfortschritt mit dem KI-Assistenten. | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li><li>Adobe Journey Optimizer B2B edition</li><li>Customer Journey Analytics</li><li>Adobe Experience Manager</li></ul> |

Sternchen (*): Auf diesen Agenten können Kunden im Explorer-Programm zugreifen. Der Explorer ist ein Nur-Einladungs-Programm, das frühzeitigen Zugriff auf die neuesten Agentenfunktionen von Adobe bietet. Wenden Sie sich an Ihren Kundenbetreuer, wenn Sie weitere Informationen benötigen.

## AI-First-Experience Cloud-Anwendungen {#ai-first-apps}

KI-First-Anwendungen werden mit generativem oder agentem Al als Kern erstellt. Sie nutzen generative oder agentische AL für wichtige Aufgaben, und die agentischen Funktionen sind bereits in der AL-FIRST-Anwendungslizenz enthalten. Daher benötigen sie keine Experience Platform Agent Orchestrator-Lizenz.

In der folgenden Tabelle sind Experience Platform-Agenten aufgeführt, die als Al-First-Anwendungen verfügbar sind. Sie werden durch die Lizenzierung dieser Al-First-Anwendungen aktiviert:

| Agent-Name | Funktionen | Unterstützte Anwendungen |
|---|----------|----------|
| [Experimentation Agent](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/content-experiment/experiment/experiment-accelerator-security) | Automatisieren, analysieren und synthetisieren Sie Einblicke, sodass Sie wirkungsvolle Experimente und Wachstumsmöglichkeiten schnell von einem zentralen Arbeitsbereich aus identifizieren können - und das bei gleichzeitiger Reduzierung manueller Prozesse. | <ul><li>AJO Experimentation Accelerator</li></ul> |
| [LLM-Optimierungsagent](https://experienceleague.adobe.com/de/docs/llm-optimizer/using/home) | Verbesserung der Sichtbarkeit, Genauigkeit und des Einflusses in KI-gesteuerten Suchumgebungen, Bereitstellung von Einblicken in die Markenpräsenz in KI-generierten Antworten, Angebot präskriptiver Inhaltsempfehlungen und Automatisierung von Optimierungskorrekturen. | <ul><li>Adobe LLM Optimizer</li></ul> |
| [Site Optimization Agent](https://experienceleague.adobe.com/de/docs/experience-manager-sites-optimizer/content/home) | Maximieren Sie die geschäftliche Auswirkung, indem Sie Website-Verbesserungen automatisch erkennen und bereitstellen. Durch die Verwendung generativer KI und mehrerer Überwachungstechnologien können Sie die Erfassung und Interaktion von Website-Traffic steigern und vieles mehr | <ul><li>AEM Sites Optimizer</li></ul> |
| [Product Advisor Agent](https://experienceleague.adobe.com/en/docs/brand-concierge/content/documentation/overview) | Steigern Sie Ihre Konversionen und Interaktionen durch intelligente, kontextbezogene Produkterkennung, die auf individuelle Vorlieben und Verhaltensweisen zugeschnitten ist. | <ul><li>Adobe Brand Concierge</li></ul> |

## Weitere Hilfe zu diesem Thema

* [KI in Experience Cloud](https://experienceleague.adobe.com/de/docs/ai) Dokumentations-Startseite
* [Überblick über Agenten in AEM](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/overview)

[!BADGE Weitere Informationen zu Adobe for Business]{type=Informative url="https://business.adobe.com/products/experience-platform/agent-orchestrator.html" tooltip="Navigieren Sie zu Business.adobe.com ."}
