---
title: "[!DNL Audience Library]"
description: Erfahren Sie, wie Sie die Übersetzung von Besucherdaten in die Zielgruppensegmentierung in Experience Cloud verwalten. [!DNL Audience Library].
solution: Experience Cloud
type: Documentation
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: 1c6e54ac-4886-46ed-9df7-201d2df31847
source-git-commit: 064f3c981b921fd5aec9b252b839d8b7f59b3dee
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 61%

---

# Experience Cloud-Zielgruppen {#topic_679810123CAA4E0CA4FA3417FB0100C7}

Die [!DNL Audience Library] Zeigt Zielgruppen im Experience Cloud an. Zielgruppen sind Sammlungen von Besuchern (eine Liste von [!DNL Experience Cloud] IDs). Sie können die Übersetzung von Besucherdaten in eine Zielgruppensegmentierung verwalten. Das Erstellen und Verwalten von Zielgruppen ist daher ähnlich wie das Erstellen und Verwenden von Segmenten. Sie können in [!DNL Experience Cloud] das Zielgruppensegment auch für Produkte und Services freigeben.

![Experience Cloud-Zielgruppen](assets/audiences.png)

Zielgruppen können aus verschiedenen Quellen erstellt bzw. abgeleitet werden:

* In der [!DNL Experience Cloud] neu erstellt
* [!DNL Analytics]-Segmente, die in [!DNL Experience Cloud] veröffentlicht werden
* [!DNL Audience Manager]

**Echtzeit- versus historische Zielgruppen**

Alle Zielgruppen stehen unabhängig von ihrer Quelle für Echtzeit-Targeting zur Verfügung. Zielgruppen, die in Analytics für Audience Manager freigegeben wurden, sind jedoch für Echtzeit-Targeting nicht verfügbar. Das System wertet Zielgruppen auf zweierlei Weise aus:

* Historische Zielgruppen aus Analytics werden alle vier Stunden ausgewertet. Die Gesamtdauer für die Verarbeitung und Freigabe kann bis zu acht Stunden dauern. Historische Zielgruppen beinhalten immer wiederkehrende Besucher.
* Echtzeit-Zielgruppen werden aus Experience Cloud-Zielgruppen bezogen und in Echtzeit ausgewertet.

## So werden Zielgruppen in Programmen verwendet {#concept_01EB9345C5344597BC94A864EDD38EE1}

Die folgende Tabelle beschreibt, wie Zielgruppen in Experience Cloud-Programmen verwendet werden:

| Lösung | Beschreibung |
|--- |--- |
| Experience Cloud-Zielgruppen | Zielgruppen nativ erstellen, verwalten und freigeben mit [[!DNL Audience Library]](audience-library.md). Sie haben folgende Möglichkeiten:<ul><li>Verwenden von Echtzeit-Zielgruppen mithilfe von Attributen für Rohanalysen</li><li>Kombinieren von Zielgruppen zur Erstellung von Composite-Daten, indem Sie Echtzeit- und historische Daten kombinieren</li><li>Siehe Grafische Ansichten der geschätzten Zielgruppengröße</li></ul><br>Vorschläge dazu, welche Art von Zielgruppe Sie erstellen möchten, finden Sie unter [Optionen zur Zielgruppenerstellung](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html?lang=de). |
| Analysen | Bei der Segmentierung können Sie ein Segment erstellen, es mit einer Report Suite kombinieren und dann das Segment auf Experience Cloud veröffentlichen. Beim Veröffentlichen des Segments wird es auf der [!DNL Audience Library] Seite in Experience Cloud. (Siehe [Veröffentlichen von Segmenten auf Experience Cloud](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-publish.html?lang=de) in [!DNL Analytics] Hilfe für Details.) Die Zielgruppe ist auch als Zielgruppe für ein von bereitgestelltes Kampagnenerlebnis verfügbar [!DNL Adobe Target]und in [!DNL Audience Manager]. Nachdem Sie eine Zielgruppe freigegeben haben von [!DNL Adobe Analytics]und zur Verwendung in einer aktiven Kampagne auswählen, werden die Besucherprofile, die in den letzten 90 Tagen den Segmentdefinitionskriterien entsprechen, an gesendet. [!UICONTROL Zielgruppen-Services]. Die Beschränkung für freigegebene Zielgruppen wurde auf 75 erhöht. Audiences, die von für Experience Cloud freigegeben wurden [!DNL Analytics] Darf nicht mehr als 20 Millionen eindeutige Mitglieder umfassen. Aufgrund der Zwischenspeicherung benötigen gelöschte Report Suites in Analytics außerdem 12 Stunden, bevor die Löschung im Experience Cloud angezeigt wird. |
| Mobile Services | Analysieren Sie den mobilen Traffic mithilfe der Sunburst-Visualisierung im Bericht „[!UICONTROL Gerätetypen]“. |
| [!DNL Target] | Mit dem [ID-Dienst](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=de) werden Besucher-IDs und Daten zu einem einsatzfähigen Profil zusammenfasst, welches dann programmübergreifend verwendet werden kann. Die [Auf Experience Cloud veröffentlichen](audience-library.md) Wenn Sie das Kontrollkästchen während des Segmenterstellungsprozesses in Adobe Analytics aktivieren, ist das Segment in der benutzerdefinierten Zielgruppenbibliothek von Adobe Target verfügbar. Ein Segment, das in erstellt wurde [!DNL Analytics] oder [!DNL Audience Manager] Kann für Aktivitäten in verwendet werden [!DNL Target]. Sie können zum Beispiel Kampagnenaktivitäten basierend auf [!DNL Analytics]-Konversionsmetriken und in [!DNL Analytics] erstellten Zielgruppensegmenten erstellen. |
| [!DNL Audience Manager] | Freigegebene Zielgruppen sind verfügbar in [!DNL Audience Manager] Segmentierung. Alle Experience Cloud-Zielgruppen sind nativ in verfügbar. [!DNL Audience Manager], das Folgendes bietet:<ul><li>Integrierte Automatisierung hinsichtlich der Freigabe und Verwendung in Programm-Workflows</li><li>Offsite-Ziele</li><li>Look-Alike-Modellierung</li></ul> |
| Campaign | <ul><li>Importieren freigegebener Zielgruppen von verschiedenen Adobe Experience Cloud-Programmen in Adobe Campaign.</li><li>Exportieren Sie Empfängerlisten in Form von freigegebenen Zielgruppen. Diese freigegebenen Zielgruppen können dann in den anderen von Ihnen verwendeten Adobe Experience Cloud-Programmen genutzt werden.</li></ul> |
| Advertising Cloud | Verwenden Sie die Zielgruppe als Ziele. |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>Wenn ein Besucher in die in Analytics freigegebene Zielgruppe aufgenommen wird, ist diese Information erst mit einer Verzögerung von 4 bis 8 Stunden in [!DNL Target], Ad Cloud und Campaign Standard verfügbar.

## Weitere Hilfestellung – Fragen, Hinweise und Anwendungsbeispiele {#section_C7F151644D8A45F7B6FC54F58845635D}

| Hilfe mit | Ressource |
|--- |--- |
| Es können keine Ressourcen gefunden werden? | Stellen Sie sicher, dass Sie bereitgestellt wurden. Siehe [Erste Schritte – Aktivieren Ihrer Programme für zentrale Services](core-services.md).<br>Klicken Sie [hier](https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=X8SVES), um Zugriff auf Profile und Zielgruppen anzufordern (Integrations-Bereitstellungsformular). |
| Forum | Das [Zielgruppenforum](https://experienceleaguecommunities.adobe.com/t5/Adobe-Experience-Cloud-Audiences/ct-p/experience-cloud-audiences-community) ist eine zusätzliche Ressource, die Hilfe bei Zielgruppen bietet. |

{style="table-layout:auto"}

## Schnittstellenelemente der Zielgruppenbibliothek {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

[!DNL Experience Cloud] verfügt über eine Bibliothek für die Erstellung und Verwaltung von Zielgruppen mit einer systemeigenen Zielgruppenidentifizierung in Echtzeit.

**[!UICONTROL Experience Cloud]** > **[!UICONTROL Experience Platform]** > **[!UICONTROL Personen]** > **[!UICONTROL Zielgruppenbibliothek]**

![Zielgruppe in Zielgruppenbibliothek hinzufügen](assets/audience_library.png)

| Element | Beschreibung |
|--- |--- |
| Neu | [Erstellen einer Zielgruppe](audience-library.md). |
| Titel und Beschreibung | Eine Spaltenüberschrift, die die Zielgruppe identifiziert und beschreibt. |
| Autor | Die Person, die das Zielgruppensegment erstellt hat. |
| Quelle | Gibt an, wo die Zielgruppe erstellt wurde.<ul><li>**Analytics:** Ein Segment, das in Adobe Analytics erstellt wurde, dann [Veröffentlicht auf Experience Cloud](audience-library.md).</li><li>**Experience Cloud:** Eine neue Zielgruppe, [die in Experience Cloud Audiences erstellt wird](audience-library.md).</li><li>**Audience Manager:** Zielgruppen, die mit dem Audience Manager erstellt wurden, werden automatisch beim Experience Cloud von Zielgruppen angezeigt.</li></ul> |
| Aktuelle Größe | Die aktuelle Zielgruppengröße. |
| Aktiv | Der aktive Status des Segments. |

{style="table-layout:auto"}
