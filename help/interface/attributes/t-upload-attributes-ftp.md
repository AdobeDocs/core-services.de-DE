---
description: Wenn Sie die Kundenattributdaten nicht per Drag-and-Drop in die Experience Cloud hochladen, können Sie die Daten auch via FTP hochladen.
keywords: Kundenattribute; Hauptdienste
seo-description: Wenn Sie die Kundenattributdaten nicht per Drag-and-Drop in die Experience Cloud hochladen, können Sie die Daten auch via FTP hochladen.
seo-title: Optional – Hochladen der Datendatei via FTP
solution: Experience Cloud
title: Optional – Hochladen der Datendatei via FTP
uuid: 5df565dd-b6f8-420e-981f-4b6fc6f7d0e4
translation-type: tm+mt
source-git-commit: f8b48077d936e289d66c1a93a96fe9ebaa4f0136

---


# Optional – Hochladen der Datendatei via FTP

Wenn Sie die Kundenattributdaten nicht per Drag-and-Drop in die Experience Cloud hochladen, können Sie die Daten auch via FTP hochladen.

Sie können die Daten hochladen, nachdem Sie in der Experience Cloud eine Kundenattributquelle und ein FTP-Konto erstellt haben. Pro Attributquelle müssen Sie ein FTP-Konto erstellen. Die hochgeladenen Dateien werden im Stammordner dieses Kontos gespeichert. Die Daten müssen im `.csv`-Format übertragen werden, wobei eine zusätzliche `.fin`-Datei am Ende angibt, dass das Hochladen abgeschlossen ist.

>[!IMPORTANT]
>
>Lesen Sie [Datendateivoraussetzungen für das Hochladen von Kundenattributen](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19), bevor Sie die Datei hochladen.


Datei-Uploads auf die FTP-Site mit den Kundenattributdaten kann via FTP oder SFTP erfolgen.

* Für SFTP benötigen Sie allerdings einen Client, der SFTP-Verbindungen unterstützt.
* Die Verbindung über SFTP können Sie mit Benutzernamen und Passwort oder, wie [hier](https://marketing.adobe.com/resources/help/en_US/whitepapers/ftp/?f=ftp_sftp_cert_auth) beschrieben, ohne Passwort herstellen.



<!-- <p>Error states - get with Matt and Dave </p> 
<p>What are the most common reasons for doing this? Retail? Do a use case example, then show an AN example. </p> 
<p>You create one FTP per attribute source. Files go to the root folder in that account. The file type .fin is user-created. (For example, upload a .csv then a .fin of the same name, which signals you have completed the upload. https://wiki.corp.adobe.com/display/marketingcloud/Customer+Record+Services#CustomerRecordServices-FileFormats (leverage for doc). Possibly link from FTP File Reqs page to a help file about naming conventions. Need a new file type page for this. Similar content here: https://marketing.adobe.com/resources/help/en_US/reference/c_general_file_structure.html and here: https://marketing.adobe.com/resources/help/en_US/whitepapers/ftp/ftp_datasources.html </p> 
<p>Drag-n-drop and zip functionality for uploads - 1/21/2015. S/b less than 100 megs for drag and drop zip file. Fin file not required for drag/drop. </p> 
<p>Preview Data - shows the last upload (?) </p> 
<p>Need a link to the "instructions" on that information icon with the image. </p> 
<p>Workflow: Drag and drop, validate schema, configure subscription, save/activate. </p> -->
**So laden Sie die Datendatei via FTP hoch**

1. [Erstellen einer Kundenattributquelle und Hochladen der Datendatei...](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

   Vergewissern Sie sich, dass Sie unter [!DNL ftp.adobe.com/ bei Ihrer FTP-Site angemeldet sind.<sftpname>].

1. Klicken Sie auf **[!UICONTROL Aktionen]** &gt; **[!UICONTROL Datei hochladen]**.

1. Laden Sie eine `.fin`-Datei hoch, damit Ihre Datei abgerufen werden kann.

   Der Dateityp `.fin` wird vom Benutzer erstellt und signalisiert, dass das Hochladen abgeschlossen ist. Sie kann eine leere Editor-Datei sein. Wenn Sie beispielsweise [!DNL crs123.csv] hochladen, wird auch [!DNL crs123.fin] hochgeladen.

   Nach einem erfolgreichen Upload werden beide Dateien in einen Ordner mit dem Namen **processed** verschoben.


   Siehe [Datendateivoraussetzungen für das Hochladen von Kundenattributen](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19), wo Sie wichtige Informationen zu Dateinamen und zur Dateistruktur erhalten.
