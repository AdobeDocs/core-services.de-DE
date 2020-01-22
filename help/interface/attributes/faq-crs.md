---
description: Häufig gestellte Fragen zu und Best Practices für Kundenattribute in Analytics und Target.
keywords: customer attributes
seo-description: Häufig gestellte Fragen zu und Best Practices für Kundenattribute in Analytics und Target.
seo-title: Häufig gestellte Fragen, Einschränkungen und Best Practices
solution: Experience Cloud
title: Häufig gestellte Fragen, Einschränkungen und Best Practices
uuid: e93eb531-23c7-4d75-92e8-75699f58546a
translation-type: tm+mt
source-git-commit: f89a6c6704c9f499e6aa2ab38b2f5f9496ccdda5

---


# Häufig gestellte Fragen, Einschränkungen und Best Practices

Häufig gestellte Fragen zu und Best Practices für Kundenattribute in Analytics und Target.

## Best Practices und Einschränkungen  {#section_7F5189B3DAA84EE6865B91D2026EE05A}

Richtlinien und Einschränkungen für die Verwendung von Kundenattributen

| Fehler | Beschreibung |
|--- |--- |
| Einschränkungen von Kundenattribut-Abonnements | Bei einem Upgrade auf Analytics Premium dauert es 24 Stunden, bis weitere Attribute verfügbar sind. Während dieser Wartezeit wird Ihnen möglicherweise eine Fehlermeldung über einen erreichten Attributabonnement-Maximalwert angezeigt. |
| Mehrere Anmeldungen auf demselben Gerät | Wenn Sie Kundenattribute verwenden, um Kundenprofile in eine Datenquelle hochzuladen, empfiehlt Adobe Benutzern, die dasselbe Gerät (d. h. dieselbe Experience Cloud-ID) nutzen. Dies kann dazu führen, dass der auf dem Gerät vorhandene ECID-Dienst mehrere Benutzer unter derselben Experience Cloud-ID verknüpft, was zu unerwarteten Ergebnissen führt [!DNL Target]. **** Hinweis: Bei Mobile ist die ECID dauerhaft, nachdem die Mobile-App installiert wurde, und Sie müssen die App neu installieren, um eine neue ECID zu generieren. Im Web wird nach dem Löschen des Browser-Cookies eine neue ECID generiert. |
| Begrenzung des täglichen Hochladevorgangs | Adobe empfiehlt, Kundenattribute nur einmal pro Tag zu aktualisieren. Sie müssen mindestens 24 Stunden warten, um eine weitere Kundenprofildatendatei für denselben Profilsatz hochzuladen. |
| Custom Analytics ID (`s.visitorID`) | In Analytics können Besucher identifiziert werden, indem eine Kunden-ID mit `s.visitorID` festgelegt wird. Integrationen, in denen Analytics-Daten mit dem ID-Dienst exportiert oder importiert werden, funktionieren jedoch nicht, wenn ein Besucher anhand `s.visitorID.`<br>dieser Funktion identifiziert wird. Dazu gehören unter anderem freigegebene Zielgruppen, Analytics for Target (A4T) und Kundenattribute.<br>Bei diesen Integrationen wird die Festlegung einer benutzerdefinierten Analytics ID nicht unterstützt. |
| Beschränkungen der Zeichenlänge in Analytics | Wenn Sie ein Analytics-Abonnement erstellen, sind die Längen der Felder für hochgeladene Dateien auf 255 Zeichen beschränkt. |

## Häufig gestellte Fragen zu Kundenattributen  {#section_E47866EEA83348E09FE43CEC5E44C461}

<table id="table_88631069013B408EBB0A810657662B36"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Frage </th> 
   <th colname="col2" class="entry"> Antwort </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Kann ich Benachrichtigungen über den Upload-Status von Kundenattributen erhalten? </p> </td> 
   <td colname="col2"> <p>Ja. Weitere Informationen finden Sie unter <a href="../admin-getting-started/organizations.md#concept_0105453AD71847B8BFCAF4A40915F157" format="dita" scope="local">Benachrichtigungen verwalten</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Was muss ich tun, damit ich Kundenattribute verwenden kann? </p> </td> 
   <td colname="col2"> 
    <ol id="ol_1FACEF0990B6486B8DE86245D17695A8"> 
     <li id="li_F0C1542853684F8591FDC1B441D31A56"> <p>Lassen Sie sich freischalten. </p> <p>Wenn Sie <b>Analytics</b>-Kunde sind, schaltet Adobe Sie für Kundenattribute frei. Wenn Sie nur <b>Target</b> verwenden und nicht über Analytics verfügen, müssen Sie die Kundenunterstützung bitten, Sie für die Hauptdienste freizuschalten. </p> </li> 
     <li id="li_444FEDEE4B7244F79BA847662F5B17CB"> <p>Besprechen Sie sich mit Ihrem CRM-Team. Finden Sie heraus, welche Arten von Kundendaten vorhanden sind und ob sie sich für die Verwendung in Analytics und in der Experience Cloud eignen. </p> </li> 
     <li id="li_32D4AAF8C29748A78801A0E1BFB37AF5"> <p>Implementieren Sie die Hauptdienste. </p> <p>Weitere Informationen finden Sie unter <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Erste Schritte - Aktivieren Ihrer Lösungen für Hauptdienste</a>. Hier erfahren Sie, wie Sie Ihre Implementierung für Hauptdienste modernisieren. (Besonders wichtige Informationen finden sich im Abschnitt über die Synchronisierung von Kunden-IDs.) </p> </li> 
    </ol> <p> <b>Hinweis:</b> Eine FAQ-Rubrik für Administratoren zur Implementierung von Hauptdiensten finden Sie  <a href="../admin-getting-started/faq.md#concept_13219B4E51784577B6FF78AAA203DE91" format="dita" scope="local">hier</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Wie viele Kundenattribute darf ich verwenden? </p> </td> 
   <td colname="col2"> <p>Sie können Hunderte von <span class="filepath">CSV</span>-Spalten für den Kundenattributdienst hochladen. Bei der Konfiguration von Abonnements und der Auswahl von Attributen gelten jedoch die folgenden Einschränkungen (pro Report Suite), je nach den Lösungen, die Sie besitzen:</p> <p> 
     <ul>
     <li>Foundation: 0</li>
     <li>Select: 3</li>
     <li>Prime: 15</li>
     <li>Ultimate: 200</li>
     <li>Standard: 3 insgesamt</li>
     <li>Premium: 200</li>
     <li>Target Standard: 5</li>
     <li>Target Premium: 200</li></ul>
     </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Ist eine Migration zum Experience Cloud ID-Dienst nötig? </p> </td> 
   <td colname="col2"> <p>Ob eine Migration nötig ist, hängt von den von Ihnen verwendeten Lösungen ab. </p> <p> 
     <ul id="ul_9C473434B5DA4C6299AAB209DEDFCDE7"> 
      <li id="li_8BC10EB2825F4ADF8CA61F71D4994A28"> <b>Adobe Analytics</b>: Dringend zu empfehlen </li> 
      <li id="li_56F518E3F3DF4C93B6F7EF3B40ACC52F"> <b>Adobe Target:</b> Erforderlich </li> 
     </ul> </p> <p>Der ID-Dienst öffnet die Türen zur modernsten Experience Cloud-Funktionalität, einschließlich Echtzeitzielgruppen, der neuesten Target-Version, der Integration von Analytics und der Pulsmessung für Video. </p> <p>Weitere Informationen finden Sie unter <a href="../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C" format="dita" scope="local"> Hauptdienste – So aktivieren Sie Ihre Lösungen</a>. </p> <p> <b>Hinweis</b>: Der <span class="term"> Experience Cloud ID-Dienst</span> ist die modernisierte Implementierung des <span class="term"> Analytics-Besucher-ID-Dienstes</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Inwieweit lässt sich die Kundenattributfunktion mit Adobe Audience Manager vergleichen? </p> </td> 
   <td colname="col2"> <p>Audience Manager kann zwar Daten empfangen und anhand dieser Daten eine Zielgruppenidentifikation vornehmen, es kann aber keine Analysefunktionen durchführen, die Attribute mit historischen Verhaltensdaten verknüpfen oder die in Adobe Analytics verfügbaren Berichts-, Analyse- und Segmentierungsfunktionen bereitstellen. Mit dem People-Hauptdienst können Rich-Daten aus verschiedenen Lösungen zusammengefasst und einer einzelnen ID zugeordnet werden, die in der Experience Cloud verwendet wird. </p> <p> In Adobe Target erscheinen Kundenattribute als einzelne Attribute, die mit anderen Regeln zum Aufbau von Zielgruppen kombiniert werden können. Im People-Hauptdienst freigegebene Zielgruppen sind vollständige Zielgruppen, die nicht geändert werden können. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Nur Analytics) </b>Worin unterscheidet sich diese Funktion von der in Analytics Premium bereitgestellten Funktionalität? </p> </td> 
   <td colname="col2"> <p>Bislang waren Kunden, die ihre Kundenattributdaten mit ihren Analytics-Daten kombinieren wollten, sehr stark vom Data Workbench-Tool dieser Funktionalität abhängig. Die Kundenattributfunktion stellt diese Funktionalität nun durch ihre Integration als Dimensionen und Metriken von Reports &amp; Analytics, Ad Hoc Analysis und Report Builder einer wesentlich größeren Zielgruppe bereit. Bereits in der Standard-Edition von Analytics ist die Kundenattributfunktion verfügbar, jedoch mit eingeschränktem Funktionsumfang. Der volle Funktionsumfang steht nur bei Analytics Premium zur Verfügung. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Nur Target)</b> Kann ich Daten für neue Kunden in Target vorab laden oder hochladen? </p> </td> 
   <td colname="col2"> <p> Ja. Wenn Besucher die erste Anforderung an Target stellen, ruft das System die vorhandenen Informationen zu ihnen aus den Kundenattributen ab und verwendet diese Daten für das Targeting. </p> <p> <p>Hinweis: Das Abrufen dieser Daten kann bis zu 20 Minuten ab der ersten Interaktion des Besuchers mit Target dauern. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Nur Target)</b> Kann ich eine übergeordnete Zielgruppe erstellen, indem ich Kundenattributdaten mit freigegebenen Zielgruppendaten verbinde? </p> </td> 
   <td colname="col2"> <p>Nein. Freigegebene Zielgruppendaten stellen eine abgeschlossene Zielgruppe dar. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Nur Target) </b>Inwiefern unterscheidet sich die Funktion von Kundenattributen von der Bulk-Profile-API von Target? </p> </td> 
   <td colname="col2"> <p> Mit der <a href="https://www.adobe.io/apis/experiencecloud/target.html" format="https" scope="external">Bulk-Profile-API</a> können Target-Profile direkt über die API aktualisiert werden – entweder als einzelne Profile oder in Profilgruppen. Diese Funktionalität ähnelt der von Kundenattributen, es gibt jedoch folgende wichtige Unterschiede: </p> 
    <ul id="ul_5AAA4A8497C04F50A8AAA9F776BB868E"> 
     <li id="li_B20AEA397F3B4C86A1140CDA61ABD575">Die Profil-API ist ein REST-API-Aufruf und wird für Kundenattribute wie FTP verwendet. </li> 
     <li id="li_7FBE428EF5D34B6AA09B6368E8210344">Die Profil-API von Target sendet nur Daten an Target und nicht an die Experience Cloud. </li> 
     <li id="li_CBB4D3FAF53944E0A066A4AD9F9C8760">Kundenattribute bilden eine einfache Schnittstelle zum Erstellen und Verwalten dieser externen Daten. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b>(Nur Target)</b> Verlängert das Hochladen von Daten von Kundenattributen zu Adobe Target die Lebensdauer des Target-Besucherprofils? </p> </td> 
   <td colname="col2"> <p>Ja. Weitere Informationen finden Sie unter <a href="https://docs.adobe.com/content/help/en/target/using/audiences/visitor-profiles/visitor-profile.html" format="https" scope="external">Lebensdauer von Besucherprofilen</a> in der Hilfe zu Adobe Target. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <b> (Nur Target)</b> Kann ich mich auf die in Kundenattributen hochgeladenen Daten sofort nach Identifikation des Besuchers durch die Kunden-ID beziehen? </p> </td> 
   <td colname="col2"> <p>Ja. </p> <p>Nach dem Server-Aufruf für Target, der die mbox-ID des Drittanbieters enthält, stehen alle Kundenattributdaten zur Verfügung. </p> </td> 
  </tr> 
    <tr> 
   <td colname="col1"> <p> <b> (Nur Target)</b> Was bedeutet die Spalte "Synchronisierungsstatus"für Dateien, die in der Kundenattributquelle hochgeladen wurden? </p> </td> 
   <td colname="col2"> <p> Die Anzahl der von Target veröffentlichten und synchronisierten Datensätze kann angezeigt werden, indem Sie auf das Symbol "Status synchronisieren"für eine bestimmte Attributdatei klicken. "Synchronisieren %"ist eine Echtzeitmetrik, die den Prozentsatz der Profile angibt, die in Target synchronisiert wurden. </p> <p> <b></b> Hinweis: Die Synchronisierung von Attributen mit Target kann bis zu 24 Stunden dauern. </p>
 </td> 
  </tr> 
 </tbody> 
</table>
