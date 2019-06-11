---
description: Erfahren Sie mehr über Lösungsdatenquellen und das Konfigurieren von Abonnements. Durch Abonnements können die Kundenattributdaten zwischen Experience Cloud und Lösungen (Analytics und Target) fließen.
keywords: Kundenattribute; Hauptdienste
seo-description: Erfahren Sie mehr über Lösungsdatenquellen und das Konfigurieren von Abonnements. Durch Abonnements können die Kundenattributdaten zwischen Experience Cloud und Lösungen (Analytics und Target) fließen.
seo-title: Konfigurieren von Abonnements
solution: Experience Cloud
title: Konfigurieren von Abonnements
uuid: f 74 a 8155-0 a 21-46 b 3-9 b 1 e -4 c 838 f 72 f 24 f
translation-type: tm+mt
source-git-commit: 979b2202a70e2a5362aa86a65a17d7c4279b3a1a

---


# Konfigurieren von Abonnements

Erfahren Sie mehr über Lösungsdatenquellen und das Konfigurieren von Abonnements. Durch Abonnements können die Kundenattributdaten zwischen Experience Cloud und Lösungen (Analytics und Target) fließen.

Eine Adobe Analytics-Mitgliedschaft ermöglicht z. B. Attributdaten in Berichten. Wenn Sie Adobe Target verwenden, können Sie Kundenattribute für Targeting und Segmentierung hochladen.

**[!UICONTROL Kundenattributquelle]** &gt; **[!UICONTROL Neue Kunden-Attributquelle erstellen]** &gt; **[!UICONTROL Neu]**

![](assets/configure_subscription_page.png)

| Element | Beschreibung |
|--- |--- |
| Lösung | **Adobe analyticsselect**<br>Analytics, geben Sie die Report Suites an, an die Sie Attributdaten erhalten möchten, und die einzuschließenden Attribute.<br>**Adobe targetsie**<br>können Kundenattribute für Targeting und Segmentierung hochladen. Diese Funktion ist nützlich, wenn Sie einen Test auf der Grundlage von Attributdaten durchführen möchten oder die Daten für die Segmentierung in Analytics zur Verfügung stellen möchten.<br>Hochgeladene Kundenattribute für einen Besucher sind bei der Anmeldung in Target &gt; Zielgruppen verfügbar.<br>Es werden mehrere Datenquellen unterstützt. Wenn Sie [Kunden-IDs](../core-services/core-services.md) auf Ihrer Website festlegen, prüfen Sie, dass mindestens eines dieser Aliasse über ein Target-Abonnement verfügt. |
| Report Suite (Analytics) | Die Report Suites aus Analytics.<br>Innerhalb einer Attributquelle können Sie dem Analytics-Abonnement maximal zehn Report Suites hinzufügen. Orientieren Sie sich bei der Auswahl der hinzuzufügenden Report Suites an folgenden Empfehlungen:<ul><li>Wählen Sie Report Suites mit dem gleichen Satz authentifizierter Kunden. Wenn die Report Suites nicht die gleichen authentifizierten Kunden enthalten, sollten Sie sie verschiedenen Attributquellen zuweisen.</li><li>Die Report Suites einer Attributquelle sollten möglichst ein ähnliches Datenverkehrsvolumen aufweisen.</li></ul><br>Falls Sie mehr als zehn Report Suites mit dem gleichen Satz authentifizierter Kunden haben, konfigurieren Sie weitere Kundenattributquellen mit jeweils bis zu zehn Report Suites. |
| Einzuschließende Attribute (Analytics und Target) | Die Attribute, die Sie zur Lösung senden möchten<br>Bei der Konfiguration von Abonnements und der Auswahl von Attributen gelten – abhängig von den Lösungen, die Sie besitzen – die folgenden Einschränkungen:<ul><li>Foundation: 0</li><li>Auswählen: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: 3 insgesamt</li><li>Premium: 200 pro Report Suite</li><li>Target Standard: 5</li><li>Target Premium: 200</li></ul><br>**Hinweis:** Bei einem Upgrade auf Analytics Premium dauert es 24 Stunden, bis weitere Attribute verfügbar sind. Während dieser Wartezeit wird Ihnen möglicherweise eine Fehlermeldung über einen erreichten Attributabonnement-Maximalwert angezeigt. |
