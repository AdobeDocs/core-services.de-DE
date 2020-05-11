---
description: Erstellen der Kundenattributquelle und Hochladen der Daten.
keywords: Customer Attributes;core services
seo-description: Erstellen der Kundenattributquelle und Hochladen der Daten.
seo-title: Erstellen einer Kundenattributquelle und Hochladen der Datendatei
solution: Experience Cloud
title: Erstellen einer Kundenattributquelle und Hochladen der Datendatei
uuid: 53dca789-9a91-4385-839d-c9d1aa36b9be
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '1175'
ht-degree: 66%

---


# Erstellen einer Kundenattributquelle und Hochladen der Datendatei

Erstellen Sie die Kundenattributquelle (CSV- und FIN-Dateien) und laden Sie die Daten hoch. Sobald Sie dazu bereit sind, aktivieren Sie die Datenquelle. Geben Sie die Attributdaten nach Aktivierung der Datenquelle an Analytics und Target weiter.

## Arbeitsablauf für Kundenattribute {#concept_BF0AF88E9EF841219ED4D10754CD7154}

![](assets/crs.png)

1. [Erstellen einer Datendatei](../attributes/t-crs-usecase.md#task_B5FB8C0649374C7A94C45DCF2878EA1A)
1. [Erstellen Sie die Attributquelle und laden Sie die Datendatei hoch.](../attributes/t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8)
1. [Prüfen des Schemas](../attributes/t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8)
1. [Konfigurieren von Abonnements und Aktivieren der Attributquelle](../attributes/t-crs-usecase.md#task_1ACA21198F0E46A897A320C244DFF6EA)


Sobald die Datenquelle aktiv ist, können Sie folgende Aufgaben ausführen:

* [Kundenattribute in Adobe Analytics verwenden](../attributes/t-crs-usecase.md#task_7EB0680540CE4B65911B2C779210915D)
* [Kundenattribute in der Adobe-Zielgruppe verwenden](../attributes/t-crs-usecase.md#task_FC5F9D9059114027B62DB9B1C7D9E257)



>[!IMPORTANT]
>
>Um auf diese Funktion zugreifen zu können, müssen Benutzer dem Produktprofil „Kundenattribute“ zugewiesen sein (Kundenattribute – Standardzugriff). ( **[!UICONTROL Administration]** > **[!UICONTROL Admin Console]** > **[!UICONTROL Users]** > ). Users that are added to the Customer Attributes group will see the [!UICONTROL Customer Attributes] menu item in [!UICONTROL Audiences], on the left side of the Experience Cloud interface.
>
>Die Mitgliedschaft in einer Lösungsgruppe ist ebenfalls erforderlich.

To use the Customer Attributes feature, users must belong to the Adobe Customer Attributes group in user management, and to solution-level groups (Analytics or [!DNL Target]).

Informationen hierzu finden Sie unter [Benutzer und Gruppen](../admin-getting-started/admin-getting-started.md#task_3295A85536BF48899A1AB40D207E77E9).

## Erstellen Sie eine Datendatei. {#task_B5FB8C0649374C7A94C45DCF2878EA1A}

Diese Daten sind Daten von Unternehmenskunden aus Ihrem CRM-System. Die Daten können Abonnentendaten für Produkte wie Mitglieds-IDs, Produkte mit Berechtigung, am häufigsten gestartete Produkte usw. enthalten.

1. Erstellen Sie eine `.csv`.


   >[!NOTE]
   >
   >Später werden Sie diese `.csv`-Datei per Drag-and-Drop hochladen. Wenn Sie jedoch [per FTP hochladen](../attributes/t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B), benötigen Sie auch eine `.fin`-Datei mit dem gleichen Namen wie die `.csv`.



   Beispiel für die Kundendatendatei eines Unternehmens:

   ![](assets/01_crs_usecase.png)

1. Überprüfen Sie vor dem Hochladen der Datei die wichtigen Informationen in den [Datendateivoraussetzungen](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19).
1. [Erstellen Sie eine Kundenattributquelle und laden Sie wie nachfolgend beschrieben die Daten hoch](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

## Erstellen Sie die Attributquelle und laden Sie die Datendatei hoch. {#task_09DAC0F2B76141E491721C1E679AABC8}

Führen Sie diese Schritte auf der Seite „Neue Kunden-Attributquelle erstellen“ der Experience Cloud aus.

>[!IMPORTANT]
>
>Beim Erstellen, Ändern oder Löschen von Kundenattributquellen dauert es bis zu einer Stunde, bis die IDs mit der neuen Datenquelle synchronisiert werden. Sie müssen über Administratorrechte in Audience Manager verfügen, um Kundenattributquellen zu erstellen oder zu ändern. Wenden Sie sich an die Audience Manager-Kundenunterstützung oder -Beratung, um Administratorrechte zu erhalten.

1. Klicken Sie in [!DNL Experience Cloud] im Menü auf das ![](assets/menu-icon.png)-Symbol.
1. Under **[!DNL Experience Platform]**, click **[!UICONTROL People]** > **[!UICONTROL Customer Attributes]**.

   Auf der Seite [!UICONTROL Kundenattribute] können Sie vorhandene Datenattributquellen verwalten und bearbeiten.

   ![Schritt Ergebnis](assets/03_crs_usecase.png)
1. Klicken Sie auf **[!UICONTROL Neu]**.

   ![Schritt Ergebnis](assets/04_crs_usecase.png)
1. Konfigurieren Sie auf der Seite [!UICONTROL Kunden-Attributquelle bearbeiten] die folgenden Felder:

   * **[!UICONTROL Name:]** Ein Anzeigename für die Datenattributquelle. Bei [!DNL Adobe Target] dürfen Attributnamen keine Leerzeichen enthalten. Wenn ein Attribut mit Leerzeichen übergeben wird, wird es von [!DNL Target] ignoriert. Weitere nicht unterstützte Zeichen: `< , >, ', "`.

   * **[!UICONTROL Beschreibung:]** (Optional) Eine Beschreibung der Quelle des Datenattributs.

   * **[!UICONTROL Alias-ID:]** Gibt die Quelle der Kundenattributdaten an, beispielsweise ein CRM-System. Eine eindeutige ID, die im Code Ihrer Kundenattributquelle verwendet wird. Die ID muss eindeutig sein und darf nur Kleinbuchstaben, aber keine Leerzeichen enthalten. Der Wert, der in der Experience Cloud-Benutzeroberfläche für eine Kundenattributquelle im Feld &quot;Alias-ID&quot;eingegeben wird, sollte mit den Werten übereinstimmen, die von der Implementierung übergeben werden (über das dynamische Tag-Management oder JavaScript des Mobile SDK).

      Die Alias-ID entspricht bestimmten Bereichen, in denen Sie zusätzliche Kunden-ID-Werte festlegen. Beispiel:

      * **Dynamisches Tag-Management:** Die Alias-ID entspricht dem *Integrationscode* -Wert unter [!UICONTROL Kundeneinstellungen]im Tool [Experience Cloud ID-Dienst](https://docs.adobe.com/content/help/de-DE/dtm/using/tools/macid.html) .

      * **Besucher-API:** Die Alias-ID entspricht den zusätzlichen [Kunden-IDs](https://docs.adobe.com/content/help/de-DE/id-service/using/reference/authenticated-state.html) , die Sie jedem Besucher zuordnen können.

         Beispiel: *„crm_ id“* in:

         ```
         "crm_id":"67312378756723456"
         ```

      * **iOS:** Die Alias-ID entspricht *&quot;idType&quot;* in visitorSyncIdentifiers:identifiers [](https://docs.adobe.com/content/help/de-DE/mobile-services/ios/overview.html).

         Beispiel:

         `[ADBMobile visitorSyncIdentifiers:@{@<`**`"idType"`**`:@"idValue"}];`

      * **Android:** Die Alias-ID entspricht *&quot;idType&quot;* in [syncIdentifiers](https://docs.adobe.com/content/help/de-DE/mobile-services/android/overview.html).

         Beispiel:

         `identifiers.put(`**`"idType"`**`, "idValue");`

         Zusätzliche Informationen zur Datenverarbeitung des Alias-ID-Feldes und von Kunden-IDs finden Sie unter [Nutzen mehrerer Data Sources](../attributes/crs-data-file.md#section_76DEB6001C614F4DB8BCC3E5D05088CB).
   * **[!UICONTROL Hochladen einer Datei:]** Die `.csv`-Datendatei kann per Drag-and-Drop oder per FTP hochgeladen werden. (Beim Upload via FTP ist zusätzlich eine `.fin`-Datei erforderlich.) Siehe [Hochladen der Daten via FTP](../attributes/t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B).

      >[!IMPORTANT]
      >
      >Für die Datendatei bestehen bestimmte Voraussetzungen. Weitere Informationen finden Sie unter [Datendateivoraussetzungen](../attributes/crs-data-file.md#concept_DE908F362DF24172BFEF48E1797DAF19).


      Nach dem Hochladen der Datei werden die Tabellendaten unter der Überschrift [!UICONTROL Datei-Upload] auf dieser Seite angezeigt. Sie können das Schema überprüfen, Abonnement konfigurieren oder den FTP einrichten.

      **Grafik zum Datei-Upload**

      ![](assets/file_upload_attributes.png)

   * **[!UICONTROL Unique Customer-ID:]** Zeigt an, wie viele eindeutige IDs Sie in diese Attributquelle hochgeladen haben.

   * **[!UICONTROL Vom Kunden bereitgestellte IDs für Experience Cloud Besucher-IDs:]** Zeigt an, wie viele IDs für Experience Cloud Besucher-IDs bereitgestellt wurden.

   * **[!UICONTROL Vom Kunden bereitgestellte IDs mit hoher Alias-Anzahl:]** Zeigt die Anzahl der vom Kunden bereitgestellten IDs mit 500 oder mehr bereitgestellten Experience Cloud Besucher-IDs an. Diese vom Kunden bereitgestellten IDs stellen höchstwahrscheinlich keine Einzelpersonen dar, sondern eine Art freigegebene Anmeldung. Das System verteilt die mit diesen IDs verknüpften Attribute auf die 500 zuletzt als Alias gespeicherten Experience Cloud-Besucher-IDs, bis die Aliasanzahl 10.000 erreicht hat. Bei Erreichen dieser Anzahl erklärt das System die vom Kunden bereitgestellte ID als ungültig und verteilt nicht länger zugewiesene Attribute.



## Prüfen des Schemas {#task_404AAC411B0D4E129AB3AC8B7BE85859}

Der Prüfungsprozess ermöglicht die Zuordnung von Anzeigenamen und Beschreibungen zu den hochgeladenen Attributen (Zeichenfolgen, Ganzzahlen, Zahlen usw.). Sie können Attribute auch löschen, indem Sie das Schema aktualisieren.

Siehe [Prüfen des Schemas](../attributes/validate-schema.md#concept_B3A01A15D04E4F998118E09B3A9B5043).

Informationen zum Löschen von Attributen finden Sie unter [Schema aktualisieren (Attribute löschen)](../attributes/t-crs-usecase.md#task_6568898BB7C44A42ABFB86532B89063C).

## (Optional) Schema aktualisieren (Attribute löschen) {#task_6568898BB7C44A42ABFB86532B89063C}

So löschen Sie Attribute und ersetzen Attribute im Schema.

1. Entfernen Sie auf der Seite [!UICONTROL Kunden-Attributquelle bearbeiten] das **[!UICONTROL Target]**- oder **[!UICONTROL Analytics]**-Abonnement (unter [!UICONTROL Abonnements konfigurieren]).
1. [Laden Sie eine neue Datendatei mit aktualisierten Feldern hoch](../attributes/t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8).

## Konfigurieren Sie Abonnements und aktivieren Sie die Attributquelle. {#task_1ACA21198F0E46A897A320C244DFF6EA}

Beim Konfigurieren eines Abonnements wird der Datenfluss zwischen Experience Cloud und Lösungen eingerichtet. Durch die Aktivierung der Attributquelle können die Daten an die abonnierten Lösungen übertragen werden. Die von Ihnen hochgeladenen Kundendatensätze werden mit den eingehenden ID-Signalen Ihrer Website oder Anwendung abgeglichen.

Siehe [Konfigurieren von Abonnements](../attributes/subscription.md#concept_ECA3C44FA6D540C89CC04BA3C49E63BF).

**So aktivieren Sie eine Attributquelle**

Suchen Sie auf der Seite [!UICONTROL Neue Kunden-Attributquelle erstellen[ oder ]Kunden-Attributquelle bearbeiten] die Überschrift [!UICONTROL Aktivieren] und klicken Sie dann auf **[!UICONTROL Aktiv]**.

![Schritt Ergebnis](assets/activate_attribute_source.png)

## Use Customer Attributes in Adobe Analytics {#task_7EB0680540CE4B65911B2C779210915D}

Mit den Daten, die jetzt in Lösungen verfügbar sind, wie z. B. in
<keyword>
Adobe Analytics
</keyword>können Sie Berichte zu den Daten erstellen, sie analysieren und die entsprechende Aktion in Ihren Marketing-Kampagnen durchführen.

Folgendes Beispiel zeigt ein [!DNL Analytics]-Segment, das auf den hochgeladenen Attributen basiert. This segment shows [!DNL Photoshop Lightroom] subscribers whose most-launched product is Photoshop.

![](assets/08_crs_usecase.png)

Wenn Sie ein Segment in der Experience Cloud veröffentlichen, steht es in Experience Cloud-Audiencen und Audience Manager zur Verfügung.

Weitere Informationen finden Sie unter Bericht [zu](https://docs.adobe.com/help/en/analytics/components/variables/dimensions-reports/reports-customer-attributes.html) Kundenattributen in der Analytics-Hilfe.

## Use Customer Attributes in Adobe Target {#task_FC5F9D9059114027B62DB9B1C7D9E257}

In [!DNL Target] können Sie beim Erstellen einer Zielgruppe im Bereich Besucherprofil ein Kundenattribut auswählen.  All Customer Attributes will have the prefix [!DNL crs.] in the list. Sie können die Attribute beim Aufbau von Zielgruppen beliebig mit anderen Datenattributen kombinieren.

![](assets/crs-add-attribute-target.png)

Siehe [Erstellen einer neuen Audience](https://docs.adobe.com/content/help/de-DE/target/using/audiences/create-audiences/audiences.html) in der [!DNL Target] Hilfe.
