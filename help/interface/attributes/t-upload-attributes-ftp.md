---
description: Wenn Sie die Kundenattributdaten nicht per Drag-and-Drop in die Experience Cloud hochladen, können Sie die Daten auch via FTP hochladen.
keywords: Kundenattribute; Hauptdienste
seo-description: Wenn Sie die Kundenattributdaten nicht per Drag-and-Drop in die Experience Cloud hochladen, können Sie die Daten auch via FTP hochladen.
seo-title: Optional – Hochladen der Datendatei via FTP
solution: Experience Cloud
title: Optional – Hochladen der Datendatei via FTP
uuid: 5df565dd-b6f8-420e-981f-4b6fc6f7d0e4
translation-type: tm+mt
source-git-commit: d304e625bd2125854d9ed932674522284995e030

---


# Optional – Hochladen der Datendatei via FTP

Wenn Sie die Kundenattributdaten nicht per Drag-and-Drop in die Experience Cloud hochladen, können Sie die Daten auch via FTP hochladen.

Sie können die Daten hochladen, nachdem Sie in der Experience Cloud eine Kundenattributquelle und ein FTP-Konto erstellt haben. Pro Attributquelle müssen Sie ein FTP-Konto erstellen. Die hochgeladenen Dateien werden im Stammordner dieses Kontos gespeichert. Die Daten müssen im `.csv`-Format übertragen werden, wobei eine zusätzliche `.fin`-Datei am Ende angibt, dass das Hochladen abgeschlossen ist.

>[!IMPORTANT]
>
>Lesen Sie [Datendateivoraussetzungen für das Hochladen von Kundenattributen](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19), bevor Sie die Datei hochladen.

Datei-Uploads auf die FTP-Site mit den Kundenattributdaten kann via FTP oder SFTP erfolgen.

* Für SFTP benötigen Sie allerdings einen Client, der SFTP-Verbindungen unterstützt.
* Die Verbindung über SFTP können Sie mit Benutzernamen und Passwort oder, wie [hier](https://docs.adobe.com/help/en/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html) beschrieben, ohne Passwort herstellen.

**So laden Sie die Datendatei via FTP hoch**

1. [Erstellen einer Kundenattributquelle und Hochladen der Datendatei...](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

   Vergewissern Sie sich, dass Sie unter [!DNL ftp.adobe.com/ bei Ihrer FTP-Site angemeldet sind.<sftpname>].

1. Klicken Sie auf **[!UICONTROL Aktionen]** &gt; **[!UICONTROL Datei hochladen]**.

1. Laden Sie eine `.fin`-Datei hoch, damit Ihre Datei abgerufen werden kann.

   Der Dateityp `.fin` wird vom Benutzer erstellt und signalisiert, dass das Hochladen abgeschlossen ist. Sie kann eine leere Editor-Datei sein. Wenn Sie beispielsweise [!DNL crs123.csv] hochladen, wird auch [!DNL crs123.fin] hochgeladen.

   Nach einem erfolgreichen Upload werden beide Dateien in einen Ordner mit dem Namen **processed** verschoben.

   Siehe [Datendateivoraussetzungen für das Hochladen von Kundenattributen](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19), wo Sie wichtige Informationen zu Dateinamen und zur Dateistruktur erhalten.
