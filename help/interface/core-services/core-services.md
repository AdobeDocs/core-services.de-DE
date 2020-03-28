---
description: Implementieren Sie Experience Cloud und werden Sie Administrator. Dieser Prozess modernisiert Ihre Lösungen für Kerndienstfunktionen wie Kundenattribute und Audiencen.
keywords: core services;customer attributes
seo-description: Implementieren Sie Experience Cloud und werden Sie Administrator. Dieser Prozess modernisiert Ihre Lösungen für Kerndienstfunktionen wie Kundenattribute und Audiencen.
seo-title: Experience Cloud-Lösungen für Hauptdienste aktivieren
solution: Experience Cloud
title: Lösungen für Hauptdienste aktivieren
index: true
translation-type: tm+mt
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e

---


# Lösungen für Hauptdienste aktivieren

Erfahren Sie für Bestandskunden, wie Sie Ihre Lösungsimplementierungen modernisieren und die Experience Cloud implementieren, damit Sie Funktionen wie Kundenattribute und Audiencen verwenden können. Um dies zu erreichen, werden Sie:

1. [Experience Cloud beitreten und Administrator werden](#section_2423F0BD3DF642658103310EE5EA6154)
1. [Implementieren des Experience Cloud ID-Diensts](#section_3C9F6DF37C654D939625BB4D485E4354)
1. [Zuordnen von Report Suites zu einer Experience Cloud-Organisation](#section_7B08516B01BA421681DF03D0E86CE3BA)
1. [Analytics-AppMeasurement-Code aktualisieren](#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [Implementierung der Adobe-Zielgruppe aktualisieren](#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [Überprüfung der Implementierung der Hauptdienste](#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [Benutzer und Produkte verwalten](#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [Verwenden von Hauptdiensten beginnen](#section_960C06093623462E8EA247B3E97274A1)

## Schritt 1. Experience Cloud beitreten und Administrator werden {#section_2423F0BD3DF642658103310EE5EA6154}

Möchten Sie Experience Cloud-Mitglied werden, benötigen Sie Folgendes:

![](assets/step1_icon.png) Stellen Sie sicher, dass Sie über gültige SKUs für Adobe Analytics oder Adobe Target verfügen.

* **Adobe Analytics:** Standard oder Premium (nicht die ältere [!DNL SiteCatalyst] SKU).
* **Adobe-Zielgruppe:** Standard oder Premium.

>[!NOTE]
>
>Migrieren Sie [!DNL Target]beispielsweise von &quot;at.js&quot;zu &quot;at.js&quot; [!DNL mbox.js]. See [Upgrading from at.js 1. x to at.js 2. x](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/upgrading-from-atjs-1x-to-atjs-20.html).

![](assets/step2_icon.png) Modernisieren Sie Ihre Implementierung und lassen Sie sich einen Administrator bereitstellen.

1. Gehen Sie wie folgt vor, um [den [!UICONTROL Experience Cloud ID-Dienst]](../core-services/core-services.md#section_3C9F6DF37C654D939625BB4D485E4354)bereitzustellen.
1. Wenden Sie sich an Ihren Kundenbetreuer und Beginn zum Bereitstellungsprozess für die Experience Cloud.

![](assets/step3_icon.png)[!UICONTROL  Verwalten Sie Benutzer und Produkte in der Admin Console].

### Administratoranmeldung

After you are an administrator, you can log in at [experiencecloud.adobe.com](https://experiencecloud.adobe.com).

Im Experience Cloud-Navigationsmenü wird der Link **[!UICONTROL Administration]** angezeigt.

Weitere Informationen finden Sie unter [Experience Cloud – Benutzer und Produkte verwalten](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

### Benutzeranmeldung

Um sich bei Experience Cloud anzumelden, müssen Ihre Benutzer:

1. Sie haben eine Adobe ID (oder Enterprise ID für Ihre Firma).
1. Sign in at [experiencecloud.adobe.com](https://experiencecloud.adobe.com).
1. Gehört zu einer Lösungsgruppe, die einer Unternehmensgruppe zugeordnet ist.
1. Verknüpfen Sie ggf. die Lösungskonten mit ihrer Adobe ID (siehe Beschreibung unten).

![](assets/step4_icon.png) Optional: Verknüpfen Sie vorhandene Benutzerkonten.

Wahrscheinlich haben Sie Benutzer, die bereits Mitglied von Lösungsgruppen sind, z. B. eine Analytics-Gruppe, die Sie zuvor unter [!UICONTROL Analytics] > [!UICONTROL Admin Tools]verwaltet haben.

Wenn Sie diese Gruppen Experience Cloud-Unternehmensgruppen zuordnen, müssen diese Benutzer ihre Anmeldeinformationen für das Lösungskonto manuell mit ihrer Adobe ID verknüpfen.

Siehe [Verknüpfen von Konten in der Experience Cloud](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)

>[!NOTE]
>
>Nach dem Mapping von Unternehmens- und Lösungsgruppen werden neue Benutzer automatisch verknüpft. (Lösungsberechtigungen werden automatisch erstellt und mit ihrer Adobe ID verknüpft.)

Die folgenden Abschnitte beschreiben, wie Sie Ihre Implementierung modernisieren. Durch die Modernisierung Ihrer Implementierung werden die Hauptdienste in der Experience Cloud aktiviert.

## Schritt 2. Implementieren des [!UICONTROL Experience Cloud ID-Diensts] mithilfe von [!UICONTROL Experience Platform Launch]oder [!UICONTROL dynamischem Tag-Management]{#section_3C9F6DF37C654D939625BB4D485E4354}

Der [!UICONTROL Experience Cloud ID-Dienst] stellt eine gemeinsame ID für lösungsübergreifende Integration bereit. Es bietet eine domänenübergreifende Besucher-Identifikation und einen Pfad für geräteübergreifendes bzw. browserübergreifendes Targeting und Personalisierung basierend auf CRM-Daten, die über [!UICONTROL Kundenattribute]hochgeladen wurden.

Die einfachste Methode zur Aktivierung der Experience Cloud-Hauptdienste besteht darin, diese automatisch für Analytics und Adobe-Zielgruppe über die [Experience Cloud ID-Diensterweiterung](https://docs.adobe.com/content/help/en/launch/using/implement/solutions/idservice-save.html) in [!UICONTROL Experience Platform Launch]oder über das ECID-Tool im [!UICONTROL dynamischen Tag-Management]zu aktivieren. (Der Start der Erlebnisplattform wird dringend empfohlen.)

![](assets/menu-activation-shell.png)

Die vollständige Hilfe zum Experience Cloud ID-Dienst (früher Besucher-ID) finden Sie [hier](https://docs.adobe.com/content/help/en/id-service/using/home.html).

**Verwenden Sie nicht[!UICONTROL Experience Platform Launch]oder[!UICONTROL dynamisches Tag-Management]?**

If you are not using [!UICONTROL Experience Platform Launch] or [!UICONTROL Dynamic Tag Management], manually implement the ID service via the JavaScript Deployment ([!DNL VisitorAPI.js]), as follows:

| Aufgabe | Beschreibung |
| -----------| ---------- |  
| [Implementieren des Experience Cloud ID-Diensts für Analytics](https://docs.adobe.com/content/help/en/id-service/using/implementation/setup-analytics.html) | Adobe empfiehlt auch, zusätzliche [Kunden-IDs](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html)festzulegen. Diese IDs sind mit jedem Besucher verknüpft und ermöglichen die aktuelle und künftige Funktionalität in Experience Cloud. |
| Aktualisieren Sie Ihre vorhandene [!DNL s_code] auf die Version H.27.3 oder höher, oder Ihre vorhandene [!DNL AppMeasurement.js] auf Version 1.4 oder höher. | Diese Dateien können im [Code-Manager](https://docs.adobe.com/content/help/en/analytics/admin/admin-tools/code-manager-admin.html) in den Analytics Admin Tools heruntergeladen werden.  (Das Implementierungshandbuch für [JavaScript](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/javascript-implementation-overview.html) ist verfügbar, wenn Sie weitere Informationen benötigen [!DNL AppMeasurement.js].) |
| Kunden-ID für Analytics synchronisieren | See [Analytics - synching the customer ID](../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437) (below). |

## Analytics &amp; Adobe Target - synching the customer ID {#section_AD473A6A21C1446498E700363F9A8437}

As a part of setting up the Experience Cloud ID Service, Adobe recommends for Analytics and [!DNL Target] that you synchronize your [customer IDs](https://docs.adobe.com/content/help/en/id-service/using/reference/authenticated-state.html) with the Experience Cloud.

In Adobe Target, the `mbox3rdpartyid` needs to get the customer ID and send it to [!DNL Target]. (Siehe [Arbeiten mit Kundenattributen](https://docs.adobe.com/content/help/en/target/using/audiences/visitor-profiles/working-with-customer-attributes.html) in [!DNL Target].)

Wenn sich ein Besucher auf Ihrer Website authentifiziert oder sich auf andere Weise identifiziert, muss Ihre Implementierung die CRM-Kunden-ID dieser Person der Seite oder App zur Verfügung stellen. Anschließend können Sie den entsprechenden Funktionsaufruf verwenden, um Ihre Kunden-ID mit der Experience Cloud zu synchronisieren. Durch diese Synchronisierung wird die CRM-Kunden-ID des Besuchers in der Experience Cloud gespeichert und die Attribute dieses Kunden für die Verwendung in der Experience Cloud aktiviert.

Beispiel: Bob hat in Ihrem CRM-System die Kunden-ID `52mc210tr42`. Wenn sich Bob bei Ihrer Site authentifiziert, müssen Sie diese ID auf der Seite bereitstellen und die ID zur Synchronisierung auf eine der beiden folgenden Arten verwenden:

* Aufruf von `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})` über den Besucher-ID-Dienst Oder,
* Füllen Sie die *`Customer ID (52mc210tr42)`* Variable in einer Eigenschaftsvariable oder eVar.

Die Kunden-ID muss in jedem Aufruf an den [!DNL Analytics]-Server angegeben sein, auf dem die Kunden-ID bekannt ist.

### Mobile SDKs 

Syntaxbeispiele zum Festlegen zusätzlicher Kunden-IDs in *Android* - und [iOS](https://docs.adobe.com/content/help/en/mobile-services/android/overview.html) Mobile-Anwendungen finden Sie im Abschnitt zum Experience Cloud ID-Dienst [](https://docs.adobe.com/content/help/en/mobile-services/ios/overview.html) .

### Aktivierung der Attribute historischer Daten

Kundenattributdaten werden nach der Anmeldung durch die Besucher bereitgestellt. Wenn Sie den neuesten Experience Cloud ID-Dienst noch nicht implementiert haben und Kunden-IDs in einer prop oder eVar historisch verfolgt haben, können Sie einen Prozess anfordern, der historische Anmeldungen an die Experience Cloud sendet. Auf diese Weise können Sie sofort mit der Verwendung von Kundenattributen beginnen.

Wenden Sie sich an den Kundendienst, um Verlaufsdaten zu aktivieren.

## Schritt 3. Map report suites to an Experience Cloud Organization {#section_7B08516B01BA421681DF03D0E86CE3BA}

Experience Cloud services (such as Experience Cloud ID Service and the [!UICONTROL People service]) are associated with an Experience Cloud organization instead of an individual Analytics report suite. Um sicherzustellen, dass diese Dienste ordnungsgemäß funktionieren, muss jede Analytics-Report Suite einer Experience Cloud-Organisation zugeordnet werden.

Weitere Informationen dazu finden Sie unter [Report Suites einer Organisation zuweisen](report-suite-mapping.md).

## Schritt 4. (Adobe Analytics) Update your Analytics AppMeasurement code {#section_1798D9D0F05C47E29816AC4EEB9A0913}

Vergewissern Sie sich, dass Sie die regionale Datenerfassung (RDC) verwenden. Wenn Ihre Datenerfassungsdomäne [!DNL omtrdc.net] lautet, oder wenn Ihr CNAME [!DNL omtrdc.net] zugeordnet ist, befinden Sie sich auf RDC. Weitere Informationen finden Sie unter [Übergang zu RDC](https://docs.adobe.com/content/help/en/analytics/technotes/rdc/regional-data-collection.html) . Wenn Sie Erstanbieter-Cookies verwenden, finden Sie unter [CNAME und Experience Cloud ID-Dienst](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html) Informationen zu Datenerfassungs-CNAMEs und domänenübergreifender Verfolgung.

Adobe empfiehlt eine Modernisierung Ihrer Analytics-Implementierung durch Aktualisierung Ihrer JavaScript-Bibliotheken einschließlich der Besucher-API. Am einfachsten erreichen Sie eine solche Modernisierung durch Hinzufügen des Tools [!DNL Adobe Analytics] im Dynamic Tag Management (DTM), das *`Automatic`* als Konfigurationsmethode angibt.

In [!UICONTROL Dynamic Tag Management], click **[!UICONTROL <Web Property Name>]**>**[!UICONTROL &#x200B;Übersicht ]**>**[!UICONTROL  Hinzufügen Tool ]**>**[!UICONTROL  Adobe Analytics ]**. Informationen zur Bereitstellung finden Sie unter[Adobe Analytics-Einstellungen](https://docs.adobe.com/content/help/en/dtm/using/tools/analytics-dtm.html)im dynamischen Tag-Management.

## Schritt 5. (Adobe Target) Update your Adobe Target implementation {#section_C2F4493C7A36406DAE2266B429A4BD24}

* Es wird empfohlen, eine [Adobe-Erweiterung des Zieldatensatzes](https://docs.adobe.com/content/help/en/launch/using/extensions-ref/adobe-extension/targetv2-extension/adobe-target-extension-v2.html) in [!UICONTROL Experience Platform Launch]hinzuzufügen, damit der Bibliotheksabruf automatisch erfolgt. Sie können auch die [Experience Cloud ID-Diensterweiterung](https://docs.adobe.com/content/help/en/launch/using/extensions-ref/adobe-extension/id-service-extension/overview.html) für Adobe Zielgruppe (und andere Lösungen) mithilfe von [!UICONTROL Experience Platform Launch]einrichten. Die Aktualisierung des [!UICONTROL Experience Cloud ID-Diensts] **ist erforderlich** , damit Adobe Zielgruppe die Hauptdienste verwenden kann. (Wenn Sie [!UICONTROL dynamisches Tag-Management]verwenden, fügen Sie ein [Adobe-Zielgruppe-Tool](https://docs.adobe.com/content/help/en/dtm/using/tools/target.html)hinzu. Sie können auch das [!UICONTROL dynamische Tag-Management] verwenden, um den Experience Cloud ID-Dienst für Adobe-Zielgruppe bereitzustellen.)
* Wenn Sie [!UICONTROL Experience Platform Launch] oder [!UICONTROL dynamisches Tag-Management]nicht verwenden, [aktualisieren Sie Ihre mbox-Bibliothek](https://docs.adobe.com/content/help/en/target/using/implement-target/client-side/mbox-implement/target-download-config-mbox.html) manuell.
* Request access to use Adobe Analytics as the reporting source for [!DNL Adobe Target]. [!DNL Target] und [!DNL Analytics] Daten während der Verarbeitung für denselben Serveraufruf kombiniert werden, sodass Besucher zwischen den beiden Lösungen verbunden werden. See [Analytics for Target Implementation](https://docs.adobe.com/content/help/en/target/using/integrate/a4t/a4t.html).

   >[!IMPORTANT]
   >
   >Alle Analytics-Kunden sind bereits für Hauptdienste wie Kundenattribute bereitgestellt. Wenn Sie kein Analytics-Kunde sind, wenden Sie sich an die Kundenunterstützung, um eine Freischaltung anzufordern.

## Schritt 6. Überprüfung der Implementierung der Hauptdienste {#section_E641782A0F4F44AF8C9C91216BE330D5}

Verwenden Sie den folgenden Prozess, um sicherzustellen, dass der Experience Cloud ID-Dienst auf Ihrer Site korrekt implementiert ist.

1. Löschen Sie die Cookies für Ihre Site, damit Sie die Anforderung an den Experience Cloud ID-Dienst sehen können (die Anforderung erfolgt beim ersten Besuch und danach etwa einmal pro Besucher und Woche).
1. Suchen Sie mit einem Paket-Sniffer oder dem Netzwerkbereich eines Webbrowser-Debuggers nach einer Anfrage für [!DNL dpm.demdex.net].
1. Überprüfen Sie, ob die Antwort `d_mid` und einen Wert enthält, z. B.: `_setMarketingCloudFields({"d_mid":"4235...`
1. Überprüfen Sie, ob die Analytics-Anforderung den `mid` Parameter enthält (die Experience Cloud ID). Während der Übergangsphase (sofern aktiviert) sollte auch ein `aid` Parameter angezeigt werden (die Analytics-Besucher-ID).

Erwartete Antwort mit der Experience Cloud ID:

![](assets/mac_id_response.png)

Analytics-Bildanforderung mit der Experience Cloud ID (auch bekannt als `mid` Besucher-ID __):

![](assets/mid.png)

Experience Cloud ID in der mbox-Anfrage:

![](assets/mbox_request.png)

### Was ist die Übergangsphase?

Nach der Bereitstellung des Experience Cloud ID-Diensts erhalten neue Besucher keine Analytics Experience Cloud-ID mehr von Ihrem Datenerfassungsserver. Wenn Bereiche Ihrer Site den Experience Cloud ID-Dienst noch nicht implementiert haben und Besucher zu diesen Abschnitten navigieren, wird die Experience Cloud ID nicht erkannt und Besuchern wird eine Legacy-Analytics-Besucher-ID zugewiesen. Dies kann zu potenziellen Problemen führen, einschließlich Besuchen von Duplikaten und falscher Zuordnung.

Wenn beispielsweise der Supportbereich Ihrer Site in einem separaten CMS verwaltet wird, haben Sie möglicherweise eine andere Analytics-JavaScript-Datei für diesen Abschnitt. Wenn Sie die Experience Cloud-ID auf Ihrer Haupt-Site bereitstellen, bevor Sie den ID-Dienst auf der Support-Site bereitstellen, erhalten neue Besucher beim Besuch des Supportbereichs eine Legacy-Analytics-ID. Besuche, die beide Sitebereiche umfassen, werden als unterschiedliche Besuche gemeldet.

Die Bereitstellung des Experience Cloud ID-Diensts auf Sites, die mehrere JavaScript-Dateien oder andere Technologien (z. B. Flash) verwenden, kann Koordinierungsprobleme verursachen, da Sie den Experience Cloud ID-Dienst auf allen Teilen Ihrer Site gleichzeitig aktivieren müssen. Durch die Konfiguration einer Übergangsphase erhalten neue Besucher weiterhin eine Analytics-Besucher-ID vom ID-Dienst, damit Besucher in Sitebereichen, die noch nicht auf die Verwendung des Besucher-ID-Diensts aktualisiert wurden, konsistent identifiziert werden können.

## Schritt 7. Benutzer und Produkte verwalten {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Once you are up and running, navigate to the [Admin Console](https://adminconsole.adobe.com/), where you can manage users and product profiles.

![](assets/menu-administration-shell.png)

Siehe [Verwalten von Experience Cloud-Benutzern und -produkten](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

### Kundenattribute

<!-- <p> 
 <note type="important">
  To use the Customer Attributes feature, users must belong to the 
  <span class="term"> Adobe Customer Attributes</span> group, and to solution-level groups (Analytics or Adobe Target). 
 </note> </p> 
 -->

Users that are added to the [!UICONTROL Customer Attributes] group will see the [!UICONTROL Customer Attributes] menu item on the left side of the Experience Cloud interface.

## Schritt 8. Begin using core services {#section_960C06093623462E8EA247B3E97274A1}

Nutzen Sie die Vorteile folgender Funktionen der Hauptdienste.

![](assets/menu-audiences-shell.png)

### [!UICONTROL Personen] > [!UICONTROL Kundenattribute]

Wenn Sie Daten von Unternehmenskunden in einer CRM-Datenbank (Customer Relationship Management) erfassen, können Sie diese Daten in eine Datenquelle für Kundenattribute in die Experience Cloud hochladen. Verarbeiten Sie die Daten nach dem Hochladen mit [!DNL Adobe Analytics] und [!DNL Adobe Target].

Weitere Informationen finden Sie unter [Kundenattribute](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)

### [!UICONTROL Personen] > [!UICONTROL Audience-Bibliothek]

Experience Cloud [!UICONTROL Audiences] is the interface that lets you create audiences, combine existing audiences to create composite audiences, and view all shared audiences.

Weitere Informationen finden Sie unter [Zielgruppen](../audience-library/audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)

## Datenspeicherung und Datenschutz

Wenn Sie Echtzeit-Zielgruppenprofile und andere Hauptdienste in der Adobe [!DNL Experience Cloud] nutzen, hat die Verwendung dieser Dienste Auswirkungen darauf, in welchem Datenzentrum (und Land) sich Ihre Daten befinden. Specifically, because the core services of the Adobe [!DNL Experience Cloud] leverage Adobe Audience Manager, data used within the [!UICONTROL People] service must reside within Audience Manager servers in the United States.

When leveraging core services made available via the [!UICONTROL People] service, the types of data sent from other Adobe products to audience management are:

* Schlüssel-/Werte-Paare aus [!DNL Analytics] (Eigenschaften, eVars, Listenvariablen usw.). Standardmäßig enthalten die Protokollzeilen die IP-Adresse, inklusive des letzten Oktetts der IP (vorausgesetzt, die IP-Adresse wurde nicht durch Einstellungen zur IP-Verschleierung innerhalb von Adobe [!DNL Analytics] verändert).
* Eigenschaften und Segmente, für die sich Besucher auf der Grundlage der in Audience Manager festgelegten Regeln qualifizieren.
* (Optional) Eine oder mehrere Ihrer IDs. Je nach Implementierung des ID-Diensts senden Sie möglicherweise auch eine oder mehrere Ihrer IDs, z. B. CRM-IDs oder Hash-E-Mail-Adressen. Werden diese Daten an Adobe [!DNL Analytics] gesendet, werden sie an das Adobe Zielgruppen-Management übergeben. Adobe empfiehlt, keine personenbezogenen Daten in Adobe [!DNL Analytics] bereitzustellen. Verwenden Sie stattdessen einen einseitigen Hash, um die Daten zu maskieren, bevor sie an Adobe gesendet werden.
* Segmente aus [!DNL Analytics] über die Back-End-Funktion zur Segmentfreigabe.
* Wenn Cookies von Drittanbietern nicht blockiert werden, wird das Cookie demdex.net gesetzt. The `AMCV_###@AdobeOrg` first-party cookie is always set with the Experience Cloud ID Service.

Alle diese Datenelemente werden in Form von Protokolldateien an Adobe Audience Manager gesendet. Audience Manager verarbeitet und speichert diese Daten in den Vereinigten Staaten. Audience Manager bietet keine Option zum Speichern oder Verarbeiten dieser Daten außerhalb der USA.

### Cookies und Opt-Outs

Bei der Profilerstellung für Zielgruppen in Echtzeit wird neben den Cookies für [!DNL Analytics] und [!DNL Target] auch das Cookie von Audience Manager verwendet.

Wenn Sie eine geeignete Funktion zum Deaktivieren von Cookies bereitstellen möchten, müssen Besucher Ihrer Site diese Funktion aus Audience Manager zum vorhandenen Opt-out-Vorgang hinzufügen.

Anweisungen finden Sie unter [Adobe Experience Cloud - Implementieren von Adobe Opt-Outs](https://docs.adobe.com/content/help/en/analytics/implementation/javascript-implementation/data-collection/opt-out.html) .

Informationen zum Aktivieren der domänenübergreifenden Verfolgung finden Sie unter CNAMEs für die [Datenerfassung und domänenübergreifende Verfolgung](https://docs.adobe.com/content/help/en/id-service/using/reference/analytics-reference/cname.html) .
