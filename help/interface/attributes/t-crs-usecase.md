---
description: Erstellen der Kundenattributquelle und Hochladen der Daten.
keywords: Kundenattribute; Hauptdienste
seo-description: Erstellen der Kundenattributquelle und Hochladen der Daten.
seo-title: Erstellen einer Kundenattributquelle und Hochladen der Datendatei
solution: Experience Cloud
title: Erstellen einer Kundenattributquelle und Hochladen der Datendatei
uuid: 53 dca 789-9 a 91-4385-839 d-c 9 d 1 aa 36 b 9
translation-type: tm+mt
source-git-commit: b6058194725c3ad50d280a3daad737cd53416204

---


# Erstellen einer Kundenattributquelle und Hochladen der Datendatei

Erstellen der Kundenattributquelle und Hochladen der Daten. Sie können die Datenquelle aktivieren, wenn Sie bereit sind. Geben Sie die Attributdaten nach Aktivierung der Datenquelle an Analytics und Target weiter.

## Arbeitsablauf für Kundenattribute {#concept_BF0AF88E9EF841219ED4D10754CD7154}

![](assets/crs.png)

1. [Erstellen einer Datendatei](../attributes/t-crs-usecase.md#task_B5FB8C0649374C7A94C45DCF2878EA1A)
1. [Erstellen Sie die Attributquelle und laden Sie die Datendatei hoch.](../attributes/t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8)
1. [Prüfen des Schemas](../attributes/t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8)
1. [Konfigurieren von Abonnements und Aktivieren der Attributquelle](../attributes/t-crs-usecase.md#task_1ACA21198F0E46A897A320C244DFF6EA)


Sobald die Datenquelle aktiv ist, können Sie folgende Aufgaben ausführen:

* [Verwenden von Kundenattributen in Adobe Analytics](../attributes/t-crs-usecase.md#task_7EB0680540CE4B65911B2C779210915D)
* [Verwenden von Kundenattributen in Adobe Target](../attributes/t-crs-usecase.md#task_FC5F9D9059114027B62DB9B1C7D9E257)



>[!IMPORTANT]
>
>Um auf diese Funktion zuzugreifen, müssen Benutzer dem Produktprofil für Kundenattribute (Kundenattribute - Standardzugriff) zugewiesen werden. ( **[!UICONTROL Administration]** &gt; **[!UICONTROL Admin-Konsole]** &gt; **[!UICONTROL Benutzer]** &gt;). Benutzer, die der Gruppe „Kundenattribute“ hinzugefügt wurden, sehen auf der linken Seite der Experience Cloud-Benutzeroberfläche unter [!UICONTROL Zielgruppen] das Menüelement [!UICONTROL Kundenattribute.]
>
>Die Mitgliedschaft in der Lösungsgruppe ist ebenfalls erforderlich.

Um die Funktion „Kundenattribute“ verwenden zu können, müssen Benutzer der Adobe-Gruppe „Kundenattribute“ in der Benutzerverwaltung sowie Gruppen auf Lösungsebene (Analytics oder Target) angehören.

Informationen hierzu finden Sie unter [Benutzer und Gruppen](../admin-getting-started/admin-getting-started.md#task_3295A85536BF48899A1AB40D207E77E9).

## Erstellen Sie eine Datendatei.{#task_B5FB8C0649374C7A94C45DCF2878EA1A}

Bei diesen Daten handelt es sich um Unternehmensdaten aus Ihrem CRM-System. Die Daten können zum Beispiel Produktabonnementdaten einschließlich Mitglieds-IDs, Produktberechtigungen, der am häufigsten gestarteten Produkte und dergleichen mehr enthalten.


1. Erstellen Sie eine [!DNL .csv].


   >[!NOTE]
   >
   >Später können Sie die [!DNL .csv] Datei per Drag &amp; Drop hochladen. Wenn Sie [jedoch über FTP](../attributes/t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B)hochladen, benötigen Sie auch eine [!DNL .fin] Datei mit demselben Namen wie die Datei [!DNL .csv].



   Beispiel für die Kundendatendatei eines Unternehmens:

   ![](assets/01_crs_usecase.png)

1. Überprüfen Sie vor dem Fortfahren die wichtigen Informationen in [den Datendateianforderungen](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19), bevor Sie die Datei hochladen.
1. [Erstellen Sie eine Kundenattributquelle und laden Sie die Daten hoch](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78), wie unten beschrieben.

## Erstellen Sie die Attributquelle und laden Sie die Datendatei hoch.{#task_09DAC0F2B76141E491721C1E679AABC8}

Führen Sie diese Schritte auf der Seite „Neue Kunden-Attributquelle erstellen“ der Experience Cloud aus.


>[!IMPORTANT]
>
>Beim Erstellen, Ändern oder Löschen von Kundenattributquellen dauert es bis zu einer Stunde, bis die IDs mit der neuen Datenquelle synchronisiert werden. Sie müssen über Administratorrechte in Audience Manager verfügen, um Kundenattributquellen zu erstellen oder zu ändern. Wenden Sie sich an den Audience Manager-Kundendienst oder beraten Sie sich, um Administratorrechte abzurufen.


1. Klicken Sie [!DNL Experience Cloud]im ![](assets/menu-icon.png) Menü auf das Menüsymbol.
1. Klicken **[!UICONTROL Sie auf Personen]** und dann auf **[!UICONTROL Kundenattribute]**.

   Auf der Seite [!UICONTROL Kundenattribute] können Sie vorhandene Datenattributquellen verwalten und bearbeiten.

   ![Schrittergebnis](assets/03_crs_usecase.png)
1. Klicken **[!UICONTROL Sie auf Neu]**.

   ![Schrittergebnis](assets/04_crs_usecase.png)
1. Konfigurieren Sie auf der Seite „[!UICONTROL Kunden-Attributquelle bearbeiten]“ die folgenden Felder:


   * **[!UICONTROL Name:]** Ein Anzeigename für die Datenattributquelle. Für Attributnamen [!DNL Adobe Target]dürfen keine Leerzeichen enthalten sein. Wenn ein Attribut mit einem Leerzeichen übergeben wird, [!DNL Target] wird es ignoriert. Weitere nicht unterstützte Zeichen: `< , >, ', "`.

   * **[!UICONTROL Beschreibung:]** (Optional) Eine Beschreibung der Datenattributquelle.

   * **[!UICONTROL Alias-ID:]** Stellt eine Quelle für Kundenattributdaten dar, z. B. ein bestimmtes CRM-System. Eine eindeutige ID, die im Code Ihrer Kundenattributquelle verwendet wird. Die ID muss eindeutig sein und darf nur Kleinbuchstaben, aber keine Leerzeichen enthalten. Der in der Experience Cloud-Oberfläche im Feld „Alias-ID“ eingegebene Wert für eine Kundenattributquelle sollte mit den Werten übereinstimmen, die (über das Dynamic Tag Management oder JavaScript des Mobile-SDK) aus der Implementierung übergeben werden.

      Die Alias-ID entspricht bestimmten Bereichen, für die Sie zusätzliche Kunden-ID-Werte eingerichtet haben. Beispiel:

      * **Dynamisches Tag-Management:** Die Alias-ID entspricht dem *Integrationscode* -Wert unter [!UICONTROL &quot;Kundeneinstellungen]«im Tool [&quot; Experience Cloud ID-Dienst](https://marketing.adobe.com/resources/help/en_US/dtm/?f=macid) &quot; .

      * **Besucher-API:** Die Alias-ID entspricht den zusätzlichen [Kunden-IDs](https://marketing.adobe.com/resources/help/en_US/mcvid/?f=mcvid_customer_ids), die den Besuchern zugeordnet werden können.

         Beispiel: *&quot;crm_ id&quot;* in:


         ```
         "crm_id":"67312378756723456"
         ```


      * **iOS:** The Alias ID corresponds to *&quot;idType&quot;* in [visitorSyncIdentifiers:identifiers](https://marketing.adobe.com/resources/help/en_US/mobile/ios/?f=methods).

         Beispiel:

         `[ADBMobile visitorSyncIdentifiers:@{@<`**`"idType"`**`:@"idValue"}];`


      * **Android:** Die Alias-ID entspricht dem *&quot; Idtype &quot;* in [syncidentifiers](https://marketing.adobe.com/resources/help/en_US/mobile/android/?f=methods).

         Beispiel:

         `identifiers.put(`**`"idType"`**`, "idValue");`

         Weitere Informationen zur Datenverarbeitung im Feld &quot;Alias-ID&quot; und Kunden-IDs finden Sie unter [Nutzen mehrerer Datenquellen](../attributes/crs-data-file.md#section_76DEB6001C614F4DB8BCC3E5D05088CB) .
   * **[!UICONTROL Datei-Upload:]** Sie können [!DNL .csv] die Datendatei per Drag &amp; Drop verschieben oder die Daten per FTP hochladen. (Bei Verwendung von FTP wird ebenfalls eine [!DNL .fin] Datei benötigt.) Siehe [Hochladen der Daten über FTP](../attributes/t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B).


      >[!IMPORTANT]
      >
      >Es gelten spezifische Datendateianforderungen. Weitere Informationen finden Sie unter [Datendateivoraussetzungen](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19) .


      Nach dem Hochladen der Datei werden die Daten auf dieser Seite unter der Überschrift „[!UICONTROL Datei-Upload]“ in tabellarischer Form angezeigt. Sie können das Schema prüfen, Abonnements konfigurieren oder die Übertragung via FTP einrichten.



      **Grafik für Datei-Uploads**

      ![](assets/file_upload_attributes.png)

   * **[!UICONTROL Unique Customer ID:]** Zeigt an, wie viele eindeutige IDs Sie zu dieser Attributquelle hochgeladen haben.

   * **[!UICONTROL Vom Kunden bereitgestellte IDs für Experience Cloud Besucher-IDs:]** Zeigt an, wie viele IDs für Experience Cloud Besucher-IDs aliase wurden.

   * **[!UICONTROL Vom Kunden bereitgestellte IDs mit hohen Alias-Zählungen:]** Zeigt die Anzahl der vom Kunden bereitgestellten IDs mit 500 oder mehr Aliasing-Experience Cloud-Besucher-IDs an. In der Regel kennzeichnen diese vom Kunden bereitgestellten IDs keine Einzelpersonen, sondern eine Art freigegebene Anmeldung. Das System verteilt die diesen IDs zugewiesenen Attribute auf die 500 zuletzt als Alias zugewiesenen Experience Cloud-Besucher-IDs, und zwar so lange, bis 10.000 Aliasse erreicht sind. Bei Erreichen dieser Anzahl erklärt das System die vom Kunden bereitgestellte ID als ungültig und verteilt nicht länger zugewiesene Attribute.










## Prüfen des Schemas {#task_404AAC411B0D4E129AB3AC8B7BE85859}

Der Prüfungsprozess ermöglicht die Zuordnung von Anzeigenamen und Beschreibungen zu den hochgeladenen Attributen (Zeichenfolgen, Ganzzahlen, Zahlen usw.). Sie können Attribute auch löschen, indem Sie das Schema aktualisieren.

Siehe [Schema überprüfen](../attributes/validate-schema.md#concept_B3A01A15D04E4F998118E09B3A9B5043).

Informationen zum Löschen von Attributen finden Sie unter [(Optional) Aktualisieren Sie das Schema (löschen Sie Attribute)](../attributes/t-crs-usecase.md#task_6568898BB7C44A42ABFB86532B89063C).

## (Optional) Schema aktualisieren (Attribute löschen) {#task_6568898BB7C44A42ABFB86532B89063C}

Löschen von Attributen und Ersetzen von Attributen im Schema.


1. Entfernen [!UICONTROL Sie auf der Seite &quot;Kunden-Attributquelle] bearbeiten&quot; das **[!UICONTROL Target]** - oder **[!UICONTROL Analytics]** -Abonnement (unter&quot; Abonnements [!UICONTROL konfigurieren]«).
1. [Laden Sie eine neue Datendatei mit aktualisierten Feldern hoch](../attributes/t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8).

## Konfigurieren Sie Abonnements und aktivieren Sie die Attributquelle.{#task_1ACA21198F0E46A897A320C244DFF6EA}

Der Datenfluss zwischen der Experience Cloud und Lösungen wird durch die Konfiguration eines Abonnements eingerichtet. Durch die Aktivierung der Attributquelle können die Daten an die abonnierten Lösungen übertragen werden. Die von Ihnen hochgeladenen Kundendatensätze werden mit den von Ihrer Website oder Anwendung eingehenden ID-Signalen abgeglichen.

Siehe [Konfigurieren von Abonnements](../attributes/subscription.md#concept_ECA3C44FA6D540C89CC04BA3C49E63BF).

**So aktivieren Sie eine Attributquelle**

Am [! UICONTROL Create New [or Edit] Customer Attributseite], suchen Sie die Überschrift [!UICONTROL Aktivieren] und klicken Sie dann **[!UICONTROL auf Aktiv]**.

![Schrittergebnis](assets/activate_attribute_source.png)

## Kundenattribute in Adobe Analytics verwenden {#task_7EB0680540CE4B65911B2C779210915D}

Mit den Daten, die jetzt in Lösungen wie
<keyword>
Adobe Analytics
</keyword>können Sie Berichte zu den Daten erstellen, sie analysieren und die entsprechende Aktion in Ihren Marketingkampagnen durchführen.

Folgendes Beispiel zeigt ein [!DNL Analytics]-Segment, das auf den hochgeladenen Attributen basiert. Dieses Segment zeigt Photoshop Lightroom-Abonnenten, deren am häufigsten geladenes Produkt Photoshop ist.

![](assets/08_crs_usecase.png)

Wenn Sie ein Segment in der Experience Cloud veröffentlichen, wird es in Experience Cloud-Zielgruppen und Audience Manager verfügbar.

Weitere Informationen hierzu finden Sie in der Analytics-Hilfe unter [Bericht „Kundenattribute“](https://marketing.adobe.com/resources/help/en_US/reference/?f=reports_customer_attributes).

## Verwenden von Kundenattributen in Adobe Target {#task_FC5F9D9059114027B62DB9B1C7D9E257}

In Target können Sie beim Erstellen einer Zielgruppe Kundenattribute im Abschnitt „Besucherprofil“ auswählen. Alle Kundenattribute enthalten das Präfix [!DNL crs.] in der Liste. Sie können die Attribute beim Aufbau von Zielgruppen beliebig mit anderen Datenattributen kombinieren.

![](assets/crs-add-attribute-target.png)

Weitere Informationen finden Sie unter [Erstellen einer neuen Zielgruppe](https://marketing.adobe.com/resources/help/en_US/target/target/?f=t_creating_a_new_audience) in der Target-Hilfe.
