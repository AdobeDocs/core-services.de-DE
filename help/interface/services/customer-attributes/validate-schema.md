---
description: Erfahren Sie, wie Sie das  [!DNL Customer Attributes] -Schema in Adobe Experience Cloud validieren.
solution: Experience Cloud
title: 'Validieren des Schemas [!DNL Customer Attributes] '
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 776d1fd3-c733-4970-a76b-4c3c0119ee77
source-git-commit: d2244e249c7af27bc1b4fc7bfe628bc25b37f4d4
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 49%

---

# Prüfen Sie das Schema

Beim Validierungsprozess können Sie hochgeladenen Attributen Anzeigenamen und Beschreibungen (Zeichenfolgen, Ganzzahlen, Zahlen usw.) zuordnen.

Basierend auf diesen Einstellungen wird ein Schema erstellt. Das Schema wird zur Überprüfung aller zukünftigen Daten verwendet, die in diese Datenquelle hochgeladen werden. Der Zuordnungsprozess ändert die Originaldaten nicht.

>[!NOTE]
>
>Durch die Aktualisierung des Schemas nach der Validierung werden Kundenattribute gelöscht. Siehe [Schema aktualisieren (auch Attribute löschen)](t-crs-usecase.md).

**Prüfen Sie das Schema**

1. Klicken Sie [!DNL Customer Attributes] auf die Attributquelle, die Sie bearbeiten möchten.

1. Klicken Sie auf der **[!UICONTROL Kundenattribut-Source bearbeiten]** auf **[!UICONTROL Datei-Upload]**.

1. Klicken Sie auf der Seite [!UICONTROL Datei-Upload und ]-Validierung auf **[!UICONTROL Aktionen]** > **[!UICONTROL Schema anzeigen/bearbeiten]**

   ![Schema bearbeiten](assets/actions.png)

   Auf der [!UICONTROL Schema bearbeiten] stellt jede Schemazeile eine Spalte der hochgeladenen CSV-Datei dar.

   ![Schemaseite in Experience Cloud bearbeiten](assets/schema-edit.png)

**Aktionen**

* **[!UICONTROL Daten hinzufügen:]** Lädt in diese Datenquelle neue Attributdaten hoch.

* **[!UICONTROL Schema anzeigen/bearbeiten:]** Ordnet den Attributdaten wie im nächsten Schritt beschrieben Anzeigenamen zu.

* **[!UICONTROL FTP-Einrichtung:]** Erstellen Sie Ihr FTP-Konto, um [Ihre Daten via FTP hochzuladen](t-upload-attributes-ftp.md) (optional).

* **[!UICONTROL ID-Suche:]** Geben Sie eine Kunden-ID (CID) aus Ihrer `.csv` ein, um Experience Cloud-Informationen für die ID zu suchen. Diese Funktion eignet sich zum Beispiel für die Fehlerbehebung, wenn Sie herausfinden möchten, weshalb die Attributdaten eines bestimmten Besuchers nicht angezeigt werden:

   * **[!UICONTROL ECID (Experience Cloud ID):]** Zeigt an, ob Sie die neueste Version des Experience Cloud ID-Dienstes verwenden. Wenn Sie sich im MCID-Service befinden, hier jedoch keine IDs aufgeführt sind, hat Experience Cloud keinen Alias für diese CID erhalten. Der Besucher hat sich also entweder nicht angemeldet, oder Ihre Implementierung lässt diese ID nicht durch.

   * **[!UICONTROL CID (Kunden-ID):]** Die mit dieser CID verknüpften Attribute. Wenn Sie eine prop oder eVar zum Hochladen von CIDs (AVID) verwenden und Attribute angezeigt werden, aber keine AVID, hat sich der Besucher vermutlich nicht bei Ihrer Site angemeldet.

   * **[!UICONTROL AVID (Analytics-Besucher-ID):]** Zeigt an, ob Sie eine „prop“ oder „eVar“ zum Hochladen von CIDs verwenden. Wenn diese IDs an Experience Cloud übergeben werden, werden hier alle Besucher-IDs angezeigt, die mit der eingegebenen CID verknüpft sind.
