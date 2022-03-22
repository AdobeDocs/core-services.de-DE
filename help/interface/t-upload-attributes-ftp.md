---
description: Erfahren Sie, wie Sie Kundenattributdaten per FTP in Experience Cloud hochladen.
keywords: Kundenattribute;zentrale Services
solution: Experience Cloud
title: 'Upload der Datendatei für Kundenattribute über FTP '
uuid: 5df565dd-b6f8-420e-981f-4b6fc6f7d0e4
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: ed9e4a8f-493a-4a0f-a87e-674c7da95b99
source-git-commit: 1fb1abc7311573f976f7e6b6ae67f60ada10a3e7
workflow-type: ht
source-wordcount: '268'
ht-degree: 100%

---

# Optional – Hochladen der Datendatei via FTP

Wenn Sie die Kundenattributdaten nicht per Drag &amp; Drop in die Experience Cloud hochladen, können Sie die Daten auch via FTP hochladen.

Sie können die Daten hochladen, nachdem Sie eine Kundenattributquelle und ein FTP-Konto in der Experience Cloud erstellt haben. Pro Attributquelle erstellen Sie ein FTP-Konto. Die hochgeladenen Dateien werden im Stammordner dieses Kontos gespeichert. Die Daten müssen im `.csv`-Format übertragen werden, wobei eine zweite `.fin`-Datei angibt, dass das Hochladen abgeschlossen ist.

>[!IMPORTANT]
>
>Lesen Sie [Datendateivoraussetzungen für das Hochladen von Kundenattributen](crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19), bevor Sie die Datei hochladen.

Datei-Uploads auf die FTP-Site für Kundenattribute können über FTP oder SFTP erfolgen:

* Sie benötigen einen Client, der SFTP-Verbindungen unterstützt.
* Sie können eine Verbindung mit SFTP entweder mit dem Benutzernamen/Kennwort oder ohne Kennwort herstellen, wie [hier](https://experienceleague.adobe.com/docs/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html?lang=de) beschrieben.

**So laden Sie die Datendatei via FTP hoch**

1. [Erstellen einer Kundenattributquelle und Hochladen der Datendatei...](t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

   Vergewissern Sie sich, dass Sie unter `ftp.adobe.com/<sftpname>` bei Ihrer FTP-Site angemeldet sind.

1. Wählen Sie **[!UICONTROL Aktionen]** > **[!UICONTROL Datei-Upload]**.

1. Laden Sie eine `.fin`-Datei hoch, damit Ihre Datei abgerufen werden kann.

   Der Dateityp `.fin` wird vom Benutzer erstellt und signalisiert, dass das Hochladen abgeschlossen ist. Sie kann eine leere Editor-Datei sein. Wenn Sie beispielsweise [!DNL crs123.csv] hochladen, wird auch [!DNL crs123.fin] hochgeladen.

   Wenn der Upload erfolgreich war, werden beide Dateien in einen Ordner mit dem Namen **verarbeitet** verschoben.

   Wichtige Informationen zu Dateinamen und zur Dateistruktur finden Sie unter [Datendateivoraussetzungen für das Hochladen von Kundenattributen](crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19).
