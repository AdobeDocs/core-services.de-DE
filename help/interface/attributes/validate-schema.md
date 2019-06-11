---
description: Der Prüfungsprozess ermöglicht die Zuordnung von Anzeigenamen und Beschreibungen zu den hochgeladenen Attributen (Zeichenfolgen, Ganzzahlen, Zahlen usw.). Aus diesen Einstellungen wird ein Schema erstellt, das zur Prüfung aller in Zukunft in diese Datenquelle hochgeladenen Daten verwendet wird. Die ursprünglichen Daten bleiben durch diese Zuordnung unverändert.
keywords: Kundenattribute; Hauptdienste
seo-description: Der Prüfungsprozess ermöglicht die Zuordnung von Anzeigenamen und Beschreibungen zu den hochgeladenen Attributen (Zeichenfolgen, Ganzzahlen, Zahlen usw.). Aus diesen Einstellungen wird ein Schema erstellt, das zur Prüfung aller in Zukunft in diese Datenquelle hochgeladenen Daten verwendet wird. Die ursprünglichen Daten bleiben durch diese Zuordnung unverändert.
seo-title: Prüfen des Schemas
solution: Experience Cloud
title: Prüfen des Schemas
uuid: 163 a 4 dbe-d 60 b -4089-8 ff 8-65 f 7461 fbdf 7
translation-type: tm+mt
source-git-commit: 979b2202a70e2a5362aa86a65a17d7c4279b3a1a

---


# Prüfen des Schemas

Der Prüfungsprozess ermöglicht die Zuordnung von Anzeigenamen und Beschreibungen zu den hochgeladenen Attributen (Zeichenfolgen, Ganzzahlen, Zahlen usw.). Aus diesen Einstellungen wird ein Schema erstellt, das zur Prüfung aller in Zukunft in diese Datenquelle hochgeladenen Daten verwendet wird. Die ursprünglichen Daten bleiben durch diese Zuordnung unverändert.


>[!NOTE]
>
>Wenn Sie das Schema nach der Validierung aktualisieren, werden Kundenattribute gelöscht. Siehe Schema [aktualisieren (auch Attribute löschen)](../attributes/t-crs-usecase.md#task_6568898BB7C44A42ABFB86532B89063C).


**[!UICONTROL Kundenattributquelle]** &gt; **[!UICONTROL Neue Kunden-Attributquelle erstellen]** &gt; Schema **[!UICONTROL anzeigen/bearbeiten]**

![](assets/view_edit_schema.png)

Auf der Seite „[!UICONTROL Schema überprüfen]“ stellt jede Schemazeile eine Spalte der hochgeladenen CSV-Datei dar.

![](assets/06_crs_usecase.png)

* **[!UICONTROL Daten hinzufügen:]** Laden Sie neue Attributdaten in diese Datenquelle hoch.

* **[!UICONTROL Schema anzeigen/bearbeiten:]** Ordnen Sie die Anzeigenamen den Attributdaten zu, wie im nächsten Schritt beschrieben.

* **[!UICONTROL FTP-Einrichtung:]**[Laden Sie die Daten per FTP hoch](../attributes/t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B).

* **[!UICONTROL ID-Suche:]** Geben Sie eine Kunden-ID (CID) aus Ihrer [!DNL .csv] zum Suchen der Experience Cloud-Informationen für die ID ein. Diese Funktion eignet sich zum Beispiel für die Fehlerbehebung, wenn Sie herausfinden möchten, weshalb die Attributdaten eines bestimmten Besuchers nicht angezeigt werden:

   * **[!UICONTROL MCID (Experience Cloud ID):]** Wird angezeigt, wenn Sie den neuesten Experience Cloud ID-Dienst verwenden. Wenn Sie den MCID-Dienst verwenden, hier aber keine IDs angezeigt werden, hat die Experience Cloud keinen Alias für diese CID erhalten. Der Besucher hat sich also entweder nicht angemeldet, oder Ihre Implementierung lässt diese ID nicht durch.

   * **[!UICONTROL CID (Kunden-ID):]** Die mit dieser CID verknüpften Attribute. Wenn Sie eine prop oder eVar zum Hochladen von CIDs (AVID) verwenden und Attribute angezeigt werden, aber keine AVID, hat sich der Besucher vermutlich nicht bei Ihrer Site angemeldet.

   * **[!UICONTROL AVID (Analytics Besucher-ID):]** Wird angezeigt, wenn Sie eine prop oder evar zum Hochladen von cids verwenden. Wenn diese IDs an die Experience Cloud weitergeleitet werden, werden hier alle mit der angegebenen CID verbundenen-Besucher-IDs angezeigt.






Wenn Sie in der Experience Cloud eine Kundenattributquelle und ein FTP-Konto erstellt haben, können Sie die Daten auch via FTP hochladen. Pro Attributquelle müssen Sie ein FTP-Konto erstellen. Die hochgeladenen Dateien werden im Stammordner dieses Kontos gespeichert. Die Daten müssen im .csv-Format übertragen werden, wobei eine zusätzliche .fin-Datei am Ende angibt, dass das Upload abgeschlossen ist.

Die Namen, die Sie auf Zeichenfolgen, Ganzzahlen und Zahlen anwenden, werden zum Erstellen [!DNL Analytics] von Metriken verwendet. Weitere [Informationen finden Sie in](https://marketing.adobe.com/resources/help/en_US/reference/?f=reports_customer_attributes) der [!DNL Analytics] Hilfe unter Kundenattribute.

* **[!UICONTROL Attribut:]** Aus der hochgeladenen [!DNL .csv] Datei gelesene Attributdaten.

* **[!UICONTROL Typ:]** Der Datentyp, z. B.:

   * **Zeichenfolge:** eine Folge von Zeichen

   * **Ganzzahl:** ganze Zahlen

   * **Zahl:** Zahl mit bis zu zwei Nachkommastellen




* **[!UICONTROL Anzeigename:]** Ein Anzeigename für das Attribut. Sie können z. B. ein Alter *des Attributs Kundenkunde* in *Kunden ändern*.

* **[!UICONTROL Beschreibung:]** Eine benutzerfreundliche Beschreibung des Attributs.



