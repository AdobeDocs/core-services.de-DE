---
description: Hier erfahren Sie, wie Sie das Kundenattribut-Schema in Adobe Experience Cloud validieren.
solution: Experience Cloud
title: Validieren des Kundenattribut-Schemas
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 776d1fd3-c733-4970-a76b-4c3c0119ee77
source-git-commit: 2f126877f6a5f090884ebe093f35e4f6d90b4df6
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 72%

---

# Prüfen Sie das Schema

Der Prüfungsprozess ermöglicht die Zuordnung von Anzeigenamen und Beschreibungen zu den hochgeladenen Attributen (Zeichenfolgen, Ganzzahlen, Zahlen usw.). Basierend auf diesen Einstellungen wird ein Schema erstellt. Das Schema wird zur Überprüfung aller zukünftigen Daten verwendet, die in diese Datenquelle hochgeladen werden. Der Zuordnungsprozess ändert die Originaldaten nicht.

>[!NOTE]
>
>Durch die Aktualisierung des Schemas nach der Validierung werden Kundenattribute gelöscht. Siehe [Schema aktualisieren (auch Attribute löschen)](t-crs-usecase.md).

**[!UICONTROL Kundenattribut Source]** > **[!UICONTROL Neues Kundenattribut Source erstellen]** > **[!UICONTROL Schema anzeigen/bearbeiten]**

![Schema bearbeiten](assets/view_edit_schema.png)

Auf der Seite [!UICONTROL Schema bearbeiten] stellt jede Schemazeile eine Spalte der hochgeladenen CSV-Datei dar.

![Validieren der Schemaseite in Experience Cloud](assets/06_crs_usecase.png)

* **[!UICONTROL Daten hinzufügen:]** Lädt in diese Datenquelle neue Attributdaten hoch.

* **[!UICONTROL Schema anzeigen/bearbeiten:]** Ordnet den Attributdaten wie im nächsten Schritt beschrieben Anzeigenamen zu.

* **[!UICONTROL FTP-Einrichtung:]**&#x200B;[ Daten per FTP hochladen](t-upload-attributes-ftp.md).

* **[!UICONTROL ID-Suche:]** Geben Sie eine Kunden-ID (CID) aus Ihrer `.csv` ein, um Experience Cloud-Informationen für die ID zu suchen. Diese Funktion eignet sich zum Beispiel für die Fehlerbehebung, wenn Sie herausfinden möchten, weshalb die Attributdaten eines bestimmten Besuchers nicht angezeigt werden:

   * **[!UICONTROL ECID (Experience Cloud ID):]** Zeigt an, ob Sie die neueste Version des Experience Cloud ID-Dienstes verwenden. Wenn Sie sich im MCID-Service befinden, hier jedoch keine IDs aufgeführt sind, hat Experience Cloud keinen Alias für diese CID erhalten. Der Besucher hat sich also entweder nicht angemeldet, oder Ihre Implementierung lässt diese ID nicht durch.

   * **[!UICONTROL CID (Kunden-ID):]** Die mit dieser CID verknüpften Attribute. Wenn Sie eine prop oder eVar zum Hochladen von CIDs (AVID) verwenden und Attribute angezeigt werden, aber keine AVID, hat sich der Besucher vermutlich nicht bei Ihrer Site angemeldet.

   * **[!UICONTROL AVID (Analytics-Besucher-ID):]** Zeigt an, ob Sie eine „prop“ oder „eVar“ zum Hochladen von CIDs verwenden. Wenn diese IDs an Experience Cloud übergeben werden, werden hier alle Besucher-IDs angezeigt, die mit der eingegebenen CID verknüpft sind.

Sie können Daten auch via FTP hochladen, nachdem Sie eine Kundenattributquelle und ein FTP-Konto in Experience Cloud erstellt haben. Pro Attributquelle erstellen Sie ein FTP-Konto. Die hochgeladenen Dateien werden im Stammordner dieses Kontos gespeichert. Die Daten müssen im `.csv`-Format übertragen werden, wobei eine zweite `.fin`-Datei am Ende angibt, dass das Hochladen abgeschlossen ist.

Die Namen, die Sie den Zeichenfolgen, Ganzzahlen und Nummern geben, werden zur Erstellung der [!DNL Analytics]-Metriken verwendet.

* **[!UICONTROL attribute:]** Attributdaten werden aus der hochgeladenen `.csv`-Datei gelesen.

* **[!UICONTROL Typ:]** Datentyp, z. B.:

   * **Zeichenfolge:** Eine Folge von Zeichen.

   * **Ganzzahlen:** Ganze Zahlen.

   * **Zahlen:** Kann bis zu zwei Dezimalstellen haben.

* **[!UICONTROL Anzeigename:]** Ein benutzerfreundlicher Anzeigename für das Attribut. Sie können beispielsweise das Attribut *Kundenalter) in* Kunde seit *ändern*.

* **[!UICONTROL Beschreibung:]** Eine benutzerfreundliche Beschreibung des Attributs.
