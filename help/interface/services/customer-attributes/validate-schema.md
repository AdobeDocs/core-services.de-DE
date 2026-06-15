---
description: Erfahren Sie, wie Sie das  [!DNL Customer Attributes] -Schema in Adobe CX Enterprise validieren.
solution: Experience Cloud
title: 'Validieren des Schemas [!DNL Customer Attributes] '
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 776d1fd3-c733-4970-a76b-4c3c0119ee77
TQID: https://experienceleague.adobe.com/J-AaDn4HtD1bS-VCPn2XiPLVBbTnYyl5o1NpJ9HFj1g
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: b75843fa-0a67-4a44-a6b1-cc627b0481dcid: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 345
ht-degree: 39%

---

# Schema prüfen

Der Prüfungsprozess ermöglicht die Zuordnung von Anzeigenamen und Beschreibungen zu den hochgeladenen Attributen (Zeichenfolgen, Ganzzahlen, Zahlen usw.).

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

   ![Schemaseite in CX Enterprise bearbeiten](assets/schema-edit.png)

**Aktionen**

* **[!UICONTROL Daten hinzufügen]** Laden Sie neue Attributdaten in diese Datenquelle hoch.

* **[!UICONTROL Schema anzeigen/bearbeiten]** Ordnen Sie den Attributdaten Anzeigenamen zu, wie im nächsten Schritt beschrieben.

* **[!UICONTROL FTP-Einrichtung:]** Erstellen Sie Ihr FTP-Konto, um [Ihre Daten via FTP hochzuladen](t-upload-attributes-ftp.md) (optional).

* **[!UICONTROL ID-Suche]** Geben Sie eine Kunden-ID (CID) aus Ihrem `.csv` ein, um CX Enterprise-Informationen für die ID zu suchen. Diese Funktion eignet sich zum Beispiel für die Fehlerbehebung, wenn Sie herausfinden möchten, weshalb die Attributdaten eines bestimmten Besuchers nicht angezeigt werden:

   * **[!UICONTROL ECID (CX Enterprise ID):]** Wird angezeigt, wenn Sie den neuesten CX Enterprise ID-Service verwenden. Wenn Sie den MCID-Service verwenden, aber hier keine IDs aufgeführt sind, hat CX Enterprise keinen Alias für diese CID erhalten. Der Besucher hat sich also entweder nicht angemeldet, oder Ihre Implementierung lässt diese ID nicht durch.

   * **[!UICONTROL CID (Kunden-ID):]** Die mit dieser CID verknüpften Attribute. Wenn Sie eine prop oder eVar zum Hochladen von CIDs (AVID) verwenden und Attribute angezeigt werden, aber keine AVID, hat sich der Besucher vermutlich nicht bei Ihrer Site angemeldet.

   * **[!UICONTROL AVID (Analytics-Besucher-ID):]** Wird angezeigt, wenn Sie zum Hochladen von CIDs ein Prop oder eVar verwenden. Wenn diese IDs an CX Enterprise übergeben werden, werden hier alle Besucher-IDs angezeigt, die mit der eingegebenen CID verknüpft sind.
