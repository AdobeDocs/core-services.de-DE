---
description: Konfigurieren von Experience Cloud Triggers
keywords: integrations;Triggers
seo-description: Konfigurieren von Experience Cloud Triggers
seo-title: Triggers
solution: Marketing Cloud
title: Triggers
uuid: dab536e3-1969-4661-919e-5b15f423fecd
translation-type: tm+mt
source-git-commit: ae97db27349940a8df7ee2ba6678683f57585678

---


# Triggers

## Übersicht über Triggers {#topic_4F21FCE9A64E46E8B6D51F494FA652A7}

*Triggers* ermöglicht es Ihnen, wichtige Verbraucherverhaltensweisen zu identifizieren, zu definieren und zu überwachen sowie lösungsübergreifende Kommunikationen zu generieren, um erneut mit Besuchern zu interagieren. Sie können Auslöser für Entscheidungen und Personalisierung in Echtzeit verwenden.

* Konfigurieren Sie schnelles Remarketing für Warenkorbabbrüche oder Warenkorbabbrüche mit entfernten Produkten
* Unvollständige Formulare und Anwendungen
* Jede Aktion oder Abfolge von Aktionen auf der Site

![](assets/trigger-abandonment-2.png)

**Triggers-typen**

Im Allgemeinen kann ein Auslöser 15 bis 90 Minuten benötigen, um eine Marketing-Kampagne zu starten. Dies hängt von der Implementierung der Datenerfassung, der Auslastung der Pipeline, der benutzerdefinierten Konfiguration des definierten Triggers und dem Workflow in Adobe Campaign ab.

* **Abbruch:** Sie können einen Auslöser für den Fall erstellen, dass ein Besucher ein Produkt anzeigt, es jedoch nicht zum Warenkorb hinzufügt. Konfigurieren Sie die [Tendenzauswertung](../activation/triggers.md#concept_A506150674AD45DB98D3CC07E560D334), um die Tendenz von Kunden zu verstehen, einen Einkauf abzubrechen.
* **Aktion:** Sie können Auslöser erstellen, der z. B. ausgelöst wird, nachdem ein Benutzer sich für einen Newsletter angemeldet, E-Mails abonniert oder eine Kreditkarte beantragt hat (Bestätigungen). Wenn Sie Einzelhändler sind, können Sie einen Auslöser für einen Besucher erstellen, der sich für ein Treueprogramm anmeldet. Erstellen Sie im Bereich Medien und Unterhaltung Auslöser für Besucher, die eine bestimmte Sendung ansehen. Vielleicht möchten Sie auch mit einer Umfrage antworten.
* **Sitzungsbeginn und Sitzungsende:** Erstellen Sie einen Auslöser für die Ereignisse „Sitzungsbeginn“ und „Sitzungsende“.

## Experience Cloud Trigger erstellen {#task_821F37183AC045E5AC8EED20317598FE}

Erstellen Sie einen Abbruchsauslöser und konfigurieren Sie die Bedingungen für den Auslöser und die Tendenzauswertung. Sie können beispielsweise die Kriterien für die Regeln eines Auslösers während eines Besuchs festlegen – etwa Metriken wie „Warenkorbabbruch“ oder Dimensionen wie den Produktnamen. Wenn die Regeln erfüllt sind, wird der Auslöser ausgeführt.

<!-- t_create-trigger.xml -->

>[!NOTE]
>
>Derzeit existiert eine technische Begrenzung von 100 Triggern.

1. Klicken Sie in der Experience Cloud auf ![](assets/menu-icon.png) und dann auf **[!UICONTROL Activation]**.
1. Klicken Sie in der Registerkarte [!UICONTROL Triggers] auf **[!UICONTROL Starten]**.

   ![Schritt Ergebnis](assets/activation-triggers.png)

1. Klicken Sie auf **[!UICONTROL Neuer Trigger]** und geben Sie dann den Trigger-Typ an:

   ![Schritt Ergebnis](assets/add-trigger.png)

1. Konfigurieren Sie den Auslöser, indem Sie die folgenden Felder vervollständigen und Metrik- und Dimensionselemente in die Regelbehälter ziehen:

   | Element | Beschreibung |
   |--- |--- |
   | Name | Der Anzeigename für diesen Auslöser. |
   | Beschreibung | Die Beschreibung dieses Auslösers, seine Verwendung usw. |
   | Report Suite | Die für diesen Auslöser verwendete Analytics-[Report Suite](https://docs.adobe.com/content/help/en/analytics/implementation/analytics-basics/ref-reports-report-suites.html). Diese Einstellung gibt die zu verwendenden Berichtsdaten an. |
   | Besuch muss beinhalten<br>Besuch darf nicht beinhalten<br>Auslöser nach ausbleibender Aktion<br> Metadaten einschließen | Sie können Kriterien oder Besucherverhalten, das auftreten soll, sowie Verhalten, das nicht auftreten soll, definieren.  Regeln für einen einfachen Warenkorbabbruchsauslöser können beispielsweise die folgenden sein:<ul><li>Besuch muss Folgendes beinhalten: „Zusatz zum Warenkorb“ (Metrik) und „Vorhanden“. (Sie können die Regel mit einer bestimmten Produktansicht oder mit Dimensionen wie „Browsertypen“ weiter verfeinern.)</li><li>Besuch darf Folgendes nicht beinhalten: Checkout.</li><li>Auslöser nach ausbleibender Aktion bei: 10 Minuten.</li><li>Metadaten einschließen: Sie können eine bestimmte Kampagnendimension oder Variablen, die für das Verhalten eines Besuchers relevant sind, hinzufügen. Dieses Feld kann für Adobe Campaign zum Verfassen der richtigen Remarketing-E-Mail nützlich sein.</li></ul><br>Sie können eine Beliebige-, Und- oder Oder-Logik innerhalb oder zwischen Behältern angeben, je nachdem, welche Kriterien Sie für die Regel für wichtig halten. |
   | Behälter | Behälter sind der Ort, an dem Sie Regeln, Bedingungen oder Filter zur Definition eines Auslösers festlegen und speichern. Wenn Ereignisse gleichzeitig eintreten sollen, speichern Sie sie in demselben Behälter. Dies bedeutet, dass jeder Behälter unabhängig auf der Trefferebene arbeitet.  Wenn Sie beispielsweise zwei Behälter mit dem Operator „Und“ verbinden, treffen die Regeln zu, wenn zwei Treffer die Anforderungen erfüllen. |
   | Neue Sitzung beginnen nach | Erstellen Sie einen Auslöser für den Beginn und das Ende von Sitzungsereignissen. |

1. (Optional) Bei Abbruchs-Triggern können Sie die [Tendenzauswertung](../activation/triggers.md#concept_A506150674AD45DB98D3CC07E560D334) anwenden.

   ![Schritt Ergebnis](assets/propensity-scoring.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. Use triggers for [real-time remarketing](https://docs.campaign.adobe.com/doc/standard/en/EMA_Transactional_messaging_Marketing_Cloud_Triggers.html) in [!DNL Adobe Campaign].

### Beispielauslöser

**Warenkorbabbruchsauslöser**

Auf der folgenden Seite finden Sie Regeln, die Sie für einen Warenkorbabbruchsauslöser verwenden könnten, die auf Produkten basieren, die während eines Besuchs angesehen wurden.

![](assets/abandonment-trigger.png)

**Verweisauslöser**

Der folgende Auslöser wird ausgelöst, wenn für das Produkt „Herrenstiefel“ ein Treffer mit Verweis auf Facebook eingeht. Damit die beiden Kriterien ( *Produkte* und *Referrer*) im selben Treffer bewertet werden, sollten sie demselben Behälter hinzugefügt werden.

![](assets/fb-boots-promo.png)

## Tendenzauswertung {#concept_A506150674AD45DB98D3CC07E560D334}

<!-- propensity-scoring.xml -->

Verstehen Sie die Tendenz der Kunden, nach dem Abbruch eines Warenkorbs zurückzukehren. Die Tendenzauswertung ist in Experience Cloud Triggers integriert und für Abbruchsauslöser verfügbar.

![Schritt Ergebnis](assets/propensity-scoring.png)

Einige Kunden brechen beispielsweise Warenkörbe ab, um von den Vorteilen von E-Mail-Anreizen zum Zurückkehren zum Warenkorb zu profitieren. Um den Einkommensverlust zu reduzieren, werden mithilfe des Tendenzauswertungsalgorithmus diejenigen Warenkorbabbrecher identifiziert, die ohne den Anreiz wahrscheinlich nicht zurückkehren würden.

Sie haben folgende Möglichkeiten:

* Verhindern, dass Ihre Kunden Remarketing übermäßig stark ausgesetzt sind.
* Die richtigen Kunden, die ihren Warenkorb abgebrochen haben, identifizieren und ihre Aktivität der richtigen Meldung zuordnen.
* Ihren Umsatz steigern – durch Wissen darüber, welche Kunden zurückkehren werden und welche nicht.

## Vorteile der Tendenzauswertung  {#section_CA99874A25434CC0BF01D0DA61608889}

Sie können von Datenerkennung Gebrauch machen, um verstecktes Verhalten oder Muster, die über Ihre Daten hinweg vorhanden sind, zu erkennen. Die Tendenzauswertung kann Ihnen durch eine fokussiertere und objektivere Herangehensweise anstelle einer einfachen Segmentierung oder Filterung insbesondere bei der Erkennung von Clustern ähnlicher Kunden helfen. Darüber hinaus können Sie mithilfe der Tendenzauswertung vorausschauende Funktionen zur Erkennung des Verhaltens eines für Ihr Unternehmen bedeutenden Kunden einrichten.

Sobald Sie die bedeutendste Zielgruppe ermittelt haben, können Sie sie zur effektivsten Interaktion bewegen. Wenn Sie beispielsweise ein Business-to-Business-Unternehmen sind, haben Sie möglicherweise Leads für Verkaufsanrufe, anhand derer Sie dann die Leads bewerten und die Wahrscheinlichkeit von späteren Offline-Konversionen bestimmen können. Da durch jeden Lead die Kosten steigen, ist das Erstellen eines Anreizes zur Ermittlung potenzieller Kunden mit der größter Wahrscheinlichkeit für die Konversion eines Verkaufs die effektivste und günstige Möglichkeit zur Konzentration Ihrer Ressourcen.

Mithilfe der Tendenzauswertung können die Faktoren, die eine bestimmte Tendenz am besten erahnen lassen, identifiziert oder die Wahrscheinlichkeit, dass ein Ereignis eintritt, erhöht werden. Darüber hinaus kann die Tendenzauswertung auch für die Beantwortung konkreter Fragen angewendet werden:

* Wird es beim Kunden zu einer Konversion kommen?
* Wird der Kunde eine E-Mail beantworten?
* Wird der Kunde erneut kaufen?

Mithilfe der Tendenzauswertung können Sie diese Fragen beantworten und Besucher mit einer Tendenz zu einer Handlung identifizieren, die dann ausgelöst und bewertet werden kann.
