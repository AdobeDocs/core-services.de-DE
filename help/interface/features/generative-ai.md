---
title: KI in Experience Cloud-Anwendungen
description: Erfahren Sie mehr über generative KI und darüber, wie Experience Cloud-Programme genAI und AI Assistant verwenden.
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: aad561869cdfa7ddbc66b296d0a46c8f49f83d94
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 4%

---

# KI in Experience Cloud-Anwendungen

Auf dieser Seite erfahren Sie mehr über generative KI und deren Verwendung in Experience Cloud-Programmen. Erfahren Sie, welche Produktfunktionen generative KI und KI-Assistenten verwenden und ob Adobe Firefly unterstützt wird.

## Über generative KI und den KI-Assistenten

Generative KI ist eine Art von künstlicher Intelligenz, die mehr tut, als nur Fragen zu beantworten. Es _erstellt_ Inhalte und _reagiert_ auf Ihre _Aufforderungen_ (Fragen und Aussagen).

* **Erstellen:** Bezieht sich auf die Fähigkeit der KI, neue Inhalte (Text, Bilder, Musik oder Videos) von Grund auf neu zu generieren, basierend auf ihren Schulungs- und Eingabeaufforderungen. Diese Fähigkeit ist der _generative_ Aspekt generativer KI.

* **Antwort:** bezieht sich auf die KI, die eine Antwort oder Reaktion auf eine bestimmte Eingabeaufforderung bereitstellt, normalerweise unter Verwendung ihrer Kenntnisse oder Argumentationsfunktionen.

Wenn Sie neu bei Experience Cloud sind, können Sie generative KI verwenden, um Produktkenntnisse schnell zu erwerben. Als erfahrener Anwender können Sie operative Einblicke in Sekunden anstatt in Stunden erlangen.

### KI-Assistent

[AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing) ist ein Dialogtool, das in Experience Platform und verwandten Programmen unterstützt wird. Verwenden Sie sie, um Ihre Workflows zu beschleunigen, Ihre Produktkenntnisse zu verbessern, Probleme zu beheben oder Informationen zu durchsuchen. Mit dem KI-Assistenten können Sie in bestimmten Anwendungen sofort operative Erkenntnisse gewinnen.

Die Antworten auf Produktkenntnisse von Experience League sind überprüfbar und werden mit Links angegeben. Erfahren Sie mehr über die Arten [ (objektbasierten Eingabeaufforderungen](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home) um den KI-Assistenten optimal zu nutzen.

<!-- **Your data remains yours**

In AI Assistant, security is the priority:

* Customer data is not used to train language models.
* AI Assistant looks at only the documents that you tell it to. You are in control.
* Your people can use AI Assistant only on documents they can access.
* It's audit-ready: Responses are attributable to source documents.
* Enterprise controls are in place to manage who has AI access in the company. -->

## Anwendungen mit Funktionen, die KI unterstützen

* [GenStudio for Performance Marketing](#gspm)
* [Erzeugen von Varianten in AEM Sites (Cloud Service)](#aem-sites)
* [KI-Assistent in Journey Optimizer](#journey-optimizer)
* [Adobe Journey Optimizer Prime und Ultimate](#ajo-prime-ultimate)
* [Journey Optimizer B2B Edition](#ajo-b2b)
* [KI-Assistent in Journey Optimizer Prime und Ultimate](#ajo-prime-ultimate)
* [KI-Assistent in Journey Optimizer B2B edition](#ajo-b2b)
* [KI-Assistent in Campaign Managed Cloud Services](#campaign-cs)
* [KI-Assistent in Customer Journey Analytics](#cja)
* [Intelligente Beschriftungen in Customer Journey Analytics](#cja-captions)
* [KI-Assistent in Real-Time CDP](#rtcdp)
* [Dynamic Chat in Marketo](#marketo)
* [KI-Assistent in Workfront](#workfront)

### GenStudio for Performance Marketing {#gspm}

[GenStudio for Performance Marketing](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home) ist eine generative KI-gesteuerte Plattform mit Funktionen, die die Erstellung, Überprüfung, Freigabe und Analyse von Marketing-Inhalten transformieren können.

Auf der [Erstellen](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)-Startseite können Sie leistungsstarke, markeninterne Erlebnisse erstellen. Inhalt generieren für:

* E-Mails
* Meta-Anzeigen
* LinkedIn-Anzeigen
* Anzeigen anzeigen
* Banner

Sie können GenStudio for Performance Marketing auch in Ihrer Markendarstellung schulen, indem Sie Beispiele, Beschreibungen von Kundenrollen und -produkten sowie Markenrichtlinien verwenden. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)

**Kompatibel mit Adobe Firefly:** geplant

### Erzeugen von Varianten in Experience Manager Sites {#aem-sites}

[Varianten generieren](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations) in AEM Sites verwendet generative KI, um Inhaltsvarianten basierend auf Eingabeaufforderungen zu erstellen. Diese Eingabeaufforderungen werden entweder von [Adobe bereitgestellt ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) von ([) erstellt und ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt).

Nachdem Sie Varianten erstellt haben, können Sie den Inhalt auf Ihrer Website verwenden und den Erfolg mithilfe der Experimentier-Funktion in Edge Delivery Services messen.

### Eingabe- und Ausgabefelder

Zu den Eingabefeldern gehören:

* Anzahl der zu erzeugenden Varianten
* Zielgruppen-Source
* Audience-Ziel
* Zusätzlicher Kontext
* Kundengesteuerte Eingabeaufforderungen

Die Ausgabe ist generierter Inhalt oder eine Marktkopie.

Sie haben auch die Möglichkeit, Bilder in Adobe Express mithilfe der Generative AI-Funktionen von Firefly zu generieren. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image)

**Kompatibel mit Adobe Firefly:** Ja

## KI-Assistent in Journey Optimizer {#journey-optimizer}

In Journey Optimizer kann Ihnen der KI-Assistent dabei helfen, Produktkenntnisse und operative Erkenntnisse zu gewinnen.

**Produktwissen:** KI-Assistent fragt Adobe-Datenspeicher (wie z. B. die Experience League-Produktdokumentation) nach insight ab. Die Ausgabe ist kundenunabhängig.

Beispiel:

* _Wie viele Live-Aktivitäten kann ich in einer Adobe Journey Optimizer-Sandbox haben?_

**Operational Insights (Beta)** - Der KI-Assistent fragt einen kundenspezifischen operativen Insights-Datenspeicher ab, der zentralisierte Betriebsdaten über Journeys enthält, die nach der Sandbox des Kunden partitioniert sind. Diese Funktion ruft Metadaten nur aus Geschäftsobjekten ab und greift nicht auf Daten innerhalb der Sandbox zu.

Beispielaufforderung:

* _Wie viele Journey wurden in den letzten sieben Tagen erstellt?_

Die Ausgabe von Operational Insights hängt von den Metadaten ab, die aus den Geschäftsobjekten des Kunden abgerufen werden. Diese Ausgabe ist kundenunabhängig.

_Journey_ ist das einzige Objekt, das für den KI-Assistenten in Journey Optimizer verfügbar ist, und die Metadaten werden aus der aktuellen Sandbox abgerufen. [Weitere Infos...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant).

**Kompatibel mit Adobe Firefly:** Nein

## KI-Assistent in Journey Optimizer Prime und Ultimate {#ajo-prime-ultimate}

Journey Optimizer Prime und Ultimate verwenden [KI-Assistenten für Content Accelerator](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) um proaktive Inhaltsvariantenvorschläge für Text und Bilder einzubringen.

Diese Funktion ist für die Kanäle [E](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email), [Push](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push), [Web-](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web), [Inhalt](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation) und [SMS](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) verfügbar. Es bietet eine sofortige Text- und Bildgenerierung.

**Hinweis:** Ausgabe von Content Accelerator in AJO Prime und Ultimate ist entschädigt.

**Kompatibel mit Adobe Firefly:** Ja

## KI-Assistent in Journey Optimizer B2B edition {#ajo-b2b}

Journey Optimizer B2B edition verwendet [KI-](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)), um Sie anhand Ihrer Produktkenntnisse mit Produktkenntnissen zu unterstützen.

**Produktwissen** - Fragt Adobe-Datenspeicher (z. B. die Experience League-Produktdokumentation) nach insight ab. Diese Ausgabe ist kundenunabhängig.

* **Eingabe:** Wie sende ich eine E-Mail auf einer Konto-Journey?

* **Ausgabe:** Produktkenntnisse werden von Experience League abgerufen (öffentliche Dokumentation). [Weitere Infos…](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/question-guidance)

**Kompatibel mit Adobe Firefly:** Nein

## KI-Assistent in Campaign Managed Cloud Services {#campaign-cs}

Campaign Managed Cloud Services verwendet [KI-Assistent für Content Accelerator](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs). Mit dieser Funktion können Sie basierend auf Ihrem Marketing-Ziel automatisch personalisierte, ansprechende und effektive Inhalte generieren, wobei Inhalte für Markenstile, Layouts, Ton und mehr optimiert sind. Sie können sie über Kanäle wie [E-Mail](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content), [SMS](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms) und [Push](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push) verwenden.

**Hinweis:** Ausgabe von Content Accelerator in Campaign Managed Cloud Services wird freigegeben.

**Kompatibel mit Adobe Firefly:** Ja

## KI-Assistent in Customer Journey Analytics {#cja}

Customer Journey Analytics verwendet [KI-](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant)), um Ihnen dabei zu helfen, Produktkenntnisse und Erkenntnisse aus Experience League zu entdecken.

**Beispielaufforderung:** Wie erstelle ich eine berechnete Metrik?

Neue Anwender können damit Customer Journey Analytics-Konzepte erlernen und sich mit Produkten und Funktionen vertraut machen, mit denen Sie nicht vertraut sind.

Erfahrene Anwender können mit dem KI-Assistenten erweiterte Anwendungsfälle oder Tipps und Tricks präsentieren und Aufgaben in kürzester Zeit erledigen. Konzepte verstehen, Probleme beheben oder nach Informationen suchen. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge)

**Kompatibel mit Adobe Firefly:** Nein

## Intelligente Beschriftungen in Customer Journey Analytics {#cja-captions}

[Intelligente Beschriftungen](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) in Customer Journey Analytics bieten Einblicke in die am häufigsten verwendete Workspace-Visualisierung in natürlicher Sprache.

**Kompatibel mit Adobe Firefly:** Nein

## KI-Assistent in Real-Time CDP {#rtcdp}

Real-Time CDP verwendet [KI-](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home)), um Ihnen dabei zu helfen, Produktkenntnisse und Erkenntnisse aus Experience League zu entdecken. [Erhalten Sie Tipps](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/questions) wenn Sie Fragen stellen.

Es bietet auch operative Einblicke (in der Beta-Phase). Der KI-Assistent fragt einen kundenspezifischen operativen Insights-Datenspeicher ab, der zentralisierte Betriebsdaten enthält, die durch die AEP-Sandbox des Kunden partitioniert sind. Es werden nur Metadaten aus Attributen, Zielgruppen, Datenflüssen, Datensätzen, Zielen, Schemas und Quellen abgerufen und nicht auf Daten innerhalb der Sandbox zugegriffen.

Bei einer Abfrage über eine Zielgruppe können [!DNL AI Assistant] beispielsweise auf den Namen der Zielgruppe und andere zugehörige Metadaten zugreifen, jedoch nicht auf die Profile innerhalb dieser Zielgruppe.

z. B.:

* Eingabe: _Wie viele Datensätze habe ich?_

* Antwort: Die Ausgabe von operativen Insights hängt von den Metadaten ab, die aus den Geschäftsobjekten des Kunden abgerufen werden (Attribute, Zielgruppen, Datenflüsse, Datensätze, Ziele, Schemata und Quellen), und enthält einen Link zu einer bestimmten Benutzeroberflächenseite mit abgefragten Daten.

Weitere Beispiele finden Sie in den Eingabetabellen _Produktwissen_ und _Operative Einblicke_ im [KI-Assistenten in Experience Platform](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home)

**Kompatibel mit Firefly:** Nein

## Dynamic Chat in Marketo {#marketo}

Die Generative AI-gestützten Funktionen in Adobe Dynamic Chat ermöglichen es Ihnen, die Produktivität Ihrer Vertriebsmitarbeiter zu optimieren, Einblicke in die Besucherabsichten Ihrer Website zu erhalten und Besucherfragen sicher zu beantworten. Sie können die Fragen, Antworten und die Konversationszusammenfassung vorab genehmigen. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

**Kompatibel mit Firefly:** Nein

## KI-Assistent in Workfront {#workfront}

Der KI-Assistent in Workfront hilft Ihnen, Ihre Arbeit zu erledigen, indem er In-App-Informationen und -Vorschläge anbietet. Sie haben folgende Möglichkeiten:

* Sie erhalten Zusammenfassungen einiger Objekte, sodass Sie einen allgemeinen Überblick über den Zweck oder die Details des Objekts erhalten.
* Stellen Sie Fragen und lassen Sie [!DNL AI Assistant] Antworten auf Experience League finden.
* Generierte Formeln basierend auf Ihren Eingabeaufforderungen abrufen. Sie können auch Fehler in Ihren ungültigen benutzerdefinierten Ausdrücken in berechneten Feldern beheben.
* Suchen Sie Projekte, Aufgaben und Probleme.

[Weitere Infos…](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

**Kompatibel mit Firefly:** Nein
