---
description: Erfahren Sie, wie Sie Abonnements in  [!DNL Customer Attributes]  für Analytics und Target konfigurieren und eine Datenquelle aktivieren.
solution: Experience Cloud
title: Konfigurieren von Abonnements in [!DNL Customer Attributes]
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: cfa2aa5c-337f-401e-80eb-cbe36cb1d41e
source-git-commit: 21120abb5ab0fcc8d556012851548f39f3875038
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 61%

---

# Konfigurieren von Abonnements und Aktivieren der Datenquelle

[!DNL Customer Attributes]-Abonnements ermöglichen den Datenfluss von Kundenattributen zwischen Experience Cloud und Programmen ([!DNL Analytics] und [!DNL Target]).

Ein Adobe Analytics-Abonnement ermöglicht beispielsweise Attributdaten in Berichten. Wenn Sie [!DNL Adobe Target] verwenden, können Sie Kundenattribute für Targeting und Segmentierung hochladen.

**So konfigurieren Sie Abonnements und aktivieren die Datenquelle**

1. Suchen Sie Ihre Datenquelle in [!DNL Customer Attributes] zur Bearbeitung:

   Klicken Sie [!DNL Experience Cloud] auf **[!UICONTROL Apps]** ![menu](assets/menu-icon.png) > **[!DNL Customer Attributes]**.

1. Klicken [!UICONTROL  unter „Kundenattribut-Source bearbeiten] auf **[!UICONTROL Datei-Upload]**.

1. Klicken Sie **[!UICONTROL Abonnements konfigurieren]**.

   ![Konfigurieren von Abonnements in Experience Cloud](assets/configure-subscriptions.png)

1. Um die Kundenattributquelle zu aktivieren, klicken Sie auf **[!UICONTROL Aktiv]** und anschließend auf **[!UICONTROL Speichern]**.

1. Um ein Abonnement für [!DNL Analytics] oder [!DNL Target] zu konfigurieren, klicken Sie auf **[!UICONTROL Konfigurieren]**.

   Das folgende Beispiel zeigt ein [!DNL Target]-Abonnement:

   ![Ergebnis des Schritts](assets/subscription-target.png)

   | Element | Beschreibung |
   |--- |--- |
   | Lösung | **Adobe Analytics**<br> Wählen Sie [!DNL Analytics] aus, geben Sie die Report Suites an, für die Sie Attributdaten empfangen möchten, und die einzuschließenden Attribute.<br>**Adobe Target**<br> Sie können Kundenattribute für Targeting und die Segmentierung hochladen. Diese Funktion ist nützlich, wenn Sie einen Test auf der Grundlage von Attributdaten durchführen möchten oder die Daten für die Segmentierung in Analytics zur Verfügung stellen möchten.<br>Hochgeladene Kundenattributdaten für einen Besucher sind bei der Anmeldung in **[!DNL Target]** > **Zielgruppen** verfügbar.<br>Es werden mehrere Datenquellen unterstützt. Wenn Sie Kunden-IDs auf Ihrer Website festlegen, stellen Sie sicher, dass mindestens einer der Aliase [!DNL Target] abonniert ist. |
   | Report Suite (Adobe Analytics) | Die Report Suites von Analytics.<br>Innerhalb einer Attributquelle können Sie dem Analytics-Abonnement maximal zehn Report Suites hinzufügen. Berücksichtigen Sie bei der Auswahl der einzuschließenden Report Suites die folgenden Vorschläge:<ul><li>Wählen Sie Report Suites mit einem gemeinsamen Satz authentifizierter Kunden aus. Wenn sich die authentifizierten Kunden in einer Report Suite nicht mit den authentifizierten Kunden in einer anderen Report Suite überschneiden, teilen Sie diese Report Suites in verschiedene Attributquellen auf.</li><li>Wenn möglich, sollten die Report Suites, die in einer Attributquelle enthalten sind, ein ähnliches Traffic-Volumen aufweisen.</li></ul><br>Falls Sie mehr als zehn Report Suites mit dem gleichen Satz authentifizierter Kunden haben, konfigurieren Sie weitere Kundenattributquellen mit jeweils bis zu zehn Report Suites. |
   | Einzuschließende Attribute (Analytics und [!DNL Target]) | Die Attribute, die Sie an das Programm senden möchten. <br>Bei der Konfiguration von Abonnements und der Auswahl von Attributen gelten – je nachdem, welche Programme Sie besitzen – die folgenden Einschränkungen _pro Report Suite_:<ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: 3 insgesamt</li><li>Premium: 200 pro Report Suite</li><li>[!DNL Target] Standard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Hinweis:** Bei einem Upgrade auf Analytics Premium dauert es 24 Stunden, bis weitere Attribute verfügbar sind. Während dieser Verzögerung wird möglicherweise ein Fehler „Attribut Max. Abonnement“ angezeigt. |

1. Klicken Sie auf **[!UICONTROL Speichern]**.
