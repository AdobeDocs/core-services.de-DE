---
description: Erfahren Sie, wie Sie Kundenattributdaten per FTP in das Experience Cloud hochladen.
keywords: Kundenattribute;Hauptdienste
solution: Experience Cloud
title: 'Upload der Datendatei für Kundenattribute über FTP '
uuid: 5df565dd-b6f8-420e-981f-4b6fc6f7d0e4
feature: 'Kundenattribute '
topic: Administration
role: Administrator
level: Erfahren
translation-type: tm+mt
source-git-commit: 61d60273e933c637dfe4400da78257e1c80015b3
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 93%

---


# Optional – Hochladen der Datendatei via FTP

Wenn Sie die Kundenattributdaten nicht per Drag &amp; Drop in die Experience Cloud hochladen, können Sie die Daten auch via FTP hochladen.

Sie können die Daten hochladen, nachdem Sie eine Kundenattributquelle und ein FTP-Konto in der Experience Cloud erstellt haben. Pro Attributquelle erstellen Sie ein FTP-Konto. Die hochgeladenen Dateien werden im Stammordner dieses Kontos gespeichert. Die Daten müssen im `.csv`-Format übertragen werden, wobei eine zusätzliche `.fin`-Datei am Ende angibt, dass das Hochladen abgeschlossen ist.

>[!IMPORTANT]
>
>Lesen Sie [Datendateivoraussetzungen für das Hochladen von Kundenattributen](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19), bevor Sie die Datei hochladen.

Datei-Uploads auf die FTP-Site für Kundenattribute können über FTP oder SFTP erfolgen:

* Sie benötigen einen Client, der SFTP-Verbindungen unterstützt.
* Sie können eine Verbindung mit SFTP entweder mit dem Benutzernamen/Kennwort oder ohne Kennwort herstellen, wie [hier](https://docs.adobe.com/help/de-DE/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html) beschrieben.

**So laden Sie die Datendatei via FTP hoch**

1. [Erstellen einer Kundenattributquelle und Hochladen der Datendatei...](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

   Vergewissern Sie sich, dass Sie unter `ftp.adobe.com/<sftpname>` bei Ihrer FTP-Site angemeldet sind.

1. Klicken Sie auf **[!UICONTROL Aktionen]** > **[!UICONTROL Datei hochladen]**.

1. Laden Sie eine `.fin`-Datei hoch, damit Ihre Datei abgerufen werden kann.

   Der Dateityp `.fin` wird vom Benutzer erstellt und signalisiert, dass das Hochladen abgeschlossen ist. Sie kann eine leere Editor-Datei sein. Wenn Sie beispielsweise [!DNL crs123.csv] hochladen, wird auch [!DNL crs123.fin] hochgeladen.

   Wenn der Upload erfolgreich war, werden beide Dateien in einen Ordner mit dem Namen **verarbeitet** verschoben.

   Wichtige Informationen zu Dateinamen und zur Dateistruktur finden Sie unter [Datendateivoraussetzungen für das Hochladen von Kundenattributen](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19).
