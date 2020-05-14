---
description: Konfigurieren von Experience Cloud Triggers
keywords: integrations;Triggers
seo-description: Konfigurieren von Experience Cloud Triggers
seo-title: Triggers
solution: Marketing Cloud
title: Triggers
uuid: dab536e3-1969-4661-919e-5b15f423fecd
translation-type: tm+mt
source-git-commit: fb03bf89bcc6ed4438daf18c8415de3052ba8fa4
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 44%

---


# Triggers

## Übersicht über Triggers {#topic_4F21FCE9A64E46E8B6D51F494FA652A7}

Auslöser ermöglichen es Ihnen, wichtige Verhaltensweisen von Verbrauchern zu identifizieren, zu definieren und zu überwachen und dann eine lösungsübergreifende Kommunikation zu generieren, um Besucher erneut zu interagieren. Sie können Auslöser bei Entscheidungen und Personalisierung in Echtzeit verwenden.

* Schnelles Remarketing für Warenkorbabbrüche oder Warenkorbabbrüche mit entfernten Produkten konfigurieren
* Unvollständige Formulare und Anwendungen
* Aktionen oder Abfolgen von Aktionen auf der Site

![](assets/trigger-abandonment-2.png)

### Triggers-typen

Im Allgemeinen kann ein Auslöser 15 bis 90 Minuten benötigen, um eine Marketing-Kampagne zu starten. Dies hängt von der Implementierung der Datenerfassung, der Auslastung der Pipeline, der benutzerdefinierten Konfiguration des definierten Triggers und dem Workflow in Adobe Campaign ab.

* **Abbruch:** Sie können einen Auslöser für den Fall erstellen, dass ein Besucher ein Produkt anzeigt, es jedoch nicht zum Warenkorb hinzufügt.
* **Aktion:** Sie können Auslöser erstellen, die z. B. nach der Newsletter-Anmeldung, E-Mail-Abonnements oder Kreditkartenanträgen (Bestätigungen) ausgelöst werden. Wenn Sie ein Händler sind, können Sie einen Auslöser für einen Besucher erstellen, der sich für ein Treueprogramm anmeldet. Erstellen Sie in Medien und Unterhaltung Auslöser für Besucher, die eine bestimmte Sendung ansehen, und vielleicht möchten Sie mit einer Umfrage reagieren.
* **Sitzungs-Beginn und Sitzungsende:** Erstellen Sie einen Auslöser für die Ereignis zum Sitzungsende und Beginn zum Sitzungsende.

## Experience Cloud Trigger erstellen {#task_821F37183AC045E5AC8EED20317598FE}

Erstellen Sie einen Auslöser und konfigurieren Sie die Bedingungen für den Auslöser. Sie können beispielsweise die Kriterien für die Regeln eines Auslösers während eines Besuchs angeben, z. B. Metriken wie Warenkorbabbruch oder Dimensionen wie den Produktnamen. Wenn die Regeln erfüllt sind, wird der Auslöser ausgeführt.

>[!NOTE]
>
>Derzeit existiert eine technische Begrenzung von 100 Triggern.

1. In the Experience Cloud, click ![](assets/menu-icon.png), then click **[!UICONTROL Launch]**.
2. Locate the [!UICONTROL Triggers] card, then click **[!UICONTROL Manage Triggers]**.
3. Klicken Sie auf **[!UICONTROL Neuer Trigger]** und geben Sie dann den Trigger-Typ an:

   ![Schritt Ergebnis](assets/add-trigger.png)

4. Konfigurieren Sie den Auslöser, indem Sie die folgenden Felder vervollständigen und Metrik- und Dimensionselemente in die Regelbehälter ziehen:

   | Element | Beschreibung |
   |--- |--- |
   | Name | Der Anzeigename für diesen Auslöser. |
   | Beschreibung | Die Beschreibung dieses Auslösers, wie Sie ihn verwenden werden usw. |
   | Report Suite | Die für diesen Auslöser verwendete Analytics- [Report Suite](https://docs.adobe.com/content/help/de-DE/analytics/implementation/analytics-basics/ref-reports-report-suites.html) . Diese Einstellung identifiziert die zu verwendenden Berichte-Daten. |
   | Visit must include<br>Visit must not include<br>Trigger after no action<br>Include meta data | Sie können Kriterien oder Besucherverhalten, das auftreten soll, sowie Verhalten, das nicht auftreten soll, definieren.  Regeln für einen einfachen Warenkorbabbruchsauslöser können beispielsweise die folgenden sein:<ul><li>Besuch muss Folgendes beinhalten: „Zusatz zum Warenkorb“ (Metrik) und „Vorhanden“. (Sie können die Regel mit einer bestimmten Produktansicht oder mit Dimensionen wie „Browsertypen“ weiter verfeinern.)</li><li>Besuch darf Folgendes nicht beinhalten: Checkout.</li><li>Auslöser nach ausbleibender Aktion bei: 10 Minuten.</li><li>Metadaten einschließen: Sie können eine bestimmte Kampagnendimension oder Variablen, die für das Verhalten eines Besuchers relevant sind, hinzufügen. Dieses Feld kann für Adobe Campaign zum Verfassen der richtigen Remarketing-E-Mail nützlich sein.</li></ul><br>Sie können eine Beliebige-, Und- oder Oder-Logik innerhalb oder zwischen Behältern angeben, je nachdem, welche Kriterien Sie für die Regel für wichtig halten. |
   | Container | Container sind der Ort, an dem Sie Regeln, Bedingungen oder Filter festlegen und speichern, die einen Auslöser definieren. Wenn Sie möchten, dass Ereignis gleichzeitig auftreten, setzen Sie sie in denselben Container. Dies bedeutet, dass jeder Behälter unabhängig auf der Trefferebene arbeitet.  Wenn Sie beispielsweise zwei Behälter mit dem Operator „Und“ verbinden, treffen die Regeln zu, wenn zwei Treffer die Anforderungen erfüllen. |
   | Beginn neue Sitzung nach | Erstellen Sie einen Auslöser für die Ereignis zum Sitzungsende und Beginn zum Sitzungsende. |

5. Klicken Sie auf **[!UICONTROL Speichern]**.
6. Use triggers for [real-time remarketing](https://docs.campaign.adobe.com/doc/standard/en/EMA_Transactional_messaging_Marketing_Cloud_Triggers.html) in [!DNL Adobe Campaign].

### Beispielauslöser

Beispiele für Experience Cloud-Auslöser:

#### Warenkorbabbruchsauslöser

Die folgende Seite zeigt beispielsweise Regeln, die Sie für einen Auslöser für den Warenkorbabbruch verwenden können, basierend auf Produkten, die während eines Besuchs angesehen wurden.

![](assets/abandonment-trigger.png)

#### Werber-Auslöser

Der folgende Auslöser wird ausgelöst, wenn ein Treffer mit dem Produkt Herrenstiefel und Werber von Facebook eingeht. For the two criteria (*products* and *referrer*) to be evaluated in the same hit, they should be added to the same container.

![](assets/fb-boots-promo.png)
