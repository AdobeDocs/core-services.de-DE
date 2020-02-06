---
description: Implementieren Sie die Experience Cloud und werden Sie Administrator. Durch diesen Prozess werden Ihre Lösungen bezüglich der Hauptdienst-Funktionen, wie Kundenattribute und Zielgruppen, modernisiert.
keywords: core services;customer attributes
seo-description: Implementieren Sie die Experience Cloud und werden Sie Administrator. Durch diesen Prozess werden Ihre Lösungen bezüglich der Hauptdienst-Funktionen, wie Kundenattribute und Zielgruppen, modernisiert.
seo-title: Experience Cloud-Lösungen für Hauptdienste aktivieren
solution: Experience Cloud
title: Lösungen für Hauptdienste aktivieren
uuid: 5820060f-9b18-4339-81e0-401d964f7a03
translation-type: tm+mt
source-git-commit: 02b0163b95c24eb58bf2379c3e0d9f5f31c40925

---


# Lösungen für Hauptdienste aktivieren

Erfahren Sie für Bestandskunden, wie Sie Ihre Lösungsimplementierungen modernisieren und die Experience Cloud implementieren, damit Sie Funktionen wie Kundenattribute und Zielgruppen verwenden können. Um dies zu erreichen, werden Sie:

1. [Experience Cloud beitreten und Administrator werden](#section_2423F0BD3DF642658103310EE5EA6154)
1. [Experience Cloud ID-Dienst implementieren](#section_3C9F6DF37C654D939625BB4D485E4354)
1. [Zuordnen von Report Suites zu einer Experience Cloud-Organisation](#section_7B08516B01BA421681DF03D0E86CE3BA)
1. [Analytics-AppMeasurement-Code aktualisieren](#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [Adobe Target-Implementierung aktualisieren](#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [Überprüfung der Implementierung der Hauptdienste](#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [Benutzer und Produkte verwalten](#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [Verwenden von Hauptdiensten beginnen](#section_960C06093623462E8EA247B3E97274A1)

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
>Migrieren Sie für Target von &quot;mbox.js&quot;zu &quot;at.js&quot;. Siehe [Aktualisieren von at.js 1. x zu at.js 2. x](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/upgrading-from-atjs-1x-to-atjs-20.html).

![](assets/step2_icon.png) Modernisieren Sie Ihre Implementierung und lassen Sie sich einen Administrator bereitstellen.

1. Folgen Sie den unten unter [Experience Cloud ID-Dienst bereitstellen](../core-services/core-services.md#section_3C9F6DF37C654D939625BB4D485E4354) beschriebenen Schritten.
1. Wenden Sie sich an Ihren Kundenbetreuer und beginnen Sie mit der Bereitstellung der Experience Cloud.

![](assets/step3_icon.png)[!UICONTROL  Verwalten Sie Benutzer und Produkte in der Admin Console].

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

Most likely, you have users who are already members of solution groups, such an Analytics group that you previously managed in [!UICONTROL Analytics] > [!UICONTROL Admin Tools].

Wenn Sie diese Gruppen Enterprise-Gruppen in der Experience Cloud zuordnen, müssen die betroffenen Benutzer die Anmeldeinformationen ihres Lösungskontos manuell mit ihrer Adobe ID verknüpfen.

Weitere Informationen finden Sie im Kapitel über die [Verknüpfung von Konten in der Experience Cloud](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1).

> [!NOTE]
> 
> Nach dem Mapping von Unternehmens- und Lösungsgruppen werden neue Benutzer automatisch verknüpft. (Anmeldeinformationen für die Lösung werden automatisch erstellt und mit der Adobe ID verknüpft.)

In den folgenden Abschnitten wird die Modernisierung der Implementierung beschrieben. Durch die Modernisierung Ihrer Implementierung werden Hauptdienste der Experience Cloud aktiviert.

## Schritt 2. Implementieren des [!UICONTROL Experience Cloud ID-Diensts] mithilfe von [!UICONTROL Experience Platform Launch]oder [!UICONTROL dynamischem Tag-Management]{#section_3C9F6DF37C654D939625BB4D485E4354}

Der [!UICONTROL Experience Cloud ID-Dienst] stellt eine gemeinsame ID für lösungsübergreifende Integration bereit. Es bietet eine domänenübergreifende Besucheridentifizierung und einen Pfad für geräteübergreifendes/Browser-Targeting und Personalisierung basierend auf CRM-Daten, die über [!UICONTROL Kundenattribute]hochgeladen wurden.

Die einfachste Methode zur Aktivierung der Hauptdienste der Experience Cloud besteht darin, diese automatisch für Analytics und Target über die Erweiterung[ des ](https://docs.adobe.com/content/help/en/launch/using/implement/solutions/idservice-save.html)Experience Cloud ID-Diensts im [!UICONTROL Experience Platform-Start]oder über das ECID-Tool im [!UICONTROL dynamischen Tag-Management]zu aktivieren. (Der Start der Erlebnisplattform wird dringend empfohlen.)

![](assets/menu-activation-shell.png)

For complete Experience Cloud ID Service help (formerly, visitor ID), go [here](https://docs.adobe.com/content/help/en/id-service/using/home.html).

**Verwenden Sie nicht[!UICONTROL Experience Platform Launch]oder[!UICONTROL dynamisches Tag-Management]?**

If you are not using [!UICONTROL Experience Platform Launch] or [!UICONTROL Dynamic Tag Management], manually implement the ID service via the JavaScript Deployment ([!DNL VisitorAPI.js]), as follows:

| Aufgabe | Beschreibung |
| -----------| ---------- |  
| [Implementieren des Experience Cloud ID-Diensts für Analytics](https://docs.adobe.com/content/help/en/id-service/using/implementation/setup-analytics.html) | Darüber hinaus empfiehlt Adobe die Einrichtung weiterer [Kunden-IDs](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html). Diese IDs sind jedem Besucher zugeordnet und ermöglichen die aktuelle und künftige Funktionalität in Experience Cloud. |
| Aktualisieren Sie Ihre vorhandene [!DNL s_code] auf die Version H.27.3 oder höher, oder Ihre vorhandene [!DNL AppMeasurement.js] auf Version 1.4 oder höher. | Diese Dateien stehen im [Code-Manager](https://docs.adobe.com/content/help/en/analytics/admin/admin-tools/code-manager-admin.html) der Analytics Admin Tools zum Download bereit.  (Eine [JavaScript-Implementierungsanleitung](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/javascript-implementation-overview.html) ist verfügbar, wenn Sie weitere Informationen zu [!DNL AppMeasurement.js] benötigen.) |
| Synchronisieren der Kunden-IDs für Analytics | Siehe [Analytics – Synchronisieren der Kunden-ID](../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437) (unten). |

## Analytics und Target – Synchronisieren der Kunden-ID {#section_AD473A6A21C1446498E700363F9A8437}

As a part of setting up the Experience Cloud ID Service, Adobe recommends for Analytics and [!DNL Target] that you synchronize your [customer IDs](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html) with the Experience Cloud.

In Adobe Target, the `mbox3rdpartyid` needs to get the customer ID and send it to [!DNL Target]. (Informationen hierzu finden sich im Kapitel zur [Arbeit mit Kundenattributen](https://docs.adobe.com/content/help/en/target/using/audiences/visitor-profiles/working-with-customer-attributes.html) in [!DNL Target].)

Wenn sich ein Besucher bei Ihrer Website authentifiziert oder sich auf andere Weise identifiziert, muss Ihre Implementierung die CRM-Kunden-ID dieser Person für die Seite oder App bereitstellen. Danach können Sie Ihre Kunden-ID mit dem entsprechenden Funktionsaufruf mit der Experience Cloud synchronisieren. Durch die Synchronisierung wird die CRM-Kunden-ID des Besuchers in der Experience Cloud gespeichert und die Attribute dieses Kunden werden für die Verwendung in der Experience Cloud aktiviert.

Beispiel: Bob hat in Ihrem CRM-System die Kunden-ID `52mc210tr42`. Wenn sich Bob bei Ihrer Site authentifiziert, müssen Sie diese ID auf der Seite bereitstellen und die ID zur Synchronisierung auf eine der beiden folgenden Arten verwenden:

* Aufruf von `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})` über den Besucher-ID-Dienst oder
* Ausfüllen der *`Customer ID (52mc210tr42)`* in eine Eigenschaft oder eVar.

Die Kunden-ID muss in jedem Aufruf an den [!DNL Analytics]-Server angegeben sein, auf dem die Kunden-ID bekannt ist.

### Mobile SDKs 

Syntaxbeispiele zum Festlegen zusätzlicher Kunden-IDs in *Android* - und [iOS](https://docs.adobe.com/content/help/en/mobile-services/android/overview.html) Mobile-Anwendungen finden Sie im Abschnitt zum Experience Cloud ID-Dienst[ ](https://docs.adobe.com/content/help/en/mobile-services/ios/overview.html).

### Aktivierung der Attribute historischer Daten

Die Kundenattributdaten stehen nach der Anmeldung eines Besuchers zur Verfügung. Wenn Sie den neuesten Experience Cloud ID-Dienst noch nicht implementiert haben und Kunden-IDs in einer prop oder eVar historisch verfolgt haben, können Sie einen Prozess anfordern, der historische Anmeldungen an die Experience Cloud sendet. Nach Ausführung dieses Prozesses können Sie die Kundenattribute sofort verwenden.

Wenden Sie sich an den Kundenservice, um Ihre historischen Daten aktivieren zu lassen.

## Schritt 3. Map report suites to an Experience Cloud Organization {#section_7B08516B01BA421681DF03D0E86CE3BA}

Experience Cloud services (such as Experience Cloud ID Service and the [!UICONTROL People service]) are associated with an Experience Cloud organization instead of an individual Analytics report suite. Damit sichergestellt ist, dass diese Dienste korrekt funktionieren, muss jede Analytics-Report Suite einer Experience Cloud-Organisation zugeordnet sein.

Weitere Informationen dazu finden Sie unter [Report Suites einer Organisation zuweisen](report-suite-mapping.md).

## Schritt 4. (Adobe Analytics) Update your Analytics AppMeasurement code {#section_1798D9D0F05C47E29816AC4EEB9A0913}

Vergewissern Sie sich, dass Sie die regionale Datenerfassung (RDC) verwenden. Wenn Ihre Datenerfassungsdomäne [!DNL omtrdc.net] lautet, oder wenn Ihr CNAME [!DNL omtrdc.net] zugeordnet ist, befinden Sie sich auf RDC. Weitere Informationen finden Sie unter [Übergang zu RDC. ](https://docs.adobe.com/content/help/en/analytics/technotes/rdc/regional-data-collection.html) If you are using first-party cookies, refer to [CNAME and the Experience Cloud ID Service](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html) for information about data collection CNAMEs and cross-domain tracking.

Adobe empfiehlt eine Modernisierung Ihrer Analytics-Implementierung durch Aktualisierung Ihrer JavaScript-Bibliotheken einschließlich der Besucher-API. Am einfachsten erreichen Sie eine solche Modernisierung durch Hinzufügen des Tools [!DNL Adobe Analytics] im Dynamic Tag Management (DTM), das *`Automatic`* als Konfigurationsmethode angibt.

In [!UICONTROL Dynamic Tag Management], click **[!UICONTROL <Web Property Name>]**>**[!UICONTROL &#x200B;Übersicht ]**>**[!UICONTROL  Tool hinzufügen ]**>**[!UICONTROL  Adobe Analytics ]**. Implementierungsinformationen erhalten Sie unter[Adobe Analytics-Einstellungen](https://docs.adobe.com/content/help/en/dtm/using/tools/analytics-dtm.html)in der Hilfe zum Dynamic Tag Management.

## Schritt 5. (Adobe Target) Update your Adobe Target implementation {#section_C2F4493C7A36406DAE2266B429A4BD24}

* It is recommended that you add an [Adobe Target extension](https://docs.adobe.com/content/help/en/launch/using/extensions-ref/adobe-extension/targetv2-extension/adobe-target-extension-v2.html) in [!UICONTROL Experience Platform Launch], so that your library retrieval is automatic. Sie können auch die [Experience Cloud ID-Diensterweiterung](https://docs.adobe.com/content/help/en/launch/using/extensions-ref/adobe-extension/id-service-extension/overview.html) für Target (und andere Lösungen) mithilfe von [!UICONTROL Experience Platform Launch]einrichten. The [!UICONTROL Experience Cloud ID Service] update **is required** for [!UICONTROL Target] to use core services. (Wenn Sie [!UICONTROL dynamisches Tag-Management]verwenden, fügen Sie ein [Adobe Target-Tool](https://docs.adobe.com/content/help/en/dtm/using/tools/target.html)hinzu. You can also use [!UICONTROL Dynamic Tag Management] to deploy the Experience Cloud ID Service for Target.)
* Wenn Sie [!UICONTROL Experience Platform Launch] oder [!UICONTROL dynamisches Tag-Management]nicht verwenden, [aktualisieren Sie Ihre mbox-Bibliothek](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/target-download-config-mbox.html) manuell.
* Request access to use Adobe Analytics as the reporting source for [!DNL Adobe Target]. [!DNL Target] und [!DNL Analytics] Daten während der Verarbeitung für denselben Serveraufruf kombiniert werden, sodass Besucher zwischen den beiden Lösungen verbunden werden. Siehe [Analytics für die Target-Implementierung](https://docs.adobe.com/content/help/en/target/using/integrate/a4t/a4t.html).

   >[!IMPORTANT]
   >
   >Alle Analytics-Kunden sind bereits für Hauptdienste wie Kundenattribute bereitgestellt. Wenn Sie kein Analytics-Kunde sind, wenden Sie sich an die Kundenunterstützung, um eine Freischaltung anzufordern.

## Schritt 6. Überprüfung der Implementierung der Hauptdienste {#section_E641782A0F4F44AF8C9C91216BE330D5}

Verwenden Sie den folgenden Prozess, um sicherzustellen, dass der Experience Cloud ID-Dienst auf Ihrer Site korrekt implementiert ist.

1. Löschen Sie die Cookies für Ihre Site, damit Sie die Anforderung an den Experience Cloud ID-Dienst sehen können (die Anforderung erfolgt beim ersten Besuch und danach etwa einmal pro Besucher pro Woche).
1. Suchen Sie mit einem Paket-Sniffer oder dem Netzwerkbereich eines Webbrowser-Debuggers nach einer Anfrage für [!DNL dpm.demdex.net].
1. Überprüfen Sie, ob die Antwort `d_mid` und einen Wert enthält, z. B.: `_setMarketingCloudFields({"d_mid":"4235...`
1. Verify that the Analytics request contains the `mid` parameter (the Experience Cloud ID). During the grace period (if it is enabled), you should also see an `aid` parameter (the Analytics visitor ID).

Erwartete Antwort mit der Experience Cloud ID:

![](assets/mac_id_response.png)

Analytics-Bildanforderung mit der Experience Cloud ID (auch als `mid` Besucher-ID __ bezeichnet):

![](assets/mid.png)

Experience Cloud ID in der mbox-Anforderung:

![](assets/mbox_request.png)

**Was ist die Übergangsphase?**

Nach der Bereitstellung des Experience Cloud ID-Diensts erhalten neue Besucher keine Analytics Experience Cloud ID mehr von Ihrem Datenerfassungsserver. Wenn Abschnitte Ihrer Site den Experience Cloud ID-Dienst noch nicht implementiert haben und Besucher zu diesen Abschnitten navigieren, wird die Experience Cloud ID nicht erkannt und Besuchern wird eine Legacy-Analytics-Besucher-ID zugewiesen. Dies kann potenziell zu Problemen führen, unter anderem zu duplizierten Besuchen und fehlerhaften Zuweisungen.

Wenn der Supportbereich der Site beispielsweise über ein gesondertes CMS verwaltet wird, verwenden Sie für diesen Bereich möglicherweise eine andere Analytics-JavaScript-Datei. Wenn Sie die Experience Cloud-ID auf Ihrer Haupt-Site bereitstellen, bevor Sie den ID-Dienst auf der Support-Site bereitstellen, erhalten neue Besucher beim Besuch des Supportbereichs eine Legacy-Analytics-ID. Besuche, die beide Site-Abschnitte umfassen, werden als unterschiedliche Besuche gemeldet.

Die Bereitstellung des Experience Cloud ID-Diensts auf Sites, die mehrere JavaScript-Dateien oder andere Technologien (z. B. Flash) verwenden, kann Koordinierungsprobleme verursachen, da Sie den Experience Cloud ID-Dienst auf allen Teilen Ihrer Site gleichzeitig aktivieren müssen. Durch die Konfiguration einer Übergangsphase erhalten neue Besucher weiterhin eine Analytics-Besucher-ID vom ID-Dienst, damit Besucher konsistent in Sitebereichen identifiziert werden können, die noch nicht auf die Verwendung des Besucher-ID-Service aktualisiert wurden.

## Schritt 7. Benutzer und Produkte verwalten {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Once you are up and running, navigate to the [Admin Console](https://adminconsole.adobe.com/), where you can manage users and product profiles.

![](assets/menu-administration-shell.png)

Siehe [Verwalten von Experience Cloud-Benutzern und -produkten](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

**Kundenattribute**

<!-- <p> 
 <note type="important">
  To use the Customer Attributes feature, users must belong to the 
  <span class="term"> Adobe Customer Attributes</span> group, and to solution-level groups (Analytics or Target). 
 </note> </p> 
 -->

Users that are added to the [!UICONTROL Customer Attributes] group will see the [!UICONTROL Customer Attributes] menu item on the left side of the Experience Cloud interface

## Schritt 8. Begin using core services {#section_960C06093623462E8EA247B3E97274A1}

Nutzen Sie die Vorteile folgender Funktionen der Hauptdienste.

![](assets/menu-audiences-shell.png)

**[!UICONTROL Personen]>[!UICONTROKundenattribute]**

Wenn Sie Daten von Unternehmenskunden in einer CRM-Datenbank (Customer Relationship Management) erfassen, können Sie diese Daten in eine Datenquelle für Kundenattribute in die Experience Cloud hochladen. Verarbeiten Sie die Daten nach dem Hochladen mit [!DNL Adobe Analytics] und [!DNL Adobe Target].

Weitere Informationen finden Sie unter [Kundenattribute](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)

**[!UICONTROL Personen]>[!UICONTROL Zielgruppenbibliothek]**

Experience Cloud [!UICONTROL Audiences] is the interface that lets you create audiences, combine existing audiences to create composite audiences, and view all shared audiences.

Weitere Informationen finden Sie unter [Zielgruppen](../audience-library/audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)

<!-- aam_mc.xml -->

## Datenspeicherung und Datenschutz

Wenn Sie Echtzeit-Zielgruppenprofile und andere Hauptdienste in der Adobe [!DNL Experience Cloud] nutzen, hat die Verwendung dieser Dienste Auswirkungen darauf, in welchem Datenzentrum (und Land) sich Ihre Daten befinden. Specifically, because the core services of the Adobe [!DNL Experience Cloud] leverage Adobe Audience Manager, data used within the [!UICONTROL People] service must reside within Audience Manager servers in the United States.

When leveraging core services made available via the [!UICONTROL People] service, the types of data sent from other Adobe products to audience management are:

* Schlüssel-/Werte-Paare aus [!DNL Analytics] (Eigenschaften, eVars, Listenvariablen usw.). Standardmäßig enthalten die Protokollzeilen die IP-Adresse, inklusive des letzten Oktetts der IP (vorausgesetzt, die IP-Adresse wurde nicht durch Einstellungen zur IP-Verschleierung innerhalb von Adobe [!DNL Analytics] verändert).
* Eigenschaften und Segmente, für die sich Besucher basierend auf den in Audience Manager festgelegten Regeln qualifizieren.
* (Optional) Eine oder mehrere Ihrer IDs. In Abhängigkeit von der Implementierung des ID-Dienstes können Sie auch eine oder mehrere Ihrer IDs senden, wie zum Beispiel CRM-IDs oder E-Mail-Adressen mit Hash. Werden diese Daten an Adobe [!DNL Analytics] gesendet, werden sie an das Adobe Zielgruppen-Management übergeben. Adobe empfiehlt, keine personenbezogenen Daten in Adobe [!DNL Analytics] bereitzustellen. Verwenden Sie stattdessen einen unidirektionalen Hash, um die Daten zu pseudonymisieren, bevor Sie sie an Adobe senden.
* Segmente aus [!DNL Analytics] über die Back-End-Funktion zur Segmentfreigabe.
* Wenn Cookies von Drittanbietern nicht blockiert werden, wird das Cookie demdex.net gesetzt. The `AMCV_###@AdobeOrg` first-party cookie is always set with the Experience Cloud ID Service.

All diese Datenelemente werden Adobe Audience Manager in Form von Protokolldateien zur Verfügung gestellt. Audience Manager verarbeitet und speichert diese Daten innerhalb der USA. Audience Manager bietet keine Option zum Speichern oder Verarbeiten dieser Daten außerhalb der USA.

**Cookies und Opt-Outs**

Bei der Profilerstellung für Zielgruppen in Echtzeit wird neben den Cookies für [!DNL Analytics] und [!DNL Target] auch das Cookie von Audience Manager verwendet.

Wenn Sie eine geeignete Funktion zum Deaktivieren von Cookies bereitstellen möchten, müssen Besucher Ihrer Site diese Funktion aus Audience Manager zum vorhandenen Opt-out-Vorgang hinzufügen.

Anleitungen hierzu finden Sie unter [Adobe Experience Cloud – Implementieren von Adobe Opt-Outs](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/data-collection/opt-out.html).

Informationen zur Aktivierung des domänenübergreifenden Trackings finden Sie unter [CNAMEs für die Datenerfassung und domänenübergreifendes Tracking](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html).
