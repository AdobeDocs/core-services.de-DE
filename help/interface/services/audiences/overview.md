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
TQID: https://experienceleague.adobe.com/QEAfCWPNI-JhDw-HjZwBGv0TlqyctIqSwz8eVQqS6Gg
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: ff2b9b37-92e0-45fc-b853-379d44c08c89
source-git-commit: 0ce4fa63a4babc195f89c595009adcf19f34cdd9
workflow-type: tm+mt
source-wordcount: 684
ht-degree: 71%

---

# Experience Cloud-Zielgruppen

[!DNL Audience Library] zeigt Zielgruppen in Experience Cloud an. Zielgruppen sind Sammlungen von Besucherinnen und Besuchern (eine Liste von [!DNL Experience Cloud]-IDs). Sie können die Umsetzung von Besucherdaten in Zielgruppensegmentierung verwalten. Auf diese Weise erfolgt das Erstellen und Verwalten von Zielgruppen so ähnlich wie das Erstellen und Verwalten von Segmenten. Sie können in [!DNL Experience Cloud] das Zielgruppensegment auch für Produkte und Services freigeben.

![Experience Cloud-Zielgruppen](assets/audiences.png)

Zielgruppen können aus verschiedenen Quellen erstellt bzw. abgeleitet werden:

* Neue in [!DNL Experience Cloud] erstellte
* In [!DNL Analytics] veröffentlichte Segmente [!DNL Experience Cloud]
* [!DNL Audience Manager]

**Echtzeit- versus historische Zielgruppen**

Alle Zielgruppen stehen unabhängig von ihrer Quelle für Echtzeit-Targeting zur Verfügung. Zielgruppen, die in Analytics für Audience Manager freigegeben wurden, sind jedoch für Echtzeit-Targeting nicht verfügbar. Das System wertet Zielgruppen auf zweierlei Weise aus:

* Historische Zielgruppen aus Analytics werden alle vier Stunden ausgewertet. Die Gesamtdauer für die Verarbeitung und Freigabe kann bis zu acht Stunden dauern. Historische Zielgruppen beinhalten immer wiederkehrende Besucherinnen und Besucher.
* Echtzeit-Zielgruppen werden in den Experience Cloud-Zielgruppen ermittelt und in Echtzeit ausgewertet.

## So werden Zielgruppen in Programmen verwendet

Die folgende Tabelle beschreibt, wie Zielgruppen in Experience Cloud-Programmen verwendet werden:

| Lösung | Beschreibung |
| --- | --- |
| Experience Cloud-Zielgruppen | Zielgruppen nativ mit der Zielgruppenbibliothek erstellen, verwalten und freigeben. Sie haben folgende Möglichkeiten:<ul><li>Verwenden Sie Echtzeit-Zielgruppen unter Verwendung von Raw-Analytics-Attributen.</li><li>Kombinieren Sie Zielgruppen, um zusammengesetzte zu erstellen, und verbinden Sie Echtzeit- und historische Daten.</li><li>Siehe grafische Ansichten der geschätzten Zielgruppengröße.</li></ul><br>Vorschläge zum Typ der Zielgruppe, die Sie erstellen möchten, finden Sie unter [Optionen zur Zielgruppenerstellung](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html?lang=de). |
| Analytics | Bei der Segmentierung können Sie ein Segment erstellen, es mit einer Report Suite verknüpfen und dann das Segment in Experience Cloud veröffentlichen. Beim Veröffentlichen des Segments wird es auf der Seite [!DNL Audience Library] in Experience Cloud angezeigt. (Weitere [&#x200B; finden Sie unter „Veröffentlichen von Segmenten &#x200B;](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-publish.html?lang=de) Experience Cloud&quot; in [!DNL Analytics] Hilfe.) Die Zielgruppe ist auch als Zielgruppe für ein Kampagnenerlebnis verfügbar, das von [!DNL Adobe Target] und in [!DNL Audience Manager] bereitgestellt wird. Nachdem Sie eine Zielgruppe aus [!DNL Adobe Analytics] freigegeben und zur Verwendung in einer aktiven Kampagne ausgewählt haben, werden die Besucherprofile, die in den letzten 90 Tagen den Segmentdefinitionskriterien entsprechen, an [!UICONTROL Audience Services] gesendet. Die Beschränkung für gemeinsam verwendete Zielgruppen wurde auf 75 erhöht. Zielgruppen, die von Experience Cloud und [!DNL Analytics] gemeinsam verwendet werden, dürfen nicht mehr als 20 Millionen eindeutige Mitglieder umfassen. Aufgrund der Caching-Funktion wird zudem die Löschung von Report Suites in Analytics erst nach 12 Stunden durch Experience Cloud übernommen. |
| Mobile Services | Analysieren Sie den Mobile-Traffic mithilfe der Sunburst-Visualisierung im [!UICONTROL Device Types]. |
| [!DNL Target] | Mit dem [ID-Dienst](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=de) werden Besucher-IDs und Daten zu einem einsatzfähigen Profil zusammenfasst, welches dann programmübergreifend verwendet werden kann. Wenn das Kontrollkästchen [!UICONTROL Publish to Experience Cloud] während der Segmenterstellung in Adobe Analytics aktiviert wird, ist das Segment in der benutzerdefinierten Zielgruppenbibliothek von Adobe Target verfügbar. Ein in [!DNL Analytics] oder [!DNL Audience Manager] erstelltes Segment kann für Aktivitäten in [!DNL Target] verwendet werden. Sie können zum Beispiel Kampagnenaktivitäten basierend auf [!DNL Analytics]-Konversionsmetriken und in [!DNL Analytics] erstellten Zielgruppensegmenten erstellen. |
| [!DNL Audience Manager] | Gemeinsam verwendete Zielgruppen sind in der Segmentierung von [!DNL Audience Manager] verfügbar. Alle Experience Cloud-Zielgruppen stehen systemintern in [!DNL Audience Manager] zur Verfügung. Dieser bietet Folgendes:<ul><li>Integrierte Automatisierung hinsichtlich der Freigabe und Verwendung in Programm-Workflows</li><li>Offsite-Ziele</li><li>Look-Alike-Modellierung</li></ul> |
| Campaign | <ul><li>Importieren freigegebener Zielgruppen von verschiedenen Adobe Experience Cloud-Programmen in Adobe Campaign.</li><li>Exportieren Sie Empfängerlisten in Form von freigegebenen Zielgruppen. Diese freigegebenen Zielgruppen können dann in den anderen von Ihnen verwendeten Adobe Experience Cloud-Programmen genutzt werden.</li></ul> |
| Advertising Cloud | Verwenden Sie die Zielgruppe als Ziele. |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>Wenn ein Besucher in die in Analytics freigegebene Zielgruppe aufgenommen wird, ist diese Information erst mit einer Verzögerung von 4 bis 8 Stunden in [!DNL Target], Ad Cloud und Campaign Standard verfügbar.

## Schnittstellenelemente der Zielgruppenbibliothek

[!DNL Experience Cloud] bietet eine Bibliothek für die Erstellung und Verwaltung von Zielgruppen mit einer systemeigenen Zielgruppenidentifizierung in Echtzeit.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL People]** > **[!UICONTROL Audience Library]**

![Zielgruppe in Zielgruppenbibliothek hinzufügen](assets/audience_library.png)


| Element | Beschreibung |
| --- | --- |
| Neu | [Erstellen einer Zielgruppe](https://experienceleague.adobe.com/de/docs/core-services/interface/services/audiences/create). |
| Titel und Beschreibung | Eine Spaltenüberschrift, die die Zielgruppe identifiziert und beschreibt. |
| Autor | Die Person, die das Zielgruppensegment erstellt hat. |
| Quelle | Gibt an, wo die Zielgruppe erstellt wurde.<ul><li>**Analytics:** Ein Segment, das in Adobe Analytics erstellt und dann in Experience Cloud veröffentlicht wurde.</li><li>**Experience Cloud:** Eine neue Zielgruppe, [die in Experience Cloud-Zielgruppen erstellt wurde](https://experienceleague.adobe.com/de/docs/core-services/interface/services/audiences/create).</li><li>**Audience Manager:** In Audience Manager erstellte Zielgruppen werden automatisch in Experience Cloud-Zielgruppen angezeigt.</li></ul> |
| Aktuelle Größe | Die aktuelle Zielgruppengröße. |
| Aktiv | Der aktive Status des Segments. |

{style="table-layout:auto"}

## Veröffentlichen von Zielgruppen aus Adobe Analytics

Weitere Informationen [&#x200B; Sie in der Adobe Analytics](https://experienceleague.adobe.com/de/docs/analytics/components/segmentation/segmentation-workflow/seg-publish)Dokumentation unter „Veröffentlichen von Segmenten in Experience Cloud&quot;.
