---
title: KI in Experience Cloud-Anwendungen
description: Erfahren Sie mehr über generative KI (GenAI) und wie Experience Cloud Anwendungen GenAI verwenden und [!DNL AI Assistant].
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: 47d3a948511714ea0ce682c205eb29118d36ce62
workflow-type: tm+mt
source-wordcount: '1421'
ht-degree: 3%

---

# Generative KI in Experience Cloud Produkten

Auf dieser Seite erfahren Sie, welche Produkte generative KI (GenAI) [!DNL AI Assistant]unterstützen und ob Adobe Systems Firefly kompatibel ist. Außerdem finden Sie Links zu Informationen über die verschiedenen Möglichkeiten, wie Sie KI in Experience Cloud Anwendungen einsetzen können.

**Über generative KI**

Generative KI ist eine Art von künstlicher Intelligenz, die mehr tut, als nur Fragen zu beantworten. Es kann _Inhalte_ und _Antwort generieren_ auf Ihre Fragen oder Aussagen (_Aufforderungen_).

* **Erstellen:** Die Möglichkeit, Inhalte (Text, Bilder, Musik oder Videos) basierend auf den Training und Eingabeaufforderungen von Grund auf neu zu generieren. Diese Fähigkeit ist der _generative_ Aspekt der generativen KI.

* **Generieren Sie eine Antwort:** KI liefert eine Antwort oder Reaktion auf eine Eingabeaufforderung und stützt sich dabei in der Regel auf ihre verfügbaren Daten und Wissensbestände.

**Was ist [!DNL AI Assistant]?**

[!DNL AI Assistant] ist eine dialogorientierte Tool, die in Experience Platform und verwandten Anwendungen unterstützt wird. Nutzen Sie es, um schnell Produktwissen _und, bei unterstützten Produkten,_ fast sofort betriebliche Einblicke zu gewinnen __.

* **Produktkenntnisse:** Produktkenntnisse beziehen sich auf Konzepte und Themen, die auf der Dokumentation zu Experience League basieren. Erfahren Sie, wie Sie effektive[objektbasierte Eingabeaufforderungen“ erstellen](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home) um [!DNL AI Assistant] optimal zu nutzen. Alle Antworten von Experience League sind überprüfbar und mit Links versehen.

* **Operative Insights:** [Operative Insights](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/questions#objects-questions) beziehen sich auf generierte Antworten zu Ihren Metadatenobjekten (Attribute, Zielgruppen, Datenflüsse, Datensätze usw.). Mit dem KI-Assistenten können Sie in Sekunden erreichen, was ansonsten Stunden oder Tage dauern könnte.

[Erfahren Sie mehr über den KI-Assistenten](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/landing)

<!-- **Your data remains yours**

In AI Assistant, security is the priority:

* Customer data is not used to train language models.
* AI Assistant looks at only the documents that you tell it to. You are in control.
* Your people can use AI Assistant only on documents they can access.
* It's audit-ready: Responses are attributable to source documents.
* Enterprise controls are in place to manage who has AI access in the company.
 -->

## KI-Verfügbarkeit in Experience Cloud-Produkten

Erfahren Sie, wie die folgenden Experience Cloud-Programme generative KI oder [!DNL AI Assistant] unterstützen. Unterstützung für Adobe Firefly ist ebenfalls angezeigt.

* [[!DNL GenStudio for Performance Marketing]](#gspm)
* [[!DNL Experience Manager]](#aem)
* [[!DNL Journey Optimizer]](#journey-optimizer)
* [[!DNL Journey Optimizer] B2B edition](#ajo-b2b)
* [[!DNL Campaign] Managed Cloud Services](#campaign-cs)
* [[!DNL Customer Journey Analytics]](#cja)
* [[!DNL Real-Time CDP]](#rtcdp)
* [[!DNL Marketo]](#marketo)
* [[!DNL Workfront]](#workfront)

## Adobe GenStudio for Performance Marketing {#gspm}

[!DNL GenStudio for Performance Marketing] ist eine KI-gesteuerte Plattform, mit der Sie Marketing-Inhalte generieren und verwalten können, die Ihren Markenstandards entsprechen und Ihren Unternehmensrichtlinien entsprechen. Generieren von Inhalten für E-Mails, Meta-Anzeigen, LinkedIn-Anzeigen, Display-Anzeigen und Banner.

Sie können GenStudio for Performance Marketing auch in Ihrer Markendarstellung schulen, indem Sie Beispiele, Beschreibungen von Kundenrollen und -produkten sowie Markenrichtlinien verwenden.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home)

Adobe Firefly-Kompatibilität: **Ja**

## Adobe [!DNL Experience Manager] {#aem}

In den folgenden Abschnitten werden generative KI in AEM-Anwendungen kurz beschrieben.

### Experience Manager Sites

In AEM Sites können Sie „Varianten _[!UICONTROL &quot;]_. Diese Funktion verwendet generative künstliche Intelligenz, um Inhaltsvarianten basierend auf Ihren Eingabeaufforderungen zu erstellen. Eingabeaufforderungen werden entweder von Adobe bereitgestellt oder von Ihnen erstellt und verwaltet.

Nachdem Sie Varianten erstellt haben, können Sie den Inhalt auf Ihrer Website verwenden und den Erfolg mithilfe der Funktion [Experimentieren](https://www.aem.live/docs/experimentation) in Edge Delivery Services messen. Sie haben auch die Möglichkeit, Bilder in Adobe Express mithilfe der Generative AI-Funktionen von Firefly zu generieren.

**Ein- und Ausgabebeispiele**

Zu den Eingabefeldern gehören:

* Anzahl der zu erzeugenden Varianten
* Zielgruppen-Source
* Audience-Ziel
* Zusätzlicher Kontext
* Kundengesteuerte Eingabeaufforderungen

Die Ausgabe ist generierter Inhalt oder eine Marktkopie.

Adobe Firefly-Kompatibilität: **Ja**

[Erfahren Sie mehr über „Varianten generieren“](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/generative-ai/generate-variations-integrated-editor)

### Experience Manager Assets

[!UICONTROL Content Hub] ist als Teil der [!DNL Experience Manager Assets as a Cloud Service] für die Demokratisierung des Zugriffs auf markeninterne Inhalte für Unternehmen und ihre Geschäftspartner verfügbar. Der Schwerpunkt liegt auf der Verteilung von Assets für die Aktivierung im großen Maßstab und der Erstellung von Inhaltsvarianten für die Marke, um die Marketing-Agilität zu verbessern.

In Content Hub können Sie Inhalte mit Adobe Express erstellen (wenn Sie über Adobe Express-Berechtigungen verfügen). Sie können vorhandene Inhalte mit einfachen Tools bearbeiten, markeninterne Varianten mit Vorlagen und Markenelementen erstellen und Inhalte mit den neuesten GenAI-Funktionen von [!DNL Adobe Firefly] erstellen.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/content-hub/product-overview)

Adobe Firefly-Kompatibilität: **Ja**

## Adobe [!DNL Journey Optimizer] {#journey-optimizer}

In [!DNL Journey Optimizer] (AJO) können Sie [KI-](https://experienceleague.adobe.com/de/docs/journey-optimizer/using/get-started/ai-assistant)) verwenden, um _Produktwissen_ und _operative Erkenntnisse_ (Beta) zu erhalten.

### Beispiele für die Verwendung des KI-Assistenten in AJO

Im Folgenden finden Sie eine Beispieleingabe für Produktkenntnisse:

* _Wie viele Live-Aktivitäten kann ich in einer Journey Optimizer-Sandbox haben?_

  Die Ausgabe wird aus Experience League und anderen Adobe-Datenspeichern generiert.

Im Folgenden finden Sie eine Beispieleingabe für operative Einblicke:

* _Wie viele Journey wurden in den letzten sieben Tagen erstellt?_

  Für die Ausgabe fragt der KI-Assistent einen kundenspezifischen Datenspeicher ab. Der Datenspeicher enthält zentralisierte, betriebliche Daten zu [!UICONTROL Journey]. Diese Funktion ist kundenunabhängig und ruft Metadaten nur aus Geschäftsobjekten ab. Es greift nicht auf Daten in Ihrer Sandbox zu.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/journey-optimizer/using/get-started/ai-assistant).

Adobe Firefly-Kompatibilität: **Nein**

### KI-Assistent für die Inhalte-Generation (AJO Prime und Ultimate) {#ajo-prime}

In AJO _Prime_ und _Ultimate_ können Sie Inhalte Generierung[&#128279;](https://experienceleague.adobe.com/de/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) für Inhalte Generierung verwenden, um proaktive Inhalte Variationsvorschläge für Text und Bilder zu machen.

Diese Funktion ist für E-Mail, Push-Benachrichtigungen, Web-Seite, Inhalte- und SMS-Kanäle verfügbar. Es bietet eine sofortige Text- und Bildgenerierung. Ausgabe aus der Inhaltserstellung in AJO Prime und Ultimate wird entschädigt.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)

Adobe Firefly-Kompatibilität: **Ja**

## [!DNL Journey Optimizer B2B Edition] {#ajo-b2b}

Journey Optimizer B2B Edition hilft [!DNL AI Assistant] Ihnen mit Produktwissen.

Beispieleingabe:

* _Wie sende ich eine E-Mail in einem Konto Journey?_

  Das Produktwissen stammt aus Experience League.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)

Adobe Firefly-Kompatibilität: **Nein**

## [!DNL Campaign] Managed Cloud Services {#campaign-cs}

Campaign Managed Cloud Services verwendet [!DNL AI Assistant] für die Inhaltserstellung. Mit dieser Funktion können Sie basierend auf Ihrem Marketing-Ziel automatisch personalisierte, ansprechende und effektive Inhalte generieren, wobei Inhalte für Markenstile, Layouts, Ton und mehr optimiert sind. Sie können sie über Kanäle wie E-Mail, SMS und Push-Benachrichtigungen verwenden.

**Hinweis** Die Ausgabe von Inhalten aus der Inhaltserstellung in Campaign Managed Cloud Services wird entschädigt.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/campaign-web/v8/content/ai-assistant/generative-gs)

Adobe Firefly-Kompatibilität: **Ja**

## [!DNL Customer Journey Analytics] {#cja}

Customer Journey Analytics können Sie generative KI auf folgende Weise verwenden:

* [!DNL AI Assistant] für Produktwissen und Einblicke
* [!UICONTROL Intelligente Beschriftungen] in Workspace-Visualisierungen
* KI und GenAI zum automatischen Zuweisen aller Asset-Metadaten in [!DNL Content Analytics]

**KI-Assistent**

Discover Produktwissen und Erkenntnisse von Experience League. Wenn Sie ein neuer User sind, sollten Sie sich schnell Customer Journey Analytics Konzepte vertraut machen und sich mit Produkten und Funktionen vertraut machen. z. B.:

* _Wie sende ich eine E-Mail in einem Konto Journey?_

Erfahrene Benutzer erhalten erweiterte Anwendungsfälle oder erlernen Strategien, um Aufgaben in einem schnellen Tempo auszuführen. Sie können Konzepte schnell verstehen, Probleme beheben oder Informationen suchen.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant)

**Intelligente Beschriftungen**

Sie können _Intelligent Captions_ in [!DNL Customer Journey Analytics] verwenden, um Erkenntnisse in natürlicher Sprache für die am häufigsten verwendeten Workspace-Visualisierungen zu erhalten. Intelligente Untertitel sind ideal für Analysten, die Erzählungen und Kontext benötigen, um sie mit anderen Benutzern zu teilen. Business-Anwender können sie verwenden, um schnell allgemeine Erkenntnisse zu gewinnen.

z. B.:

* **Eingabe** Führen Sie in CJA eine unterstützte Visualisierung aus (einschließlich Linie, Bereich, Balkendiagramm, Fluss oder Fallout) und klicken Sie dann auf **[!UICONTROL Intelligente Beschriftungen]**.

* **Ausgabe:** automatisch generierte Untertitel in natürlicher Sprache anzeigen, die Kontext und wichtige Erkenntnisse zeigen. Anschließend können Sie Aktionen für die generierten Daten durchführen, z. B. sie überprüfen, kopieren und für Ihr Unternehmen freigeben. [Siehe wie](https://video.tv.adobe.com/v/3443147/?quality=12&learn=on#_blank&captions=ger)

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions)

**Content Analytics**

Content Analytics verwendet KI und GenAI, um alle Asset-Metadaten automatisch zuzuweisen, z. B. Themen, Szenen, Vordergrundfarben usw. Ein Attribut ist ein von KI zugewiesenes Metadaten-Tag, das beschreibt, was sich in einem Asset oder Erlebnis befindet.

Beispiel: `color: red` ist ein automatisch zugewiesenes Attribut. Anhand der Visualisierungen können Sie erkennen, welche Attribute Ihrer Assets am meisten zur Konversion beitragen. [Weitere Informationen](https://experienceleague.adobe.com/de/docs/analytics-platform/using/content-analytics/report/report#template)

Adobe Firefly-Kompatibilität: **Nein**

## [!DNL Real-Time CDP] {#rtcdp}

Real-Time CDP verwendet [!DNL AI Assistant], um Sie mit den Produktkenntnissen aus Experience League zu unterstützen. Es bietet auch operative Einblicke (in der Beta-Phase). [!DNL AI Assistant] Abfragen sind kundenspezifische operative Insights-Datenspeicher, die zentralisierte Betriebsdaten enthalten, die in Ihrer AEP-Sandbox partitioniert sind. Das System ruft Metadaten nur aus Attributen, Zielgruppen, Datenflüssen, Datensätzen, Zielen, Schemas und Quellen ab und greift nicht auf Daten innerhalb der Sandbox zu.

Wenn Sie beispielsweise eine Zielgruppe abfragen, können [!DNL AI Assistant] auf den Namen der Zielgruppe und andere zugehörige Metadaten zugreifen, jedoch nicht auf die Profile innerhalb dieser Zielgruppe.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home)

Adobe Firefly-Kompatibilität: **Nein**

## [!DNL Marketo] {#marketo}

In Marketo ist generative KI in interaktiven Webinaren und Dynamic Chat verfügbar.

**Interaktive Webinare**

Automatische Generierung von Kapiteln und Zusammenfassungen für aufgezeichnete Webinare, wodurch die Zugänglichkeit verbessert und die Navigation für Ihre Zielgruppe erleichtert werden. Zu den Funktionen gehören:

* Automatische Kapitelerstellung
* KI-generierte Textzusammenfassung
* Bearbeitbare Inhalte - Ändern von generierten Kapiteln und Zusammenfassungen
* Einfache Integration - Fügen Sie Ihren Landingpages Kapitel und Zusammenfassungen hinzu, indem Sie den HTML-Code in den gewünschten Web-Seiten-Editor kopieren

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/gen-ai)

**Dynamic Chat**

Die Generative AI-gestützten Funktionen in Adobe Dynamic Chat ermöglichen es Ihnen, die Produktivität Ihrer Vertriebsmitarbeiter zu optimieren, Einblicke in die Besucherabsichten Ihrer Website zu erhalten und Besucherfragen sicher zu beantworten. Sie können die Fragen, Antworten und die Konversationszusammenfassung vorab genehmigen.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

Adobe Firefly-Kompatibilität: **Nein**

## [!DNL Workfront] {#workfront}

[!DNL AI Assistant] in [!DNL Workfront] hilft Ihnen bei Ihrer Arbeit, indem es In-App-Informationen und -Vorschläge anbietet. Sie haben folgende Möglichkeiten:

* Erhalten Sie Zusammenfassungen einiger Objekte, um einen allgemeinen Ansicht über die Absicht oder Details des Objekts zu erhalten.
* Stellen Sie Fragen und lassen Sie [!DNL AI Assistant] Antworten auf Experience League finden.
* Generierte Formeln basierend auf Ihren Eingabeaufforderungen abrufen. Sie können auch Fehler in Ihren ungültigen benutzerdefinierten Ausdrücken in berechneten Feldern beheben.
* Suchen Sie Projekte, Aufgaben und Probleme.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

Adobe Firefly-Kompatibilität: **Nein**
