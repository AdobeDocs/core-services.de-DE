---
title: KI in Experience Cloud-Anwendungen
description: Erfahren Sie mehr über generative KI und darüber, wie Experience Cloud-Programme genAI und  [!DNL AI Assistant] verwenden.
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
source-git-commit: d84fcf64b7019f0146340a423e8e20a932cd7874
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 3%

---

# KI in Experience Cloud-Produkten

Auf dieser Seite erfahren Sie, welche Produkte generative KI, [!DNL AI Assistant] unterstützen und ob Adobe Firefly kompatibel ist. Außerdem finden Sie hier Links zu produktspezifischen Hilferessourcen zur Verwendung von KI in Experience Cloud.

**Über generative KI**

Generative KI ist eine Art von künstlicher Intelligenz, die mehr tut, als nur Fragen zu beantworten. Es kann _Inhalte_ und _Antwort generieren_ auf Ihre Fragen oder Aussagen (_Aufforderungen_).

* **Erstellen** Die Möglichkeit, Inhalte (Text, Bilder, Musik oder Videos) von Grund auf basierend auf ihren Schulungs- und Eingabeaufforderungen zu generieren. Diese Fähigkeit ist der _generative_ Aspekt generativer KI.

* **Antwort generieren:** KI bietet eine Antwort oder Reaktion auf eine Eingabeaufforderung, wobei in der Regel die verfügbaren Daten und Wissens-Repositorys genutzt werden.

**Was ist [!DNL AI Assistant]?**

[!DNL AI Assistant] ist ein Konversationstool, das in Experience Platform und verwandten Programmen unterstützt wird. Nutzen Sie sie, um schnell _Produktwissen_ zu gewinnen und in unterstützten Anwendungen _operative Erkenntnisse_ beinahe sofort zu gewinnen.

* **Produktwissen:** Produktwissen bezieht sich auf Konzepte und Themen, die auf der Dokumentation zu Experience League basieren. Die Antworten von Experience League sind überprüfbar und mit Links versehen. Erfahren Sie mehr über die Arten [ (objektbasierten ](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home)), um [!DNL AI Assistant] optimal zu nutzen.

* **Operative Einblicke:** Operative Einblicke beziehen sich auf Antworten, die der KI-Assistent zu Ihren Metadatenobjekten (Attributen, Zielgruppen, Datenflüssen, Datensätzen, Zielen, Journey, Schemata und Quellen) generiert, einschließlich Zählungen, Suchen und Auswirkungen auf die Herkunft. Mit dem KI-Assistenten können Sie operative Einblicke in Sekunden anstatt in Stunden erhalten.

[Weitere Informationen](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing)

<!-- **Your data remains yours**

In AI Assistant, security is the priority:

* Customer data is not used to train language models.
* AI Assistant looks at only the documents that you tell it to. You are in control.
* Your people can use AI Assistant only on documents they can access.
* It's audit-ready: Responses are attributable to source documents.
* Enterprise controls are in place to manage who has AI access in the company.
 -->

## KI-Verfügbarkeit in Experience Cloud-Produkten

Erfahren Sie mehr über die Unterstützung für generative KI oder [!DNL AI Assistant] in Experience Cloud-Produkten. Unterstützung für Adobe Firefly ist ebenfalls angezeigt.

* [[!DNL GenStudio for Performance Marketing]](#gspm)
* [[!DNL Experience Manager Sites]](#aem-sites)
* [[!DNL Journey Optimizer]](#journey-optimizer)
* [[!DNL Journey Optimizer] B2B edition](#ajo-b2b)
* [[!DNL Campaign] Managed Cloud Services](#campaign-cs)
* [[!DNL Customer Journey Analytics]](#cja)
* [[!DNL Customer Journey Analytics]](#cja-captions)
* [[!DNL Real-Time CDP]](#rtcdp)
* [[!DNL Marketo]](#marketo)
* [[!DNL Workfront]](#workfront)

## Adobe GenStudio for Performance Marketing {#gspm}

[!DNL GenStudio for Performance Marketing] ist eine KI-gesteuerte Plattform, mit der Sie Marketing-Inhalte generieren und verwalten können, die Ihren Markenstandards entsprechen und Ihren Unternehmensrichtlinien entsprechen. Generieren von Inhalten für E-Mails, Meta-Anzeigen, LinkedIn-Anzeigen, Display-Anzeigen und Banner.

Sie können GenStudio for Performance Marketing auch in Ihrer Markendarstellung schulen, indem Sie Beispiele, Beschreibungen von Kundenrollen und -produkten sowie Markenrichtlinien verwenden.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home)

Kompatibilität mit Adobe Firefly: **Ja**

## Adobe [!DNL Experience Manager Sites] {#aem-sites}

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

[Erfahren Sie mehr über „Varianten generieren“](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations-integrated-editor)

Kompatibilität mit Adobe Firefly: **Ja**

## Adobe [!DNL Journey Optimizer] {#journey-optimizer}

In [!DNL Journey Optimizer] (AJO) können Sie [KI-](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant)) verwenden, um _Produktwissen_ und _operative Erkenntnisse_ (Beta) zu erhalten.

### Beispiele für die Verwendung des KI-Assistenten in AJO

Im Folgenden finden Sie eine Beispieleingabe für Produktkenntnisse:

* _Wie viele Live-Aktivitäten kann ich in einer Journey Optimizer-Sandbox haben?_

  Die Ausgabe wird aus Experience League und anderen Adobe-Datenspeichern generiert.

Im Folgenden finden Sie eine Beispieleingabe für operative Einblicke:

* _Wie viele Journey wurden in den letzten sieben Tagen erstellt?_

  Für die Ausgabe fragt der KI-Assistent einen kundenspezifischen Datenspeicher ab. Der Datenspeicher enthält zentralisierte, betriebliche Daten zu [!UICONTROL Journey]. Diese Funktion ist kundenunabhängig und ruft Metadaten nur aus Geschäftsobjekten ab. Es greift nicht auf Daten in Ihrer Sandbox zu.

[Weitere Informationen](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant).

Kompatibilität mit Adobe Firefly: **Nein**

### KI-Assistent für die Inhaltserstellung (AJO Prime und Ultimate) {#ajo-prime}

In AJO _Prime_ und _Ultimate_ können Sie die [Inhaltserstellung](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) für die Inhaltserstellung verwenden, um proaktive Inhaltsvariantenvorschläge für Text und Bilder einzubringen.

Diese Funktion ist für E-Mail-, Push-Benachrichtigungen, Web-Seiten-, Inhalts- und SMS-Kanäle verfügbar. Es bietet eine sofortige Text- und Bildgenerierung. Ausgabe aus der Inhaltserstellung in AJO Prime und Ultimate wird entschädigt.

[Weitere Informationen](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)

Kompatibilität mit Adobe Firefly: **Ja**

## [!DNL Journey Optimizer B2B Edition] {#ajo-b2b}

Journey Optimizer B2B edition verwendet [!DNL AI Assistant], um Sie mit Produktkenntnissen vertraut zu machen.

Beispieleingabe:

* _Wie sende ich eine E-Mail auf einer Konto-Journey?_

  Die Ausgabe des Produktwissens wird von Experience League abgerufen.

[Weitere Informationen](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)

Kompatibilität mit Adobe Firefly: **Nein**

## [!DNL Campaign] Managed Cloud Services {#campaign-cs}

Campaign Managed Cloud Services verwendet [!DNL AI Assistant] für die Inhaltserstellung. Mit dieser Funktion können Sie basierend auf Ihrem Marketing-Ziel automatisch personalisierte, ansprechende und effektive Inhalte generieren, wobei Inhalte für Markenstile, Layouts, Ton und mehr optimiert sind. Sie können sie über Kanäle wie E-Mail, SMS und Push-Benachrichtigungen verwenden.

**Hinweis** Die Ausgabe von Inhalten aus der Inhaltserstellung in Campaign Managed Cloud Services wird entschädigt.

[Weitere Informationen](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs)

Kompatibilität mit Adobe Firefly: **Ja**

## [!DNL Customer Journey Analytics] {#cja}

Customer Journey Analytics verwendet [!DNL AI Assistant], um Sie beim Auffinden von Produktkenntnissen und Einblicken aus Experience League zu unterstützen.

Wenn Sie neu sind, lernen Sie schnell Customer Journey Analytics-Konzepte kennen und machen Sie sich mit Produkten und Funktionen vertraut. z. B.:

* _Wie sende ich eine E-Mail auf einer Konto-Journey?_

Erfahrene Anwender erhalten erweiterte Anwendungsfälle oder lernen Strategien kennen, um Aufgaben schnell auszuführen. Sie können Konzepte schnell verstehen, Probleme beheben oder nach Informationen suchen.

[Weitere Informationen](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant)

Kompatibilität mit Adobe Firefly: **Nein**

## [!DNL Customer Journey Analytics] {#cja-captions}

Sie können _Intelligent Captions_ in [!DNL Customer Journey Analytics] verwenden, um Erkenntnisse in natürlicher Sprache für die am häufigsten verwendeten Workspace-Visualisierungen zu erhalten. Intelligente Untertitel sind ideal für Analysten, die Erzählungen und Kontext benötigen, um sie mit anderen Benutzern zu teilen. Business-Anwender können sie verwenden, um schnell allgemeine Erkenntnisse zu gewinnen.

z. B.:

* **Eingabe** Führen Sie in CJA eine unterstützte Visualisierung aus (einschließlich Linie, Bereich, Balkendiagramm, Fluss oder Fallout) und klicken Sie dann auf **[!UICONTROL Intelligente Beschriftungen]**.

* **Ausgabe:** automatisch generierte Untertitel in natürlicher Sprache anzeigen, die Kontext und wichtige Erkenntnisse zeigen. Anschließend können Sie Aktionen für die generierten Daten durchführen, z. B. sie überprüfen, kopieren und für Ihr Unternehmen freigeben. [Siehe wie](https://video.tv.adobe.com/v/3420131/?quality=12&learn=on#_blank)

[Weitere Informationen](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions)

Kompatibilität mit Adobe Firefly: **Nein**

## [!DNL Real-Time CDP] {#rtcdp}

Real-Time CDP verwendet [!DNL AI Assistant], um Sie mit den Produktkenntnissen aus Experience League zu unterstützen. Es bietet auch operative Einblicke (in der Beta-Phase). [!DNL AI Assistant] Abfragen sind kundenspezifische operative Insights-Datenspeicher, die zentralisierte Betriebsdaten enthalten, die in Ihrer AEP-Sandbox partitioniert sind. Das System ruft Metadaten nur aus Attributen, Zielgruppen, Datenflüssen, Datensätzen, Zielen, Schemas und Quellen ab und greift nicht auf Daten innerhalb der Sandbox zu.

Wenn Sie beispielsweise eine Zielgruppe abfragen, können [!DNL AI Assistant] auf den Namen der Zielgruppe und andere zugehörige Metadaten zugreifen, jedoch nicht auf die Profile innerhalb dieser Zielgruppe.

[Weitere Informationen](https://experienceleague.adobe.com/de/docs/experience-platform/ai-assistant/home)

Kompatibilität mit Adobe Firefly: **Nein**

## [!DNL Marketo] {#marketo}

Die Generative AI-gestützten Funktionen in Adobe Dynamic Chat ermöglichen es Ihnen, die Produktivität Ihrer Vertriebsmitarbeiter zu optimieren, Einblicke in die Besucherabsichten Ihrer Website zu erhalten und Besucherfragen sicher zu beantworten. Sie können die Fragen, Antworten und die Konversationszusammenfassung vorab genehmigen.

[Weitere Informationen](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

Kompatibilität mit Adobe Firefly: **Nein**

## [!DNL Workfront] {#workfront}

[!DNL AI Assistant] in [!DNL Workfront] hilft Ihnen, Ihre Arbeit zu erledigen, indem Sie In-App-Informationen und -Vorschläge anbieten. Sie haben folgende Möglichkeiten:

* Sie erhalten Zusammenfassungen einiger Objekte, sodass Sie einen allgemeinen Überblick über den Zweck oder die Details des Objekts erhalten.
* Stellen Sie Fragen und lassen Sie [!DNL AI Assistant] Antworten auf Experience League finden.
* Generierte Formeln basierend auf Ihren Eingabeaufforderungen abrufen. Sie können auch Fehler in Ihren ungültigen benutzerdefinierten Ausdrücken in berechneten Feldern beheben.
* Suchen Sie Projekte, Aufgaben und Probleme.

[Weitere Informationen](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

Kompatibilität mit Adobe Firefly: **Nein**
