---
description: Erfahren Sie, wie Sie das  [!DNL Customer Attributes] -Schema in Adobe Experience Cloud validieren.
solution: Experience Cloud
title: 'Validieren des Schemas [!DNL Customer Attributes] '
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 776d1fd3-c733-4970-a76b-4c3c0119ee77
source-git-commit: a1cfa6c69d8e95ceb0d4c3c72c24541867173fcc
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 37%

---

# Schema prüfen

Beim Validierungsprozess können Sie hochgeladenen Attributen Anzeigenamen und Beschreibungen (Zeichenfolgen, Ganzzahlen, Zahlen usw.) zuordnen.

Basierend auf diesen Einstellungen wird ein Schema erstellt. Das Schema wird zur Überprüfung aller zukünftigen Daten verwendet, die in diese Datenquelle hochgeladen werden. Der Zuordnungsprozess ändert die Originaldaten nicht.

>[!NOTE]
>
>Durch die Aktualisierung des Schemas nach der Validierung werden Kundenattribute gelöscht. Siehe [Schema aktualisieren (auch Attribute löschen)](t-crs-usecase.md).

**Prüfen Sie das Schema**

1. Klicken Sie [!DNL Customer Attributes] auf die Attributquelle, die Sie bearbeiten möchten.

1. Klicken Sie auf der **[!UICONTROL Edit Customer Attribute Source]** auf **[!UICONTROL File Upload]**.

1. Klicken Sie auf der [!UICONTROL File Upload and Schema Validation] Seite auf **[!UICONTROL Actions]** > **[!UICONTROL View/Edit Schema]**

   ![Schema bearbeiten](assets/actions.png)

   Auf der Seite [!UICONTROL Edit Schema] stellt jede Schemazeile eine Spalte der hochgeladenen CSV-Datei dar.

   ![Schemaseite in Experience Cloud bearbeiten](assets/schema-edit.png)

**Aktionen**

* **[!UICONTROL Add Data:]** Laden Sie neue Attributdaten in diese Datenquelle hoch.

* **[!UICONTROL View/Edit Schema:]** Ordnen Sie den Attributdaten Anzeigenamen zu, wie im nächsten Schritt beschrieben.

* **[!UICONTROL FTP Setup:]** Erstellen Sie Ihr FTP-Konto, um [Ihre Daten via FTP hochzuladen](t-upload-attributes-ftp.md) (optional).

* **[!UICONTROL ID Lookup:]** Geben Sie eine Kunden-ID (CID) aus Ihrem `.csv` ein, um Experience Cloud-Informationen für die ID zu suchen. Diese Funktion eignet sich zum Beispiel für die Fehlerbehebung, wenn Sie herausfinden möchten, weshalb die Attributdaten eines bestimmten Besuchers nicht angezeigt werden:

   * **[!UICONTROL ECID (Experience Cloud ID):]** Wird angezeigt, wenn Sie den neuesten Experience Cloud ID-Service verwenden. Wenn Sie sich im MCID-Service befinden, hier jedoch keine IDs aufgeführt sind, hat Experience Cloud keinen Alias für diese CID erhalten. Der Besucher hat sich also entweder nicht angemeldet, oder Ihre Implementierung lässt diese ID nicht durch.

   * **[!UICONTROL CID (customer ID):]** Die dieser CID zugeordneten Attribute. Wenn Sie eine prop oder eVar zum Hochladen von CIDs (AVID) verwenden und Attribute angezeigt werden, aber keine AVID, hat sich der Besucher vermutlich nicht bei Ihrer Site angemeldet.

   * **[!UICONTROL AVID (Analytics visitor ID):]** Wird angezeigt, wenn Sie zum Hochladen von CIDs ein Prop oder eVar verwenden. Wenn diese IDs an Experience Cloud übergeben werden, werden hier alle Besucher-IDs angezeigt, die mit der eingegebenen CID verknüpft sind.

