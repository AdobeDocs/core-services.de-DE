---
title: '[!DNL Audience Library]'
description: Erfahren Sie, wie Sie in der Experience Cloud  [!DNL Audience Library] die Übersetzung von Besucherdaten in eine Zielgruppensegmentierung verwalten können.
solution: Experience Cloud
type: Documentation
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: 1c6e54ac-4886-46ed-9df7-201d2df31847
source-git-commit: b257260bdbb7870dd6da807bceddfcddd2aef779
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 90%

---

# Experience Cloud-Zielgruppen {#topic_679810123CAA4E0CA4FA3417FB0100C7}

Die [!DNL Audience Library] zeigt Zielgruppen in Experience Cloud an. Zielgruppen sind Sammlungen von Besucherinnen und Besuchern (eine Liste von [!DNL Experience Cloud]-IDs). Sie können die Umsetzung von Besucherdaten in Zielgruppensegmentierung verwalten. Das Erstellen und Verwalten von Zielgruppen ist daher ähnlich wie das Erstellen und Verwenden von Segmenten. Sie können in [!DNL Experience Cloud] das Zielgruppensegment auch für Produkte und Services freigeben.

![Experience Cloud-Zielgruppen](assets/audiences.png)

Zielgruppen können aus verschiedenen Quellen erstellt bzw. abgeleitet werden:

* In der [!DNL Experience Cloud] neu erstellt
* [!DNL Analytics]-Segmente, die in [!DNL Experience Cloud] veröffentlicht werden
* [!DNL Audience Manager]

**Echtzeit- versus historische Zielgruppen**

Alle Zielgruppen stehen unabhängig von ihrer Quelle für Echtzeit-Targeting zur Verfügung. Zielgruppen, die in Analytics für Audience Manager freigegeben wurden, sind jedoch für Echtzeit-Targeting nicht verfügbar. Das System wertet Zielgruppen auf zweierlei Weise aus:

* Historische Zielgruppen aus Analytics werden alle vier Stunden ausgewertet. Die Gesamtdauer für die Verarbeitung und Freigabe kann bis zu acht Stunden dauern. Historische Zielgruppen beinhalten immer wiederkehrende Besucherinnen und Besucher.
* Echtzeit-Zielgruppen werden in den Experience Cloud-Zielgruppen ermittelt und in Echtzeit ausgewertet.

## So werden Zielgruppen in Programmen verwendet {#concept_01EB9345C5344597BC94A864EDD38EE1}

Die folgende Tabelle beschreibt, wie Zielgruppen in Experience Cloud-Programmen verwendet werden:

| Lösung | Beschreibung |
|--- |--- |
| Experience Cloud-Zielgruppen | Erstellen, verwalten und teilen Sie Zielgruppen nativ mithilfe der Zielgruppenbibliothek. Sie haben folgende Möglichkeiten:<ul><li>Verwenden von Echtzeit-Zielgruppen mithilfe von Attributen für Rohanalysen</li><li>Kombinieren von Zielgruppen zur Erstellung von Composite-Daten, indem Sie Echtzeit- und historische Daten kombinieren</li><li>Siehe Grafische Ansichten der geschätzten Zielgruppengröße</li></ul><br>Vorschläge zum Typ der Zielgruppe, die Sie erstellen möchten, finden Sie unter [Optionen zur Zielgruppenerstellung](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html?lang=de). |
| Analytics | Bei der Segmentierung können Sie ein Segment erstellen, es mit einer Report Suite verknüpfen und dann das Segment in Experience Cloud veröffentlichen. Beim Veröffentlichen des Segments wird es auf der Seite [!DNL Audience Library] in Experience Cloud angezeigt. (Weitere Informationen finden Sie unter [Publish-Segmente zu Experience Cloud](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-publish.html?lang=de) in der [!DNL Analytics] -Hilfe.) Die Zielgruppe ist auch als Zielgruppe für ein Kampagnenerlebnis verfügbar, das von [!DNL Adobe Target] und in [!DNL Audience Manager] bereitgestellt wird. Nachdem Sie eine Zielgruppe aus [!DNL Adobe Analytics] freigegeben und zur Verwendung in einer aktiven Kampagne ausgewählt haben, werden die Besucherprofile, die in den letzten 90 Tagen den Segmentdefinitionskriterien entsprachen, an [!UICONTROL Zielgruppendienste] gesendet. Die Beschränkung für gemeinsam verwendete Zielgruppen wurde auf 75 erhöht. Zielgruppen, die von Experience Cloud und [!DNL Analytics] gemeinsam verwendet werden, dürfen nicht mehr als 20 Millionen eindeutige Mitglieder umfassen. Aufgrund der Caching-Funktion wird zudem die Löschung von Report Suites in Analytics erst nach 12 Stunden durch Experience Cloud übernommen. |
| Mobile Services | Analysieren Sie den mobilen Traffic mithilfe der Sunburst-Visualisierung im Bericht „[!UICONTROL Gerätetypen]“. |
| [!DNL Target] | Mit dem [ID-Dienst](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=de) werden Besucher-IDs und Daten zu einem einsatzfähigen Profil zusammenfasst, welches dann programmübergreifend verwendet werden kann. Wenn das Kontrollkästchen [!UICONTROL In Experience Cloud veröffentlichen] während der Segmenterstellung in Adobe Analytics aktiviert wird, ist das Segment in der benutzerdefinierten Zielgruppenbibliothek von Adobe Target verfügbar. Ein in [!DNL Analytics] oder [!DNL Audience Manager] erstelltes Segment kann für Aktivitäten in [!DNL Target] verwendet werden. Sie können zum Beispiel Kampagnenaktivitäten basierend auf [!DNL Analytics]-Konversionsmetriken und in [!DNL Analytics] erstellten Zielgruppensegmenten erstellen. |
| [!DNL Audience Manager] | Gemeinsam verwendete Zielgruppen sind in der Segmentierung von [!DNL Audience Manager] verfügbar. Alle Experience Cloud-Zielgruppen stehen systemintern in [!DNL Audience Manager] zur Verfügung. Dieser bietet Folgendes:<ul><li>Integrierte Automatisierung hinsichtlich der Freigabe und Verwendung in Programm-Workflows</li><li>Offsite-Ziele</li><li>Look-Alike-Modellierung</li></ul> |
| Campaign | <ul><li>Importieren freigegebener Zielgruppen von verschiedenen Adobe Experience Cloud-Programmen in Adobe Campaign.</li><li>Exportieren Sie Empfängerlisten in Form von freigegebenen Zielgruppen. Diese freigegebenen Zielgruppen können dann in den anderen von Ihnen verwendeten Adobe Experience Cloud-Programmen genutzt werden.</li></ul> |
| Advertising Cloud | Verwenden Sie die Zielgruppe als Ziele. |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>Wenn ein Besucher in die in Analytics freigegebene Zielgruppe aufgenommen wird, ist diese Information erst mit einer Verzögerung von 4 bis 8 Stunden in [!DNL Target], Ad Cloud und Campaign Standard verfügbar.

## Schnittstellenelemente der Zielgruppenbibliothek {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

[!DNL Experience Cloud] verfügt über eine Bibliothek für die Erstellung und Verwaltung von Zielgruppen mit einer systemeigenen Zielgruppenidentifizierung in Echtzeit.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL Personen]** > **[!UICONTROL Zielgruppenbibliothek]**

![Zielgruppe in Zielgruppenbibliothek hinzufügen](assets/audience_library.png)


| Element | Beschreibung |
|--- |--- |
| Neu | [Erstellen einer Zielgruppe](create.md). |
| Titel und Beschreibung | Eine Spaltenüberschrift, die die Zielgruppe identifiziert und beschreibt. |
| Autor | Die Person, die das Zielgruppensegment erstellt hat. |
| Quelle | Gibt an, wo die Zielgruppe erstellt wurde.<ul><li>**Analytics:** Ein Segment, das in Adobe Analytics erstellt und dann auf Experience Cloud veröffentlicht wurde.</li><li>**Experience Cloud:** Eine neue Zielgruppe, [die in Experience Cloud-Zielgruppen erstellt wurde](create.md).</li><li>**Audience Manager:** In Audience Manager erstellte Zielgruppen werden automatisch in Experience Cloud-Zielgruppen angezeigt.</li></ul> |
| Aktuelle Größe | Die aktuelle Zielgruppengröße. |
| Aktiv | Der aktive Status des Segments. |

{style="table-layout:auto"}

## Publish-Zielgruppen aus Adobe Analytics

Weitere Informationen finden Sie unter [Publish-Segmente zu Experience Cloud](https://experienceleague.adobe.com/en/docs/analytics/components/segmentation/segmentation-workflow/seg-publish) in der Adobe Analytics-Dokumentation.
