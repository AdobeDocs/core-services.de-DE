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
source-git-commit: bc1f602df5a4b6f2d6eb9a3b00f2756a09d97e2b
workflow-type: tm+mt
source-wordcount: '1662'
ht-degree: 5%

---


# KI in Experience Cloud-Anwendungen

Auf dieser Seite erfahren Sie, wie Experience Cloud-Programme generative KI verwenden und wo Sie die programmspezifischen Informationen finden. Erfahren Sie mehr über die Klassen von Fragen, Eingabeaufforderungen sowie Eingabe- und Ausgabemodellen.

## Über generative KI und den KI-Assistenten

Generative KI ist eine Art von künstlicher Intelligenz, die _(neue_) und _(_) auf Ihre Aussagen und Fragen (Eingabeaufforderungen) reagieren kann:

* **Erstellen:** Bezieht sich auf die Fähigkeit der KI, neue Inhalte (Text, Bilder, Musik oder Videos) von Grund auf neu zu generieren, basierend auf ihren Schulungs- und Eingabeaufforderungen. Diese Fähigkeit ist der _generative_ Aspekt generativer KI.

* **Antwort:** Bezieht sich auf die KI, die eine Antwort oder Reaktion auf eine bestimmte Frage, Erklärung oder Eingabeaufforderung bereitstellt, normalerweise unter Verwendung ihrer Kenntnisse oder Argumentationsfunktionen.

Bestimmte Experience Cloud-Anwendungen nutzen generative KI, um neuen Anwendern schnell Produktkenntnisse zu vermitteln und erfahrenen Anwendern in Sekundenschnelle statt Stunden operative Erkenntnisse zu liefern.

### KI-Assistent

[AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing) ist ein Dialogtool, das in Experience Platform und verwandten Programmen unterstützt wird. Verwenden Sie sie, um Ihre Workflows zu beschleunigen, Ihre Produktkenntnisse zu verbessern, Probleme zu beheben oder Informationen zu durchsuchen. Der KI-Assistent ermöglicht es Ihnen, betriebliche Einblicke in Sekunden anstatt in Stunden zu erhalten.

Alle Antworten auf das Produktwissen sind überprüfbar und werden mit Links zur Produktdokumentation in Experience League zitiert. [Erfahren Sie mehr über ](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home) KI-Assistenten und die Arten von objektbasierten Eingabeaufforderungen, um den KI-Assistenten optimal zu nutzen.

## Experience Cloud-Anwendungen, die KI verwenden

Unterkopfversion (unfertig)…

* [GenStudio for Performance Marketing](#gspm)
* [Experience Manager Sites (Cloud Service)](#aem-sites)
* Weitere folgen…

### GenStudio for Performance Marketing {#gspm}

[GenStudio for Performance Marketing](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home) ist eine generative KI-gesteuerte Plattform. Sie fügt dem Lebenszyklus der Inhaltserstellung generative KI-Funktionen hinzu, die die Erstellung, Überprüfung, Freigabe und Analyse von Marketing-Inhalten transformieren.

_GenStudio for Performance Marketing Create_ nutzt die Leistungsfähigkeit von Adobe GenAI, um Marketing-Fachleute und verteilte Teams in die Lage zu versetzen, leistungsstarke On-Brand-Erlebnisse zu schaffen. Inhalt generieren für:

* E-Mails
* Meta-Anzeigen
* LinkedIn-Anzeigen
* Anzeigen anzeigen
* Banner

Sie können GenStudio for Performance Marketing anhand von Beispielen, Beschreibungen von Kundenrollen und -produkten sowie Markenrichtlinien in Ihrer Marke schulen. [Weitere Informationen.](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)

**Kompatibilität mit Adobe Firefly:** geplant

### Experience Manager Sites {#aem-sites}

AEM Sites verwendet [Varianten generieren](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations). Varianten generieren verwendet generative KI, um Inhaltsvarianten basierend auf Eingabeaufforderungen zu erstellen. Diese Eingabeaufforderungen werden entweder von [Adobe bereitgestellt ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) von ([) erstellt und ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt).

Nachdem Sie Varianten erstellt haben, können Sie den Inhalt auf Ihrer Website verwenden und den Erfolg mithilfe der Experimentierfunktion von Edge Delivery Services messen.

**Eingabe** Zu den Eingabefeldern gehören:

* Anzahl der zu erzeugenden Varianten
* Zielgruppen-Source
* Audience-Ziel
* Zusätzlicher Kontext
* Kundengesteuerte Eingabeaufforderungen

**Ausgabe:** generierte Inhalte / Marktkopie. Sie haben auch die Möglichkeit, Bilder in Adobe Express mithilfe der Generative AI-Funktionen von Firefly zu generieren.

Siehe [Bild generieren](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image).

**Kompatibilität mit Adobe Firefly:** Ja



Tabellenversion…

## Experience Cloud-Anwendungen, die KI verwenden

Erfahren Sie, wie Experience Cloud-Programme generative KI oder KI-Assistenten verwenden und ob Adobe Firefly unterstützt wird.

| Anwendung | Verwendung der generativen KI | Beispiele | Adobe Firefly? |
|----------|------------|-----------|----------------|
| GenStudio for Performance Marketing | [GenStudio for Performance Marketing](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home) ist eine generative KI-gesteuerte Plattform. Sie fügt dem Lebenszyklus der Inhaltserstellung generative KI-Funktionen hinzu, die die Erstellung, Überprüfung, Freigabe und Analyse von Marketing-Inhalten transformieren.<br>Sie können GenStudio for Performance Marketing anhand von Beispielen, Beschreibungen von Kundenrollen und -produkten sowie Markenrichtlinien in Ihrer Marke schulen. | Mit _GenStudio for Performance Marketing Create_ können Sie Inhalte für E-Mails, Meta-Anzeigen, LinkedIn-Anzeigen, Display-Anzeigen und Banner generieren. <br>**Eingänge:** <ul><li>Verwenden Sie Vorlagen, um den Inhaltserstellungsprozess zu starten. </li><li>Fügen Sie Parameter wie Marken, Produkte und Personas (Richtlinien) und Inhalte (Assets) hinzu, um das generierte Erlebnis zu gestalten. </li><li>Geben Sie beschreibende Eingabeaufforderungen ein, die den Kontext oder das Erlebnis beschreiben, das Sie generieren möchten. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)</li></ul> | Ja |
| Adobe Experience Manager Sites (Cloud Service) | AEM Sites verwendet [Varianten generieren](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations). <br>Varianten generieren verwendet generative KI, um Inhaltsvarianten basierend auf Eingabeaufforderungen zu erstellen. Diese Eingabeaufforderungen werden entweder von Adobe bereitgestellt oder von Benutzenden erstellt und verwaltet. | Nachdem Sie Varianten erstellt haben, können Sie den Inhalt auf Ihrer Website verwenden und den Erfolg mithilfe der Experimentierfunktion von Edge Delivery Services messen. <br>**Eingabe:** Eingabefelder enthalten die Anzahl der zu generierenden Varianten; Zielgruppen-Source / Zielgruppen-Target; Zusätzlicher Kontext und kundengesteuerte Eingabeaufforderungen. <ul><li>[Adobe-Eingabeaufforderungsvorlage](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) </li><li>[Benutzergenerierte Eingabeaufforderung](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt)</li></ul> **Ausgabe:** generierte Inhalte / Marktkopie. Sie haben auch die Möglichkeit, Bilder in Adobe Express mithilfe der Generative AI-Funktionen von Firefly zu generieren. Siehe [Bild generieren](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image). | Ja |
| Adobe Journey Optimizer | Journey Optimizer verwendet [KI-](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home)) mit zwei Fragenklassen:<ul><li>**Produktwissen** - Fragt Adobe-Datenspeicher (z. B. die Experience League-Produktdokumentation) nach insight ab. Diese Ausgabe ist kundenunabhängig. </li><li>**Operational Insights (Beta)** fragt einen kundenspezifischen operativen Insights-Datenspeicher ab, der zentralisierte Betriebsdaten über Journeys enthält, die nach der Sandbox des Kunden unterteilt sind. ruft Metadaten nur aus Geschäftsobjekten ab und greift nicht auf Daten innerhalb der Sandbox zu.</li></ul> | <ul><li>**Produktinformationen** Wie viele Live-Aktivitäten kann ich in einer Adobe Journey Optimizer-Sandbox haben?</li><li>**Ausgabe von Produktkenntnissen:** Produktkenntnisse werden von Experience League abgerufen (öffentliche Dokumentation). </li><li>**Operational Insights Input** Wie viele Journey wurden in den letzten sieben Tagen erstellt? </li><li>**Operative Insights-Ausgabe:** operative Insights-Ausgabe hängt von den Metadaten ab, die aus den Geschäftsobjekten des Kunden abgerufen werden. Journey ist das einzige in AJO verfügbare Objekt, und Metadaten werden aus der aktuellen Sandbox abgerufen. </li></ul> Siehe [Arbeiten mit dem KI-Assistenten](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) und [Außenbereitschaft](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11) | Nein |
| Journey Optimizer: _Prime_ und _Ultimate_ | [KI-Assistent für Content Accelerator](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) bietet proaktive Vorschläge für Inhaltsvarianten für Text und Bilder. Es ist für E-Mail-, Push-, Web- und SMS-Kanäle verfügbar. Diese neue Funktion ermöglicht eine sofortige Text- und Bildgenerierung. | <ul><li> **E-**: Generieren einer vollständigen E-Mail, nur Text oder Bild. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email) </li><li> **Push-Benachrichtigung** - Nur Text oder Bild als vollständige Push-Benachrichtigung generieren. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push) </li><li> **SMS** - Vollständige SMS oder nur Text generieren. [Weitere Informationen](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) </li><li> **WebPage** - Generieren von Web-Seitenbildern oder Web-Seitentext. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web) </li><li> **Content** - Generieren von Inhalten für verschiedene Messaging-Kampagnen. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)</li></ul> **Hinweis:** Ausgabe von Content Accelerator in AJO Prime und Ultimate ist entschädigt. | Ja |
| Journey Optimizer B2B Edition | Verwendet [KI-](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)) mit einer Klasse von Fragen: <br> **Produktwissen** - Fragt Adobe-Datenspeicher (z. B. die Experience League-Produktdokumentation) nach insight ab. Diese Ausgabe ist kundenunabhängig. | <ul><li>**Eingabe:** Wie sende ich eine E-Mail auf einer Konto-Journey?</li><li>**Ausgabe:** Produktkenntnisse werden von Experience League abgerufen (öffentliche Dokumentation). [Weitere Infos…](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul> | Nein |
| Campaign Managed Cloud Services | [KI-Assistent für Content Accelerator](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs) generiert automatisch personalisierte, ansprechende und effektive Inhalte basierend auf dem Marketing-Ziel mit Inhalten, die für Markenstile, Layouts, Ton und mehr auf Kanälen wie E-Mail, SMS und Push optimiert sind. | <ul><li> **E-**: Nur eine vollständige E-Mail, nur Text oder Bild generieren. [Weitere Informationen](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content) </li><li> **SMS** - Nur vollständige SMS oder Text generieren. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms) </li><li> **Push** - Erstellen Sie überzeugende Nachrichten und generieren Sie Inhalte. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push) </li></ul> **Hinweis:** Ausgabe von Content Accelerator in Campaign Managed Cloud Services wird freigegeben. | Ja |
| Customer Journey Analytics | CJA verwendet [KI-](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant)), um Ihnen dabei zu helfen, Produktkenntnisse und Erkenntnisse aus Experience League zu entdecken. <br>Beispielsweise können neue Benutzende damit Customer Journey Analytics-Konzepte erlernen und sich mit Produkten und Funktionen vertraut machen, die ihnen nicht bekannt sind. <br>Erfahrene Anwender können den KI-Assistenten verwenden, um komplexere Anwendungsfälle oder Tipps und Tricks vorzustellen und Aufgaben schnell durchzuführen. Konzepte verstehen, Probleme beheben oder nach Informationen suchen. [Weitere Infos…](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge) | <ul><li>**Produktinformationen** Wie erstelle ich eine berechnete Metrik? </li><li> **Ausgabe von Produktkenntnissen:** Produktkenntnisse werden von Experience League abgerufen (öffentliche Dokumentation). </li></ul> | Nein |
| Customer Journey Analytics | [Intelligente Beschriftungen](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) bietet Einblicke in natürlicher Sprache für Linienvisualisierungen in Workspace-Visualisierungen. | <ul><li>**Eingabe:** Linienvisualisierungen. Beschriftungen werden basierend auf diesen Linienvisualisierungen automatisch generiert, wenn Sie auf &quot;**Beschriftungen** klicken. </li><li> **Ausgabe:** automatisch generierte Untertitel in natürlicher Sprache.</li></ul> | Nein |
| Real-Time CDP | Verwendet [KI-](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home)), um Ihnen dabei zu helfen, Produktkenntnisse und Erkenntnisse aus Experience League zu entdecken. Es fragt eine Datenbank ab und übersetzt Daten aus der Datenbank in eine für Menschen lesbare Antwort. Zwei Fragenklassen: <br> **Produktwissen** - Fragt Adobe-Datenspeicher (z. B. die Experience League-Produktdokumentation) nach insight ab. Diese Ausgabe ist kundenunabhängig. <br> **Operational Insights (Beta)** Abfragen eines kundenspezifischen operativen Insights-Datenspeichers, der zentralisierte Betriebsdaten enthält, die durch die AEP-Sandbox des Kunden partitioniert werden. ruft Metadaten nur aus Attributen, Zielgruppen, Datenflüssen, Datensätzen, Zielen, Schemas und Quellen ab und greift nicht auf Daten innerhalb der Sandbox zu. <br>Bei einer Abfrage über eine Zielgruppe können [!DNL AI Assistant] beispielsweise auf den Namen der Zielgruppe und andere zugehörige Metadaten zugreifen, jedoch nicht auf die Profile innerhalb dieser Zielgruppe. | <ul><li>**Produktinformationen** Wie wird die Profilreichhaltigkeit berechnet? </li><li>**Ausgabe von Produktkenntnissen:** Produktkenntnisse werden von Experience League abgerufen (öffentliche Dokumentation). </li><li> **Input für operative Insights:** viele Datensätze habe ich? </li><li> **Operative Insights-Ausgabe:** Operative Insights-Ausgabe hängt von den Metadaten ab, die aus den Geschäftsobjekten des Kunden abgerufen werden (Attribute, Zielgruppen, Datenflüsse, Datensätze, Ziele, Schemata und Quellen) und enthält einen Link zu einer bestimmten Benutzeroberflächenseite mit abgefragten Daten. </li></ul>Beispiele finden Sie in den Eingabetabellen _Produktwissen_ und _Operative_&quot; im [KI-Assistenten in Experience Platform](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home) | Nein |
| Marketo | [Dynamic Chat](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview) erstellt KI-unterstützte Konversationen mit benutzerdefinierten und vorab genehmigten Fragen und Antworten sowie eine Konversationszusammenfassung | <ul><li> **Fragen generieren:** Geben Sie die URLs an, aus denen Inhalte extrahiert und zum Generieren von Fragen/Antworten verwendet werden sollen. </li><li> **Konversationszusammenfassung:** Erzeugt eine Zusammenfassung einer Chat-Konversation. </li></ul> [Weitere Infos…](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/response-library) | Nein |
| Workfront | [AI Assistant](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview) in Workfront hilft Ihnen, Ihre Arbeit zu erledigen, indem Sie In-App-Informationen und -Vorschläge in einem Gespräch in natürlicher Sprache anbieten. Der KI-Assistent bietet die folgenden Funktionen: Fasst Projekte/Aufgaben/Probleme/Dokumente zusammen, stellt Anweisungen oder Referenzinformationen bereit, die aus der Workfront-Dokumentation in Experience League abgerufen werden, generiert oder verfeinert Formeln für berechnete benutzerdefinierte Felder. | <ul><li>**Projekteingabe zusammenfassen** Dieses Projekt zusammenfassen </li><li> **Projektausgabe zusammenfassen** Gibt kurze Beschreibungen des Zwecks und Status des Projekts zurück, gibt Beispiele für abgeschlossene und noch ausstehende Aufgaben und liefert einige zusätzliche Details und Hinweise.</li><li> **Formeleingabe generieren/verfeinern:** „Diese Formel neu schreiben, um den Fehler wegen ungültigem Ausdruck zu entfernen.“ </li><li> **Formelausgabe generieren/verfeinern:** generierte oder verfeinerte Formel. </li></ul>**Hinweis:** KI-Assistent kann je nach Größe und Komplexität der Formel einige Minuten dauern, um die überarbeitete Formel zu erstellen. | Nein |
