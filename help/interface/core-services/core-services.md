---
description: Implementieren Sie die Experience Cloud und werden Sie Administrator. Durch diesen Prozess werden Ihre Lösungen bezüglich der Hauptdienst-Funktionen, wie Kundenattribute und Zielgruppen, modernisiert.
keywords: core services;customer attributes
seo-description: Implementieren Sie die Experience Cloud und werden Sie Administrator. Durch diesen Prozess werden Ihre Lösungen bezüglich der Hauptdienst-Funktionen, wie Kundenattribute und Zielgruppen, modernisiert.
seo-title: Experience Cloud-Lösungen für Hauptdienste aktivieren
solution: Experience Cloud
title: Lösungen für Hauptdienste aktivieren
uuid: 5820060f-9b18-4339-81e0-401d964f7a03
translation-type: tm+mt
source-git-commit: ae97db27349940a8df7ee2ba6678683f57585678

---


# Lösungen für Hauptdienste aktivieren

Implementieren Sie die Experience Cloud und werden Sie Administrator. Durch diesen Prozess werden Ihre Lösungen bezüglich der Hauptdienst-Funktionen, wie Kundenattribute und Zielgruppen, modernisiert.

<!-- <p>https://marketing-beta.adobe.com/resources/help/core/core-services.html </p> 
<p>https://adobe.sharepoint.com/sites/AGSConsulting/CoreServices/PA/_layouts/15/start.aspx#/ </p> -->

<!-- Core services architecture and data flow wiki: https://wiki.corp.adobe.com/pages/viewpage.action?pageId=1004285689 -->

## Schritt 1. Experience Cloud beitreten und Administrator werden {#section_2423F0BD3DF642658103310EE5EA6154}

Möchten Sie Experience Cloud-Mitglied werden, benötigen Sie Folgendes:

![](assets/step1_icon.png) Stellen Sie sicher, dass Sie über gültige SKUs für Adobe Analytics oder Adobe Target verfügen.

* **Adobe Analytics:** Standard oder Premium (nicht die frühere SiteCatalyst-SKU).
* **Adobe Target:** Standard oder Premium.

>[!NOTE]
>
>For Target, [migrate to at.js from mbox.js](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/upgrading-from-atjs-1x-to-atjs-20.html).

![](assets/step2_icon.png) Modernisieren Sie Ihre Implementierung und lassen Sie sich einen Administrator bereitstellen.


1. Folgen Sie den unten unter [Experience Cloud ID-Dienst bereitstellen](../core-services/core-services.md#section_3C9F6DF37C654D939625BB4D485E4354) beschriebenen Schritten.
1. Wenden Sie sich an Ihren Kundenbetreuer und beginnen Sie mit der Bereitstellung der Experience Cloud.

![](assets/step3_icon.png) Verwalten Sie Benutzer und Produkte in der Admin Console.

**Administratorzugang**

After you are an administrator, you can log in at [experiencecloud.adobe.com](https://experiencecloud.adobe.com).

Im Experience Cloud-Navigationsmenü wird der Link **[!UICONTROL Administration]** angezeigt.

Weitere Informationen finden Sie unter [Experience Cloud – Benutzer und Produkte verwalten](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

**Benutzerzugriff**

Wenn Sie sich bei der Experience Cloud anmelden möchten, müssen Sie wie folgt vorgehen:


1. Verwenden Sie eine Adobe ID.
1. Sign in at [experiencecloud.adobe.com](https://experiencecloud.adobe.com).
1. Treten Sie einer Lösungsgruppe bei, die einer Unternehmensgruppe zugeordnet ist.
1. Falls nötig, verknüpfen Sie Lösungskonten mit der entsprechenden Adobe ID (siehe Beschreibung unten).

![](assets/step4_icon.png) Optional: Verknüpfen Sie vorhandene Benutzerkonten.

Höchstwahrscheinlich gibt es Benutzer, die bereits Mitglieder von Lösungsgruppen sind, z. B. eine Analytics-Gruppe, die Sie unter „Analytics“ &gt; „Admin Tools“ verwaltet haben.

Wenn Sie diese Gruppen Enterprise-Gruppen in der Experience Cloud zuordnen, müssen die betroffenen Benutzer die Anmeldeinformationen ihres Lösungskontos manuell mit ihrer Adobe ID verknüpfen.

Weitere Informationen finden Sie im Kapitel über die [Verknüpfung von Konten in der Experience Cloud](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1).

> [!NOTE]
> 
> Nach dem Mapping von Unternehmens- und Lösungsgruppen werden neue Benutzer automatisch verknüpft. (Anmeldeinformationen für die Lösung werden automatisch erstellt und mit der Adobe ID verknüpft.)

In den folgenden Abschnitten wird die Modernisierung der Implementierung beschrieben. Durch die Modernisierung Ihrer Implementierung werden Hauptdienste der Experience Cloud aktiviert.

## Schritt 2. Implementieren Sie den Experience Cloud ID-Dienst mit dem dynamischen Tag-Manager oder mit Experience Platform Launch {#section_3C9F6DF37C654D939625BB4D485E4354}

Die einfachste Methode zur Aktivierung der Hauptdienste der Experience Cloud besteht darin, sie für Analytics und Target mithilfe des [Experience Cloud ID-Dienst-Tools](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/standard.html) im dynamischen Tag-Manager automatisch zu aktivieren. (oder in Experience Platform Launch)

![](assets/menu-activation-shell.png)

For complete Experience Cloud ID service help (formerly, visitor ID), go [here](https://docs.adobe.com/content/help/en/id-service/using/home.html).

Die nächste Generation des Tag-Managements ist [Launch von Adobe](https://docs.adobelaunch.com/getting-started).

**Sie verwenden Dynamic Tag Management oder Launch nicht?**

Wenn Sie kein Dynamic Tag Management verwenden, können Sie den ID-Dienst manuell wie folgt via JavaScript-Implementierung ([!DNL VisitorAPI.js]) bereitstellen:

1. Führen Sie die in [Implementierung des Experience Cloud ID-Dienstes für Analytics](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/setup-analytics.html) beschriebenen Schritte durch.

   Darüber hinaus empfiehlt Adobe die Einrichtung weiterer [Kunden-IDs](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html). Jeder Besucher benötigt eine solche ID, um die aktuellen und zukünftigen Funktionen der Experience Cloud-Hauptdienste zu aktivieren.

1. Aktualisieren Sie Ihre vorhandene [!DNL s_code] auf die Version H.27.3 oder höher, oder Ihre vorhandene [!DNL AppMeasurement.js] auf Version 1.4 oder höher.

   Diese Dateien stehen im [Code-Manager](https://docs.adobe.com/content/help/en/analytics/admin/admin-tools/code-manager-admin.html) der Analytics Admin Tools zum Download bereit.

   (Eine [JavaScript-Implementierungsanleitung](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/javascript-implementation-overview.html) ist verfügbar, wenn Sie weitere Informationen zu [!DNL AppMeasurement.js] benötigen.)

1. Synchronisieren der Kunden-IDs für Analytics. Siehe [Analytics – Synchronisieren der Kunden-ID](../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437) (unten).

## Analytics und Target – Synchronisieren der Kunden-ID {#section_AD473A6A21C1446498E700363F9A8437}

Im Zuge der Einrichtung des Experience Cloud ID-Dienstes empfiehlt Adobe für Analytics und Target die Synchronisierung Ihrer [Kunden-IDs](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html) mit der Experience Cloud.

In Target muss [!DNL mbox3rdpartyid] die Kunden-ID abrufen und an Target senden können. (Informationen hierzu finden sich im Kapitel zur [Arbeit mit Kundenattributen](https://docs.adobe.com/content/help/en/target/using/audiences/visitor-profiles/working-with-customer-attributes.html) in Target.)

Wenn sich ein Besucher bei Ihrer Website authentifiziert oder sich auf andere Weise identifiziert, muss Ihre Implementierung die CRM-Kunden-ID dieser Person für die Seite oder App bereitstellen. Danach können Sie Ihre Kunden-ID mit dem entsprechenden Funktionsaufruf mit der Experience Cloud synchronisieren. Durch die Synchronisierung wird die CRM-Kunden-ID des Besuchers in der Experience Cloud gespeichert und die Attribute dieses Kunden werden für die Verwendung in der Experience Cloud aktiviert.

Beispiel: Bob hat in Ihrem CRM-System die Kunden-ID `52mc210tr42`. Wenn sich Bob bei Ihrer Site authentifiziert, müssen Sie diese ID auf der Seite bereitstellen und die ID zur Synchronisierung auf eine der beiden folgenden Arten verwenden:

* Aufruf von `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})` über den Besucher-ID-Dienst oder
* Ausfüllen der *`Customer ID (52mc210tr42)`* in eine Eigenschaft oder eVar.


Die Kunden-ID muss in jedem Aufruf an den [!DNL Analytics]-Server angegeben sein, auf dem die Kunden-ID bekannt ist.

### Mobile SDKs 

Syntaxbeispiele zum Festlegen zusätzlicher Kunden-IDs in *Android* - und [iOS](https://docs.adobe.com/content/help/en/mobile-services/android/overview.html) Mobile-Anwendungen finden Sie im Abschnitt zum Dienst[ ](https://docs.adobe.com/content/help/en/mobile-services/ios/overview.html)für die Experience Cloud ID.

### Aktivierung der Attribute historischer Daten

Die Kundenattributdaten stehen nach der Anmeldung eines Besuchers zur Verfügung. Wenn Sie die aktuelle Version des Experience Cloud ID-Dienstes noch nicht implementiert haben, sondern Kunden-IDs in einer prop oder eVar aufzeichnen, können Sie einen Prozess anfordern, der historische Anmeldungen an die Experience Cloud sendet. Nach Ausführung dieses Prozesses können Sie die Kundenattribute sofort verwenden.

Wenden Sie sich an den Kundenservice, um Ihre historischen Daten aktivieren zu lassen.

## Schritt 3. Report Suites einer Experience Cloud-Organisation zuweisen {#section_7B08516B01BA421681DF03D0E86CE3BA}

Experience Cloud-Dienste (z. B. der Experience Cloud ID-Dienst und People) sind einer Experience Cloud-Organisation zugeordnet und keiner einzelnen Report Suite. Damit sichergestellt ist, dass diese Dienste korrekt funktionieren, muss jede Analytics-Report Suite einer Experience Cloud-Organisation zugeordnet sein.

Weitere Informationen dazu finden Sie unter [Report Suites einer Organisation zuweisen](report-suite-mapping.md).

## Schritt 4. (Adobe Analytics) Modernisierung des Analytics-AppMeasurement-Codes {#section_1798D9D0F05C47E29816AC4EEB9A0913}

Vergewissern Sie sich, dass Sie die regionale Datenerfassung (RDC) verwenden. Wenn Ihre Datenerfassungsdomäne [!DNL omtrdc.net] lautet, oder wenn Ihr CNAME [!DNL omtrdc.net] zugeordnet ist, befinden Sie sich auf RDC. Weitere Informationen finden Sie unter [Übergang zu RDC. ](https://docs.adobe.com/content/help/en/analytics/technotes/rdc/regional-data-collection.html) If you are using first-party cookies, refer to [CNAME and the Experience Cloud ID Service](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html) for information about data collection CNAMEs and cross-domain tracking.

Adobe empfiehlt eine Modernisierung Ihrer Analytics-Implementierung durch Aktualisierung Ihrer JavaScript-Bibliotheken einschließlich der Besucher-API. Am einfachsten erreichen Sie eine solche Modernisierung durch Hinzufügen des Tools [!DNL Adobe Analytics] im Dynamic Tag Management (DTM), das *`Automatic`* als Konfigurationsmethode angibt.

Klicken Sie im Dynamic Tag Management auf **[!UICONTROL <Web Property Name>]**&gt;**[!UICONTROL Übersicht]**&gt;**[!UICONTROL Tool hinzufügen]**&gt;**[!UICONTROL Adobe Analytics]**. Implementierungsinformationen erhalten Sie unter[Adobe Analytics-Einstellungen](https://docs.adobe.com/content/help/en/dtm/using/tools/analytics-dtm.html)in der Hilfe zum Dynamic Tag Management.

## Schritt 5. (Adobe Target) Modernisierung der Adobe Target-Implementierung {#section_C2F4493C7A36406DAE2266B429A4BD24}

* Adobe empfiehlt das Hinzufügen des Tools [Adobe Target](https://docs.adobe.com/content/help/en/dtm/using/tools/target.html) im Dynamic Tag Management (DTM), damit der Bibliotheksabruf automatisch erfolgt. Klicken Sie im Dynamic Tag Management auf **[!UICONTROL <Web Property Name>]**&gt;**[!UICONTROL Übersicht]**&gt;**[!UICONTROL Tool hinzufügen]**&gt;**[!UICONTROL Adobe Target]**.** Hinweis:**Sie können auch das Dynamic Tag Management verwenden, um den Experience Cloud ID-Dienst für Target (und andere Lösungen) bereitzustellen. Die Aktualisierung des Experience Cloud ID-Dienstes** ist erforderlich **, damit Target Hauptdienste verwenden kann.
* Wenn Sie kein Dynamic Tag Management verwenden, [aktualisieren Sie Ihre mbox-Bibliothek](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/target-download-config-mbox.html) manuell.
* Fordern Sie Zugriff auf Adobe Analytics als Berichtsquelle für Adobe Target an. Die Target- und Analytics-Daten werden bei der Verarbeitung bei demselben Server-Aufruf zusammengeführt, damit Besucher lösungsübergreifend verknüpft werden. Siehe [Analytics für die Target-Implementierung](https://docs.adobe.com/content/help/en/target/using/integrate/a4t/a4t.html).
* 
   >[!IMPORTANT]
   >
   >Alle Analytics-Kunden sind bereits für Hauptdienste wie Kundenattribute freigeschaltet. Wenn Sie kein Analytics-Kunde sind, wenden Sie sich an die Kundenunterstützung, um eine Freischaltung anzufordern.

## Schritt 6. Überprüfung der Implementierung der Hauptdienste {#section_E641782A0F4F44AF8C9C91216BE330D5}

Stellen Sie mithilfe des folgenden Verfahrens sicher, dass der Experience Cloud ID-Dienst auf der Site richtig implementiert ist.

1. Löschen Sie die Cookies für die Site, damit die Anforderung an den Experience Cloud ID-Dienst angezeigt wird (die Anforderung wird beim ersten Besuch und danach pro Besucher etwa einmal wöchentlich gesendet).1. Suchen Sie mit einem Paket-Sniffer oder dem Netzwerkbereich eines Webbrowser-Debuggers nach einer Anfrage für [!DNL dpm.demdex.net].
1. Überprüfen Sie, ob die Antwort `d_mid` und einen Wert enthält, z. B.: `_setMarketingCloudFields({"d_mid":"4235...`
1. Überprüfen Sie, ob die Analytics-Anforderung den mid-Parameter (die Experience Cloud ID) enthält. Während der Übergangsphase (sofern aktiviert) muss außerdem ein aid-Parameter angezeigt werden (die Analytics-Besucher-ID).

Erwartete Antwort mit der Experience Cloud ID:

![](assets/mac_id_response.png)

Analytics-Image-Anforderung mit der Experience Cloud ID (mid):

![](assets/mid.png)

Experience Cloud ID in der mbox-Anforderung:

![](assets/mbox_request.png)

**Was ist die Übergangsphase?**

Nach der Bereitstellung des Besucher-ID-Service wird neuen Besuchern vom Datenerfassungsserver keine Analytics-Besucher-ID zugewiesen. Wenn der Besucher-ID-Dienst für manche Bereiche der Site noch nicht implementiert ist, wenn Besucher diese Bereiche aufrufen, wird die Experience Cloud ID nicht erkannt und den Besuchern wird eine veraltete Analytics-Besucher-ID zugewiesen. Dies kann potenziell zu Problemen führen, unter anderem zu duplizierten Besuchen und fehlerhaften Zuweisungen.

Wenn der Supportbereich der Site beispielsweise über ein gesondertes CMS verwaltet wird, verwenden Sie für diesen Bereich möglicherweise eine andere Analytics-JavaScript-Datei. Wenn Sie die Besucher-ID zuerst auf der Hauptsite und erst dann auf der Support-Site bereitstellen, wird Besuchern beim Besuch des Supportbereichs eine Legacy-Analytics-ID zugewiesen, und Besuche, bei denen beide Sitebereiche aufgerufen werden, werden als verschiedene Besuche erfasst.

Wird der Besucher-ID-Service auf Sites bereitgestellt, die mehrere JavaScript-Dateien oder weitere Technologien (z. B. Flash) verwenden, kann dies Koordinierungsprobleme verursachen, da der Besucher-ID-Service für alle Sitebereiche gleichzeitig aktiviert werden muss. Mit der Konfiguration einer Übergangsphase wird neuen Besuchern vom Besucher-ID-Service weiterhin eine Analytics-Besucher-ID zugewiesen, damit sie richtig in Sitebereichen identifiziert werden, die noch nicht auf den Besucher-ID-Service aktualisiert wurden.

## Schritt 7. Benutzer und Produkte verwalten {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Navigieren Sie nach der erfolgreichen Einrichtung zu **[!UICONTROL Administration]** &gt; **[!UICONTROL Admin Console starten]**, von wo aus Sie Benutzer und Produktprofile verwalten können.

![](assets/menu-administration-shell.png)

Siehe [Verwalten von Experience Cloud-Benutzern und -produkten](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

**Kundenattribute**

<!-- <p> 
 <note type="important">
  To use the Customer Attributes feature, users must belong to the 
  <span class="term"> Adobe Customer Attributes</span> group, and to solution-level groups (Analytics or Target). 
 </note> </p> 
 -->

Benutzer, die der Gruppe „Kundenattribute“ hinzugefügt wurden, sehen auf der linken Seite der Experience Cloud-Benutzeroberfläche das Menüelement [!UICONTROL Kundenattribute]

## Schritt 8. Einführung in die Hauptdienste {#section_960C06093623462E8EA247B3E97274A1}

Nutzen Sie die Vorteile folgender Funktionen der Hauptdienste.

![](assets/menu-audiences-shell.png)

**Personen &gt; Kundenattribute**

Wenn Sie Daten von Unternehmenskunden in einer CRM-Datenbank (Customer Relationship Management) erfassen, können Sie diese Daten in eine Datenquelle für Kundenattribute in die Experience Cloud hochladen. Verarbeiten Sie die Daten nach dem Hochladen mit [!DNL Adobe Analytics] und [!DNL Adobe Target].

Weitere Informationen finden Sie unter [Kundenattribute](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)

**Personen &gt; Zielgruppenbibliothek**

In Experience Cloud-Zielgruppen können Sie Zielgruppen erstellen, mehrere bereits vorhandene Zielgruppen zu einer gemeinsamen Zielgruppe zusammenfassen und alle freigegebenen Zielgruppen anzeigen.

Weitere Informationen finden Sie unter [Zielgruppen](../audience-library/audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)

<!-- aam_mc.xml -->

## Informationen zu Datenspeicherung und Datenschutz

Wenn Sie Echtzeit-Zielgruppenprofile und andere Hauptdienste in der Adobe [!DNL Experience Cloud] nutzen, hat die Verwendung dieser Dienste Auswirkungen darauf, in welchem Datenzentrum (und Land) sich Ihre Daten befinden. Da die Hauptdienste der Adobe [!DNL Experience Cloud] Adobe Audience Manager nutzen, müssen in den People-Hauptdiensten verwendete Daten sich auf Audience Manager-Servern in den USA befinden.

Wenn Sie Hauptdienste nutzen, die über den People-Hauptdienst verfügbar gemacht werden, werden die folgenden Datentypen von anderen Adobe-Produkten an das Zielgruppen-Management gesendet:

* Schlüssel-/Werte-Paare aus [!DNL Analytics] (Eigenschaften, eVars, Listenvariablen usw.). Standardmäßig enthalten die Protokollzeilen die IP-Adresse, inklusive des letzten Oktetts der IP (vorausgesetzt, die IP-Adresse wurde nicht durch Einstellungen zur IP-Verschleierung innerhalb von Adobe [!DNL Analytics] verändert).
* Eigenschaften und Segmente, für die sich Besucher basierend auf den in Audience Manager festgelegten Regeln qualifizieren.
* (Optional) Eine oder mehrere Ihrer IDs. In Abhängigkeit von der Implementierung des ID-Dienstes können Sie auch eine oder mehrere Ihrer IDs senden, wie zum Beispiel CRM-IDs oder E-Mail-Adressen mit Hash. Werden diese Daten an Adobe [!DNL Analytics] gesendet, werden sie an das Adobe Zielgruppen-Management übergeben. Adobe empfiehlt, keine personenbezogenen Daten in Adobe [!DNL Analytics] bereitzustellen. Verwenden Sie stattdessen einen unidirektionalen Hash, um die Daten zu pseudonymisieren, bevor Sie sie an Adobe senden.
* Segmente aus [!DNL Analytics] über die Back-End-Funktion zur Segmentfreigabe.
* Wenn Cookies von Drittanbietern nicht blockiert werden, wird das Cookie demdex.net gesetzt. Bei Verwendung des Experience Cloud ID-Dienstes (früher Besucher-ID) wird das Erstanbieter-Cookie `AMCV_###@AdobeOrg` immer aktiviert.


All diese Datenelemente werden Adobe Audience Manager in Form von Protokolldateien zur Verfügung gestellt. Audience Manager verarbeitet und speichert diese Daten innerhalb der USA. Audience Manager bietet keine Option zum Speichern oder Verarbeiten dieser Daten außerhalb der USA.

**Cookies und Opt-Outs**

Bei der Profilerstellung für Zielgruppen in Echtzeit wird neben den Cookies für [!DNL Analytics] und [!DNL Target] auch das Cookie von Audience Manager verwendet.

Wenn Sie eine geeignete Funktion zum Deaktivieren von Cookies bereitstellen möchten, müssen Besucher Ihrer Site diese Funktion aus Audience Manager zum vorhandenen Opt-out-Vorgang hinzufügen.

Anleitungen hierzu finden Sie unter [Adobe Experience Cloud – Implementieren von Adobe Opt-Outs](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/data-collection/opt-out.html).

Informationen zur Aktivierung des domänenübergreifenden Trackings finden Sie unter [CNAMEs für die Datenerfassung und domänenübergreifendes Tracking](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html).
