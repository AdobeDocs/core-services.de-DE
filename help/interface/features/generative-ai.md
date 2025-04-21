---
title: KI in Experience Cloud-Anwendungen
description: Erfahren Sie, wie Experience Cloud-Programme generative KI und den KI-Assistenten verwenden.
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
hide: false
hidefromtoc: true
index: n
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: 4f51bc948f3d109f8c1211fda44adee17cc05170
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 8%

---

# KI in Experience Cloud-Anwendungen

Auf dieser Seite erfahren Sie mehr über generative KI und deren Verwendung in Experience Cloud-Programmen. Erfahren Sie, welche Produktfunktionen generative KI und KI-Assistenten verwenden und ob Adobe Firefly unterstützt wird.

## Über generative KI und den KI-Assistenten

Generative KI ist eine Art von künstlicher Intelligenz, die mehr tut, als nur Fragen zu beantworten. Es _erstellt_ Inhalte und _reagiert_ auf Ihre _Aufforderungen_ (Fragen und Aussagen).

* **Erstellen:** Bezieht sich auf die Fähigkeit der KI, neue Inhalte (Text, Bilder, Musik oder Videos) von Grund auf neu zu generieren, basierend auf ihren Schulungs- und Eingabeaufforderungen. Diese Fähigkeit ist der _generative_ Aspekt generativer KI.

* **Antwort:** Bezieht sich auf die KI, die eine Antwort oder Reaktion auf eine bestimmte Frage, Erklärung oder Eingabeaufforderung bereitstellt, normalerweise unter Verwendung ihrer Kenntnisse oder Argumentationsfunktionen.

Bestimmte Experience Cloud-Anwendungen nutzen generative KI, um neuen Anwendern schnell Produktkenntnisse zu vermitteln und erfahrenen Anwendern in Sekundenschnelle statt Stunden operative Erkenntnisse zu liefern.

### KI-Assistent

[AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing) ist ein Dialogtool, das in Experience Platform und verwandten Programmen unterstützt wird. Verwenden Sie sie, um Ihre Workflows zu beschleunigen, Ihre Produktkenntnisse zu verbessern, Probleme zu beheben oder Informationen zu durchsuchen. Der KI-Assistent ermöglicht es Ihnen, betriebliche Einblicke in Sekunden anstatt in Stunden zu erhalten.

Alle Antworten auf das Produktwissen sind überprüfbar und werden mit Links zur Produktdokumentation in Experience League zitiert. [Erfahren Sie mehr über ](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home) KI-Assistenten und die Arten von objektbasierten Eingabeaufforderungen, um den KI-Assistenten optimal zu nutzen.

## Experience Cloud-Anwendungen, die KI verwenden

* [Adobe GenStudio for Performance Marketing](#gspm)
* [Adobe Experience Manager Sites (Cloud Service)](#aem-sites)
* [Adobe Journey Optimizer](#journey-optimizer)
* [Adobe Journey Optimizer Prime und Ultimate](#ajo-prime-ultimate)
* [Journey Optimizer B2B Edition](#ajo-b2b)

### GenStudio for Performance Marketing {#gspm}

[GenStudio for Performance Marketing](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home) ist eine generative KI-gesteuerte Plattform, mit der Sie Kampagnen-Assets erstellen, bereitstellen und optimieren können. Die generativen KI-Funktionen transformieren, wie Marketing-Inhalte erstellt, geprüft, freigegeben und analysiert werden.

Mit der Funktion _GenStudio for Performance Marketing Create_ (oder einfach _Create_) können Marketing-Fachleute und verteilte Teams leistungsstarke On-Brand-Erlebnisse erstellen. Sie können Inhalte generieren für:

* E-Mails
* Meta-Anzeigen
* LinkedIn-Anzeigen
* Anzeigen anzeigen
* Banner

Sie können GenStudio for Performance Marketing auch in Ihrer Markendarstellung schulen, indem Sie Beispiele, Beschreibungen von Kundenrollen und -produkten sowie Markenrichtlinien verwenden. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)

**Kompatibilität mit Adobe Firefly:** geplant

### Experience Manager Sites {#aem-sites}

AEM Sites verwendet [Varianten generieren](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations). Varianten generieren verwendet generative KI, um Inhaltsvarianten basierend auf Eingabeaufforderungen zu erstellen. Diese Eingabeaufforderungen werden entweder von [Adobe bereitgestellt ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) von ([) erstellt und ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt).

Nachdem Sie Varianten erstellt haben, können Sie den Inhalt auf Ihrer Website verwenden und den Erfolg mithilfe der Experimentier-Funktion in Edge Delivery Services messen.

**Eingabe** Zu den Eingabefeldern gehören:

* Anzahl der zu erzeugenden Varianten
* Zielgruppen-Source
* Audience-Ziel
* Zusätzlicher Kontext
* Kundengesteuerte Eingabeaufforderungen

**Ausgabe:** generierte Inhalte / Marktkopie. Sie haben auch die Möglichkeit, Bilder in Adobe Express mithilfe der Generative AI-Funktionen von Firefly zu generieren.

Siehe [Bild generieren](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image).

**Kompatibilität mit Adobe Firefly:** Ja

## Journey Optimizer {#journey-optimizer}

Journey Optimizer verwendet [KI-](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home)) mit zwei Fragenklassen:

**Produktwissen** - Fragt Adobe-Datenspeicher (z. B. die Experience League-Produktdokumentation) nach insight ab. Diese Ausgabe ist kundenunabhängig. Beispiel:

* Wie viele Live-Aktivitäten kann ich in einer Adobe Journey Optimizer-Sandbox haben?

**Operational Insights (Beta)** fragt einen kundenspezifischen operativen Insights-Datenspeicher ab, der zentralisierte Betriebsdaten über Journeys enthält, die nach der Sandbox des Kunden unterteilt sind. ruft Metadaten nur aus Geschäftsobjekten ab und greift nicht auf Daten innerhalb der Sandbox zu.

* Wie viele Journey wurden in den letzten sieben Tagen erstellt?

Die Ausgabe von Operational Insights hängt von den Metadaten ab, die aus den Geschäftsobjekten des Kunden abgerufen werden.

Journey ist das einzige für den KI-Assistenten in Journey Optimizer verfügbare Objekt, und Metadaten werden aus der aktuellen Sandbox abgerufen.

Siehe [Arbeiten mit dem KI-Assistenten](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) und [Außenbereitschaft](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11) für weitere Informationen.

**Kompatibilität mit Adobe Firefly:** Nein

## Journey Optimizer Prime und Ultimate {#ajo-prime-ultimate}

Journey Optimizer Prime und Ultimate verwenden [KI-Assistenten für Content Accelerator](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) um proaktive Inhaltsvariantenvorschläge für Text und Bilder einzubringen.

Diese Funktion ist für E-Mail-, Push-, Web- und SMS-Kanäle verfügbar. Es bietet eine sofortige Text- und Bildgenerierung.

**E-**: Generieren einer vollständigen E-Mail, nur Text oder Bild. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email)

**Push-Benachrichtigung** - Nur Text oder Bild als vollständige Push-Benachrichtigung generieren. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push)

**SMS** - Vollständige SMS oder nur Text generieren. [Weitere Informationen](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms)

**WebPage** - Generieren von Web-Seitenbildern oder Web-Seitentext. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web)

**Content** - Generieren von Inhalten für verschiedene Messaging-Kampagnen. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)

**Hinweis:** Ausgabe von Content Accelerator in AJO Prime und Ultimate ist entschädigt.

**Kompatibilität mit Adobe Firefly:** Ja

## Journey Optimizer B2B Edition {#ajo-b2b}

Verwendet [KI-](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)) für Produktinformationen.

**Produktwissen** - Fragt Adobe-Datenspeicher (z. B. die Experience League-Produktdokumentation) nach insight ab. Diese Ausgabe ist kundenunabhängig. | <ul><li>**Eingabe:** Wie sende ich eine E-Mail auf einer Konto-Journey?</li><li>**Ausgabe:** Produktkenntnisse werden von Experience League abgerufen (öffentliche Dokumentation). [Weitere Infos…](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul>   | Nein   |

<!-- ## Experience Cloud applications that use AI

Learn how Experience Cloud applications use generative AI or AI Assistant, and whether Adobe Firefly is supported. 

| Application | How Generative AI Is Used | Examples | Adobe Firefly? |
|----------|------------|-----------|----------------|
| GenStudio for Performance Marketing | [GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) is a generative AI-driven platform. It infuses the content creation lifecycle with generative AI capabilities that transform how marketing content is created, reviewed, shared, and analyzed.<br>You can train GenStudio for Performance Marketing on your brand using examples, descriptions of customer personas and products, and brand guidelines. |_GenStudio for Performance Marketing Create_ lets you generate content for emails, Meta ads, LinkedIn ads, display ads, and banners. <br>**Inputs:** <ul><li>Use templates to start the content creation process. </li><li>Add parameters like Brands, Products, and Personas (guidelines) and Content (assets) to shape the generated experience. </li><li>Enter descriptive prompts that describe the context or experience you intend to generate. [Learn more...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)</li></ul> |Yes |
|Adobe Experience Manager Sites (Cloud Service)  | AEM Sites uses [Generate Variations](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations). <br>Generate Variations uses generative AI to create content variations based on prompts. These prompts are either provided by Adobe or created and managed by users. |After creating variations, you can use the content on your website and measure its success using the Experimentation functionality of Edge Delivery Services. <br>**Input:** Input fields include Number of Variations to generate; Audience Source / Audience Target; Additional Context, and customer-driven prompts. <ul><li>[Adobe prompt template](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) </li><li>[User generated prompt](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt)</li></ul> **Output:** Generated Content / Market Copy. You also have the option to generate images in Adobe Express using the generative AI capabilities of Firefly. See [Generate Image](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image). | Yes|
| Adobe Journey Optimizer |Journey Optimizer uses [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) with two classes of questions:<ul><li>**Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. </li><li>**Operational Insights (Beta)** - queries a customer-specific operational insights data store that contains centralized operational data about Journeys, partitioned by the customer's sandbox. Pulls metadata only from business objects and does not access data within the sandbox.</li></ul>|<ul><li>**Product Knowledge Input:** How many live activities can I have in one Adobe Journey Optimizer sandbox?</li><li>**Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li><li>**Operational Insights Input:** How many Journeys have been created in the last seven days? </li><li>**Operational Insights Output:** Operational Insights output depends on metadata pulled from customer's business objects. Journeys is the only object available in AJO, and metadata is pulled from the current sandbox. </li></ul> See [Work with the AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) and [Field Readiness](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11) | No |
| Journey Optimizer: _Prime_ and _Ultimate_  | [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) brings proactive content variation suggestions for text and images. It is available for email, push, web and SMS channels. This new capability provides prompt-based text and image generation. |<ul><li> **Email** - generate a full email, text only or image only. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email) </li><li> **Push Notification** - Generate a full push notification, text only or image only. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push) </li><li> **SMS** - Generate a full SMS, or text only. [Learn more](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) </li><li> **Webpage** - Generate web page images or web page text. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web) </li><li> **Content** - Generate content for various messaging campaigns. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)</li></ul> **Note:** Output from Content Accelerator in AJO Prime and Ultimate is indemnified. | Yes   |
| Journey Optimizer B2B Edition  | Uses [AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant) with one class of questions: <br> **Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. | <ul><li>**Input:** How do I send an email in an account journey?</li><li>**Output:** Product Knowledge pulls from Experience League (public documentation). [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul>   | No   |
| Campaign Managed Cloud Services | [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs) auto-generates personalized, engaging, and effective content based on the marketing objective with content optimized for brand outlined styles, layouts, tone, and more across channels like Email, SMS, Push. |<ul><li> **Email** - Generate a full email, text only or image only. [Learn more](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content) </li><li> **SMS** - Generate full SMS or text only. [Learn more...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms) </li><li> **Push** - Craft compelling messaging and generate content. [Learn more...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push) </li></ul> **Note:** Output from Content Accelerator in Campaign Managed Cloud Services is indemnified. | Yes  |
| Customer Journey Analytics   | CJA uses [AI Assistant](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant) to help you discover product knowledge and insights from Experience League. <br>For example, new users can use it to learn Customer Journey Analytics concepts and onboard yourself to products and features that you are unfamiliar with. <br>Experienced users can use AI Assistant to present more advanced use cases or tips and tricks and perform tasks at a fast pace. Understand concepts, troubleshoot problems, or search for information. [Learn more...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge) | <ul><li>**Product Knowledge Input:** How do I build a calculated metric? </li><li> **Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li></ul> | No |
| Customer Journey Analytics    | [Intelligent Captions](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) provides natural-language insights for line visualizations in Workspace visualizations.| <ul><li>**Input:** Line visualizations. Captions are auto-generated based on such line visualizations when you click **Intelligent captions**. </li><li> **Output:** Auto-generated natural-language captions.</li></ul>  | No             |
| Real-Time CDP |Uses [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) to help you discover product knowledge and insights from Experience League. It queries a database and translates data from the database into a human-readable answer. Two classes of questions: <br> **Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. <br> **Operational Insights (Beta)** - Queries a customer-specific operational insights data store that contains centralized operational data, partitioned by the customer's AEP sandbox. Pulls metadata only from Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources, and does not access data within the sandbox. <br>For example, for a query about an audience [!DNL AI Assistant] can access the name of the audience and other associated metadata but cannot access the profiles within that audience. | <ul><li>**Product Knowledge Input:** How is profile richness calculated? </li><li>**Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li><li> **Operational Insights Input:** How many datasets do I have? </li><li> **Operational Insights Output:** Operational Insights output depends on metadata pulled from Customer's business objects (Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources), and includes a link to specific UI page containing queried data. </li></ul>For examples, see the _Product Knowledge_ and _Operational Insights_ input tables in [AI Assistant in Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)  | No |
| Marketo  | [Dynamic Chat](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview) creates AI-assisted conversations with customized and pre-approved questions and answers, as well as conversation summary |<ul><li> **Generate Questions:** Provide URLs from which content is extracted and used to generate questions / responses. </li><li> **Conversation Summary:** Generates a summary of a chat conversation. </li></ul> [Learn more...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/response-library)  | No |
| Workfront | [AI Assistant](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview) in Workfront helps you accomplish your work by offering in-app information and suggestions in a natural-language conversation. AI Assistant offers the following functionality: Summarizes projects/tasks/issues/documents, provides instructions or reference information pulled from the Workfront documentation on Experience League, generates or refines formulas for calculated custom fields.  | <ul><li>**Summarize Project Input:** Summarize this project </li><li> **Summarize Project Output:** Returns brief descriptions of the project's purpose and status, gives examples of tasks that are completed and that are still pending, and provides some additional details and notes.</li><li> **Generate/Refine Formula Input:** "Rewrite this formula to remove the invalid expression error." </li><li> **Generate/Refine Formula Output:** Generated or refined formula. </li></ul>**Note:** AI Assistant may take a few moments to generate the revised formula, depending on the size and complexity of the formula. | No  | -->
