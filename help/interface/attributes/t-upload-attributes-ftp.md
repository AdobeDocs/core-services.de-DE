---
description: Wenn Sie die Kundenattributdaten nicht per Drag & Drop in die Experience Cloud hochladen, können Sie die Daten auch via FTP hochladen.
keywords: Customer Attributes;core services
seo-description: Wenn Sie die Kundenattributdaten nicht per Drag & Drop in die Experience Cloud hochladen, können Sie die Daten auch via FTP hochladen.
seo-title: Optional – Hochladen der Datendatei via FTP
solution: Experience Cloud
title: Optional – Hochladen der Datendatei via FTP
uuid: 5df565dd-b6f8-420e-981f-4b6fc6f7d0e4
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 85%

---


# Optional – Hochladen der Datendatei via FTP

Wenn Sie die Kundenattributdaten nicht per Drag &amp; Drop in die Experience Cloud hochladen, können Sie die Daten auch via FTP hochladen.

Sie können die Daten hochladen, nachdem Sie eine Kundenattributquelle und ein FTP-Konto in der Experience Cloud erstellt haben. Pro Attributquelle erstellen Sie ein FTP-Konto. Die hochgeladenen Dateien werden im Stammordner dieses Kontos gespeichert. Die Daten müssen im `.csv`-Format übertragen werden, wobei eine zusätzliche `.fin`-Datei am Ende angibt, dass das Hochladen abgeschlossen ist.

>[!IMPORTANT]
>
>Review [Data file requirements for uploading Customer Attributes](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) before uploading the file.

Datei-Uploads auf die FTP-Site &quot;Kundenattribute&quot;können über FTP oder SFTP erfolgen.

* Sie benötigen einen Client, der SFTP-Verbindungen unterstützt.
* Sie können eine Verbindung mit SFTP entweder mit dem Benutzernamen/Kennwort oder ohne Kennwort herstellen, wie [hier](https://docs.adobe.com/help/de-DE/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html) beschrieben.

**So laden Sie die Datendatei via FTP hoch**

1. [Erstellen einer Kundenattributquelle und Hochladen der Datendatei...](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

   Vergewissern Sie sich, dass Sie unter [!DNL ftp.adobe.com/ bei Ihrer FTP-Site angemeldet sind.<sftpname>].

1. Klicken Sie auf **[!UICONTROL Aktionen]** > **[!UICONTROL Datei hochladen]**.

1. Laden Sie eine `.fin`-Datei hoch, damit Ihre Datei abgerufen werden kann.

   Der Dateityp `.fin` wird vom Benutzer erstellt und signalisiert, dass das Hochladen abgeschlossen ist. Sie kann eine leere Editor-Datei sein. Wenn Sie beispielsweise [!DNL crs123.csv] hochladen, wird auch [!DNL crs123.fin] hochgeladen.

   Wenn der Upload erfolgreich war, werden beide Dateien in einen Ordner mit dem Namen **verarbeitet** verschoben.

   See [Data file requirements for uploading Customer Attributes](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) for important information about file names and structure.
