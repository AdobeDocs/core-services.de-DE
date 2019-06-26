---
description: Umsetzung von Besucherdaten in Zielgruppensegmentierung verwalten.
seo-description: Umsetzung von Besucherdaten in Zielgruppensegmentierung verwalten.
seo-title: Zielgruppen
solution: Experience Cloud
title: Zielgruppen
uuid: 92faf3a8-1375-4e32-905b-74cad48144d3
translation-type: ht
source-git-commit: 979b2202a70e2a5362aa86a65a17d7c4279b3a1a

---


# Zielgruppen{#topic_679810123CAA4E0CA4FA3417FB0100C7}

Zielgruppen sind Besuchersammlungen (Listen mit Besucher-IDs). Durch die Zielgruppendienste von Adobe wird die Umsetzung von Besucherdaten in Zielgruppensegmentierung verwaltet. Auf diese Weise erfolgt die Erstellung und Verwaltung von Zielgruppen so ähnlich wie die Erstellung und Verwendung von Segmenten, mit dem zusätzlichen Vorteil, dass die Zielgruppensegmente für die [!DNL Experience Cloud] freigegeben werden können.

![](assets/audiences.png)

Zielgruppen können aus verschiedenen Quellen erstellt bzw. abgeleitet werden:

* In der [!DNL Experience Cloud] neu erstellt
* Aus [!DNL Analytics]-Segmenten, die in der [!DNL Experience Cloud] veröffentlicht werden
* Aus [!DNL Audience Manager]

**Echtzeit- und historische Zielgruppen**

Alle Zielgruppen stehen unabhängig von ihrer Quelle für Echtzeit-Targeting zur Verfügung. Zielgruppen, die in Analytics für Audience Manager freigegeben wurden, sind jedoch für Echtzeit-Targeting nicht verfügbar. Das System wertet Zielgruppen auf zweierlei Arten aus:

* Historische Zielgruppen aus Analysen werden alle 12 Stunden ausgewertet. Historische Zielgruppen beinhalten immer wiederkehrende Besucher.
* Echtzeit-Zielgruppen werden in den Experience Cloud Audiences ermittelt und in Echtzeit ausgewertet.


## So werden Zielgruppen in Lösungen verwendet {#concept_01EB9345C5344597BC94A864EDD38EE1}

In der folgenden Tabelle wird beschrieben, wie Zielgruppen in Lösungen der Experience Cloud eingesetzt werden:

| Lösung | Beschreibung |
|--- |--- |
| Experience Cloud Audiences | Erstellen, verwalten und teilen Sie Zielgruppen systemintern mithilfe der Benutzeroberfläche der [Zielgruppenbibliothek](../audience-library/audience-library.md). Sie haben folgende Möglichkeiten:<ul><li>Echtzeit-Zielgruppen mit Attributen für Analytics-Rohdaten verwenden</li><li>Zielgruppen zu Mischgruppen kombinieren, indem Sie Echtzeitdaten und historische Daten kombinieren</li><li>Siehe „Grafische Ansicht geschätzter Zielgruppengrößen“</li></ul><br>Vorschläge zur Art der zu erstellenden Zielgruppe finden Sie unter: [Experience Cloud Audiences](https://helpx.adobe.com/de/marketing-cloud-core/kb/People/Audience-Creation-Options.html). |
| Analytics | Bei der Segmentierung können Sie ein Segment erstellen, es mit einer Report Suite verknüpfen und das  [ Segment dann in Experience Cloud veröffentlichen](../audience-library/audience-library.md). Nach seiner Veröffentlichung erscheint das Segment auf der Seite [Zielgruppen](../audience-library/audience-library.md). Die Zielgruppe steht auch als eine für ein Kampagnenerlebnis anvisierte Zielgruppe in Adobe Target und in Audience Manager bereit.   Nachdem eine Zielgruppe in Analytics freigegeben und zur Verwendung in einer aktiven Kampagne ausgewählt wurde, werden alle Besucherprofile, die in den letzten 90 Tagen den Segmentdefinitionskriterien entsprochen haben, an die Experience Cloud Audience Services-Plattform gesendet.   Wichtig: Begrenzen Sie die Anzahl der von Analytics freigegebenen Zielgruppen auf 20, um zusätzliche Verarbeitungsverzögerungen zu vermeiden. Zielgruppen, die von der Experience Cloud und Analytics gemeinsam verwendet werden, dürfen nicht mehr als 20 Millionen eindeutige Mitglieder umfassen. Aufgrund der Caching-Funktion wird die Löschung von Report Suites in Analytics erst nach 12 Stunden durch die Experience Cloud übernommen. |
| Mobile Services | Analysieren Sie den mobilen Datenverkehr mit Hilfe der Sunburst-Visualisierung in den [Gerätetypen](https://marketing.adobe.com/resources/help/de_DE/mobile/?f=reports_devices). |
| Target | Der [ID-Dienst](https://marketing.adobe.com/resources/help/de_DE/mcvid/) vereinheitlicht Besucher-IDs und Daten zu einem einzigen, umsetzbaren Profil für die lösungsübergreifende Verwendung. Wenn das Kontrollkästchen [In der Experience Cloud veröffentlichen](../audience-library/audience-library.md) während der Segmenterstellung in Adobe Analytics aktiviert wird, ist das Segment in der benutzerdefinierten Zielgruppenbibliothek von Adobe Target verfügbar. Ein in Analytics oder Audience Manager erstelltes Segment kann für Aktivitäten in Target verwendet werden.  Sie können zum Beispiel Kampagnenaktivitäten basierend auf Analytics-Konversionsmetriken und in Analytics erstellten Zielgruppensegmenten erstellen. |
| Audience Manager | Freigegebene Zielgruppen stehen in der Segmentierungsfunktion von Audience Manager zur Verfügung. Alle Experience Cloud-Zielgruppen stehen systemintern in Audience Manager zur Verfügung. Dieser bietet Folgendes:<ul><li>Integrierte Automatisierung hinsichtlich der Freigabe und Verwendung in Lösungsabläufen</li><li>Offsite-Ziele</li><li>Look-Alike-Modellierung</li></ul> |
| Kampagne | <ul><li>Importieren freigegebener Zielgruppen von verschiedenen Adobe Experience Cloud-Lösungen in Adobe Campaign</li><li>Exportieren von Empfängerlisten in Form von freigegebenen Zielgruppen. Diese freigegebenen Zielgruppen können in verschiedenen von Ihnen genutzten Adobe Experience Cloud-Lösungen verwendet werden.</li></ul> |
| Media Optimizer | Verwendung der Zielgruppen als Ziele. |


>[!IMPORTANT]
>
>Wenn ein Besucher in die in Analytics freigegebene Zielgruppe aufgenommen wird, ist diese Information erst mit einer Verzögerung von 24 bis 48 Stunden in Target, Media Optimizer und Campaign verfügbar.

## Weitere Hilfestellung – Fragen, Hinweise und Anwendungsbeispiele {#section_C7F151644D8A45F7B6FC54F58845635D}


| Hilfethema | Ressource |
|--- |--- |
| Sie finden Ihre Zielgruppen nicht? | Stellen Sie sicher, dass Ihnen die entsprechenden Lösungen bereitgestellt wurden. Siehe  [Erste Schritte - Aktivieren Ihrer Lösungen für Hauptdienste](../core-services/core-services.md).<br>Klicken Sie [hier](https://www.adobe.com/go/audiences), um Zugriff auf Profiles &amp; Audiences anzufordern (Integrations-Bereitstellungsformular). |
| Anwendungsbeispiele | Weitere Anleitungen zu der zu verwendenden Lösung finden Sie in der Wissensdatenbank unter [Einstellungen für die Zielgruppenerstellung](https://helpx.adobe.com/de/marketing-cloud-core/kb/People/Audience-Creation-Options.html). |
| Forum | Das [Zielgruppenforum](https://forums.adobe.com/community/experience-cloud/platform/core-services/people-service/audiences) ist eine zusätzliche Ressource, die Hilfe bei Zielgruppen bietet. |


## Schnittstellenelemente der Zielgruppenbibliothek {#section_D04ACEF61CEF4B189AE6BA9F40D0DBF4}

Die [!DNL Experience Cloud] verfügt über eine Bibliothek für die Erstellung und Verwaltung von Zielgruppen mit einer systemeigenen Zielgruppenidentifizierung in Echtzeit.

**[!UICONTROL Experience Cloud]** &gt; **[!UICONTROL Zielgruppenbibliothek]**

![](assets/audience_library.png)

| Element | Beschreibung |
|--- |--- |
| Neu | [Erstellen einer Zielgruppe](../audience-library/audience-library.md). |
| Titel und Beschreibung | Eine Spaltenüberschrift, die die Zielgruppe identifiziert und beschreibt. |
| Autor | Die Person, die das Zielgruppensegment erstellt hat. |
| Quelle | Gibt an, wo die Zielgruppe erstellt wurde.<ul><li>**Analytics:** Ein Segment, das in Reports &amp; Analytics oder Ad Hoc Analysis erstellt und dann in der [Experience Cloud veröffentlicht](../audience-library/audience-library.md) wird.</li><li>**Experience Cloud:** Eine neue Zielgruppe, [die in Experience Cloud Audiences erstellt wird](../audience-library/audience-library.md).</li><li>**Audience Manager:** In Audience Manager erstellte Zielgruppen werden automatisch in Experience Cloud-Zielgruppen angezeigt.</li></ul> |
| Aktuelle Größe | Die aktuelle Zielgruppengröße. |
| Aktiv | Der aktive Status des Segments. |
