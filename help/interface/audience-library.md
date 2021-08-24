---
solution: Experience Cloud
type: Documentation
title: 'Adobe Experience Cloud Audiences '
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
description: Erfahren Sie, wie Sie im Experience Cloud Audience-Dienst die Übersetzung von Besucherdaten in eine Zielgruppensegmentierung verwalten können.
feature: Zielgruppenbibliothek
topic: Administration
role: Admin
level: Experienced
exl-id: 1c6e54ac-4886-46ed-9df7-201d2df31847
source-git-commit: 1fb1abc7311573f976f7e6b6ae67f60ada10a3e7
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 98%

---

# Experience Cloud-Zielgruppen {#topic_679810123CAA4E0CA4FA3417FB0100C7}

Zielgruppen sind Sammlungen von Besuchern (eine Liste von Besucher-IDs). Über die Zielgruppenbibliothek von Adobe können Sie die Übersetzung von Besucherdaten in die Zielgruppensegmentierung verwalten. Das Erstellen und Verwalten von Audiences ist daher ähnlich wie das Erstellen und Verwenden von Segmenten. Sie können in [!DNL Experience Cloud] das Zielgruppensegment auch für Produkte und Services freigeben.

![](assets/audiences.png)

Zielgruppen können aus verschiedenen Quellen erstellt bzw. abgeleitet werden:

* In der [!DNL Experience Cloud] neu erstellt
* [!DNL Analytics]-Segmente, die in [!DNL Experience Cloud] veröffentlicht werden
* [!DNL Audience Manager]

**Echtzeit- versus historische Zielgruppen**

Alle Zielgruppen stehen unabhängig von ihrer Quelle für Echtzeit-Targeting zur Verfügung. Zielgruppen, die in Analytics für Audience Manager freigegeben wurden, sind jedoch für Echtzeit-Targeting nicht verfügbar. Das System bewertet Zielgruppen auf zweierlei Weise:

* Historische Zielgruppen aus Analytics werden alle vier Stunden ausgewertet. Die Gesamtdauer für die Verarbeitung und Freigabe kann bis zu acht Stunden dauern. Historische Zielgruppen beinhalten immer wiederkehrende Besucher.
* Echtzeit-Zielgruppen werden in den Experience Cloud Audiences ermittelt und in Echtzeit ausgewertet.

## So werden Zielgruppen in Lösungen verwendet {#concept_01EB9345C5344597BC94A864EDD38EE1}

Die folgende Tabelle beschreibt, wie Zielgruppen in Experience Cloud-Lösungen verwendet werden:

| Lösung | Beschreibung |
|--- |--- |
| Experience Cloud-Zielgruppen | Erstellen, verwalten und teilen Sie Zielgruppen systemintern mithilfe der Benutzeroberfläche der [Zielgruppenbibliothek](audience-library.md). Sie haben folgende Möglichkeiten:<ul><li>Verwenden von Echtzeit-Zielgruppen mithilfe von Attributen für Rohanalysen</li><li>Kombinieren von Zielgruppen zur Erstellung von Composite-Daten, indem Sie Echtzeit- und historische Daten kombinieren</li><li>Siehe Grafische Ansichten der geschätzten Zielgruppengröße</li></ul><br>Vorschläge zum Typ der Zielgruppe, die Sie erstellen möchten, finden Sie unter: [Experience Cloud-Zielgruppen](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html?lang=de). |
| Analytics | Bei der Segmentierung können Sie ein Segment erstellen, es mit einer Report Suite verknüpfen und das Segment dann in Experience Cloud veröffentlichen. Beim Veröffentlichen des Segments wird es auf der Seite [!UICONTROL Zielgruppenbibliothek] in Experience Cloud angezeigt. (Weitere Informationen finden Sie unter [Segmente in Experience Cloud veröffentlichen](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-publish.html?lang=de) in der Analytics-Hilfe.) Die Zielgruppe steht auch als eine für ein Kampagnenerlebnis anvisierte Zielgruppe in Adobe Target und in Audience Manager bereit. Nachdem Sie eine Zielgruppe aus Adobe Analytics freigegeben und zur Verwendung in einer aktiven Kampagne ausgewählt haben, werden die Besucherprofile, die in den letzten 90 Tagen den Segmentdefinitionskriterien entsprechen, an [!UICONTROL Zielgruppendienste] gesendet. Die Beschränkung für freigegebene Zielgruppen wurde auf 75 erhöht. Zielgruppen, die von Experience Cloud und Analytics gemeinsam verwendet werden, dürfen nicht mehr als 20 Millionen eindeutige Mitglieder umfassen Aufgrund der Caching-Funktion wird zudem die Löschung von Report Suites in Analytics erst nach 12 Stunden durch Experience Cloud übernommen. |
| Mobile Services | Analysieren Sie den mobilen Traffic mithilfe der Sunburst-Visualisierung im Bericht „[!UICONTROL Gerätetypen]“. |
| [!DNL Target] | Mit dem [ID-Dienst](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=de) werden Besucher-IDs und Daten zu einem einsatzfähigen Profil zusammenfasst, welches dann lösungsübergreifend verwendet werden kann. Wenn das Kontrollkästchen „[In Experience Cloud veröffentlichen](audience-library.md)“ während der Segmenterstellung in Adobe Analytics aktiviert wird, ist das Segment in der benutzerdefinierten Zielgruppenbibliothek von Adobe Target verfügbar. Ein in Analytics oder Audience Manager erstelltes Segment kann für Aktivitäten in [!DNL Target] verwendet werden. Sie können zum Beispiel Kampagnenaktivitäten basierend auf [!DNL Analytics]-Konversionsmetriken und in [!DNL Analytics] erstellten Zielgruppensegmenten erstellen. |
| Audience Manager | Freigegebene Zielgruppen sind in der Segmentierung von Audience Manager verfügbar. Alle Experience Cloud-Zielgruppen stehen systemintern in Audience Manager zur Verfügung. Dieser bietet Folgendes:<ul><li>Integrierte Automatisierung hinsichtlich der Freigabe und Verwendung in Lösungs-Workflows</li><li>Offsite-Ziele</li><li>Look-Alike-Modellierung</li></ul> |
| Campaign | <ul><li>Importieren freigegebener Zielgruppen von verschiedenen Adobe Experience Cloud-Lösungen in Adobe Campaign.</li><li>Exportieren Sie Empfängerlisten in Form von freigegebenen Zielgruppen. Diese freigegebenen Zielgruppen können dann in den anderen von Ihnen verwendeten Adobe Experience Cloud-Lösungen genutzt werden.</li></ul> |
| Advertising Cloud | Verwenden Sie die Zielgruppe als Ziele. |

{style=&quot;table-layout:auto&quot;}

>[!IMPORTANT]
>
>Wenn ein Besucher in die in Analytics freigegebene Zielgruppe aufgenommen wird, ist diese Information erst mit einer Verzögerung von 4 bis 8 Stunden in [!DNL Target], Ad Cloud und Campaign Standard verfügbar.

## Weitere Hilfestellung – Fragen, Hinweise und Anwendungsbeispiele {#section_C7F151644D8A45F7B6FC54F58845635D}

| Hilfe mit | Ressource |
|--- |--- |
| Es können keine Ressourcen gefunden werden? | Stellen Sie sicher, dass Sie bereitgestellt wurden. Siehe [Erste Schritte – Aktivieren Ihrer Lösungen für zentrale Dienste](core-services.md).<br>Rufen Sie  [](https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=X8SVES) hier den Zugriff auf Profile und Zielgruppen an (Integrations-Bereitstellungsformular). |
| Anwendungsbeispiele | Weitere Anleitungen zu der zu verwendenden Lösung finden Sie in der Knowledgebase unter [Optionen zur Zielgruppenerstellung](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html?lang=en). |
| Forum | Das [Zielgruppenforum](https://experienceleaguecommunities.adobe.com/t5/Adobe-Experience-Cloud-Audiences/ct-p/experience-cloud-audiences-community) ist eine zusätzliche Ressource, die Hilfe bei Zielgruppen bietet. |

{style=&quot;table-layout:auto&quot;}

## Schnittstellenelemente der Zielgruppenbibliothek {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

[!DNL Experience Cloud] verfügt über eine Bibliothek für die Erstellung und Verwaltung von Zielgruppen mit einer systemeigenen Zielgruppenidentifizierung in Echtzeit.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL Personen]** > **[!UICONTROL Zielgruppenbibliothek]**

![](assets/audience_library.png)

| Element | Beschreibung |
|--- |--- |
| Neu | [Erstellen einer Zielgruppe](audience-library.md). |
| Titel und Beschreibung | Eine Spaltenüberschrift, die die Zielgruppe identifiziert und beschreibt. |
| Autor | Die Person, die das Zielgruppensegment erstellt hat. |
| Quelle | Gibt an, wo die Zielgruppe erstellt wurde.<ul><li>**Analytics:** Ein Segment, das in Adobe Analytics erstellt und dann in [Experience Cloud veröffentlicht wurde](audience-library.md).</li><li>**Experience Cloud:** Eine neue Zielgruppe, [die in Experience Cloud Audiences erstellt wird](audience-library.md).</li><li>**Audience Manager:** In Audience Manager erstellte Zielgruppen werden automatisch in Experience Cloud-Zielgruppen angezeigt.</li></ul> |
| Aktuelle Größe | Die aktuelle Zielgruppengröße. |
| Aktiv | Der aktive Status des Segments. |

{style=&quot;table-layout:auto&quot;}
