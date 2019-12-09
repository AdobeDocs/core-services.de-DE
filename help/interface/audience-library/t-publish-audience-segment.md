---
description: Für Ihre Zielgruppen-Marketingaktivitäten müssen Sie ein Analytics-Zielgruppensegment in der Experience Cloud und in Adobe Target veröffentlichen.
keywords: core services
seo-description: Für Ihre Zielgruppen-Marketingaktivitäten müssen Sie ein Analytics-Zielgruppensegment in der Experience Cloud und in Adobe Target veröffentlichen.
seo-title: Veröffentlichen eines Analytics-Zielgruppensegments
solution: Experience Cloud
title: Veröffentlichen eines Analytics-Zielgruppensegments
uuid: 4201dc22-4b79-457c-a614-949bba087617
translation-type: tm+mt
source-git-commit: ae97db27349940a8df7ee2ba6678683f57585678

---


# Veröffentlichen eines Analytics-Zielgruppensegments

Für Ihre Zielgruppen-Marketingaktivitäten müssen Sie ein Analytics-Zielgruppensegment in der Experience Cloud und in Adobe Target veröffentlichen.

1. [Erstellen Sie in Analytics ein Segment](https://docs.adobe.com/content/help/en/analytics/components/segmentation/segmentation-workflow/seg-build.html).
1. Aktivieren Sie in Segment Builder die Option **[!UICONTROL Publish this segment to the Experience Cloud]**.

   ![](assets/ec_audience_example.png)

   | Element | Beschreibung |
   |--- |---|
   | Publish this segment to the Experience Cloud (für &lt;Name der Report Suite&gt;) | Veröffentlicht dieses Segment in Experience Cloud. Sie können die Zielgruppe für Marketing- und Segmentierungsaktivitäten in Adobe Target, Audience Manager, Advertising Cloud, Campaign und Audience Analytics verwenden.<br>Die Felder „Titel“ und „Beschreibung“ sind für die Veröffentlichung des Segments erforderlich.<br>Wenn diese Option deaktiviert ist, werden zwar Titel und Definition des Zielgruppensegments freigegeben, die eigentlichen Daten jedoch nicht. Wenn die Zielgruppe einer Aktivität in Target zugewiesen wird, beginnt Analytics damit, IDs für Besucher zu senden, die sich für diese Experience Cloud- und Target-Zielgruppe qualifizieren. Ab diesem Zeitpunkt werden der Zielgruppenname und die zugehörigen Daten auf der Experience Cloud Audiences-Seite angezeigt.<br>Zielgruppen, die von der Experience Cloud und Analytics gemeinsam verwendet werden, dürfen nicht mehr als 20 Millionen Zielgruppen-Mitglieder umfassen.<br>Aufgrund der Caching-Funktion wird die Löschung von Report Suites in Analytics erst nach 12 Stunden durch Experience Cloud übernommen.<br>Um ein in Experience Cloud veröffentlichtes Segment zu löschen, müssen Sie zuerst die Veröffentlichung rückgängig machen. Um die Veröffentlichung eines Segments rückgängig zu machen, **deaktivieren Sie einfach das Kontrollkästchen**, das Sie zum Veröffentlichen aktiviert haben. Sie können die Veröffentlichung eines Segments **nicht** rückgängig machen, das aktuell von einer der folgenden Adobe-Lösungen verwendet wird: [!DNL Analytics] (in [!DNL Audience Analytics]), [!DNL Campaign], [!DNL Advertising Cloud] (für Kunden von [!DNL Core Service] und [!DNL Audience Manager]) und alle anderen externen Partner (für Kunden von [!DNL Audience Manager]). Die Veröffentlichung eines Segments, das von [!DNL Target] verwendet wird, **kann** rückgängig gemacht werden.<br>Wenn ein Besucher in die in Analytics freigegebene Zielgruppe aufgenommen wird, ist diese Information erst mit einer Verzögerung von 24 bis 48 Stunden in Target, Advertising Cloud und Campaign verfügbar.<br>**Datenschutz**<br>Zielgruppen werden nicht nach dem Authentifizierungsstatus der Besucher gefiltert. Wenn Besucher Ihre Site sowohl authentifiziert als auch nicht authentifiziert anzeigen können, kann eine Aktion, die ein nicht authentifizierter Benutzer durchführt, dennoch dazu führen, dass der Besucher in die Zielgruppe aufgenommen wird. Welche Implikationen die Zielgruppenfreigabe auf den Datenschutz hat, lesen Sie unter [Übersicht über den Datenschutz in Analytics](https://docs.adobe.com/help/en/analytics/technotes/privacy-overview.html). |
   | Fenster für Zielgruppenerstellung auswählen | Beachten Sie, dass es sich um ein **rollierendes** Zeitfenster und kein festgelegtes Zeitfenster handelt. |

1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. Rufen Sie [!DNL Adobe Target] auf, klicken Sie auf [!UICONTROL Zielgruppen].
1. Suchen Sie auf der Seite [!UICONTROL Zielgruppen] die aus der Experience Cloud stammende Zielgruppe.

   Diese Zielgruppen sind für Aktivitäten verfügbar.
