---
description: Hier erfahren Sie mehr über Lösungsdatenquellen und das Konfigurieren von Abonnements. Abonnements ermöglichen den Datenfluss von Kundenattributen zwischen Experience Cloud und Programmen (Analytics und Target).
solution: Experience Cloud
title: Konfigurieren von Abonnements
uuid: f74a8155-0a21-46b3-9b1e-4c838f72f24f
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: cfa2aa5c-337f-401e-80eb-cbe36cb1d41e
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 82%

---

# Konfigurieren von Abonnements in Experience Cloud

Erfahren Sie mehr über Programmdatenquellen und das Konfigurieren von Abonnements. Abonnements ermöglichen den [!DNL Customer Attribute] Datenfluss zwischen Experience Cloud und Anwendungen ([!DNL Analytics] und [!DNL Target]).

Ein Adobe Analytics-Abonnement ermöglicht beispielsweise Attributdaten in Berichten. Wenn Sie Adobe Target verwenden, können Sie Kundenattribute für Targeting und Segmentierung hochladen.

**[!UICONTROL Kunden-Attributquelle]** > **[!UICONTROL Neue Kunden-Attributquelle erstellen]** > **[!UICONTROL Neu]**

![Konfigurieren von Abonnements in Experience Cloud](assets/configure_subscription_page.png)

| Element | Beschreibung |
|--- |--- |
| Lösung | **Adobe Analytics**<br> Wählen Sie [!DNL Analytics] aus, geben Sie die Report Suites an, für die Sie Attributdaten empfangen möchten, und die einzuschließenden Attribute.<br>**Adobe Target:**<br> Sie können Kundenattribute für Targeting und die Segmentierung hochladen. Diese Funktion ist nützlich, wenn Sie einen Test auf der Grundlage von Attributdaten durchführen möchten oder die Daten für die Segmentierung in Analytics zur Verfügung stellen möchten.<br>Hochgeladene Kundenattributdaten für einen Besucher sind bei der Anmeldung in **[!DNL Target]** > **Zielgruppen** verfügbar.<br>Es werden mehrere Datenquellen unterstützt. Wenn Sie Kunden-IDs auf Ihrer Website festlegen, stellen Sie sicher, dass mindestens einer der Aliase [!DNL Target] abonniert ist. |
| Report Suite (Analytics) | Die Report Suites von Analytics.<br>Innerhalb einer Attributquelle können Sie dem Analytics-Abonnement maximal zehn Report Suites hinzufügen. Berücksichtigen Sie bei der Auswahl der einzuschließenden Report Suites die folgenden Vorschläge:<ul><li>Wählen Sie Report Suites mit einem gemeinsamen Satz authentifizierter Kunden aus. Wenn sich die authentifizierten Kunden in einer Report Suite nicht mit den authentifizierten Kunden in einer anderen Report Suite überschneiden, teilen Sie diese Report Suites in verschiedene Attributquellen auf.</li><li>Wenn möglich, sollten die Report Suites, die in einer Attributquelle enthalten sind, ein ähnliches Traffic-Volumen aufweisen.</li></ul><br>Wenn Sie über mehr als 10 Report Suites mit einem gemeinsamen Satz authentifizierter Kunden verfügen, können Sie zusätzliche Kundenattributquellen mit jeweils bis zu 10 Report Suites konfigurieren. |
| Einzuschließende Attribute (Analytics und [!DNL Target]) | Die Attribute, die Sie an das Programm senden möchten. <br>Bei der Konfiguration von Abonnements und der Auswahl von Attributen gelten – je nachdem, welche Programme Sie besitzen – die folgenden Einschränkungen _pro Report Suite_:<ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: 3 insgesamt</li><li>Premium: 200 pro Report Suite</li><li>[!DNL Target] Standard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Hinweis:** Bei einem Upgrade auf Analytics Premium dauert es 24 Stunden, bis weitere Attribute verfügbar sind. Während dieser Wartezeit wird Ihnen möglicherweise eine Fehlermeldung über einen erreichten Attributabonnement-Maximalwert angezeigt. |

{style="table-layout:auto"}
