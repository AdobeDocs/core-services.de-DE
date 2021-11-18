---
description: „Neueste Funktionen, Versionshinweise und bekannte Probleme für die Experience Cloud-Dienste wie Kundenattribute, Zielgruppen und Benutzerverwaltung.“
keywords: Hauptdienste
solution: Experience Cloud
title: 'Gesammelte Versionshinweise '
uuid: fcff8cc6-e587-4bf2-9a75-261d4eabc7d4
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: b71d144c-a097-4cdb-9721-671519d38aff
source-git-commit: ae14748aa7b0f0d803d48fe980a6743f53d996ab
workflow-type: tm+mt
source-wordcount: '4276'
ht-degree: 94%

---

# Gesammelte Versionshinweise

Funktionen, Versionshinweise und bekannte Probleme in Verbindung mit der Experience Cloud-Schnittstelle.

Eine Liste der Aktualisierungen der Dokumentation finden Sie unter [Experience Cloud](doc-updates.md#concept_4C8983FCD23848A4B1E4C2D99ED82784).

Versionshinweise zu allen Anwendungen finden Sie unter [Experience Cloud - Versionshinweise](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=de).

## August 2021

| Funktion | Datum | Beschreibung |
| ------- | ------- | -------|
| [!UICONTROL Unified Recents] – Erweiterte Unterstützung für kürzlich aufgerufene Geschäftsobjekte | 10. August 2021 | [!UICONTROL Unified Recents] wurde auf zusätzliche Geschäftsobjekte in Journey Optimizer und Experience Platform erweitert. Journey Optimizer-Kunden können ihre kürzlich aufgerufenen Objekte (Nachrichten, Journeys, Segmente, Schemas, Data Sources, Datenquellen, Ereignisse, Aktionen, Quellen und Ziele) über die Adobe Journey Optimizer-Startseite finden. |

## Juli 2021

Die einheitliche Suche wird aktualisiert und ist nun für Journey Optimizer, Angebote und Experience League verfügbar. Zuvor war diese Funktion nur für Experience Platform-Benutzer verfügbar.

## Juni 2021

| Funktion | Datum | Beschreibung |
| ------- | ------- | ------- |
| Single-Sign-On-Unterstützung für Adobe Federated IDs | 17. Juni 2021 | Wenn Sie Federated IDs verwenden, können Sie sich bei Experience Cloud anmelden, ohne eine E-Mail-Adresse oder ein Passwort eingeben zu müssen. Um diese Funktion zu verwenden, fügen Sie `#/sso:@domain` zur Experience Cloud-URL hinzu. <br>Nehmen wir beispielsweise an, Sie sind der Eigentümer der Domain `adobecustomer.com` und möchten sich bei Adobe Analytics anmelden. Die URL lautet: `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`. |
| Experience League Search | 1. Juni 2021 | Die Suche in der Dokumentation zu Experience Leaguen wurde verbessert. Navigieren Sie zu [Experience League](https://experienceleague.adobe.com/docs/?lang=de) und verwenden Sie das Feld **[!UICONTROL Suchen]**, um Tutorials, Dokumentationen, Kurse und mehr zu finden. |

{style=&quot;table-layout:auto&quot;}

## Mai – 2021

| Funktion | Datum | Beschreibung |
| ------- | ------- | ------- |
| Experience Cloud-Kopfzeile und -Navigation | 20. Mai 2021 | Adobe Experience Cloud-Aktualisierungen beinhalten eine Änderung des hellen Designs für die Kopfzeile. Sie können einfach wieder zu einem dunklem Design wechseln und erhalten einen Link zur Steuerung zusätzlicher Voreinstellungen von Ihrem Benutzeravatar in der Kopfzeile von Experience Cloud. Obwohl nicht alle Anwendungen in Experience Cloud das Design unterstützen, wird durch diese Funktion die Unterstützung künftiger Designs freigeschaltet. |
| Experience Cloud Global Search | 20. Mai 2021 | Mit dieser Version können Sie mit der globalen Experience Cloud-Suche nach allen [Experience League](https://experienceleague.adobe.com/?lang=de#home)-Dokumentationen, -Kursen und -Tutorials suchen. (Derzeit steht die globale Suche nur Benutzern von Experience Platform zur Verfügung. Die globale Suchfunktion für die [!UICONTROL Platform] ermöglicht es Ihnen, in Experience Cloud nach beliebigen Geschäftsobjekten zu suchen, z. B. nach Segmenten, Datensätzen, Schemas und mehr.) |
| Experience Cloud-Spracheinstellungen | 20. Mai 2021 | Dieses Update bietet die Möglichkeit, Ihre bevorzugten Sprachen in den Experience Cloud-[Voreinstellungen](https://experience.adobe.com/preferences) festzulegen. |

{style=&quot;table-layout:auto&quot;}

## August 2020

| Funktion | Beschreibung |
| -----------| ---------- |
| Admin-Tool – Richtlinien | Auf dieser Seite finden Sie eine vollständige Liste der Experience Cloud-Richtlinien in Ihrem Unternehmen. Sie enthält Informationen zu Produkten, Instanzen, Benutzern und Entwicklern. Sie können nach benutzerdefinierten Ansichten der Richtlinienliste suchen, sortieren und filtern. Weitere Informationen finden Sie in der Hilfe zum [Experience Cloud-Admin-Tool](admin-tool-experience-cloud.md). |

{style=&quot;table-layout:auto&quot;}

## April 2020

* Die Seite „Experience Cloud- [!UICONTROL Feed]“ wurde entfernt. (EXC-8505)
* Die Experience Cloud-Anmeldeseite wurde aktualisiert und enthält jetzt neue Branding-Elemente. (EXC-10747)

## Februar 2020

| Funktion | Beschreibung |
| -----------| ---------- |
| Admin-Tool – Benutzerdetails anzeigen | Administratoren können im neuen Admin-Tool eine sortierbare und filterbare Liste aller Experience Cloud-Benutzer und deren Details anzeigen. Zu den Benutzerdetails zählen der Produktzugriff, die Rollen und die zuletzt aufgerufenen Informationen. Weitere Informationen finden Sie in der Hilfe zum [Experience Cloud-Admin-Tool](admin-tool-experience-cloud.md). |

{style=&quot;table-layout:auto&quot;}

**Fehlerbehebungen**

* **Kundenattribute:** Auf der Benutzeroberfläche „Kundenattribute“ werden jetzt zusätzliche Status zu den in Target synchronisierten Profilen angezeigt. (MCUI-10231)
* **Triggers Hauptdienst:** Aufgrund der mangelnden Verwendung wurde der Tendenzwert „Wahrscheinlichkeit einer Rückkehr in 30 Tagen“ beim Erstellen eines Auslösers vom Typ „Abbruch“ entfernt. (MCUI-10056)

## Januar 2020

* Die Feed-Seite wird seit Dezember 2019 nicht mehr unterstützt. Innerhalb des Produkts finden Sie eine Benachrichtigung zur Einstellung. (MCUI-10039)

## August 2019

* Ein kritisches Problem bei der Experience Cloud-Anmeldung wurde behoben, durch das manche Sitzungen unterbrochen wurden. (MCUI-6908)
* Die Anmeldung von Experience Cloud wurde aktualisiert, um die Leistung zu verbessern und die Latenz zu reduzieren. (MCUI-6854, MCUI-6869, MCUI-6883)
* Die Benutzeroberfläche wurde aktualisiert. (MCUI-6861, MCUI-6911, MCUI-6862)
* Ein Problem mit Experience Cloud [!UICONTROL Triggers] wurde behoben, das zur falschen Interpretation der _Like_-Bedingung in der [!UICONTROL Trigger]-Definition geführt hatte. (MCUI-6611)

## April 2019

* Aktualisierung des App-Switchers, um Marketo in die Experience Cloud-Anwendungs-Suite und Branding-Updates in Experience Platform aufzunehmen. (MCUI-6529)
* Aktualisierung der Experience Cloud-Startseite mit Navigationslinks zur Feed- und Admin-Seite. (MCUI-6682)
* Es wurde ein Problem in der [!UICONTROL Auslöserdefinition] behoben, damit der „like“-Satz korrekt verwendet wird. (MCUI-6611)
* Verbesserungen an den Kundenattributen zur besseren Anmeldung im Abonnementdienst. (MCUI-6519)

## Version 19.1.1 – 17. Januar 2019

**Hinweis:** Im März 2019 wird Internet Explorer 11 von der Experience Cloud-Benutzeroberfläche nicht unterstützt.

* Es wurde ein Fehler behoben, der verhinderte, dass die Suche in der Hilfe Ergebnisse zurückgab. (MCUI-1670)
* Korrigierte und verbesserte eVar-Verwaltung in Triggers. (MCUI-6400)

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
   <td colname="col1"> <p>Vorkonfigurierte Produktkonfigurationen in der Admin Console </p> </td> 
   <td colname="col2"> <p>Kundenadministratoren in Experience Cloud können Produktkonfigurationen nutzen, die zuvor erstellt und Standardberechtigungsgruppen für Analytics und das Dynamic Tag Management zugeordnet wurden. </p> <p>Diese Optimierung ist für neu bereitgestellte Organisationen verfügbar und verringert die Zeit, die Organisationen zur Verwaltung von Benutzern in der Admin Console benötigen. </p> </td> 
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
   <td colname="col1"> <p>Verbesserungen in Experience Cloud Assets </p> </td> 
   <td colname="col2"> <p>In Experience Cloud Assets können Sie Ihre digitalen Assets an einem zentralen Speicherort speichern, freigeben und synchronisieren. Experience Cloud Assets nutzen einige in <span class="keyword"> Adobe Experience Manager</span> (AEM) verfügbare Funktionen. </p> <p>Weitere Informationen finden Sie unter <a href="experience-cloud-assets.md#concept_DDA5224C907D4A4F817D795DA0ED64D0" format="dita" scope="local">Experience Cloud</a></p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Verbesserungen bei der Kontoverknüpfung </p> </td> 
   <td colname="col2"> <p>Der Arbeitsablauf für die Verknüpfung von Anwendungskonten mit dem Experience Cloud (Adobe ID) wurde verbessert. Dieser neue Arbeitsablauf ermittelt alle Konten des Benutzers, die mit einem Unternehmen verbunden sind, und ermöglicht Ihnen die Auswahl des Kontos, das verknüpft werden soll. Außerdem wurde die Erfahrung bei der Kontoverknüpfung optimiert, sodass Sie nicht mehr auf die Seite „Unternehmen verwalten“ zugreifen müssen, um Konten manuell zu verknüpfen. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Es wurde ein Fehler behoben, durch den die Verknüpfung und die einmalige Anmeldung für Analytics verhindert wurde. Bei diesem Problem wurde der Hinweis bzw. die Fehlermeldung „FEHLER IMS SSO fehlgeschlagen: Verknüpfte Firma konnte nicht gefunden werden.“ angezeigt.

**Bekanntes Problem**

Wenn Sie über **[!UICONTROL Experience Cloud]** > **[!UICONTROL Activation]** auf das Dynamic Tag Management zugreifen, Ihr Konto für das Dynamic Tag Management jedoch nicht mit der Experience Cloud (Adobe ID) verknüpft ist, können Sie sich nicht beim Dynamic Tag Management anmelden. Um dieses Problem zu umgehen, müssen Sie in einem neuen Browser-Tab direkt zu `dtm.adobe.com` navigieren.

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
   <td colname="col1"> Meldungen zur Zielgruppenbibliothek </td> 
   <td colname="col2"> <p> Die Zielgruppenbibliothek wurde so verbessert, dass beim Erstellen von Zielgruppen oder Auftreten eines Timouts hilfreiche Meldungen angezeigt werden. </p> <p>Wenn Sie beispielsweise mehr als fünf Regeln hinzufügen, wird eine Meldung mit dem Hinweis angezeigt, dass Sie die maximal zulässige Anzahl Regeln überschritten haben. (MAC-27376, MAC-27375) </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Microsoft® [beendet den Support](https://www.microsoft.com/de-de/WindowsForBusiness/End-of-IE-support) für Internet Explorer 8, 9 und 10. Aus diesem Grund werden keine Probleme mehr behoben, die in Verbindung mit diesen speziellen Versionen von Internet Explorer gemeldet werden.

## Version 15.10 – 14. Oktober 2015 {#section_68123833D3634BD3A473C12862BF9606}

**Bekannte Probleme**

* Kunden können sich nicht bei Report Builder anmelden, wenn sie sich über Experience Cloud per SSO bei Analytics anmelden. Dieses Problem hat keine Auswirkungen auf Kunden, die ältere Analytics-Anmeldeinformationen verwenden.
* Bekanntes Problem mit der Funktion „Link zum Bericht“ in Analytics. Kunden, die sich über Experience Cloud bei Analytics anmelden, werden beim Versuch, einen Bericht gemeinsam zu nutzen, zu einer Analytics-Anmeldeseite geleitet, auf der SSO nicht möglich ist.

## Version 15.9 – 10. September 2015 {#section_BCCE3E7DF62A4FF5A57B9C8FE2A5F37B}

* Es wurde ein Leistungsproblem mit der Audience Manager API behoben, das zeitweise zu Timeouts beim Hochladen von Kundenattributdaten geführt hat. (MAC-26305)
* Es wurde ein Fehler behoben, der verhinderte, dass Benutzer einem Abonnement bis zu 200 Kundenattribute hinzufügen konnten. (MAC-26188)
* Es wurde ein Problem mit der Zielgruppenbibliothek behoben, das die Freigabe von Zielgruppen aus der Analytics-Segmentierung verhinderte. Dieses Problem verursachte die Anzeige von „Erfassen von Daten“ (0 Zielgruppen). Zum Vermeiden dieses Problems empfiehlt Adobe, die Segmentgrößen pro Segment unter 50.000 Zielgruppenmitgliedern zu halten. (MAC-25788)
* Ein vorheriges bekanntes Problem mit den Kundenattributen wurde behoben: Die Seite „Schema bearbeiten“ verursachte einen Fehler mit der Inhaltsbewahrung, der beim Ändern des Anzeigenamens ausgegeben wurde. (MAC-25589, AN-103834)

## Version 15.7 – 22. Juli 2015 {#section_2683A152176944E48EF6C943892975B7}

* Es wurde ein Fehler behoben, der verhinderte, dass auf der Seite „Schema anzeigen/bearbeiten“ (in Kundenattributen) angegebene Attributbeschreibungen in Analytics-Berichten aktualisiert wurden. (MAC-25985)
* Es wurde ein Fehler behoben, der verhinderte, dass die Miniaturansichten für hochgeladene Assets gerendert wurden. (MAC-25863)
* Es wurde ein Problem behoben, bei dem neue Segmente, die in Reports &amp; Analytics erstellt wurden, nicht in Experience Cloud-Zielgruppen verfügbar waren. (MAC-25817)
* Es wurde ein Fehler behoben, der bei Verwendung des Besucher-ID-Dienstes die Freigabe von Zielgruppen in Analytics verhinderte. (MAC-25788, MAC-25747)
* Die Unterstützung für Multibyte-Zeichen in Kundenattributen wurde hinzugefügt. (MAC-25552)

**Bekanntes Problem**

Ein bekanntes Problem verursacht die Erstellung doppelter automatisch generierter Konten in Audience Manager und die automatische Verknüpfung dieser Konten mit der Experience Cloud-Identität eines Benutzers. Dieses Problem tritt auf, wenn Sie versuchen, zu Audience Manager zu navigieren, bevor Sie Ihre Konten verknüpfen. Adobe empfiehlt Ihnen, die Verknüpfung Ihrer Audience Manager-Konten mit der Experience Cloud vorzunehmen, bevor Sie zu Audience Manager navigieren. (MAC-25640)

## Version 15.6.1 – 11. Juni 2015 {#section_AD2019F8D2F84C9EB2B0533FAACF7043}

Keine Informationen verfügbar.

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
   <td colname="col2"> <p>Die linken Navigationsmenüs wurden aktualisiert und wurden so gestaltet, dass sie Zugriff auf alle Hauptdienste und Anwendungen bieten. Wichtige Änderungen umfassen Folgendes: </p> 
    <ul id="ul_5BEBAB86B9234A239C4E2DAF8826D8E3"> 
     <li id="li_7FA9F64CE69144B8A8A92746BF40E5A1">Die Menüauswahlmöglichkeiten für die <span class="term">Zielgruppenbibliothek</span> und die <span class="term">Kundenattribute</span> sind nun unter <span class="term">Zielgruppen</span> zu finden. </li> 
     <li id="li_95D62A43AE6243DBB2A65EDB830D05C4">Die <span class="term">Exchange</span>-Menüauswahl wurde vom Dropdown-Menü „Hilfe“ zur linken Navigationsleiste verlegt. </li> 
     <li id="li_0443FD50C78446CD8AA27A4F272CAD31"> <span class="term">Lösungen</span> wurde entfernt. Sie können alle Anwendungen von der unteren Hälfte der Navigationsleiste aus starten. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

* Ein Problem wurde behoben, infolge dessen die Kundenattribute einiger Kunden nicht synchronisiert werden konnten.
* Es wurde ein Problem behoben, durch das die Seite [Adobe Target-Produktdokumentation](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html?lang=de) nicht auf Japanisch angezeigt wurde.
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
   <td colname="col1"> <p>Verwaltungsverbesserungen: </p> 
    <ul id="ul_7D5FCBEFA262435D865CA1018BFB792E"> 
     <li id="li_6E98974CCB094ABBAB57C51ED56C3F00"> <span class="wintitle"> Admin Console</span> </li> 
     <li id="li_8CDAB6301FD44C3999EE4EEB1A0A2FD6">Enterprise und Federated ID-Unterstützung </li> 
    </ul> </td> 
   <td colname="col2"> <p>Die Funktionen zur Benutzer- und Gruppenverwaltung wurden in die Admin Console verschoben. Der neue Navigationspfad lautet: </p> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol">Administration</span> &gt; <span class="uicontrol">Admin Console starten</span></p> <p> Außerdem wurde die Unterstützung für Enterprise IDs und Federated IDs hinzugefügt. Sie können Enterprise IDs, Federated IDs und Adobe-IDs in derselben Unternehmensimplementierung verwenden. Verwenden Sie beispielsweise Adobe-IDs für Benutzer, die andere Adobe-Produkte und -Dienste verwenden dürfen. Verwenden Sie Enterprise IDs oder Federated IDs für Benutzer, deren Konten Sie streng verwalten möchten. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Es wurde ein Problem behoben, durch das Single Sign-On zwischen dem [!DNL Experience Cloud] und [!DNL Media Optimizer] verhindert wurde.

**Bekannte Probleme**

* Die Verknüpfung und Aufhebung der Verknüpfung Ihres dynamischen Tag-Management-Unternehmens mit der Experience Cloud funktioniert nicht für neu erstellte Experience Cloud-Unternehmen. Adobe arbeitet daran, dieses Problem zu beheben und die normale Funktionalität im Rahmen der Mai-Version wiederherzustellen. Sollten Sie Probleme mit Single Sign-on beim Dynamic Tag Management über die Experience Cloud haben, melden Sie sich unter [!DNL dtm.adobe.com] mit Ihrem gewohnten Konto an.
* Ein bekanntes Problem verhindert die Freigabe von Zielgruppen aus Report Suites, die nicht dem verknüpften Analytics-Konto gehören. An einer Lösung wird bereits gearbeitet.

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
   <td colname="col2"> <p>Wenn Sie Daten von Unternehmenskunden in einer CRM-Datenbank (Customer Relationship Management) erfassen, können Sie diese Daten in eine Datenquelle für Kundenattribute in die Experience Cloud hochladen. Nach dem Hochladen der Daten können Sie die Berichte <span class="uicontrol">Besucherprofil</span> &gt; <span class="uicontrol">Kundenattribute</span> in Analytics ausführen. </p> <p>Die hochgeladenen Daten können Sie in <span class="keyword">Adobe Target</span> auch als Zielgruppensegment verwenden. </p> <p>Siehe <a href="attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1" format="dita" scope="local">Produktdokumentation zu Kundenattributen</a>. </p> <p> Informationen zur Modernisierung Ihrer Anwendungen für Hauptdienste finden Sie unter <a href="core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Anwendungen für Hauptdienste aktivieren</a>. </p> </td> 
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
   <td colname="col1"> <p>Gruppe  Zuordnen </p> </td> 
   <td colname="col2"> <p>Die Seite "Gruppenverwaltung"wurde neu als Verwaltungsoberfläche konzipiert, über die Sie Gruppen erstellen, Experience Cloud-Benutzer Gruppen hinzufügen und Berechtigungen für mehrere Anwendungen zuweisen können. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Eins-zu-viele-Zuordnung </p> </td> 
   <td colname="col2"> <p>Wenn Sie Anwendungskonten im Experience Cloud verknüpfen und mehrere Anwendungen und Organisationen verwenden, können Sie jetzt mehrere Produkte und Dienste einer Organisation zuordnen. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Activation </p> </td> 
   <td colname="col2"> <p> <a href="activation.md#concept_EE756B6B0A0643DAB8CA3A00E665406C" format="dita" scope="local"> Activation</a> wird nun im linken Navigationsbereich der <span class="keyword">Experience Cloud</span> angezeigt. <span class="wintitle">Activation</span> ist ein <span class="keyword">Experience Cloud</span>-Service, der die Technologie des dynamischen Tag-Managements nutzt. Bei der Auswahl dieses Services werden Sie zum dynamischen Tag-Management weiterleitet. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Aktualisierungen der Dokumentation – Zentrale Dienste </p> </td> 
   <td colname="col2"> <p>Thema hinzugefügt <a href="core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Anwendungen für Hauptdienste aktivieren</a> , um Sie bei der Implementierung der Hauptdienste zu unterstützen. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Version 15.2.1 – 19. Februar 2015 {#section_BC694D5AE16A4E16B44B353ED67947F3}

Fehlerbehebungen:

* Der Arbeitsablauf für die Einladung per E-Mail zur Kontobereitstellung wurde verbessert.
* Es wurde ein Problem mit dem Asset-Ordner behoben, das die [!DNL Experience Cloud] und [!DNL Adobe Campaign] Assets daran hinderte, identische Ordnerhierarchien anzuzeigen.
* Behebung eines Fehlers, der das Löschen von Zielgruppen verhinderte, die zu deaktivierten [!DNL Target]-Aktivitäten gehörten.
* Behebung eines Fehlers, der dazu führte, dass das Hinzufügen (Plus)-Symbol unter [!UICONTROL Regeln] auf der Seite [!UICONTROL Neue Zielgruppe erstellen] nicht angezeigt wurde.
* Verbesserte Unterstützung der Experience Cloud-Benutzeroberfläche für Internet Explorer 9.

## Version 15.1.1 – 15. Januar 2015 {#section_F1A352E928AF432E94CC0A289C345184}

Neue Funktionen und Fehlerbehebungen in der Benutzeroberfläche für die Zusammenarbeit und Freigabe der [!DNL Adobe Experience Cloud].

<table id="table_AD0A8CA760E64227BB04BA6B0E425E80"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Schreibgeschützter Zugriff. </p> </td> 
   <td colname="col2"> <p>Administratoren können Benutzern ohne Administratorrechte jetzt schreibgeschützten Zugriff gewähren. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Es wurde ein Problem behoben, durch das PNG-Dateien nicht auf einer Karte wiedergegeben werden konnten.
* Es wurde ein Problem beim Hochladen von Dateien in Experience Cloud-Assets per Drag &amp; Drop behoben.

**Bekannte Probleme**

* Benutzer können auf Pinnwänden keine PowerPoint-Dateien freigeben.
* Änderungen an Gruppen und Berechtigungen, die über die Benutzerverwaltung durchgeführt werden, werden erst nach einer erneuten Anmeldung wirksam.
* Bei einigen Benutzern treten möglicherweise Probleme beim Hochladen großer Dateitypen in Experience Cloud Assets auf.
* Einigen Benutzern fehlen möglicherweise Links von Media Optimizer auf ihren Experience Cloud-Karten.
* Bei einigen Benutzern ohne Administratorrechte treten möglicherweise Probleme beim Verknüpfen ihrer Konten auf, nachdem sie eine Einladung zum Beitritt zur Experience Cloud angenommen haben.
* Die Leistung der Benutzeroberfläche der Experience Cloud ist u. U. reduziert, wenn sie von mehreren Benutzern gleichzeitig verwendet wird.
* Für einige Benutzer ist das Löschen nicht mehr aktueller Assets möglich, ohne dabei eine Fehlermeldung zu empfangen.
* Bei einigen Benutzern treten möglicherweise Probleme auf, wenn sie sich mit derselben Adobe-ID gleichzeitig bei zwei Browsern anmelden.
* Einige Benutzer können möglicherweise einen Creative Cloud-Benutzer nicht erneut einem Freigabeordner hinzufügen, nachdem der Creative Cloud-Benutzer gelöscht wurde.
* Bei einigen Benutzern ist möglicherweise die Benachrichtigung verzögert, die erfolgt, wenn ein Ordner aus der Experience Cloud für die Creative Cloud freigegeben wird.
* Bei einigen Benutzern tritt möglicherweise ein Problem beim Freigeben eines Ordners zwischen der Experience Cloud und der Creative Cloud auf.
* Einige Benutzer haben möglicherweise Probleme beim Erstellen einer Zielgruppe in einer Analytics-Report Suite, nachdem freigegebene Zielgruppen aktiviert wurden.
* Einige Benutzer haben möglicherweise Probleme beim Hochladen von Assets auf eine Pinnwand.

## Version 14.11.1 – 13. November 2014 {#section_A6CF1D4F27B9496892A89C983EB39102}

Bekannte Probleme:

* Für einige Benutzer ist das Löschen nicht mehr aktueller Assets möglich, ohne dabei eine Fehlermeldung zu empfangen.
* Manche [!DNL .png]-Dateien können nicht auf einer Karte dargestellt werden.
* Einige Benutzer haben möglicherweise Probleme beim Hochladen von Assets auf eine Pinnwand.
* Änderungen an Gruppen und Berechtigungen, die über die Benutzerverwaltung durchgeführt werden, werden erst bei einer erneuten Anmeldung wirksam.
* Administratoren müssen sich ab- und wieder anmelden, um die in den Kontoeinstellungen vorgenommenen Änderungen zu sehen.
* Benutzer können auf Pinnwänden keine PowerPoint-Dateien freigeben.
* Die Leistung der Benutzeroberfläche der [!DNL Experience Cloud] ist u. U. reduziert, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* Die Synchronisierung zwischen Adobe Experience Manager und Creative Cloud funktioniert nicht.

## Version 14.10.1 – 16. Oktober 2014 {#section_E3A0F4423B814707AA3745E083500835}

Neue Funktionen und Fehlerbehebungen in der Benutzeroberfläche für die Zusammenarbeit und Freigabe der [!DNL Adobe Experience Cloud].

<table id="table_7C1ACE8108D54782AE128ACD35069DF5"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Bearbeiten von Benutzerberechtigungen </p> </td> 
   <td colname="col2"> <p>Inhaber einer Pinnwand können jetzt Benutzerberechtigungen auf der jeweiligen Pinnwand bearbeiten. </p> <p> 
     <ol id="ol_B12251C510744538AF9BCE60ACB04016"> 
      <li id="li_87B3EDE9542B47CEBE0BE7F2D1DE844D">Wählen Sie auf der Pinnwand die Option <span class="uicontrol">Einstellungen</span> aus. </li> 
      <li id="li_0F4786B0E1E743069D082E7DC488A031">Geben Sie neben jedem Eigentümer <span class="uicontrol">Eigentümer</span>, <span class="uicontrol">Viewer</span> oder <span class="uicontrol">Editor</span> an. </li> 
     </ol> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Beim Erstellen einer Karte aus einer PDF-Datei und deren Freigabe auf der Pinnwand wurde eine Fehlermeldung zurückgegeben.

**Bekannte Probleme**

* Einige Benutzer haben möglicherweise Probleme beim Hochladen von Assets auf eine Pinnwand.
* Manche [!DNL .png]-Dateien können nicht auf einer Karte dargestellt werden.
* Änderungen an Gruppen und Berechtigungen, die über die Benutzerverwaltung durchgeführt werden, werden erst bei einer erneuten Anmeldung wirksam.
* Einige Benutzer können eine Karte möglicherweise nicht aus einer PDF-Datei erstellen und auf einer Pinnwand freigeben.
* Für einige Benutzer ist das Löschen nicht mehr aktueller Assets möglich, ohne dabei eine Fehlermeldung zu empfangen.
* Benutzer können auf Pinnwänden keine PowerPoint-Dateien freigeben.
* Die Leistung der Benutzeroberfläche der [!DNL Experience Cloud] ist u. U. reduziert, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* Die [!DNL Search&Promote]-Verknüpfungen stehen auf der Seite [!UICONTROL Unternehmen und Produktzugriff] nicht zur Verfügung.

## Version 14.9.1 – 18. September 2014 {#section_20F156A9CC2F4FC59C4970075C181D3A}

**Fehlerbehebungen und Verbesserungen**

* Wenn Sie zu [!DNL experience.adobe.com] navigieren, ist die Anmeldungserfahrung nun mit der Anmeldung von Creative Cloud von Adobe konsistent.
* Auf der Seite &quot;Unternehmen verwalten&quot;ist das Verknüpfungserlebnis (nach Erhalt einer Einladung) nun für jede Anwendung konsistent.

**Bekannte Probleme**

* Änderungen an Gruppen und Berechtigungen, die über die Benutzerverwaltung durchgeführt werden, werden erst bei einer erneuten Anmeldung wirksam.
* Manche Benutzer können aus einer PDF-Datei keine Karte erstellen und auf einer Pinnwand veröffentlichen.
* Einige Benutzer haben möglicherweise Probleme beim Hochladen von Assets auf eine Pinnwand.
* Für einige Benutzer ist das Löschen nicht mehr aktueller Assets möglich, ohne dabei eine Fehlermeldung zu empfangen.
* Benutzer können auf Pinnwänden keine PowerPoint-Dateien freigeben.
* Manche [!DNL .png]-Dateien können nicht auf einer Karte dargestellt werden.
* Die Leistung der Benutzeroberfläche der [!DNL Experience Cloud] ist u. U. reduziert, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* Die [!DNL Search&Promote]-Verknüpfungen stehen auf der Seite [!UICONTROL Unternehmen und Produktzugriff] nicht zur Verfügung.
* Einige Benutzer stellen möglicherweise fest, dass [!DNL Creative Cloud]-Inhalte aus ihrem Ordner entfernt wurden, wenn die Inhalte nicht in [!DNL Experience Cloud] freigegeben sind.

## Version 14.8.1 – 21. August 2014 {#section_03BF00F6A95A490C91BCC0A1988FA7AA}

Neue Funktionen und Fehlerbehebungen in der Benutzeroberfläche für die Zusammenarbeit und Freigabe der [!DNL Adobe Experience Cloud].

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
* Einige Benutzer können eine Karte möglicherweise nicht aus einer PDF-Datei erstellen und auf einer Pinnwand freigeben.
* Einige Benutzer haben möglicherweise Probleme beim Hochladen von Assets auf eine Pinnwand.
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

Neue Funktionen und Fehlerbehebungen in der Benutzeroberfläche für die Zusammenarbeit und Freigabe der [!DNL Adobe Experience Cloud].

**Bekannte Probleme**

* Aus der [!DNL Experience Cloud] gelöschte Dateien werden nicht aus dem [!DNL Digital Asset Management] gelöscht.
* Bei einigen [!UICONTROL Exchange]-Benutzern wird der Name in den Kommentaren möglicherweise als lange ID anstelle des richtigen Namens angezeigt.
* Manche [!DNL .png]-Dateien können nicht auf einer Karte dargestellt werden
* Beim Hochladen von Dateien sind mehr Dateitypen zulässig als bei der Drag &amp; Drop-Methode. Die besten Ergebnisse erzielen Sie bei einem Upload mit [!UICONTROL Assets].
* Die [!DNL Search&Promote]-Verknüpfungen stehen auf der Seite [!UICONTROL Unternehmen und Produktzugriff] nicht zur Verfügung.
* [!DNL Exchange]-Benutzer müssen ihre Cookies löschen, um ihres Benutzererlebnis zu verbessern.
* Die Benutzeroberfläche der [!DNL Experience Cloud] ist u. U. beeinträchtigt, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* Einige Benutzer werden möglicherweise feststellen, dass ihre [!DNL Creative Cloud]-Inhalte aus ihrem Ordner entfernt wurden, wenn die Inhalte in [!DNL Experience Cloud] nicht freigegeben sind.
* Nach 15 Minuten Inaktivität werden Sie abgemeldet. Zudem werden Sie, wenn Sie sich an einem Ort abmelden, von der [!DNL Experience Cloud] abgemeldet.
* Einige Benutzer sind u. U. nicht in der Lage, ihre Audience Manager-Konten mit der [!DNL Experience Cloud] zu verknüpfen.
* [!UICONTROL Exchange]-Benutzer können nur Englisch in der Sprachauswahl anzeigen.

**Fehlerbehebungen**

Keine zu melden.

## Version 14.6.1 – 19. Juni 2014 {#marketing_cloud_interface}

Neue Funktionen und Fehlerbehebungen in der Benutzeroberfläche für die Zusammenarbeit und Freigabe der [!DNL Adobe Experience Cloud].

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
* Beim Hochladen von Dateien sind mehr Dateitypen zulässig als bei der Drag &amp; Drop-Methode. Die besten Ergebnisse erzielen Sie bei einem Upload mit Assets.
* Die [!DNL Search&Promote]-Verknüpfungen stehen auf der Seite [!UICONTROL Unternehmen und Produktzugriff] nicht zur Verfügung.
* Filter, die auf Trendberichte aus [!DNL Analytics] angewendet werden, werden nicht auf Karten in der [!DNL Experience Cloud] angewendet.
* Einige Benutzer können ihr Zielgruppen-Management-Konto nicht mit ihrem [!DNL Experience Cloud]-Konto verknüpfen.
* Nach 15 Minuten Inaktivität werden Sie abgemeldet. Zudem werden Sie, wenn Sie sich an einem Ort abmelden, von der Experience Cloud abgemeldet.
* Bei einigen Exchange-Benutzern wird der Name in den Kommentaren möglicherweise als lange ID anstelle des richtigen Namens angezeigt.

**Fehlerbehebungen**

* Es wurde ein Problem behoben, das das Hochladen von Videos in Apps verhinderte.

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
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol">Hilfe</span> &gt; <span class="uicontrol">Exchange</span></p> <p><span class="keyword">Experience Cloud</span><span class="wintitle">Exchange</span> ist eine zentrale Stelle, an der Sie Digital Marketing-Erweiterungen über Apps suchen, durchsuchen, auswählen, bezahlen und herunterladen können. </p> <p>Zu den Apps gehören Data Connectors, benutzerdefinierte Konfigurationen des Hauptprodukts von Adobe, Anwendungen von Drittherstellern, Berichte und <span class="keyword">Experience Cloud</span>-Karten. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Experience Cloud-Zielgruppen </p> </td> 
   <td colname="col2"> <p> <span class="uicontrol"> Experience Cloud</span> &gt; <span class="uicontrol">Zielgruppen</span></p> <p> In <span class="wintitle">Zielgruppen</span> erstellen, bearbeiten und verwalten Sie Zielgruppen in etwa so, wie Sie mit Segmenten arbeiten. Sie können z. B. ein Segment in Reports &amp; Analytics erstellen und es dann in <span class="wintitle"> Experience Cloud</span><span class="wintitle"> Zielgruppen</span> freigeben. Nach der Freigabe ist die Zielgruppe in <span class="keyword">Adobe Target</span> für Kampagnenaktivitäten und in Adobe Audience Manager für die Segmentierung verfügbar. </p> <p> <p>Hinweis: Um die Aktivierung in Target anzufordern, besuchen Sie<a href="https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=X8SVES" format="http" scope="external"> https://adobe.allegiancetech.com/cgi-bin/qwebcorporate.dll?idx=X8SVES</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Benutzer, die auf <span class="keyword">Experience Cloud</span>-Karten erwähnt werden, haben nun die Berechtigung für diese Karte. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> </p> </td> 
   <td colname="col2"> <p>Neue Benutzer von Adobe können ihre Scene7-Konten mit einer Adobe ID und ihren Team-Mitgliedern verknüpfen. Administratoren können auch die Verknüpfung von Benutzern mit Scene7-Konten aufheben. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Asset-Synchronisierung. </p> </td> 
   <td colname="col2"> <p> Assets innerhalb von Experience Manager-(-)Assets können Sie über die Experience Cloud und die Creative Cloud freigeben. Alle Änderungen an diesen Assets werden in den freigegebenen Kopien der Assets in Experience Cloud und Creative Cloud übernommen. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Die [!DNL Experience Cloud] wurde nicht mit [!DNL Adobe Target] verknüpft. Dieses Problem trat auf, wenn die [!DNL Adobe Target]-Anmeldung auf mehreren [!DNL Target]-Servern zur Verfügung stand.
* [!DNL Adobe Media Optimizer] erstellte Benutzer nicht automatisch, wenn der Benutzer in der [!DNL Experience Cloud] erstellt worden war.
* Optionen in Kombinationsfeldern zum Hinzufügen neuer Benutzer wurden bei der Eingabe vorübergehend ausgeblendet.
* Der Link „Kommentare“ auf der Assets-Kartenansicht konnte nicht ausgewählt werden.
* Nachdem einem Asset ein benutzerdefiniertes Tag hinzugefügt wurde, blieben keine weiteren Änderungen an den Metadaten erhalten.
* Beim Löschen eines Bildes gibt Assets keine Warnung aus, wenn das Bild in Adobe Target Essentials verwendet wird.
* Die Benutzeroberfläche der [!UICONTROL Experience Cloud] arbeitete langsam, wenn sie von vielen Benutzern gleichzeitig verwendet wurde.
* Beim Löschen eines Bildes in [!UICONTROL Experience Cloud Assets] wurde keine Warnmeldung ausgegeben, wenn das Bild in [!DNL Adobe Target Essentials] in Verwendung war.
* Wenn die Option **[!UICONTROL Angaben speichern]** nicht während des Anmeldevorgangs ausgewählt wurde, wurde der Benutzer nach 15 Minuten abgemeldet.
* Benutzer mussten sich ab- und wieder anmelden, damit alle Änderungen an Berechtigungen wirksam wurden.
* Die Anmeldung bei der [!DNL Experience Cloud] dauerte länger als eine Sekunde.
* Beim Löschen von Dateien aus [!DNL Experience Cloud] wurde dieser Vorgang bei manchen Benutzern nicht mit dem [!DNL Digital Asset Management] synchronisiert.
* Benutzer wurden nach nur 15 Minuten Browserinaktivität abgemeldet.
* Benutzer konnten auf Pinnwänden keine PowerPoint-Dateien freigeben.
* Bei einigen Benutzern war das visuelle Layout im Internet Explorer 10 schlecht.

## Version 14.4.1 – 22. April 2014 {#section_E2A699764E744D2E8D418E9A3D40AF6B}

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
   <td colname="col2"> <p>Nachdem Sie die Funktion „Mit Adobe Experience Cloud teilen“ in der Symbolleiste „Lesezeichen“ Ihres Browsers aktiviert haben, können Sie jetzt Hilfeseiten über die Microsite-URL freigeben. </p> <p> <b>Freigeben eines Hilfethemas</b> </p> 
    <ol id="ol_F94B816121494B0FA16CC07B0E96AED8"> 
     <li id="li_F47187D4B5FE46D3A51D257DD569B4D6"> <p>Wählen Sie in <span class="keyword">Experience Cloud</span> die Option <span class="uicontrol"> Administration</span> aus. </p> </li> 
     <li id="li_94EF58E7A4974B63951E14F72A710183"> <p>Ziehen Sie die Schaltfläche <span class="uicontrol">Für Adobe Experience Cloud freigeben</span> in die Symbolleiste „Lesezeichen“. </p> </li> 
     <li id="li_69EEC4F25D8F4AD7AA106A10B7F50FF6"> <p>Navigieren Sie zu einer Hilfeseite (oder bleiben Sie auf dieser Seite) und wählen Sie dann in Ihrem Browser in der Symbolleiste „Lesezeichen“ die Option <span class="uicontrol"> Für Adobe Experience Cloud freigeben</span> aus. </p> <p>Auf diese Weise wird eine Karte erstellt, die Sie in der <span class="wintitle">Experience Cloud</span> anzeigen können. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Nachdem einem Asset ein benutzerdefiniertes Tag hinzugefügt wurde, können keine weiteren Änderungen an den Metadaten gespeichert bleiben.
* Die Benutzer müssen die Pinnwand aktualisieren, damit die gelöschten Karten nicht mehr in der Ansicht angezeigt werden.
* Wenn die Option **[!UICONTROL Angaben speichern]** nicht während des Anmeldevorgangs ausgewählt wird, wird der Benutzer nach 15 Minuten abgemeldet.
* [!DNL Analytics] Auf der Landingpage der Anwendung werden Formatierungsfehler angezeigt.
* Benutzer müssen sich ab- und wieder anmelden, damit alle Änderungen an Berechtigungen wirksam werden.
* Beim Löschen eines Bildes gibt [!UICONTROL Assets] keine Warnung aus, wenn das Bild in [!DNL Adobe Target Essentials] verwendet wird.
* Der Link „Kommentare“ auf der Asset-Kartenansicht kann nicht ausgewählt werden.
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

Version 14.3.1 ist ein Maintenance Release zur Verbesserung der Geschwindigkeit, Stabilität und Sicherheit. Sie enthält keine wichtigen neuen Funktionen.

**Fehlerbehebungen**

* Es wurde die Möglichkeit zum Entfernen Ihres Avatar-Bildes hinzugefügt.
* Ein Problem wurde behoben, das dazu geführt hat, dass Sie die Verknüpfung Ihrer [!DNL Adobe Media Optimizer]-Konten nicht aufheben konnten.

**Bekannte Probleme**

* Beim Löschen eines Bildes in Experience Cloud-Assets wird keine Warnung ausgegeben, wenn das Bild in Adobe Target Essentials verwendet wird.
* Das Aktualisieren einer Karte aus [!DNL Analytics] kann in der erweiterten Karte gelegentlich zu einem leeren Diagramm führen.
* Benutzer müssen sich ab- und wieder anmelden, damit alle Änderungen an Berechtigungen wirksam werden.
* Wenn bei der Anmeldung *`Remember me`* nicht aktiviert ist, wird der Benutzer nach 15 Minuten abgemeldet.
* [!DNL Analytics] Auf der Landingpage der Anwendung werden Formatierungsfehler angezeigt.
* Der Link „Kommentare“ auf der Assets-Kartenansicht kann nicht ausgewählt werden.
* Die Experience Cloud-Benutzeroberfläche ist u. U. beeinträchtigt, wenn sie von vielen Benutzern gleichzeitig verwendet wird.
* Die Experience Cloud kann nicht mit [!DNL Adobe Target] verknüpft werden, wenn die [!DNL Adobe Target]-Anmeldung auf mehreren Target-Servern verwendet werden kann.
* Die Anmeldung bei Experience Cloud dauert länger als eine Sekunde.
* Nachdem einem Asset ein benutzerdefiniertes Tag hinzugefügt wurde, können keine weiteren Änderungen an den Metadaten gespeichert bleiben.
* [!DNL Adobe Media Optimizer] erstellt Benutzer nicht automatisch, wenn der Benutzer in der Experience Cloud erstellt wurde.
* Optionen in Kombinationsfeldern zum Hinzufügen neuer Benutzer werden bei der Eingabe vorübergehend ausgeblendet.
* In [!DNL Media Optimizer] freigegebene Daten werden in der Experience Cloud falsch angezeigt.
* Die Freigabe von Bildern aus Flickr schlägt fehl.
* Filter, die auf Trendberichte aus [!DNL Analytics] angewendet werden, werden nicht auf Karten in der Experience Cloud angewendet.
* Änderungen an Gruppen und Berechtigungen, die über die Benutzerverwaltung durchgeführt werden, werden erst bei einer erneuten Anmeldung wirksam.
* [!DNL Search&Promote]-Verknüpfungen stehen in [!UICONTROL Organisationen und Produktzugriff] nicht zur Verfügung.
* Die Benutzer müssen die Pinnwand aktualisieren, damit die gelöschten Karten nicht mehr in der Ansicht angezeigt werden.
* Manche Excel- oder CSV-Dateien können nicht in eine Pinnwand hochgeladen werden.
* Simulationskarten in [!DNL Adobe Media Optimizer] werden nicht ordnungsgemäß dargestellt.
* Einige PNG-Dateien können nicht auf einer Karte dargestellt werden.
* Beta-Feedback kann nicht gesendet werden.

## Version 14.2.1 – 24. Februar 2014 {#section_5AD81B0737C843AFB4BE9C4420D70EB3}

<table id="table_DFAB002358C94A17A7F91DAB323A488F"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Funktion </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>OEmbed </p> </td> 
   <td colname="col2"> <p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Daten aktualisieren </p> </td> 
   <td colname="col2"> <p> 
     <!--MAC-18174-->Die <span class="uicontrol"> Daten aktualisieren</span> -Symbol für ein Diagramm auf einer Karte ist jetzt ausgeblendet, wenn das Programm keine Aktualisierung von Daten zulässt. </p> </td> 
  </tr> 
 </tbody> 
</table>

**Fehlerbehebungen**

* Es wurde ein Problem behoben, das das Anwenden von Segmentfiltern bei freigegebenen [!DNL Analytics]-Berichten verhinderte.
* Es wurde ein Fehler behoben, der dazu führte, dass Anwendungen im [!UICONTROL Experience Cloud Solutions] -Seite als verknüpft, auch wenn die Anwendungskonten nicht verknüpft waren.
* Es wurde ein Problem behoben, das [!DNL Adobe Target]-Kunden in Asien daran hinderte, auf der Verknüpfungsseite die Schaltfläche **[!UICONTROL Weiter zu Experience Cloud]** auszuwählen.
* Es wurde ein Problem behoben, das die Freigabe von YouTube-Videos verhinderte.
