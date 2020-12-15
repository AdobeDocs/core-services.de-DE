---
description: Erfahren Sie, wie Sie das Adobe Experience Cloud implementieren und Administrator werden.
keywords: core services;Customer Attributes
solution: Experience Cloud
title: 'Lösungen für zentrale Dienste aktivieren '
index: true
translation-type: tm+mt
source-git-commit: 3f26c1af19a0838913eec2b4135304f5f3fcf0b4
workflow-type: tm+mt
source-wordcount: '2362'
ht-degree: 97%

---


# Implementierung für Experience Cloud Services aktivieren

Wenn Sie kürzlich Experience Cloud mit Experience Platform Launch implementiert haben, sind Sie bereits für Kundenattribute und Experience Cloud-Audiences eingerichtet. Sie können auch Benutzer und Produkte in der Admin Console verwalten.

Für bestehende Kunden müssen Sie möglicherweise Ihre Lösungsimplementierungen modernisieren und Experience Cloud implementieren. Auf diese Weise können Sie Kundenattribute und Audience-Funktionen in Adobe Analytics, Audience Manager und Adobe Target nutzen. Dazu werden Sie:

1. [Experience Cloud beitreten und Administrator werden](#section_2423F0BD3DF642658103310EE5EA6154)
1. [Den Experience Cloud ID-Dienst implementieren](#section_3C9F6DF37C654D939625BB4D485E4354)
1. [Report Suites einer Experience Cloud-Organisation zuweisen](#section_7B08516B01BA421681DF03D0E86CE3BA)
1. [Den Analytics-AppMeasurement-Code aktualisieren](#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [Die Implementierung der Adobe Target aktualisieren](#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [Überprüfen der Implementierung](#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [Benutzer und Produkte verwalten](#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [Freigabe von Attributen und Zielgruppendaten beginnen](#section_960C06093623462E8EA247B3E97274A1)

## Schritt 1. Experience Cloud beitreten und Administrator werden {#section_2423F0BD3DF642658103310EE5EA6154}

Was müssen Sie tun, um dem Experience Cloud beizutreten?

![](assets/step1_icon.png) Stellen Sie sicher, dass Sie über gültige SKUs für Adobe Analytics oder Adobe Target verfügen.

* **Adobe Analytics:** Standard oder Premium (nicht die ältere [!DNL SiteCatalyst]-SKU).
* **Adobe Target:** Standard oder Premium.

>[!NOTE]
>
>Migrieren Sie für [!DNL Target] beispielsweise von [!DNL mbox.js] zu „at.js“. Siehe [Aktualisieren von at.js 1.x auf at.js 2.x](https://docs.adobe.com/content/help/de-DE/target/using/implement-target/client-side/upgrading-from-atjs-1x-to-atjs-20.html).

![](assets/step2_icon.png) Modernisieren Sie Ihre Implementierung und lassen Sie sich einen Administrator bereitstellen.

1. Führen Sie die Schritte unter [Bereitstellen des [!UICONTROL Experience Cloud ID-Dienstes]](../core-services/core-services.md#section_3C9F6DF37C654D939625BB4D485E4354) aus.
1. Wenden Sie sich an Ihren Kundenbetreuer und starten Sie den Bereitstellungsprozess für die Experience Cloud.

![](assets/step3_icon.png) Verwalten Sie Benutzer und Produkte in der [!UICONTROL Admin Console].

### Administratoranmeldung

Sobald Sie Administrator sind, können Sie sich unter [experiencecloud.adobe.com](https://experiencecloud.adobe.com) anmelden.

Im Experience Cloud-Navigationsmenü wird der Link **[!UICONTROL Administration]** angezeigt.

Weitere Informationen finden Sie unter [Experience Cloud – Benutzer und Produkte verwalten](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

### Benutzeranmeldung

Für die Anmeldung bei der Experience Cloud müssen Ihre Benutzer:

1. Eine Adobe ID (oder Enterprise ID für Ihr Unternehmen) haben.
1. Sich bei [experiencecloud.adobe.com](https://experiencecloud.adobe.com) anmelden.
1. Zu einer Lösungsgruppe gehören, die einer Unternehmensgruppe zugeordnet ist.
1. Verknüpfen Sie ggf. die Lösungskonten mit ihrer Adobe ID (Beschreibung unten).

![](assets/step4_icon.png) Optional: Verknüpfen Sie vorhandene Benutzerkonten.

Wahrscheinlich haben Sie Benutzer, die bereits Mitglied von Lösungsgruppen sind, z. B. eine Analytics-Gruppe, die Sie zuvor unter [!UICONTROL Analytics] > [!UICONTROL Admin Tools] verwaltet haben.

Wenn Sie diese Gruppen Experience Cloud-Unternehmensgruppen zuordnen, müssen diese Benutzer ihre Anmeldeinformationen für das Lösungskonto manuell mit ihrer Adobe ID verknüpfen.

Siehe [Verknüpfen von Konten in der Experience Cloud](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1)

>[!NOTE]
>
>Nach dem Mapping von Unternehmens- und Lösungsgruppen werden neue Benutzer automatisch verknüpft. (Lösungsanmeldeinformationen werden automatisch erstellt und mit ihrer Adobe ID verknüpft.)

In den folgenden Abschnitte wird die Modernisierung Ihrer Implementierung beschrieben. Durch die Modernisierung Ihrer Implementierung werden die zentralen Dienste in der Experience Cloud aktiviert.

## Schritt 2. Implementieren Sie den [!UICONTROL Experience Cloud ID-Dienst] mithilfe von [!UICONTROL Experience Platform Launch] oder des [!UICONTROL Dynamic Tag Managements] {#section_3C9F6DF37C654D939625BB4D485E4354}

Der [!UICONTROL Experience Cloud ID-Dienst] stellt eine allgemeine ID für lösungsübergreifende Integrationen bereit. Er bietet eine domänenübergreifende Besucheridentifikation und einen Pfad für geräte-/browserübergreifendes Targeting und die Personalisierung basierend auf CRM-Daten, die über [!UICONTROL Kundenattribute] hochgeladen wurden.

Die einfachste Methode zur Aktivierung der zentralen Experience Cloud-Dienste besteht darin, diese über die [Experience Cloud ID-Diensterweiterung](https://docs.adobe.com/content/help/en/launch/using/implement/solutions/idservice-save.html) in [!UICONTROL Experience Platform Launch] oder über das ECID-Tool im [!UICONTROL Dynamic Tag Management] automatisch für Analytics und Adobe Target zu aktivieren. (Experience Platform Launch wird dringend empfohlen.)

Die vollständige Hilfe zum Experience Cloud ID-Dienst (früher Besucher-ID) finden Sie [hier](https://docs.adobe.com/content/help/de-DE/id-service/using/home.html).

**Sie verwenden nicht [!UICONTROL Experience Platform Launch] oder [!UICONTROL Dynamic Tag Management]?**

Wenn Sie [!UICONTROL Experience Platform Launch] oder das [!UICONTROL Dynamic Tag Management] nicht verwenden, implementieren Sie den ID-Dienst über die JavaScript-Implementierung ([!DNL VisitorAPI.js]) wie folgt:

| Aufgabe | Beschreibung |
| -----------| ---------- |  
| [Implementieren des Experience Cloud ID-Dienstes für Analytics](https://docs.adobe.com/content/help/de-DE/id-service/using/implementation/setup-analytics.html) | Adobe empfiehlt auch, zusätzliche [Kunden-IDs](https://docs.adobe.com/content/help/de-DE/id-service/using/reference/authenticated-state.html) festzulegen. Diese IDs werden den einzelnen Besuchern zugeordnet und dienen der Aktivierung der aktuellen und zukünftigen Funktionen in Experience Cloud. |
| Aktualisieren Sie Ihre vorhandene [!DNL s_code] auf die Version H.27.3 oder höher, oder Ihre vorhandene [!DNL AppMeasurement.js] auf Version 1.4 oder höher. | Diese Dateien können im [Code-Manager](https://docs.adobe.com/content/help/de-DE/analytics/admin/admin-tools/code-manager-admin.html) in den Analytics Admin Tools heruntergeladen werden. (Das Handbuch für die [JavaScript-Implementierung](https://docs.adobe.com/content/help/de-DE/analytics/implementation/js/overview.html) ist verfügbar, wenn Sie weitere Informationen zu [!DNL AppMeasurement.js] benötigen.) |
| Synchronisieren der Kunden-ID für Analytics | Siehe [Analytics – Synchronisieren der Kunden-ID](../core-services/core-services.md#section_AD473A6A21C1446498E700363F9A8437) (unten). |

## Analytics und Adobe Target – Synchronisieren der Kunden-ID {#section_AD473A6A21C1446498E700363F9A8437}

Adobe empfiehlt im Zuge der Einrichtung des Experience Cloud ID-Dienstes für Analytics und [!DNL Target] die Synchronisierung Ihrer [Kunden-IDs](https://docs.adobe.com/content/help/de-DE/id-service/using/reference/authenticated-state.html) mit der Experience Cloud.

In Adobe Target muss `mbox3rdpartyid` die Kunden-ID abrufen und an [!DNL Target] senden. (Siehe [Arbeiten mit Kundenattributen](https://docs.adobe.com/content/help/de-DE/target/using/audiences/visitor-profiles/working-with-customer-attributes.html) in [!DNL Target].)

Wenn sich ein Besucher auf Ihrer Website authentifiziert oder sich auf andere Weise identifiziert, muss Ihre Implementierung die CRM-Kunden-ID dieser Person für die Seite oder App zur Verfügung stellen. Anschließend können Sie den entsprechenden Funktionsaufruf verwenden, um Ihre Kunden-ID mit der Experience Cloud zu synchronisieren. Durch diese Synchronisierung wird die CRM-Kunden-ID des Besuchers in der Experience Cloud gespeichert und die Attribute dieses Kunden werden für die Verwendung in der Experience Cloud aktiviert.

Beispiel: Bob hat in Ihrem CRM-System die Kunden-ID `52mc210tr42`. Wenn sich Bob bei Ihrer Site authentifiziert, müssen Sie diese ID auf der Seite bereitstellen und die ID zur Synchronisierung auf eine der beiden folgenden Arten verwenden:

* Aufruf von `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})` über den Besucher-ID-Dienst Oder
* Füllen Sie die *`Customer ID (52mc210tr42)`* in einer prop oder eVar.

Die Kunden-ID muss in jedem Aufruf an den [!DNL Analytics]-Server angegeben sein, auf dem die Kunden-ID bekannt ist.

### Mobile SDKs

Im Abschnitt zum *Experience Cloud ID-Dienst* finden Sie Syntaxbeispiele zum Festlegen zusätzlicher Kunden-IDs in [Android](https://docs.adobe.com/content/help/de-DE/mobile-services/android/overview.html)- und [iOS](https://docs.adobe.com/content/help/de-DE/mobile-services/ios/overview.html)-Apps.

### Aktivierung der Attribute historischer Daten

Kundenattributdaten werden nach der Anmeldung durch die Besucher bereitgestellt. Wenn Sie den neuesten Experience Cloud ID-Dienst noch nicht implementiert haben und Sie Kunden-IDs zuvor in einer prop oder eVar verfolgt haben, können Sie einen Prozess anfordern, der historische Anmeldungen an die Experience Cloud sendet. Auf diese Weise können Sie sofort mit der Verwendung von Kundenattributen beginnen.

Wenden Sie sich an die Kundenunterstützung, um historische Daten zu aktivieren.

## Schritt 3. Zuweisen von Report Suites zu einer Experience Cloud-Organisation {#section_7B08516B01BA421681DF03D0E86CE3BA}

Experience Cloud-Dienste (z. B. der Experience Cloud ID-Dienst und [!UICONTROL People-Dienst]) sind einer Experience Cloud-Organisation und keiner einzelnen Analytics Report Suite zugeordnet. Um sicherzustellen, dass diese Dienste ordnungsgemäß funktionieren, muss jede Analytics Report Suite einer Experience Cloud-Organisation zugeordnet werden.

Weitere Informationen dazu finden Sie unter [Report Suites einer Organisation zuweisen](report-suite-mapping.md).

## Schritt 4. (Adobe Analytics) Aktualisieren des Analytics-AppMeasurement-Codes {#section_1798D9D0F05C47E29816AC4EEB9A0913}

Vergewissern Sie sich, dass Sie die regionale Datenerfassung (RDC) verwenden. Wenn Ihre Datenerfassungsdomäne [!DNL omtrdc.net] lautet, oder wenn Ihr CNAME [!DNL omtrdc.net] zugeordnet ist, befinden Sie sich auf RDC. Weitere Informationen finden Sie unter [Übergang zu RDC](https://docs.adobe.com/content/help/de-DE/analytics/technotes/rdc/regional-data-collection.html). Wenn Sie Erstanbieter-Cookies verwenden, finden Sie unter [CNAME und Experience Cloud ID-Dienst](https://docs.adobe.com/content/help/de-DE/id-service/using/reference/analytics-reference/cname.html) Informationen zu CNAMES für die Datenerfassung und zur domänenübergreifenden Verfolgung.

Adobe empfiehlt eine Modernisierung Ihrer Analytics-Implementierung durch Aktualisierung Ihrer JavaScript-Bibliotheken einschließlich der Besucher-API. Am einfachsten erreichen Sie eine solche Modernisierung durch Hinzufügen des Tools [!DNL Adobe Analytics] im Dynamic Tag Management (DTM), das *`Automatic`* als Konfigurationsmethode angibt.

Klicken Sie unter [!UICONTROL Dynamic Tag Management] auf **`<Web Property Name>`** > **[!UICONTROL Übersicht]** > **[!UICONTROL Tool hinzufügen]** > **[!UICONTROL Adobe Analytics]**. Informationen zur Implementierung finden Sie unter [Adobe Analytics-Einstellungen](https://docs.adobe.com/content/help/de-DE/dtm/using/tools/analytics-dtm.html) im Dynamic Tag Management.

## Schritt 5. (Adobe Target) Aktualisieren der Adobe Target-Implementierung {#section_C2F4493C7A36406DAE2266B429A4BD24}

* Es wird empfohlen, eine [Adobe Target-Erweiterung](https://docs.adobe.com/content/help/de-DE/launch/using/extensions-ref/adobe-extension/targetv2-extension/adobe-target-extension-v2.html) in [!UICONTROL Experience Platform Launch] hinzuzufügen, damit der Bibliotheksabruf automatisch erfolgt. Sie können auch die [Experience Cloud ID-Diensterweiterung](https://docs.adobe.com/content/help/de-DE/launch/using/extensions-ref/adobe-extension/id-service-extension/overview.html) für Adobe Target (und andere Lösungen) mithilfe von [!UICONTROL Experience Platform Launch] einrichten. Die Aktualisierung des [!UICONTROL Experience Cloud ID-Dienstes] **ist erforderlich**, damit Adobe Target die zentralen Dienste verwenden kann. (Wenn Sie das [!UICONTROL Dynamic Tag Management] verwenden, fügen Sie ein [Adobe Target-Tool](https://docs.adobe.com/content/help/de-DE/dtm/using/tools/target.html) hinzu. Sie können auch das [!UICONTROL Dynamic Tag Management] verwenden, um den Experience Cloud ID-Dienst für Adobe Target bereitzustellen.)
* Wenn Sie [!UICONTROL Experience Platform Launch] oder das [!UICONTROL Dynamic Tag Management] nicht verwenden, [aktualisieren Sie Ihre mbox-Bibliothek](https://docs.adobe.com/content/help/de-DE/target/using/implement-target/client-side/mbox-implement/target-download-config-mbox.html) manuell.
* Fordern Sie Zugriff auf Adobe Analytics als Berichtsquelle für [!DNL Adobe Target] an. [!DNL Target]- und [!DNL Analytics]-Daten werden bei der Verarbeitung bei demselben Server-Aufruf zusammengeführt, damit Besucher lösungsübergreifend verknüpft werden. Siehe [Analytics für die Target-Implementierung](https://docs.adobe.com/content/help/de-DE/target/using/integrate/a4t/a4t.html).

   >[!IMPORTANT]
   >
   >Alle Analytics-Kunden sind bereits für zentrale Dienste wie Kundenattribute freigeschaltet. Wenn Sie kein Analytics-Kunde sind, wenden Sie sich an die Kundenunterstützung, um eine Freischaltung anzufordern.

## Schritt 6. Überprüfen der Implementierung {#section_E641782A0F4F44AF8C9C91216BE330D5}

Verwenden Sie den folgenden Prozess, um sicherzustellen, dass der Experience Cloud ID-Dienst auf Ihrer Site korrekt implementiert ist.

1. Löschen Sie die Cookies für Ihre Site, damit Sie die Anforderung an den Experience Cloud ID-Dienst sehen können (die Anforderung erfolgt beim ersten Besuch und danach etwa einmal pro Besucher und Woche).
1. Suchen Sie mit einem Paket-Sniffer oder dem Netzwerkbereich eines Webbrowser-Debuggers nach einer Anfrage für [!DNL dpm.demdex.net].
1. Überprüfen Sie, ob die Antwort `d_mid` und einen Wert enthält, z. B.: `_setMarketingCloudFields({"d_mid":"4235...`
1. Stellen Sie sicher, dass die Analytics-Anforderung den `mid`-Parameter enthält (die Experience Cloud ID). Während der Übergangsphase (sofern aktiviert) sollte auch ein `aid`-Parameter angezeigt werden (die Analytics-Besucher-ID).

Erwartete Antwort mit der Experience Cloud ID:

![](assets/mac_id_response.png)

Analytics-Bildanforderung mit der Experience Cloud ID (auch bekannt als `mid` oder _Besucher-ID_):

![](assets/mid.png)

Experience Cloud ID in der mbox-Anfrage:

![](assets/mbox_request.png)

### Was ist die Übergangsphase?

Nach der Bereitstellung des Experience Cloud ID-Dienstes erhalten neue Besucher vom Datenerfassungsserver keine Analytics Experience Cloud ID mehr. Wenn der Experience Cloud ID-Dienst für manche Bereiche der Site noch nicht implementiert wurde und Besucher diese Bereiche aufrufen, wird die Experience Cloud ID nicht erkannt und den Besuchern wird eine alte Analytics-Besucher-ID zugewiesen. Dies kann zu potenziellen Problemen führen, einschließlich doppelten Besuchen und falscher Zuordnung.

Wenn beispielsweise der Supportbereich Ihrer Site in einem separaten CMS verwaltet wird, haben Sie möglicherweise eine andere Analytics-JavaScript-Datei für diesen Bereich. Wenn Sie die Experience Cloud ID auf Ihrer Haupt-Site bereitstellen, bevor Sie den ID-Dienst auf der Support-Site bereitstellen, erhalten neue Besucher beim Besuch des Supportbereichs eine alte Analytics-ID. Besuche, die beide Sitebereiche umfassen, werden als unterschiedliche Besuche gemeldet.

Die Bereitstellung des Experience Cloud-ID-Diensts auf Sites, die mehrere JavaScript-Dateien oder andere Technologien (z. B. Flash) verwenden, kann Koordinierungsprobleme verursachen, da Sie den Experience Cloud-ID-Dienst auf allen Sitebereichen gleichzeitig aktivieren müssen. Mit der Konfiguration einer Übergangsphase wird neuen Besuchern vom ID-Dienst weiterhin eine Analytics-Besucher-ID zugewiesen, damit sie richtig in Sitebereichen identifiziert werden, die noch nicht auf den Besucher-ID-Dienst aktualisiert wurden.

## Schritt 7. Benutzer und Produkte verwalten {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Navigieren Sie nach der erfolgreichen Einrichtung zur [Admin Console](https://adminconsole.adobe.com/), wo Sie Benutzer und Produktprofile verwalten können.

![](assets/menu-administration-shell.png)

Siehe [Verwalten von Experience Cloud-Benutzern und -produkten](../admin-getting-started/admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

### Kundenattribute

Benutzer, die der Gruppe [!UICONTROL Kundenattribute] hinzugefügt wurden, sehen auf der linken Seite der Experience Cloud-Benutzeroberfläche das Menüelement [!UICONTROL Kundenattribute].

## Schritt 8. Freigabe von Attributen und Zielgruppendaten beginnen {#section_960C06093623462E8EA247B3E97274A1}

Nutzen Sie die Vorteile folgender Funktionen.

### [!UICONTROL Personen] > [!UICONTROL Kundenattribute]

Wenn Sie Daten von Unternehmenskunden in einer CRM-Datenbank (Customer Relationship Management) erfassen, können Sie diese Daten in eine Datenquelle für Kundenattribute in die Experience Cloud hochladen. Verarbeiten Sie die Daten nach dem Hochladen mit [!DNL Adobe Analytics] und [!DNL Adobe Target].

Weitere Informationen finden Sie unter [Kundenattribute](../attributes/attributes.md#concept_ACFEE7C8B8E94875BA0825CDF4913AF1)

### [!UICONTROL Personen] > [!UICONTROL Zielgruppenbibliothek]

In Experience Cloud-[!UICONTROL Zielgruppen] können Sie Zielgruppen erstellen, bereits vorhandene Zielgruppen zu einer gemeinsamen Zielgruppe zusammenfassen und alle freigegebenen Zielgruppen anzeigen.

Weitere Informationen finden Sie unter [Zielgruppen](../audience-library/audience-library.md#topic_679810123CAA4E0CA4FA3417FB0100C7)

## Datenspeicherung und Datenschutz

Wenn Sie Echtzeit-Zielgruppenprofile und andere Hauptdienste in der Adobe [!DNL Experience Cloud] nutzen, hat die Verwendung dieser Dienste Auswirkungen darauf, in welchem Datenzentrum (und Land) sich Ihre Daten befinden. Da die zentralen Dienste der Adobe [!DNL Experience Cloud] Adobe Audience Manager nutzen, müssen sich im [!UICONTROL People]-Dienst verwendete Daten auf Audience Manager-Servern in den USA befinden.

Wenn Sie zentrale Dienste nutzen, die über den [!UICONTROL People]-Dienst zur Verfügung gestellt werden, lauten von anderen Adobe-Produkten an das Zielgruppen-Management gesendeten Datentypen wie folgt:

* Schlüssel-/Werte-Paare aus [!DNL Analytics] (Eigenschaften, eVars, Listenvariablen usw.). Standardmäßig enthalten die Protokollzeilen die IP-Adresse, inklusive des letzten Oktetts der IP (vorausgesetzt, die IP-Adresse wurde nicht durch Einstellungen zur IP-Verschleierung innerhalb von Adobe [!DNL Analytics] verändert).
* Eigenschaften und Segmente, für die sich Besucher auf der Grundlage der in Audience Manager festgelegten Regeln qualifizieren.
* (Optional) Eine oder mehrere Ihrer IDs. Je nach Implementierung des ID-Dienstes senden Sie möglicherweise auch eine oder mehrere Ihrer IDs, z. B. CRM-IDs oder Hash-E-Mail-Adressen. Werden diese Daten an Adobe [!DNL Analytics] gesendet, werden sie an das Adobe Zielgruppen-Management übergeben. Adobe empfiehlt, keine personenbezogenen Daten in Adobe [!DNL Analytics] bereitzustellen. Verwenden Sie stattdessen einen unidirektionalen Hash, um die Daten zu maskieren, bevor sie an Adobe gesendet werden.
* Segmente aus [!DNL Analytics] über die Back-End-Funktion zur Segmentfreigabe
* Wenn Cookies von Drittanbietern nicht blockiert werden, wird das Cookie demdex.net gesetzt. Bei Verwendung des Experience Cloud ID-Dienstes wird das Erstanbieter-Cookie `AMCV_###@AdobeOrg` immer gesetzt.

Alle diese Datenelemente werden in Form von Protokolldateien an Adobe Audience Manager gesendet. Audience Manager verarbeitet und speichert diese Daten in den USA. Audience Manager bietet keine Option zum Speichern oder Verarbeiten dieser Daten außerhalb der USA.

### Cookies und Opt-Outs

Bei der Profilerstellung für Zielgruppen in Echtzeit wird neben den Cookies für [!DNL Analytics] und [!DNL Target] auch das Cookie von Audience Manager verwendet.

Wenn Sie eine geeignete Funktion zum Deaktivieren von Cookies bereitstellen möchten, müssen Besucher Ihrer Site diese Funktion aus Audience Manager zum vorhandenen Opt-out-Vorgang hinzufügen.

Anweisungen finden Sie unter [Adobe Experience Cloud – Implementieren von Adobe Opt-Outs](https://docs.adobe.com/content/help/de-DE/analytics/implementation/js/opt-out.html).

Informationen zum Aktivieren der domänenübergreifenden Verfolgung finden Sie unter [CNAMEs für die Datenerfassung und domänenübergreifende Verfolgung](https://docs.adobe.com/content/help/de-DE/id-service/using/reference/analytics-reference/cname.html).
