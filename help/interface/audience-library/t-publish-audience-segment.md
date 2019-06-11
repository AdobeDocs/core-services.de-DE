---
description: Für Ihre Zielgruppen-Marketingaktivitäten müssen Sie ein Analytics-Zielgruppensegment in der Experience Cloud und in Adobe Target veröffentlichen.
keywords: Hauptdienste
seo-description: Für Ihre Zielgruppen-Marketingaktivitäten müssen Sie ein Analytics-Zielgruppensegment in der Experience Cloud und in Adobe Target veröffentlichen.
seo-title: Veröffentlichen eines Analytics-Zielgruppensegments
solution: Experience Cloud
title: Veröffentlichen eines Analytics-Zielgruppensegments
uuid: 4201 dc 22-4 b 79-457 c-a 614-949 bba 87617
translation-type: tm+mt
source-git-commit: 85879d92104d8b6d739fb4d17dc8cfb7483a9343

---


# Veröffentlichen eines Analytics-Zielgruppensegments

Für Ihre Zielgruppen-Marketingaktivitäten müssen Sie ein Analytics-Zielgruppensegment in der Experience Cloud und in Adobe Target veröffentlichen.

1. [Erstellen Sie in Analytics ein Segment](https://marketing.adobe.com/resources/help/en_US/analytics/segment/seg_build.html).
1. Aktivieren Sie im Segmentaufbau die **[!UICONTROL Option Make This Form Cloud Audience]** .

   ![](assets/ec_audience_example.png)

   | Element | Beschreibung |
   |--- |---|
   | Als Experience Cloud-Zielgruppe festlegen (für &lt;report suite name&gt;) | Veröffentlicht dieses Segment in Experience Cloud. Die Zielgruppe können Sie für Marketingaktivitäten in Adobe Target und für die Segmentierung in Audience Manager verwenden.<br>Die Felder „Titel“ und „Beschreibung“ sind für die Veröffentlichung des Segments erforderlich.<br>Wenn diese Option deaktiviert ist, werden zwar Titel und Definition des Zielgruppensegments freigegeben, die eigentlichen Daten jedoch nicht. Wenn die Zielgruppe einer Aktivität in Target zugewiesen wird, beginnt Analytics damit, IDs für Besucher zu senden, die sich für diese Experience Cloud- und Target-Zielgruppe qualifizieren. Ab diesem Zeitpunkt werden der Zielgruppenname und die zugehörigen Daten auf der Experience Cloud Audiences-Seite angezeigt.<br>Zielgruppen, die für die Experience Cloud aus Analytics freigegeben wurden, dürfen 20 Millionen Mitglieder nicht überschreiten.<br>Aufgrund der Zwischenspeicherung müssen Report Suites in Analytics 12 Stunden vor dem Löschen in der Experience Cloud angezeigt werden.<br>In Analytics können Sie ein veröffentlichtes Segment bearbeiten oder löschen. Wird das Segment aktuell verwendet, wird ein Warnhinweis eingeblendet, wenn Sie das Segment bearbeiten. Ein veröffentlichtes Segment, das aktuell in Adobe Target verwendet wird, kann nicht gelöscht werden.<br>Wenn ein Besucher für die aus Analytics freigegebene Zielgruppe qualifiziert ist, gibt es eine Verzögerung von 24 bis 48 Stunden, bevor diese Informationen in Target, Advertising Cloud und Campaign nachvollziehbar sind.<br>**Data privacyaudiences**<br>wird nicht basierend auf dem Authentifizierungsstatus eines Besuchers gefiltert. Wenn Besucher Ihre Site sowohl authentifiziert als auch nicht authentifiziert anzeigen können, kann eine Aktion, die ein nicht authentifizierter Benutzer durchführt, dennoch dazu führen, dass der Besucher in die Zielgruppe aufgenommen wird. Welche Implikationen die Zielgruppenfreigabe auf den Datenschutz hat, lesen Sie unter [Übersicht über den Datenschutz in Analytics](https://marketing.adobe.com/resources/help/en_US/reference/?f=c_Privacy_Overview). |
   | Fenster für Zielgruppenerstellung auswählen | Beachten Sie, dass es sich um ein **rollierendes** Zeitfenster und kein festgelegtes Zeitfenster handelt. |

1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. Zugriff [!DNL Adobe Target], klicken Sie auf [!UICONTROL Zielgruppen].
1. Suchen Sie auf der Seite [!UICONTROL Zielgruppen] die Zielgruppe, die aus der Experience Cloud stammt.

   Diese Zielgruppen sind für Aktivitäten verfügbar.
