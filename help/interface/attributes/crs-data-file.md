---
description: Datendateianforderungen und mehrere Datenquellen für das Hochladen von Kundenattributen in der Experience Cloud.
keywords: Kundenattribute; Hauptdienste
seo-description: Datendateianforderungen und mehrere Datenquellen für das Hochladen von Kundenattributen in der Experience Cloud.
seo-title: Informationen zur Datendatei und den Datenquellen für Kundenattribute
solution: Experience Cloud
title: Informationen zur Datendatei und den Datenquellen für Kundenattribute
uuid: 9dd0e364-889b-45db-b190-85c0930a101e
translation-type: ht
source-git-commit: bae7ac2bc620fc0f9ac149f7dce84fa70e1355c9

---


# Informationen zur Datendatei und den Datenquellen für Kundenattribute

Datendateianforderungen und mehrere Datenquellen für das Hochladen von Kundenattributen in der Experience Cloud.

Sie benötigen Zugriff auf CRM- oder ähnliche Daten aus Ihrem Unternehmen. Die in die Experience Cloud hochzuladenden Daten müssen im [!DNL .csv]-Format vorliegen. Wenn das Upload über FTP oder sFTP erfolgt, wird auch eine [!DNL .fin]-Datei hochgeladen.

Kundenattribute sind für die Verarbeitung einiger Dateien pro Tag ausgelegt. Um das Problem einer großen Anzahl kleiner Dateien zu reduzieren, die die Verarbeitung verzögern, werden Dateien, die innerhalb von 30 Minuten nach einem vorherigen Batch von derselben Organisation gesendet werden, in eine Warteschlange mit niedrigerer Priorität weitergeleitet.

<!-- <p>Articulate difference between this and SAINT. </p> -->

## Zulässige Dateitypen und Namensanforderungen {#section_6F64FA02ACCC4215B0862CB6A1821FBF}


<table id="table_C27955F6B52A45B28BEEAAF14FFC86D8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Dateityp </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .csv </span> </p> </td> 
   <td colname="col2"> <p>Eine Datei mit kommagetrennten Werten (z. B. aus Excel). Dies ist die Datei mit den Kundenattributdaten. </p> <p> <b>Namensanforderungen:</b> Die Dateinamenserweiterung darf keine Leerstellen enthalten. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .fin </span> </p> </td> 
   <td colname="col2"> <p>(Erforderlich) Die <span class="filepath">.fin</span>-Datei teilt dem System mit, dass das Upload der Daten abgeschlossen ist. <span class="filepath">.fin</span>- und <span class="filepath">.csv</span>-Datei müssen den gleichen Namen haben. </p> <p>Adobe empfiehlt die Erstellung einer leeren Textdatei mit der Erweiterung <span class="filepath">.fin</span>. Eine leere Datei spart Speicherplatz und Übertragungszeit. </p> <p> <p>Hinweis: Nach dem Upload darf die <span class="filepath">.fin</span>-Datei nicht mehr umbenannt werden. Die <span class="filepath">.fin</span>-Datei muss gesondert hochgeladen werden, und es darf sich nicht um eine schon einmal hochgeladene Datei handeln, die einfach umbenannt wurde. </p> </p> <p>Nach dem Hochladen der <span class="filepath">.fin</span>-Datei auf die FTP-Site mit den Kundenattributen ruft das System die Daten unverzüglich ab (innerhalb einer Minute). Dies unterscheidet sich von anderen FTP-Systemen von Adobe, die die Daten weniger häufig sammeln (etwa einmal pro Stunde). </p> <p>Beim Upload mittels Drag-and-Drop ist keine <span class="filepath">.fin</span>-Datei erforderlich. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .gz</span> oder <span class="filepath">.zip </span> </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> .gz</span> (gzip) oder <span class="filepath">.zip</span> – bei komprimierten Dateien. Eine <span class="filepath">.zip</span>-Datei darf nur eine Datei enthalten. </p> <p> <b>Namensanforderungen:</b> Die <span class="filepath">.zip</span>- bzw. <span class="filepath">.gz</span>-Datei und die <span class="filepath">.csv</span>-Datei sollten den gleichen Namen haben. Beispiel: Wenn der Name der <span class="filepath">.csv</span>-Datei <span class="filepath">crm_klein.csv</span> lautet, sollte der Name der <span class="filepath">.zip</span>-Datei <span class="filepath">crm_klein.csv.zip</span> lauten. </p> <p>Der Name der .fin-Datei muss mit dem Namen der .csv-Datei übereinstimmen. </p> </td> 
  </tr> 
 </tbody> 
</table>


## Voraussetzungen für Attributdatendateien {#section_169FBF5B7BBA47CE825B7A330CF3FE98}



**Beispiel für die .csv-Datei**

Die .csv-Datei muss folgendes Format haben:

Beispiel-CSV:

![](assets/cvs.png)

Die gleiche Datei in einem Texteditor:

![](assets/csv_txt.png)

**Richtlinien**

<table id="table_A9849CC9AA784763921DE057F0F61515"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Element </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Drag-and-Drop </p> </td> 
   <td colname="col2"> <p>Per Drag-and-Drop hochgeladene Dateien sollten kleiner als 100 MB sein. </p> <p>Beim Upload mittels Drag-and-Drop ist keine <span class="filepath">.fin</span>-Datei erforderlich. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Spalte mit Kunden-ID </p> </td> 
   <td colname="col2"> <p> Die erste Spalte muss eine Unique Customer-ID enthalten. Die verwendete ID muss mit der an den Experience Cloud ID-Dienst übergebenen ID übereinstimmen. </p> <p>Bei Analytics die in einer prop oder eVar gespeicherte ID. </p> <p>Bei Target der Wert von setCustomerID. (Siehe <a href="../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437" format="dita" scope="local">Analytics und Target – Synchronisieren der Kunden-ID</a>.) </p> <p> Diese Kunden-ID stellt den eindeutigen Bezeichner dar, den Ihr CRM-System für jede Person in Ihrer Datenbank verwendet. Alle anderen Spalten enthalten Attribute aus Ihrem CRM-System. Sie selbst legen fest, wie viele Attribute hochgeladen werden. </p> <p>Als Spaltentitel werden aussagekräftige, gut lesbare Namen empfohlen, allerdings ist dies keine Voraussetzung. Auch bei der Prüfung des Schemas nach dem Upload können Sie den hochgeladenen Zeilen und Spalten noch Anzeigenamen zuordnen. </p> <p> <b>Informationen zu Kunden-IDs</b> </p> <p>Für gewöhnlich verwendet ein Unternehmen eine Kunden-ID aus einem CRM-System. Diese ID wird mithilfe des Aufrufs <span class="codeph">setCustomerIDs</span> festgelegt, wenn sich eine Person anmeldet. Diese ID wird auch als Schlüssel in der CRM-Datei verwendet, die in die Experience Cloud hochgeladen wird. Eine  <a href="../attributes/t-crs-usecase.md#task_09DAC0F2B76141E491721C1E679AABC8" format="dita" scope="local"> Alias-ID</a> ist ein benutzerfreundlicher Name für einen Datenspeicher in Audience Manager, in dem die Aliasdaten gespeichert werden. Das System sendet Alias zu diesem Datenspeicher (über „setCustomerIDs“). Die CRM-Datei wird auf die Daten in diesem Datenspeicher angewendet. </p> <p>Informationen zu <span class="codeph">setCustomerIDs</span> finden Sie unter <a href="https://marketing.adobe.com/resources/help/de_DE/mcvid/?f=mcvid-authenticated-state" format="https" scope="external">Kunden-IDs und Authentifizierungszustände </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Weitere Spaltentitel bzw. Spalten </p> </td> 
   <td colname="col2"> <p>Die Titel aller weiteren Spalten sollten den Namen des jeweiligen Attributs angeben. </p> <p> Diese Spalten sollten die Kundenattribute aus Ihrem CRM-System enthalten. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Zulässige Anzahl an Attributen </p> </td> 
   <td colname="col2"> <p>Sie können Hunderte von <span class="filepath">CSV</span>-Spalten für den Kundenattributdienst in die Experience Cloud hochladen. Bei der Konfiguration von Abonnements und der Auswahl von Attributen gelten jedoch die folgenden Einschränkungen, abhängig von den Lösungen, die Sie besitzen: </p> <p> 
     <ul id="ul_2BB85067918D4BB3B59394F3E3E37A6D"> 
      <li id="li_93703988B9934384B4B94A839D028380"> <b>Analytics Standard</b>: insgesamt 3 Attribute </li> 
      <li id="li_D1E5E7BD24C54591B14D15DE97447835"> <b>Analytics Premium</b>: 200 pro Report Suite </li> 
      <li id="li_8C891FE3D1EF49FA9F81E2E32CD0B9CA"> <b>Target Standard:</b> 5 </li> 
      <li id="li_2B66D43023F34EA685CE2C38A9250CEA"> <b>Target Premium:</b> 200 </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Zulässige Anzahl Zeilen </p> </td> 
   <td colname="col2"> <p>Die Anzahl der Zeilen ist unbegrenzt bzw. es ist keine Grenze bekannt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Zulässige Anzahl an Spalten </p> </td> 
   <td colname="col2"> <p>Aus praktischen Gründen sollten Sie sich auf etwa 200 Spalten beschränken. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Längenbeschränkungen </p> </td> 
   <td colname="col2"> <p>Wenn Sie ein Analytics-Abonnement erstellen, sind die Längen der Felder für hochgeladene Dateien auf 255 Zeichen beschränkt. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>FTP-Richtlinien und Größenbeschränkungen </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_E157EE6F98914EADA0C103D1D1E705D3"> 
      <li id="li_84FBD455DD164A28AC16F4A5AB19E4B3">Die maximale Dateigröße für die Übertragung mittels FTP ist 4 GB pro Upload. </li> 
      <li>Die minimale Dateigröße für jeden Upload-Vorgang ist 10 MB. </li>
      <li>Sie können jede halbe Stunde eine Datei hochladen. </li>
      <li id="li_B69A20C51D824727AA99C1F6F78537A4"> Sie sollten Ihre <span class="filepath">.csv</span>-Datei (und auch die <span class="filepath">.fin</span>-Datei) im Stammordner der FTP-Site ablegen. </li> 
     </ul> </p> <p> <p>Wichtig: Der zulässige Gesamtspeicherplatz für das FTP-Konto beträgt 40 GB. Es liegt in Ihrer Verantwortung, die verarbeiteten Dateien zu löschen. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Dateivoraussetzungen </p> </td> 
   <td colname="col2"> <p> Jede Attributquelle sollte die gleiche Anzahl kommagetrennter Felder enthalten. </p> <p> Felder mit Zeilenumbrüchen, doppelten Anführungszeichen oder Kommas müssen in Anführungszeichen stehen. </p> <p> Doppelten Anführungszeichen in einem Feld muss als Escape-Zeichen ein umgekehrter Schrägstrich (\) vorangestellt werden. </p> <p> Leere Spalten werden als  <span class="term"> null </span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Mehrere Dateien </p> </td> 
   <td colname="col2"> <p>Wenn Sie Kundenattributdaten in mehrere Dateien in schneller Folge hochladen möchten und die Dateien groß sind, stellen Sie sicher, dass die vorherige Datei verarbeitet wurde, bevor Sie die nächste Datei hochladen. Sie können dies überwachen, indem Sie überprüfen, wann die vorherige Datei in den Ordner mit verarbeiteten oder fehlgeschlagenen Vorgängen innerhalb Ihres FTP-Kontos für Kundenattribute verschoben wurde. </p> <p> Die Aufspaltung einer großen Datei in kleinere Dateien und deren schnelle Übermittlung kann die Verarbeitung verlangsamen, es sei denn, Sie können sicherstellen, dass jede Datei vollständig verarbeitet wird, bevor Sie die nächste versenden. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Zeichenkodierung </p> </td> 
   <td colname="col2"> <p>Für Japanisch ist die UTF-8-Zeichenkodierung obligatorisch. </p> </td> 
  </tr> 
   <tr> 
   <td colname="col1"> <p>Verlaufsdaten </p> </td> 
   <td colname="col2"> <p> Kundenattribute sind an das zugrunde liegende Besucherprofil in Analytics gebunden. So sind Kundenattribute über die gesamte Lebensdauer des Besucherprofils in Analytics hinweg mit dem Besucher verknüpft. Dies beinhaltet ein Verhalten, das auftrat, bevor sich der Besucher zum ersten Mal angemeldet hat. </p> <p> Wenn Sie die Data Warehouse-Aufstockungsmethode verwenden, sind die Daten an ein Element „post_vidid_high/low“ gebunden, das auf der Analytics-ID (AID) basiert. Wenn Sie den Experience Cloud ID-Service verwenden, sind die Daten an ein Element „post_visid_high/low“ gebunden, das auf der Experience Cloud ID (MID) basiert. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Datenfeeds </p> </td> 
   <td colname="col2"> <p>Kundenattribute sind nicht in Datenfeeds verfügbar. </p> </td> 
  </tr> 
 </tbody> 
</table>


## Nutzen mehrerer Datenquellen {#section_76DEB6001C614F4DB8BCC3E5D05088CB}

Beim Erstellen, Ändern oder Löschen von Kundenattributquellen dauert es ca. eine Stunde, bis die IDs mit der neuen Datenquelle synchronisiert werden.

Die Alias-ID für jede Kundenattributquelle muss eindeutig sein. Wenn Sie über mehrere Datenquellen verfügen, die dieselbe ID verwenden, müssen Sie sie wie folgt einrichten:

**In VisitorAPI.js oder dem Experience Cloud ID-Tool im Dynamic Tag Management:**

Legen Sie zwei Kunden-IDs fest, die mit den entsprechenden Datenquellen übereinstimmen:

```
Visitor.setCustomerIDs({ 
     "ds_id1”:"123456", 
     "ds_id2":"123456" 
});
```

(Weitere Informationen finden Sie unter [Kunden-IDs und Authentifizierungsstatus](https://marketing.adobe.com/resources/help/de_DE/mcvid/?f=mcvid_customer_ids).)

In der **[!UICONTROL Experience Cloud]** &gt; **[!UICONTROL Personen]** &gt; **[!UICONTROL Kundenattribute]**:

Erstellen Sie mithilfe eindeutiger Alias-IDs, die den obigen Kunden-IDs entsprechen, zwei Kundenattributquellen. Durch die Verwendung dieser Methode kann dieselbe Referenz-ID an verschiedene Kundenattributquellen gesendet werden.
