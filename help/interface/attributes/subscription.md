---
description: Erfahren Sie mehr über Lösungsdatenquellen und das Konfigurieren von Abonnements. Abonnement ermöglichen den Datenfluss von Kundenattributen zwischen Experience Cloud und Lösungen (Analytics und Zielgruppe).
keywords: Customer Attributes;core services
seo-description: Erfahren Sie mehr über Lösungsdatenquellen und das Konfigurieren von Abonnements. Abonnement ermöglichen den Datenfluss von Kundenattributen zwischen Experience Cloud und Lösungen (Analytics und Zielgruppe).
seo-title: Konfigurieren von Abonnements
solution: Experience Cloud
title: Konfigurieren von Abonnements
uuid: f74a8155-0a21-46b3-9b1e-4c838f72f24f
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 39%

---


# Konfigurieren von Abonnements

Erfahren Sie mehr über Lösungsdatenquellen und das Konfigurieren von Abonnements. Abonnement ermöglichen den Datenfluss von Kundenattributen zwischen Experience Cloud und Lösungen (Analytics und [!DNL Target]).

Ein Adobe Analytics-Abonnement aktiviert beispielsweise Attributdaten in Berichten. Wenn Sie Adobe Zielgruppe verwenden, können Sie Kundenattribute für Targeting und Segmentierung hochladen.

**[!UICONTROL Kunden-Attributquelle]** > **[!UICONTROL Neue Kunden-Attributquelle]** erstellen > **[!UICONTROL Neu]**

![](assets/configure_subscription_page.png)

| Element | Beschreibung |
|--- |--- |
| Lösung | **Adobe Analytics **<br>Wählen Sie Analytics und die Report Suites aus, die Attributdaten erhalten sollen, sowie die einzuschließenden Attribute.<br>**Adobe**<br>TargetSie können Kundenattribute für Targeting und Segmentierung hochladen. Diese Funktion ist nützlich, wenn Sie einen Test auf der Grundlage von Attributdaten durchführen möchten oder die Daten für die Segmentierung in Analytics zur Verfügung stellen möchten.<br>Hochgeladene Kundenattributdaten für einen Besucher stehen bei der Anmeldung unter **[!DNL Target]**>** Audiencen **zur Verfügung.<br>Es werden mehrere Datenquellen unterstützt. When you[set customer IDs](../core-services/core-services.md)on your website, verify that at least one of the aliases is subscribed to[!DNL Target]. |
| Report Suite (Analytics) | Die Report Suites von Analytics.<br>Innerhalb einer Attributquelle können Sie dem Analytics-Abonnement maximal zehn Report Suites hinzufügen. Berücksichtigen Sie bei der Auswahl der einzuschließenden Report Suites die folgenden Vorschläge:<ul><li>Wählen Sie Report Suites mit einem gemeinsamen Satz authentifizierter Kunden. Wenn sich die authentifizierten Kunden in einer Report Suite nicht mit den authentifizierten Kunden in einer anderen Report Suite überschneiden, trennen Sie diese Report Suites in verschiedene Attributquellen.</li><li>Wenn möglich, sollten die Report Suites, die in einer Attributquelle enthalten sind, ein ähnliches Traffic-Volumen aufweisen.</li></ul><br>Falls Sie mehr als zehn Report Suites mit dem gleichen Satz authentifizierter Kunden haben, konfigurieren Sie weitere Kundenattributquellen mit jeweils bis zu zehn Report Suites. |
| Einzuschließende Attribute (Analytics und [!DNL Target]) | Die Attribute, die Sie an die Lösung senden möchten. <br>Beim Konfigurieren von Abonnements und beim Auswählen von Attributen gelten die folgenden Einschränkungen je nach _Report Suite,_ je nachdem, welche Lösungen Sie besitzen:<ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: 3 insgesamt</li><li>Premium: 200 pro Report Suite</li><li>[!DNL Target] Standard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Hinweis:**Bei einem Upgrade auf Analytics Premium dauert es 24 Stunden, bis weitere Attribute verfügbar sind. Während dieser Wartezeit wird Ihnen möglicherweise eine Fehlermeldung über einen erreichten Attributabonnement-Maximalwert angezeigt. |
