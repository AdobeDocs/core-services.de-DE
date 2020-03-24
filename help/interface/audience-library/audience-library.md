---
description: Umsetzung von Besucherdaten in Zielgruppensegmentierung verwalten.
seo-description: Umsetzung von Besucherdaten in Zielgruppensegmentierung verwalten.
seo-title: Zielgruppen
solution: Experience Cloud
title: Zielgruppen
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
translation-type: tm+mt
source-git-commit: 14d6e0ae15b023ad4dd3f8aca0606f26b39a21e9

---


# Zielgruppen {#topic_679810123CAA4E0CA4FA3417FB0100C7}

Audiencen sind Sammlungen von Besuchern (eine Liste von Besucher-IDs). Die Audience Services von Adobe verwalten die Übersetzung von Besucher-Daten in die Segmentierung von Audiencen. Auf diese Weise erfolgt die Erstellung und Verwaltung von Zielgruppen so ähnlich wie die Erstellung und Verwendung von Segmenten, mit dem zusätzlichen Vorteil, dass die Zielgruppensegmente für die [!DNL Experience Cloud] freigegeben werden können.

![](assets/audiences.png)

Zielgruppen können aus verschiedenen Quellen erstellt bzw. abgeleitet werden:

* In der [!DNL Experience Cloud] neu erstellt
* Aus [!DNL Analytics]-Segmenten, die in der [!DNL Experience Cloud] veröffentlicht werden
* Aus [!DNL Audience Manager]

**Echtzeit- und historische Zielgruppen**

Alle Zielgruppen stehen unabhängig von ihrer Quelle für Echtzeit-Targeting zur Verfügung. Zielgruppen, die in Analytics für Audience Manager freigegeben wurden, sind jedoch für Echtzeit-Targeting nicht verfügbar. Das System bewertet Audiencen auf zweierlei Weise:

* Historische Audiencen aus Analytics werden alle 4 Stunden ausgewertet. Die Gesamtdauer für die Verarbeitung und Freigabe kann bis zu 8 Stunden dauern.  Historische Audiencen beinhalten immer rückkehrende Besucher.
* Echtzeit-Zielgruppen werden in den Experience Cloud Audiences ermittelt und in Echtzeit ausgewertet.

## So werden Zielgruppen in Lösungen verwendet {#concept_01EB9345C5344597BC94A864EDD38EE1}

Die folgende Tabelle beschreibt, wie Audiencen in Experience Cloud-Lösungen verwendet werden:

| Lösung | Beschreibung |
|--- |--- |
| Experience Cloud Audiences | Erstellen, verwalten und teilen Sie Zielgruppen systemintern mithilfe der Benutzeroberfläche der [Zielgruppenbibliothek](../audience-library/audience-library.md). Sie haben folgende Möglichkeiten:<ul><li>Echtzeit-Audiencen mithilfe von Attributen für Rohanalysen verwenden</li><li>Kombinieren von Audiencen zur Erstellung von Composite-Daten, indem Sie Echtzeit- und historische Daten kombinieren</li><li>Siehe Grafische Ansichten der geschätzten Audiencen</li></ul><br>Vorschläge zur Art der Audience, die Sie erstellen möchten, finden Sie unter: [Experience Cloud-Audiencen](https://helpx.adobe.com/marketing-cloud-core/kb/People/Audience-Creation-Options.html). |
| Analytics | Bei der Segmentierung können Sie ein Segment erstellen, es mit einer Report Suite verknüpfen und das  [ Segment dann in Experience Cloud veröffentlichen](../audience-library/audience-library.md). Nach seiner Veröffentlichung erscheint das Segment auf der Seite [Zielgruppen](../audience-library/audience-library.md). Die Zielgruppe steht auch als eine für ein Kampagnenerlebnis anvisierte Zielgruppe in Adobe Target und in Audience Manager bereit.   Nachdem eine Zielgruppe in Analytics freigegeben und zur Verwendung in einer aktiven Kampagne ausgewählt wurde, werden alle Besucherprofile, die in den letzten 90 Tagen den Segmentdefinitionskriterien entsprochen haben, an die Experience Cloud Audience Services-Plattform gesendet.   Die Beschränkung für freigegebene Audiencen wurde auf 75 erhöht.  Audiencen, die von Analytics für die Experience Cloud freigegeben wurden, dürfen 20 Millionen individuelle Mitglieder nicht überschreiten. Aufgrund der Zwischenspeicherung müssen gelöschte Report Suites in Analytics 12 Stunden vor dem Löschen in der Experience Cloud angezeigt werden. |
| Mobile Services | Analysieren Sie den mobilen Traffic mithilfe der Sunburst-Visualisierung im Bericht &quot; [!UICONTROL Gerätetypen] &quot;. |
| Target | The [ID service](https://docs.adobe.com/content/help/en/id-service/using/home.html) unifies visitor IDs and data into a single, actionable profile for use across solutions. Wenn das Kontrollkästchen [In der Experience Cloud veröffentlichen](../audience-library/audience-library.md) während der Segmenterstellung in Adobe Analytics aktiviert wird, ist das Segment in der benutzerdefinierten Zielgruppenbibliothek von Adobe Target verfügbar. Ein in Analytics oder Audience Manager erstelltes Segment kann für Aktivitäten in Target verwendet werden.  Sie können zum Beispiel Kampagnenaktivitäten basierend auf Analytics-Konversionsmetriken und in Analytics erstellten Zielgruppensegmenten erstellen. |
| Audience Manager | Freigegebene Audiencen sind in der Segmentierung von Audience Manager verfügbar. Alle Experience Cloud-Zielgruppen stehen systemintern in Audience Manager zur Verfügung. Dieser bietet Folgendes:<ul><li>Integrierte Automatisierung hinsichtlich der Freigabe und Verwendung in Workflows</li><li>Offsite-Ziele</li><li>Look-like-Modellierung</li></ul> |
| Kampagne | <ul><li>Importieren freigegebener Zielgruppen von verschiedenen Adobe Experience Cloud-Lösungen in Adobe Campaign</li><li>Exportieren Sie Empfänger-Listen in Form freigegebener Audiencen. Diese freigegebenen Audiencen können in den verschiedenen Adobe Experience Cloud-Lösungen verwendet werden, die Sie verwenden.</li></ul> |
| Media Optimizer | Verwenden Sie die Audience als Zielgruppen. |

>[!IMPORTANT]
>
>Sobald sich ein Besucher für die in Analytics freigegebene Audience qualifiziert hat, erfolgt eine Verzögerung von 4-8 Stunden, bevor diese Informationen in Zielgruppe, Ad Cloud und Campaign Standard verarbeitet werden können.

## Weitere Hilfestellung – Fragen, Hinweise und Anwendungsbeispiele {#section_C7F151644D8A45F7B6FC54F58845635D}

| Hilfe mit | Ressource |
|--- |--- |
| Kann keine Audiencen finden? | Stellen Sie sicher, dass Sie bereitgestellt wurden. See [Getting started - enable your solutions for core services](../core-services/core-services.md).<br>Klicken Sie [hier](https://www.adobe.com/go/audiences) , um den Zugriff auf Profil und Audiencen anzufordern (Integrations-Bereitstellungsformular). |
| Anwendungsbeispiele | Weitere Anleitungen zu der zu verwendenden Lösung finden Sie in der Wissensdatenbank unter [Optionen](https://helpx.adobe.com/marketing-cloud-core/kb/People/Audience-Creation-Options.html) zur Audience-Erstellung. |
| Forum | The [Audiences forum](https://forums.adobe.com/community/experience-cloud/platform/core-services/people-service/audiences) is an additional resource to get help with audiences. |

## Schnittstellenelemente der Zielgruppenbibliothek {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

Die [!DNL Experience Cloud] verfügt über eine Bibliothek für die Erstellung und Verwaltung von Zielgruppen mit einer systemeigenen Zielgruppenidentifizierung in Echtzeit.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL People]** > **[!UICONTROL Audience Library]**

![](assets/audience_library.png)

| Element | Beschreibung |
|--- |--- |
| Neu | [Erstellen einer Zielgruppe](../audience-library/audience-library.md). |
| Titel und Beschreibung | Eine Spaltenüberschrift, die die Zielgruppe identifiziert und beschreibt. |
| Autor | Die Person, die das Audiencen-Segment erstellt hat. |
| Quelle | Gibt an, wo die Audience erstellt wurde.<ul><li>**Analytics:** Ein Segment, das in Reports &amp; Analytics oder Ad Hoc Analysis erstellt und dann in der [Experience Cloud veröffentlicht](../audience-library/audience-library.md) wird.</li><li>**Experience Cloud:** Eine neue Zielgruppe, [die in Experience Cloud Audiences erstellt wird](../audience-library/audience-library.md).</li><li>**Audience Manager:** In Audience Manager erstellte Zielgruppen werden automatisch in Experience Cloud-Zielgruppen angezeigt.</li></ul> |
| Aktuelle Größe | Die aktuelle Audience. |
| Aktiv | Der aktive Status des Segments. |
