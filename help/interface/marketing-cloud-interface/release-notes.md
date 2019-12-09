---
description: Funktionen, Versionshinweise und bekannte Probleme in Verbindung mit der Experience Cloud-Schnittstelle
keywords: core services
seo-description: Funktionen, Versionshinweise und bekannte Probleme in Verbindung mit der Experience Cloud-Schnittstelle
seo-title: Gesammelte Versionshinweise
solution: Experience Cloud
title: Gesammelte Versionshinweise
uuid: fcff8cc6-e587-4bf2-9a75-261d4eabc7d4
translation-type: tm+mt
source-git-commit: ae97db27349940a8df7ee2ba6678683f57585678

---


# Gesammelte Versionshinweise

Funktionen, Versionshinweise und bekannte Probleme in Verbindung mit der Experience Cloud-Schnittstelle

Eine Liste der Aktualisierungen der Dokumentation finden Sie unter [Experience Cloud](../doc-updates.md#concept_4C8983FCD23848A4B1E4C2D99ED82784).

Versionshinweise zu allen Lösungen finden Sie unter [Experience Cloud-Versionshinweise](https://docs.adobe.com/content/help/en/release-notes/experience-cloud/current.html).

## August 2019

* Ein kritisches Problem bei der Experience Cloud-Anmeldung wurde behoben, durch das manche Sitzungen unterbrochen wurden. (MCUI-6908)
* Die Anmeldung von Experience Cloud wurde aktualisiert, um die Leistung zu verbessern und die Latenz zu reduzieren. (MCUI-6854, MCUI-6869, MCUI-6883)
* Die Benutzeroberfläche wurde aktualisiert. (MCUI-6861, MCUI-6911, MCUI-6862)
* Ein Problem mit Experience Cloud [!UICONTROL Triggers] wurde behoben, das zur falschen Interpretation der _Like_-Bedingung in der [!UICONTROL Trigger]-Definition geführt hatte. (MCUI-6611)

## April 2019

* Aktualisierung des App-Switchers durch Aufnahme von Marketo in die Experience Cloud-Lösungssuite und Branding-Updates in Experience Platform. (MCUI-6529)
* Aktualisierung der Experience Cloud-Startseite mit Navigationslinks zur Feed- und Admin-Seite. (MCUI-6682)
* Es wurde ein Problem in der [!UICONTROL Auslöserdefinition] behoben, damit der „like“-Satz korrekt verwendet wird. (MCUI-6611)
* Verbesserungen an den Kundenattributen zur besseren Anmeldung im Abonnementdienst. (MCUI-6519)

## Version 19.1.1 – 17. Januar 2019

**Hinweis:** Im März 2019 wird Internet Explorer 11 von der Experience Cloud-Benutzeroberfläche nicht unterstützt.

* Es wurde ein Problem behoben, das verhinderte, dass die Hilfesuche Ergebnisse lieferte. (MCUI-1670)
* Die eVar-Verwaltung in Triggers wurde korrigiert und verbessert. (MCUI-6400)

## Version 16.5.1 – 26. Mai 2016 {#section_3785F182BC13493F84903CA69EB6D0A8}

**Funktionen und Verbesserungen**

<table id="table_ABBCE1A66F534059BD728BC2B9AEFA80"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Vorab konfigurierte Produktkonfigurationen der Admin Console </p> </td> 
   <td colname="col2"> <p>Kundenadministratoren in der Experience Cloud können Produktkonfigurationen nutzen, die zuvor erstellt und für Analytics und das Dynamic Tag Management Standardberechtigungsgruppen zugeordnet wurden. </p> <p>Diese Optimierung ist für neu bereitgestellte Organisationen verfügbar und verringert die Zeit, die Organisationen zur Verwaltung von Benutzern in der Admin Console benötigen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Feed-Verbesserung </p> </td> 
   <td colname="col2"> <p> Beim Erstellen eines neuen Beitrags im Experience Cloud-Feed wird in der Zeile „An“ jetzt standardmäßig das derzeit aktive Thema anstelle der Organisation verwendet.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Es wurde ein Problem behoben, bei dem Miniaturansichten für Assets, die aus Assets on Demand für den Experience Cloud-Feed freigegeben worden waren, nicht angezeigt wurden. (MAC-29955)

## Version 16.2 – 18. Februar 2016 {#section_D9610373116C4D77A38F67815C725EA3}

<table id="table_C9B288CF42034F329C3C72D95D22E515"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Verbesserungen in Experience Cloud-Assets </p> </td> 
   <td colname="col2"> <p>In Experience Cloud Assets können Sie Ihre digitalen Assets an einem zentralen Speicherort speichern, freigeben und synchronisieren. Experience Cloud Assets nutzen einige in <span class="keyword">Adobe Experience Manager</span> (AEM) verfügbare Funktionen. </p> <p>Weitere Informationen finden Sie unter <a href="../experience-cloud-assets/experience-cloud-assets.md#concept_DDA5224C907D4A4F817D795DA0ED64D0" format="dita" scope="local">Experience Cloud</a></p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verbesserte Verknüpfung von Konten </p> </td> 
   <td colname="col2"> <p>Der Arbeitsablauf für die Verknüpfung von Konten der Lösung mit der Experience Cloud (Adobe ID) wurde verbessert. Der neue Arbeitsablauf ermittelt alle Konten des Benutzers, die einer Organisation zugeordnet sind, und ermöglicht die Auswahl des zu verknüpfenden Kontos. Auch der Ablauf der Kontoverknüpfung wurde optimiert, weshalb es nicht mehr notwendig ist, auf die Seite für die Verwaltung von Organisationen zuzugreifen, um Konten manuell zu verknüpfen. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Ein Problem wurde behoben, das die Verknüpfung von SSO für Analytics verhindert hatte. Dabei wurde folgende Meldung angezeigt: „Notice: The error message: ERROR IMS SSO Failed: Unable to find linked company.“

**Bekanntes Problem**

Wenn Sie über **[!UICONTROL Experience Cloud]** &gt; **[!UICONTROL Activation]** auf das dynamische Tag-Management zugreifen, Ihr Konto für das dynamische Tag-Management jedoch nicht mit der Experience Cloud (Adobe ID) verknüpft ist, können Sie sich nicht beim Dynamic Tag Management anmelden. Um dieses Problem zu umgehen, müssen Sie in einem neuen Browser-Tab direkt zu [!DNL dtm.adobe.com] navigieren.

## Version 16.1 – 21. Januar 2016 {#section_33B3F7DF6CA347E3AA93801BAC6232CE}

<table id="table_4223658257DA41C999AC710A10D26771"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Meldungen in der Zielgruppenbibliothek </td> 
   <td colname="col2"> <p> Die Zielgruppenbibliothek wurde so verbessert, dass beim Erstellen von Zielgruppen oder Auftreten eines Timouts hilfreiche Meldungen angezeigt werden. </p> <p>Wenn Sie beispielsweise mehr als fünf Regeln hinzufügen, wird eine Meldung angezeigt, dass Sie das zulässige Maximum für Regeln überschritten haben. (MAC-27376, MAC-27375) </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Microsoft [beendet den Support](https://www.microsoft.com/en-us/WindowsForBusiness/End-of-IE-support) für Internet Explorer 8, 9 und 10. Aus diesem Grund werden keine Probleme mehr behoben, die in Verbindung mit diesen speziellen Versionen von Internet Explorer gemeldet werden.

## Version 15.10 – 14. Oktober 2015  {#section_68123833D3634BD3A473C12862BF9606}

**Bekannte Probleme**

* Kunden können sich nicht bei Report Builder anmelden, wenn sie sich über die Experience Cloud per SSO bei Analytics anmelden. Dieses Problem tritt nicht bei Kunden auf, die ihre alten Analytics-Zugangsdaten verwenden.
* Bekanntes Problem mit der Funktion „Link zum Bericht“ in Analytics. Kunden, die sich über die Experience Cloud bei Analytics anmelden, werden beim Versuch, einen Bericht gemeinsam zu nutzen, zu einer Analytics-Anmeldeseite geleitet, auf der SSO nicht möglich ist.

## Version 15.9 – 10. September 2015 {#section_BCCE3E7DF62A4FF5A57B9C8FE2A5F37B}

* Leistungsproblem der Audience Manager-API behoben, das temporäre Timeouts beim Hochladen von Kundenattributdaten verursachte. (MAC-26305)
* Problem behoben, das Benutzer daran hinderte, bis zu 200 Kundenattribute zu einer Mitgliedschaft hinzuzufügen. (MAC-26188)
* Problem mit der Zielgruppenbibliothek behoben, bei dem die Freigabe der Zielgruppe aus der Analytics-Segmentierung nicht möglich war. Dieses Problem verursachte die Anzeige von „Erfassen von Daten“ (0 Zielgruppen). Um dieses Problem zu vermeiden, empfiehlt Adobe, nicht mehr als 50.000 Zielgruppenmitglieder pro Segment zu verwenden. (MAC-25788)
* Zuvor bekanntes Problem der Kundenattribute behoben, bei dem die Seite „Schema bearbeiten“ beim Ändern des Anzeigenamens den Fehler „Inhalt bewahren“ anzeigte. (MAC-25589, AN-103834)

## Version 15.7 – 22. Juli 2015  {#section_2683A152176944E48EF6C943892975B7}

* Problem behoben, bei dem die Attributbeschreibungen, die auf der Seite „Schema anzeigen/bearbeiten“ (in Kundenattributen) angegeben wurde, nicht in Analytics-Berichten aktualisiert wurden. (MAC-25985)
* Es wurde ein Problem behoben, bei dem die Miniaturansichten für hochgeladene Assets nicht gerendert wurden. (MAC-25863)
* Es wurde ein Problem behoben, bei dem neue Segmente, die in Reports &amp; Analytics erstellt wurden, nicht in Experience Cloud Audiences verfügbar waren. (MAC-25817)
* Es wurde ein Problem behoben, bei dem die Zielgruppenfreigabe in Analytics bei Verwendung des Besucher-ID-Services nicht möglich war. (MAC-25788, MAC-25747)
* Es wurde Unterstützung für Multibyte-Zeichen in Kundenattributen hinzugefügt. (MAC-25552)

**Bekanntes Problem**

Ein bekanntes Problem verursacht die Erstellung doppelter automatisch generierter Konten in Audience Manager und die automatische Verknüpfung dieser Konten mit der Experience Cloud-Identität eines Benutzers. Dieses Problem tritt auf, wenn Sie versuchen, zu Audience Manager zu navigieren, bevor Sie Ihre Konten verknüpft haben. Adobe empfiehlt Ihnen, die Verknüpfung Ihrer Audience Manager-Konten mit der Experience Cloud vorzunehmen, bevor Sie zu Audience Manager navigieren. (MAC-25640)

## Version 15.6.1 – 11. Juni 2015  {#section_AD2019F8D2F84C9EB2B0533FAACF7043}

Keine Informationen verfügbar

## Version 15.5.1 – 13. Mai 2015 {#section_EF197410964E40D294D0D8024738CFBA}

<table id="table_14E7B35E06C84A258A21D09691B58354"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Die linken Navigationsmenüs wurden aktualisiert und es besteht nun Zugang zu allen Hauptdiensten und Lösungen. Die relevanten Änderungen beinhalten Folgendes: </p> 
    <ul id="ul_5BEBAB86B9234A239C4E2DAF8826D8E3"> 
     <li id="li_7FA9F64CE69144B8A8A92746BF40E5A1">Die Menüauswahlmöglichkeiten für die  Menüauswahlmöglichkeiten für die <span class="term">Zielgruppenbibliothek</span> und die <span class="term">Kundenattribute</span> sind nun unter <span class="term">Audiences</span> zu finden. </li> 
     <li id="li_95D62A43AE6243DBB2A65EDB830D05C4">Die <span class="term">Exchange</span>-Menüauswahl wurde vom Dropdown-Menü „Hilfe“ zur linken Navigationsleiste verlegt. </li> 
     <li id="li_0443FD50C78446CD8AA27A4F272CAD31"> <span class="term">Lösungen</span> wurde entfernt. Sie können alle Lösungen von der unteren Hälfte der Navigationsleiste aus starten. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

* Ein Problem wurde behoben, infolge dessen die Kundenattribute einiger Kunden nicht synchronisiert werden konnten.
* Ein Problem wurde behoben, durch das die Anzeige der Seite [Adobe Target-Produktdokumentation](https://docs.adobe.com/content/help/en/target/using/integrate/a4t/a4t.html) auf Japanisch verhindert wurde.
* Es wurde ein Problem behoben, das die Verwendung von japanischem Text in Kommentaren zwischen dem [!DNL Creative Cloud] und dem [!DNL Experience Cloud] verhinderte.

## Version 15.4.1 – 8. April 2015 {#section_75634120CC934B3381EDEA7F6F976F0A}

<table id="table_3A6FBAE36558425A803B078150862C92"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Verbesserungen der Administration: </p> 
    <ul id="ul_7D5FCBEFA262435D865CA1018BFB792E"> 
     <li id="li_6E98974CCB094ABBAB57C51ED56C3F00"> <span class="wintitle"> Admin Console</span> </li> 
     <li id="li_8CDAB6301FD44C3999EE4EEB1A0A2FD6">Unterstützung von Enterprise ID und Federated ID </li> 
    </ul> </td> 
   <td colname="col2"> <p>Die Funktionen für die Benutzer- und Gruppenverwaltung wurden in die Admin Console verschoben. Der neue Navigationspfad lautet: </p> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol">Administration</span> &gt; <span class="uicontrol">Admin Console starten</span></p> <p> Darüber hinaus wurde Unterstützung für Enterprise IDs und Federated IDs hinzugefügt. In derselben Unternehmensimplementierung können sowohl Enterprise IDs als auch Federated IDs und Adobe IDs verwendet werden. Adobe IDs können beispielsweise für Benutzer verwendet werden, die andere Adobe-Produkte und -Dienste verwenden dürfen. Enterprise oder Federated IDs können für Benutzer verwendet werden, deren Konten Sie streng verwalten möchten. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Es wurde ein Problem behoben, durch das Single Sign-On zwischen dem [!DNL Experience Cloud] und [!DNL Media Optimizer] verhindert wurde.

**Bekannte Probleme**

* Verlinkung und Aufhebung der Verlinkung von dynamischer Tag-Managementorganisation mit Experience Cloud funktioniert bei neu erstellten Experience Cloud-Organisationen nicht. Wir arbeiten derzeit an einer Lösung, mit der die normale Funktionalität mit der Mai-Version wiederhergestellt werden kann. Sollten Sie Probleme mit Single Sign-on beim Dynamic Tag Management über die Experience Cloud haben, melden Sie sich unter [!DNL dtm.adobe.com] mit Ihrem gewohnten Konto an.
* Ein bekanntes Problem verhindert das Teilen von Inhalten aus Report Suites, die nicht dem verlinkten Analytics-Konto gehören, mit Zielgruppen. An einer Lösung wird bereits gearbeitet.

## Version 15.3.2 – 19. März 2015 {#section_07760FD9CA43497FA8BDCCA990A24BFD}

<table id="table_54025DBE2D094FF1BE837BA60816C6DF"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Kundenattribute </p> </td> 
   <td colname="col2"> <p>Wenn Sie Daten von Unternehmenskunden in einer CRM-Datenbank (Customer Relationship Management) erfassen, können Sie diese Daten in eine Datenquelle für Kundenattribute in die Experience Cloud hochladen. Nach dem Hochladen der Daten können Sie die Berichte <span class="uicontrol">Besucherprofil</span> &gt; <span class="uicontrol">Kundenattribute</span> in Analytics ausführen. </p> <p>Die hochgeladenen Daten können Sie in <span class="keyword">Adobe Target</span> auch als Zielgruppensegment verwenden. </p> <p>Siehe <a href="../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1" format="dita" scope="local">Produktdokumentation zu Kundenattributen</a>. </p> <p> Informationen zur Modernisierung Ihrer Lösungen für Hauptdienste finden Sie unter <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Aktivieren Ihrer Lösungen für Hauptdienste</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Version 15.3.1 – 4. März 2015 {#section_57CB69C044DD47BDBC1A1BEC38957551}

<table id="table_EB3FFBA2DF904546A5185EC9A63BBA98"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Gruppenzuordnung </p> </td> 
   <td colname="col2"> <p>Die Seite „Gruppenverwaltung“ wurde neu als Verwaltungsoberfläche konzipiert, über die Sie Gruppen erstellen, Benutzer Gruppen hinzufügen und Berechtigungen für Experience Cloud-Lösungen zuweisen können. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>1-zu-n-Zuordnung </p> </td> 
   <td colname="col2"> <p>Bei der Verknüpfung von Lösungskonten in Experience Cloud können Sie einer Organisation nun mehrere Produkte und Dienste zuordnen, wenn mehrere Lösungen und Organisationen vorhanden sind. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Activation </p> </td> 
   <td colname="col2"> <p> <a href="../activation/activation.md#concept_EE756B6B0A0643DAB8CA3A00E665406C" format="dita" scope="local"> Activation</a> wird nun im linken Navigationsbereich der <span class="keyword">Experience Cloud</span> angezeigt. <span class="wintitle"> Activation</span> ist ein <span class="keyword">Experience Cloud</span>-Hauptdienst, der derzeit die Dynamic Tag Management-Technologie nutzt und Sie beim Klicken dorthin weiterleitet. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Aktualisierungen an der Dokumentation – Hauptdienste </p> </td> 
   <td colname="col2"> <p>Thema hinzugefügt: <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Aktiveren Ihrer Lösungen für Hauptdienste</a>. Unterstützt Sie bei der Implementierung von Hauptdiensten. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Version 15.2.1 – 19. Februar 2015 {#section_BC694D5AE16A4E16B44B353ED67947F3}

Fehlerbehebungen:

* Verbesserung des Arbeitsablaufs der Kontobereitstellung per E-Mail-Einladung
* Es wurde ein Problem mit dem Asset-Ordner behoben, das die [!DNL Experience Cloud] und [!DNL Adobe Campaign] Assets daran hinderte, identische Ordnerhierarchien anzuzeigen.
* Behebung eines Fehlers, der das Löschen von Zielgruppen verhinderte, die zu deaktivierten [!DNL Target]-Aktivitäten gehörten.
* Behebung eines Fehlers, der dazu führte, dass das Hinzufügen(Plus)-Symbol unter [!UICONTROL Regeln] auf der Seite [!UICONTROL Neue Zielgruppe erstellen] nicht angezeigt wurde.
* Verbesserte Unterstützung von Internet Explorer 9 in der Experience Cloud-Oberfläche

## Version 15.1.1 – 15. Januar 2015  {#section_F1A352E928AF432E94CC0A289C345184}

Neue Funktionen und Fehlerbehebungen in der Benutzeroberfläche für die Zusammenarbeit und Freigabe der [!DNL Adobe Experience Cloud]

<table id="table_AD0A8CA760E64227BB04BA6B0E425E80"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Lesezugriff. </p> </td> 
   <td colname="col2"> <p>Administratoren können Benutzern ohne Administratorberechtigung nun Lesezugriff erteilen. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Es wurde ein Problem behoben, bei dem PNG-Dateien nicht auf einer Karte gerendert werden konnten.
* Es wurde ein Problem beim Hochladen von Dateien in Experience Cloud-Assets per Drag-and-Drop behoben.

**Bekannte Probleme**

* Benutzer können auf Pinnwänden keine PowerPoint-Dateien freigeben.
* Änderungen an Gruppen und Berechtigungen, die über die Benutzerverwaltung durchgeführt werden, werden erst bei einer erneuten Anmeldung wirksam.
* Bei einigen Benutzern treten möglicherweise Probleme beim Hochladen großer Dateitypen in Experience Cloud Assets auf.
* Einigen Benutzern fehlen möglicherweise Links von Media Optimizer auf ihren Experience Cloud-Karten.
* Bei einigen Benutzern ohne Administratorrechte treten möglicherweise Probleme beim Verknüpfen ihrer Konten auf, nachdem sie eine Einladung zum Beitritt zur Experience Cloud angenommen haben.
* Die Leistung der Benutzeroberfläche der Experience Cloud ist u. U. reduziert, wenn sie von mehreren Benutzern gleichzeitig verwendet wird.
* Für einige Benutzer ist das Löschen nicht mehr aktueller Assets möglich, ohne dabei eine Fehlermeldung zu empfangen.
* Bei einigen Benutzern treten möglicherweise Probleme auf, wenn sie sich gleichzeitig bei zwei Browsern mit derselben Adobe ID anmelden.
* Einige Benutzer können möglicherweise einen Creative Cloud-Benutzer nicht erneut einem Freigabeordner hinzufügen, nachdem der Creative Cloud-Benutzer gelöscht wurde.
* Bei einigen Benutzern ist möglicherweise die Benachrichtigung verzögert, die erfolgt, wenn ein Ordner aus der Experience Cloud für die Creative Cloud freigegeben wird.
* Bei einigen Benutzern tritt möglicherweise ein Problem beim Freigeben eines Ordners zwischen der Experience Cloud und der Creative Cloud auf.
* Einige Benutzer haben möglicherweise Probleme beim Erstellen einer Zielgruppe in einer Analytics Report Suite, nachdem die Freigabe von Zielgruppen aktiviert wurde.
* Einige Benutzer haben unter Umständen Probleme beim Hochladen von Assets auf eine Pinnwand.

## Version 14.11.1 – 13. November 2014  {#section_A6CF1D4F27B9496892A89C983EB39102}

Bekannte Probleme:

* Für einige Benutzer ist das Löschen nicht mehr aktueller Assets möglich, ohne dabei eine Fehlermeldung zu empfangen.
* Manche [!DNL .png]-Dateien können nicht auf einer Karte dargestellt werden.
* Einige Benutzer haben unter Umständen Probleme beim Hochladen von Assets auf eine Pinnwand.
* Änderungen an Gruppen und Berechtigungen, die über die Benutzerverwaltung durchgeführt werden, werden erst bei einer erneuten Anmeldung wirksam.
* Administratoren müssen sich ab- und wieder anmelden, um in den Kontoeinstellungen vorgenommene Änderungen zu sehen.
* Benutzer können auf Pinnwänden keine PowerPoint-Dateien freigeben.
* Die Leistung der Benutzeroberfläche der [!DNL Experience Cloud] ist u. U. reduziert, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* Die Synchronisierung zwischen Adobe Experience Manager und Creative Cloud funktioniert nicht.

## Version 14.10.1 – 16. Oktober 2014  {#section_E3A0F4423B814707AA3745E083500835}

Neue Funktionen und Fehlerbehebungen in der Benutzeroberfläche für die Zusammenarbeit und Freigabe der [!DNL Adobe Experience Cloud]

<table id="table_7C1ACE8108D54782AE128ACD35069DF5"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Benutzerberechtigungen bearbeiten </p> </td> 
   <td colname="col2"> <p>Eigentümer einer Pinnwand können nun die Benutzerberechtigungen zu dieser Pinnwand bearbeiten. </p> <p> 
     <ol id="ol_B12251C510744538AF9BCE60ACB04016"> 
      <li id="li_87B3EDE9542B47CEBE0BE7F2D1DE844D">Klicken Sie auf der Pinnwand auf <span class="uicontrol">Einstellungen</span>. </li> 
      <li id="li_0F4786B0E1E743069D082E7DC488A031">Geben Sie neben jedem Eigentümer <span class="uicontrol">Eigentümer</span>, <span class="uicontrol">Viewer</span> oder <span class="uicontrol">Editor</span> an. </li> 
     </ol> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Beim Erstellen einer Karte aus einer PDF und deren Freigabe auf der Pinnwand wurde eine Fehlermeldung zurückgegeben.

**Bekannte Probleme**

* Einige Benutzer haben unter Umständen Probleme beim Hochladen von Assets auf eine Pinnwand.
* Manche [!DNL .png]-Dateien können nicht auf einer Karte dargestellt werden.
* Änderungen an Gruppen und Berechtigungen, die über die Benutzerverwaltung durchgeführt werden, werden erst bei einer erneuten Anmeldung wirksam.
* Für einige Benutzer ist die Erstellung einer Karte aus einer PDF und deren Freigabe auf einer Pinnwand unter Umständen nicht möglich.
* Für einige Benutzer ist das Löschen nicht mehr aktueller Assets möglich, ohne dabei eine Fehlermeldung zu empfangen.
* Benutzer können auf Pinnwänden keine PowerPoint-Dateien freigeben.
* Die Leistung der Benutzeroberfläche der [!DNL Experience Cloud] ist u. U. reduziert, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* Die [!DNL Search&Promote]-Verknüpfungen stehen auf der Seite [!UICONTROL Unternehmen und Produktzugriff] nicht zur Verfügung.

## Version 14.9.1 – 18. September 2014 {#section_20F156A9CC2F4FC59C4970075C181D3A}

**Fehlerbehebungen und Verbesserungen**

* Wenn Sie zu [!DNL experiencecloud.adobe.com] navigieren, ist die Anmeldungserfahrung nun mit der Anmeldung von Creative Cloud von Adobe konsistent.
* Die Verknüpfung erfolgt nun auf der Seite „Unternehmen verwalten“ für jede Lösung gleich (nach dem Erhalt einer entsprechenden Einladung).

**Bekannte Probleme**

* Änderungen an Gruppen und Berechtigungen, die über die Benutzerverwaltung durchgeführt werden, werden erst bei einer erneuten Anmeldung wirksam.
* Für einige Benutzer ist die Erstellung einer Karte aus einer PDF und deren Freigabe auf einer Pinnwand unter Umständen nicht möglich.
* Einige Benutzer haben unter Umständen Probleme beim Hochladen von Assets auf eine Pinnwand.
* Für einige Benutzer ist das Löschen nicht mehr aktueller Assets möglich, ohne dabei eine Fehlermeldung zu empfangen.
* Benutzer können auf Pinnwänden keine PowerPoint-Dateien freigeben.
* Manche [!DNL .png]-Dateien können nicht auf einer Karte dargestellt werden.
* Die Leistung der Benutzeroberfläche der [!DNL Experience Cloud] ist u. U. reduziert, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* Die [!DNL Search&Promote]-Verknüpfungen stehen auf der Seite [!UICONTROL Unternehmen und Produktzugriff] nicht zur Verfügung.
* Einige Benutzer stellen möglicherweise fest, dass [!DNL Creative Cloud]-Inhalte aus ihrem Ordner entfernt wurden, wenn die Inhalte nicht in [!DNL Experience Cloud] freigegeben sind.

## Version 14.8.1 – 21. August 2014 {#section_03BF00F6A95A490C91BCC0A1988FA7AA}

Neue Funktionen und Fehlerbehebungen in der Benutzeroberfläche für die Zusammenarbeit und Freigabe der [!DNL Adobe Experience Cloud]

<table id="table_1E7DBEB5E83B4E4285B6FD1D718CD16D"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Der Zugriff auf <span class="keyword">Adobe Mobile Services</span> ist jetzt über das Navigationsmenü auf der linken Seite möglich. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Bekannte Probleme**

* Änderungen an Gruppen und Berechtigungen, die über die Benutzerverwaltung durchgeführt werden, werden erst bei einer erneuten Anmeldung wirksam.
* Für einige Benutzer ist die Erstellung einer Karte aus einer PDF und deren Freigabe auf einer Pinnwand unter Umständen nicht möglich.
* Einige Benutzer haben unter Umständen Probleme beim Hochladen von Assets auf eine Pinnwand.
* Einige Benutzer können sich von [!DNL Target] aus möglicherweise nicht bei der [!DNL Experience Cloud] anmelden.
* Manche Audience Manager-Benutzer können sich nicht bei der [!DNL Experience Cloud] anmelden.
* Für einige Benutzer ist das Löschen nicht mehr aktueller Assets möglich, ohne dabei eine Fehlermeldung zu empfangen.
* Aus der [!DNL Experience Cloud] gelöschte Dateien werden nicht aus dem [!DNL Digital Asset Management] gelöscht.
* Benutzer können auf Pinnwänden keine PowerPoint-Dateien freigeben.
* Manche [!DNL .png]-Dateien können nicht auf einer Karte dargestellt werden.
* Die Leistung der Benutzeroberfläche der [!DNL Experience Cloud] ist u. U. reduziert, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* Die [!DNL Search&Promote]-Verknüpfungen stehen auf der Seite [!UICONTROL Unternehmen und Produktzugriff] nicht zur Verfügung.
* Einige Benutzer stellen möglicherweise fest, dass [!DNL Creative Cloud]-Inhalte aus ihrem Ordner entfernt wurden, wenn die Inhalte nicht in [!DNL Experience Cloud] freigegeben sind.

## Version 14.7.1 – 24. Juli 2014 {#section_B22D4F830756463DB27BB4D508D9ADD5}

Neue Funktionen und Fehlerbehebungen in der Benutzeroberfläche für die Zusammenarbeit und Freigabe der [!DNL Adobe Experience Cloud]

**Bekannte Probleme**

* Aus der [!DNL Experience Cloud] gelöschte Dateien werden nicht aus dem [!DNL Digital Asset Management] gelöscht.
* Bei einigen [!UICONTROL Exchange]-Benutzern wird der Name in den Kommentaren möglicherweise als lange ID anstelle des richtigen Namens angezeigt.
* Manche [!DNL .png]-Dateien können nicht auf einer Karte dargestellt werden
* Das Hochladen von Dateien ermöglicht mehr Dateitypen als die Drag-and-drop-Methode. Die besten Ergebnisse werden beim Hochladen mithilfe von [!UICONTROL Assets] erzielt.
* Die [!DNL Search&Promote]-Verknüpfungen stehen auf der Seite [!UICONTROL Unternehmen und Produktzugriff] nicht zur Verfügung.
* [!DNL Exchange]-Benutzer müssen ihre Cookies löschen, um ihres Benutzererlebnis zu verbessern.
* Die Benutzeroberfläche der [!DNL Experience Cloud] ist u. U. beeinträchtigt, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* Einige Benutzer werden möglicherweise feststellen, dass ihre [!DNL Creative Cloud]-Inhalte aus ihrem Ordner entfernt wurden, wenn die Inhalte in [!DNL Experience Cloud] nicht freigegeben sind.
* Nach 15 Minuten Inaktivität werden Sie abgemeldet. Zudem werden Sie, wenn Sie sich an einem Ort abmelden, von der [!DNL Experience Cloud] abgemeldet.
* Einige Benutzer sind u. U. nicht in der Lage, ihre Audience Manager-Konten mit der [!DNL Experience Cloud] zu verknüpfen.
* [!UICONTROL Exchange]-Benutzer können nur Englisch in der Sprachauswahl sehen.

**Fehlerbehebungen**

Keine nennenswerten

## Version 14.6.1 – 19. Juni 2014  {#marketing_cloud_interface}

Neue Funktionen und Fehlerbehebungen in der Benutzeroberfläche für die Zusammenarbeit und Freigabe der [!DNL Adobe Experience Cloud]

**Verbesserung**

<table id="table_C9BD63436BF0414B97B8D07387D1993B"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> Schaltfläche <span class="wintitle">Speichern</span> in Audiences </p> </td> 
   <td colname="col2"> <p>Beim Erstellen einer Zielgruppe ist die Schaltfläche <span class="wintitle">Speichern</span> auf der Seite <span class="wintitle">Neue Zielgruppe erstellen</span> nun deaktiviert, bis alle erforderlichen Felder ausgefüllt wurden. 
     <!--MAC-19712 --></p> </td> 
  </tr> 
 </tbody> 
</table>

**Bekannte Probleme**

* Aus der [!DNL Experience Cloud] gelöschte Dateien werden nicht aus dem [!DNL Digital Asset Management] gelöscht.
* Das Hochladen von Dateien ermöglicht mehr Dateitypen als die Drag-and-drop-Methode. Die besten Ergebnisse werden beim Hochladen mithilfe von Assets erzielt.
* Die [!DNL Search&Promote]-Verknüpfungen stehen auf der Seite [!UICONTROL Unternehmen und Produktzugriff] nicht zur Verfügung.
* Filter, die auf Trendberichte aus [!DNL Analytics] angewendet werden, werden nicht auf Karten in der [!DNL Experience Cloud] angewendet.
* Einige Benutzer können ihr Zielgruppen-Management-Konto nicht mit ihrem [!DNL Experience Cloud]-Konto verknüpfen.
* Nach 15 Minuten Inaktivität werden Sie abgemeldet. Zudem werden Sie, wenn Sie sich an einem Ort abmelden, aus der Experience Cloud abgemeldet.
* Bei einigen Exchange-Benutzern wird der Name in den Kommentaren möglicherweise als lange ID anstelle des richtigen Namens angezeigt.

**Fehlerbehebungen**

* Ein Problem wurde behoben, das Video-Uploads in Apps verhinderte.

## Version 14.5.1 – 22. Mai 2014 {#section_7E22B2CB3ABA4D6EAED8CA8EFDE5433E}

<table id="table_4E4B34EEE3D94D78BA1A1FBC62950559"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Experience Cloud Exchange </p> </td> 
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol">Hilfe</span> &gt; <span class="uicontrol">Exchange</span></p> <p><span class="keyword">Experience Cloud</span><span class="wintitle">Exchange</span> ist eine zentrale Stelle, an der Sie Digital Marketing-Erweiterungen über Apps suchen, durchsuchen, auswählen, bezahlen und herunterladen können. </p> <p>Zu den Apps gehören Data Connectors, benutzerdefinierte Konfigurationen des Hauptprodukts von Adobe, Anwendungen von Drittherstellern, Berichte und <span class="keyword">Experience Cloud</span>-Karten. </p> <p>Siehe <a href="../exchange.md#concept_E07F16F070544B82B56527A845C41D59" format="dita" scope="local"> Exchange Marketplace</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Experience Cloud Audiences </p> </td> 
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol">Zielgruppen</span></p> <p> In <span class="wintitle">Zielgruppen</span> erstellen, bearbeiten und verwalten Sie Zielgruppen in etwa so, wie Sie mit Segmenten arbeiten. Sie können z. B. ein Segment in Reports &amp; Analysen erstellen und es dann in <span class="wintitle">Experience Cloud</span><span class="wintitle">Audiences</span> freigeben. Nach der Freigabe ist die Zielgruppe in <span class="keyword">Adobe Target</span> für Kampagnenaktivitäten und in Adobe Audience Manager für die Segmentierung verfügbar. </p> <p> <p>Hinweis: Besuchen Sie <a href="https://www.adobe.com/go/audiences" format="http" scope="external">https://www.adobe.com/go/audiences</a>, um die Aktivierung in Target anzufordern. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Benutzer, die auf <span class="keyword">Experience Cloud</span>-Karten erwähnt werden, haben nun die Berechtigung für diese Karte. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Neue Benutzer von Adobe können ihre Scene7-Konten mit einer Adobe ID und ihren Team-Mitgliedern verknüpfen. Administratoren haben die Möglichkeit, die Verknüpfung von Benutzern und Scene7-Konten aufzuheben. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Asset-Synchronisierung </p> </td> 
   <td colname="col2"> <p> Sie können Assets aus Adobe Experience Manager (AEM) für die Adobe Experience Cloud und Adobe Creative Cloud freigeben. Änderungen an diesen Assets werden dann automatisch mit deren freigegebenen Kopien in der Adobe Experience Cloud bzw. Adobe Creative Cloud synchronisiert. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Die [!DNL Experience Cloud] wurde nicht mit [!DNL Adobe Target] verknüpft. Dieses Problem trat auf, wenn die [!DNL Adobe Target]-Anmeldung auf mehreren [!DNL Target]-Servern zur Verfügung stand.
* [!DNL Adobe Media Optimizer] erstellte Benutzer nicht automatisch, wenn der Benutzer in der [!DNL Experience Cloud] erstellt worden war.
* Optionen in Kombinationsfeldern zum Hinzufügen neuer Benutzer wurden bei der Eingabe vorübergehend ausgeblendet.
* Der Link „Kommentare“ auf der Ansicht der Assets und Karten konnte nicht angeklickt werden.
* Nachdem einem Asset ein benutzerdefinierter Tag hinzugefügt wurde, blieben keine weiteren Änderungen an Metadaten bestehen.
* Beim Löschen eines Bildes gibt Assets keine Warnung aus, wenn das Bild in Adobe Target Essentials verwendet wird.
* Die Benutzeroberfläche der [!UICONTROL Experience Cloud] arbeitete langsam, wenn sie von vielen Benutzern gleichzeitig verwendet wurde.
* Beim Löschen eines Bildes in [!UICONTROL Experience Cloud Assets] wurde keine Warnmeldung ausgegeben, wenn das Bild in [!DNL Adobe Target Essentials] in Verwendung war.
* Wenn die Option **[!UICONTROL Angaben speichern]** nicht während des Anmeldevorgangs ausgewählt wurde, wurde der Benutzer nach 15 Minuten abgemeldet.
* Benutzer mussten sich ab- und wieder anmelden, damit alle Änderungen an Berechtigungen wirksam wurden.
* Die Anmeldung bei der [!DNL Experience Cloud] dauerte länger als eine Sekunde.
* Beim Löschen von Dateien aus [!DNL Experience Cloud] wurde dieser Vorgang bei manchen Benutzern nicht mit dem [!DNL Digital Asset Management] synchronisiert.
* Benutzer wurden nach nur 15 Minuten Browserinaktivität abgemeldet.
* Benutzer konnten auf Pinnwänden keine PowerPoint-Dateien freigeben.
* Bei manchen Benutzern hatte die visuelle Darstellung in Internet Explorer 10 im Vergleich zu anderen Browsern eine geringere Qualität.

## Version 14.4.1 – 22. April 2014  {#section_E2A699764E744D2E8D418E9A3D40AF6B}

<table id="table_D95C0DC64F2A4B47BAC83E504CFD6825"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Erstellen von Karten aus Hilfethemen </p> </td> 
   <td colname="col2"> <p>Wenn Sie in der Symbolleiste „Lesezeichen“ Ihres Browsers die Funktion „Mit Adobe Experience Cloud teilen“ aktivieren, können Sie jetzt Hilfeseiten von der Microsite-URL freigeben. </p> <p> <b>So teilen Sie ein Hilfethema</b> </p> 
    <ol id="ol_F94B816121494B0FA16CC07B0E96AED8"> 
     <li id="li_F47187D4B5FE46D3A51D257DD569B4D6"> <p>Klicken Sie in der <span class="keyword">Experience Cloud</span> auf <span class="uicontrol">Administration</span>. </p> </li> 
     <li id="li_94EF58E7A4974B63951E14F72A710183"> <p>Ziehen Sie die Schaltfläche <span class="uicontrol">Mit Adobe Experience Cloud teilen</span> in Ihre Symbolleiste „Lesezeichen“. </p> </li> 
     <li id="li_69EEC4F25D8F4AD7AA106A10B7F50FF6"> <p>Navigieren Sie zu einer Hilfeseite (oder bleiben Sie auf dieser Seite) und klicken Sie dann in Ihrem Browser in der Symbolleiste „Lesezeichen“ auf <span class="uicontrol">Mit Adobe Experience Cloud teilen</span>. </p> <p>Auf diese Weise wird eine Karte erstellt, die Sie in der <span class="wintitle">Experience Cloud</span> anzeigen können. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Nachdem einem Asset ein benutzerdefiniertes Tag hinzugefügt wurde, bleiben keine weiteren Änderungen an Metadaten bestehen.
* Benutzer müssen das Forum aktualisieren, damit die gelöschten Karten aus der Ansicht entfernt werden.
* Wenn die Option **[!UICONTROL Angaben speichern]** nicht während des Anmeldevorgangs ausgewählt wird, wird der Benutzer nach 15 Minuten abgemeldet.
* Die Landingpage der [!DNL Analytics]-Lösung weist Formatierungsfehler auf.
* Benutzer müssen sich ab- und wieder anmelden, damit alle Änderungen an Berechtigungen wirksam werden.
* Beim Löschen eines Bildes gibt [!UICONTROL Assets] keine Warnung aus, wenn das Bild in [!DNL Adobe Target Essentials] verwendet wird.
* Der Link „Kommentare“ auf der Ansicht der Assets und Karten kann nicht angeklickt werden.
* Optionen in Kombinationsfeldern zum Hinzufügen neuer Benutzer werden bei der Eingabe vorübergehend ausgeblendet.
* Die Anmeldung bei der [!DNL Experience Cloud] dauert länger als eine Sekunde.
* In [!DNL Media Optimizer] freigegebene Daten werden in [!DNL Experience Cloud] falsch angezeigt.
* Adobe [!DNL Media Optimizer] erstellt Benutzer nicht automatisch, wenn der Benutzer in der [!DNL Experience Cloud] erstellt wurde.
* Die [!DNL Experience Cloud] kann nicht mit [!DNL Adobe Target] verknüpft werden, wenn die [!DNL Adobe Target]-Anmeldung auf mehreren [!DNL Target]-Servern verwendet werden kann.
* Die Benutzeroberfläche der [!DNL Experience Cloud] ist u. U. beeinträchtigt, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* [!DNL Search&Promote]-Verknüpfungen stehen auf der Seite [!UICONTROL Unternehmen und Produktzugriff] nicht zur Verfügung.
* Simulationskarten in [!DNL Adobe Media Optimizer] werden nicht ordnungsgemäß dargestellt.
* Filter, die auf Trendberichte aus [!DNL Analytics] angewendet werden, werden nicht auf Karten in der [!DNL Experience Cloud] angewendet.
* Filter, die auf Trendberichte aus Analytics angewendet werden, werden nicht auf Karten in der Experience Cloud angewendet.
* Manche Excel- oder CSV-Dateien können nicht in eine Pinnwand hochgeladen werden.
* Manche Benutzer können möglicherweise ihr Zielgruppen-Management-Konto nicht mit ihrer [!DNL Experience Cloud] verknüpfen.
* Einigen Benutzern wird u. U. ein Fehler angezeigt, wenn sie [!DNL Analytics]-Segmente in der [!DNL Experience Cloud] teilen.
* Manche Benutzer können in der [!UICONTROL Asset-Auswahl] möglicherweise keine Unterordner anzeigen.
* Manche Benutzer können möglicherweise keine AdLens-Geräte in der [!DNL Experience Cloud] freigeben.

## Version 14.3.1 – 13. März 2014 {#section_5D142E3225E3477A84DC01B8197D39BC}

Version 14.3.1 ist ein Maintenance Release zur Verbesserung der Geschwindigkeit, Stabilität und Sicherheit. Sie umfasst keine wichtigen neuen Funktionen.

**Fehlerbehebungen**

* Sie haben nun die Möglichkeit, Ihre Avatar-Abbildung zu entfernen.
* Ein Problem wurde behoben, das dazu geführt hat, dass Sie die Verknüpfung Ihrer [!DNL Adobe Media Optimizer]-Konten nicht aufheben konnten.

**Bekannte Probleme**

* Beim Löschen eines Bildes in Experience Cloud-Assets wird keine Warnung ausgegeben, wenn das Bild in Adobe Target Essentials verwendet wird.
* Das Aktualisieren einer Karte aus [!DNL Analytics] kann in der erweiterten Karte gelegentlich zu einem leeren Diagramm führen.
* Benutzer müssen sich ab- und wieder anmelden, damit alle Änderungen an Berechtigungen wirksam werden.
* Wenn bei der Anmeldung *`Remember me`* nicht aktiviert ist, wird der Benutzer nach 15 Minuten abgemeldet.
* Die Landingpage der [!DNL Analytics]-Lösung weist Formatierungsfehler auf.
* Der Link „Kommentare“ auf der Ansicht der Assets und Karten kann nicht angeklickt werden.
* Die Benutzeroberfläche der Experience Cloud ist u. U. beeinträchtigt, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* Die Experience Cloud kann nicht mit [!DNL Adobe Target] verknüpft werden, wenn die [!DNL Adobe Target]-Anmeldung auf mehreren Target-Servern verwendet werden kann.
* Die Anmeldung bei der Experience Cloud dauert länger als eine Sekunde.
* Nachdem einem Asset ein benutzerdefiniertes Tag hinzugefügt wurde, bleiben keine weiteren Änderungen an Metadaten bestehen.
* [!DNL Adobe Media Optimizer] erstellt Benutzer nicht automatisch, wenn der Benutzer in der Experience Cloud erstellt wurde.
* Optionen in Kombinationsfeldern zum Hinzufügen neuer Benutzer werden bei der Eingabe vorübergehend ausgeblendet.
* In [!DNL Media Optimizer] freigegebene Daten werden in der Experience Cloud falsch angezeigt.
* Die Freigabe von Bildern aus Flickr schlägt fehl.
* Filter, die auf Trendberichte aus [!DNL Analytics] angewendet werden, werden nicht auf Karten in der Experience Cloud angewendet.
* Änderungen an Gruppen und Berechtigungen, die über die Benutzerverwaltung durchgeführt werden, werden erst bei einer erneuten Anmeldung wirksam.
* [!DNL Search&Promote]-Verknüpfungen stehen in [!UICONTROL Organisationen und Produktzugriff] nicht zur Verfügung.
* Benutzer müssen die Pinnwand aktualisieren, damit die gelöschten Karten aus der Ansicht entfernt werden.
* Manche Excel- oder CSV-Dateien können nicht in eine Pinnwand hochgeladen werden.
* Simulationskarten in [!DNL Adobe Media Optimizer] werden nicht ordnungsgemäß dargestellt.
* Manche PNG-Dateien können nicht auf einer Karte dargestellt werden.
* Beta-Feedback kann nicht übermittelt werden.

## Version 14.2.1 – 24. Februar 2014  {#section_5AD81B0737C843AFB4BE9C4420D70EB3}

<table id="table_DFAB002358C94A17A7F91DAB323A488F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>oEmbed </p> </td> 
   <td colname="col2"> <p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Daten aktualisieren </p> </td> 
   <td colname="col2"> <p> 
     <!--MAC-18174-->Das Symbol <span class="uicontrol">Daten aktualisieren</span> für ein Diagramm auf einer Karte ist nun ausgeblendet, wenn die Lösung keine Aktualisierung von Daten zulässt. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Es wurde ein Problem behoben, das das Anwenden von Segmentfiltern bei freigegebenen [!DNL Analytics]-Berichten verhinderte.
* Es wurde ein Problem behoben, bei dem Lösungen auf der Seite [!UICONTROL Experience Cloud-Lösungen] als zugeordnet angezeigt wurden, selbst wenn die Konten der Lösung nicht zugeordnet waren.
* Es wurde ein Problem behoben, das [!DNL Adobe Target]-Kunden in Asien daran hinderte, auf der Zuordnungsseite auf die Schaltfläche **[!UICONTROL Weiter zu Experience Cloud]** zu klicken.
* Es wurde ein Problem behoben, das die Freigabe von YouTube-Videos verhinderte.
