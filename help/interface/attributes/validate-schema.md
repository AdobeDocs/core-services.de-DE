---
description: Hier erfahren Sie, wie Sie das Kundenattribut-Schema in Adobe Experience Cloud validieren.
keywords: Kundenattribute;Experience Cloud-Services
solution: Experience Cloud
title: 'Validieren des Kundenattribut-Schemas '
uuid: 163a4dbe-d60b-4089-8ff8-65f7461fbdf7
feature: 'Kundenattribute '
topic: Administration
role: Administrator
level: Erfahren
translation-type: tm+mt
source-git-commit: 61d60273e933c637dfe4400da78257e1c80015b3
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 98%

---


# Prüfen des Schemas

Der Prüfungsprozess ermöglicht die Zuordnung von Anzeigenamen und Beschreibungen zu den hochgeladenen Attributen (Zeichenfolgen, Ganzzahlen, Zahlen usw.). Basierend auf diesen Einstellungen wird ein Schema erstellt. Das Schema wird zur Überprüfung aller zukünftigen Daten verwendet, die in diese Datenquelle hochgeladen werden. Dieser Zuordnungsprozess ändert die Originaldaten nicht.

>[!NOTE]
>
>Durch die Aktualisierung des Schemas nach der Validierung werden Kundenattribute gelöscht. Siehe [Schema aktualisieren (auch Attribute löschen)](../attributes/t-crs-usecase.md#task_6568898BB7C44A42ABFB86532B89063C).

**[!UICONTROL Kunden-Attributquelle]** > **[!UICONTROL Neue Kundenattributquelle erstellen]** > **[!UICONTROL Schema anzeigen/bearbeiten]**

![](assets/view_edit_schema.png)

Auf der Seite „[!UICONTROL Schema überprüfen]“ stellt jede Schemazeile eine Spalte der hochgeladenen CSV-Datei dar.

![](assets/06_crs_usecase.png)

* **[!UICONTROL Daten hinzufügen:]** Lädt in diese Datenquelle neue Attributdaten hoch.

* **[!UICONTROL Schema anzeigen/bearbeiten:]** Ordnet den Attributdaten wie im nächsten Schritt beschrieben Anzeigenamen zu.

* **[!UICONTROL FTP-Einrichtung:]**[ Daten per FTP hochladen](../attributes/t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B).

* **[!UICONTROL ID-Suche:]** Geben Sie eine Kunden-ID (CID) aus Ihrer `.csv` ein, um Experience Cloud-Informationen für diese ID zu suchen. Diese Funktion eignet sich zum Beispiel für die Fehlerbehebung, wenn Sie herausfinden möchten, weshalb die Attributdaten eines bestimmten Besuchers nicht angezeigt werden:

   * **[!UICONTROL ECID (Experience Cloud ID):]** Zeigt an, ob Sie die neueste Version des Experience Cloud ID-Dienstes verwenden. Wenn Sie den MCID-Dienst nutzen, aber hier keine IDs aufgelistet sind, hat Experience Cloud keinen Alias für diese CID erhalten. Der Besucher hat sich also entweder nicht angemeldet, oder Ihre Implementierung lässt diese ID nicht durch.

   * **[!UICONTROL CID (Customer ID):]** Die mit dieser CID verbundenen Attribute. Wenn Sie eine prop oder eVar zum Hochladen von CIDs (AVID) verwenden und Attribute angezeigt werden, aber keine AVID, hat sich der Besucher vermutlich nicht bei Ihrer Site angemeldet.

   * **[!UICONTROL AVID (Analytics-Besucher-ID):]** Zeigt an, ob Sie eine „prop“ oder „eVar“ zum Hochladen von CIDs verwenden. Wenn diese IDs an Experience Cloud weitergegeben werden, werden hier die Besucher-IDs angezeigt, die mit der von Ihnen eingegebenen CID verknüpft sind.

Sie können Daten auch via FTP hochladen, nachdem Sie eine Kundenattributquelle und ein FTP-Konto in der Experience Cloud erstellt haben. Pro Attributquelle erstellen Sie ein FTP-Konto. Die hochgeladenen Dateien werden im Stammordner dieses Kontos gespeichert. Die Daten müssen im .csv-Format übertragen werden, wobei eine zweite .fin-Datei angibt, dass das Hochladen abgeschlossen ist.

Die Namen, die Sie den Zeichenfolgen, Ganzzahlen und Nummern geben, werden zur Erstellung der [!DNL Analytics]-Metriken verwendet. Weitere Informationen finden Sie unter [Bericht „Kundenattribute“](https://docs.adobe.com/content/help/de-DE/core-services/interface/customer-attributes/attributes.html) in der [!DNL Analytics]-Hilfe.

* **[!UICONTROL Attribut:]** Die aus der hochgeladenen `.csv`-Datei gelesenen Attributdaten.

* **[!UICONTROL Typ:]** Datentyp, z. B.:

   * **Zeichenfolge:** Eine Folge von Zeichen.

   * **Ganzzahlen:** Ganze Zahlen.

   * **Zahlen:** Kann bis zu zwei Dezimalstellen haben.

* **[!UICONTROL Anzeigename:]** Ein benutzerfreundlicher Anzeigename für das Attribut. Beispielsweise können Sie das Attribut *Kundenalter* in *Kunde seit* ändern.

* **[!UICONTROL Beschreibung:]** Eine benutzerfreundliche Beschreibung des Attributs.
