---
description: Modernisieren Sie Ihre Adobe Analytics- und Adobe Target-Programme für programmübergreifende Services. Erfahren Sie, wie Sie CX Enterprise Services verwenden.
solution: Experience Cloud
title: Erste Schritte mit Experience Cloud Services
index: true
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
hide: true
hidefromtoc: true
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: '2092'
ht-degree: 46%

---

# Erste Schritte mit CX Enterprise-Services

Wenn Sie kürzlich CX Enterprise mit Experience Platform-Tags implementiert haben, sind Sie bereits für Kundenattribute und CX Enterprise-Zielgruppen eingerichtet. Sie können auch Benutzende und Produkte in der Admin Console verwalten.

Bestehende Kunden können ihre Anwendungsimplementierungen modernisieren und CX Enterprise implementieren. Auf diese Weise können Sie Kundenattribute und Zielgruppenfunktionen in Adobe Analytics, Audience Manager und Adobe Target verwenden.

## Werden Sie Administrator bei CX Enterprise {#section_2423F0BD3DF642658103310EE5EA6154}

Was Sie tun müssen, um CX Enterprise beizutreten:

1. Stellen Sie sicher, dass Sie über gültige SKUs für Adobe Analytics oder Adobe Target verfügen.

   * **Adobe Analytics:** Standard oder Premium (nicht die ältere [!DNL SiteCatalyst]-SKU).
   * **Adobe Target:** Standard oder Premium.

   >[!NOTE]
   >
   >Migrieren Sie für [!DNL Target] beispielsweise von `mbox.js` zu „at.js“. Siehe [Aktualisieren von at.js 1. x zu at.js 2. x](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/upgrading-from-atjs-1x-to-atjs-20.html?lang=de).

1. Verwalten Sie Benutzer und Produkte in der [!UICONTROL Admin Console].

### Administrator-Anmeldung

Sobald Sie Administrator sind, können Sie sich unter [experience.adobe.com](https://experience.adobe.com) anmelden.

Der **[!UICONTROL Admin Console]** Link ist in der Menünavigation von CX Enterprise verfügbar.

### Benutzeranmeldung

Um sich bei CX Enterprise anzumelden, müssen Ihre Benutzer:

* Eine Adobe ID (oder Enterprise ID für Ihr Unternehmen) haben.
* Sich bei [experience.adobe.com](https://experience.adobe.com) anmelden.
* Zu einer Programmgruppe gehören, die einer Unternehmensgruppe zugeordnet ist.
* Verknüpfen Sie ggf. die Programmkonten mit ihrer Adobe ID (Beschreibung unten).

### Optional: Verknüpfen Sie vorhandene Benutzerkonten.

Wahrscheinlich haben Sie Benutzer, die bereits Mitglied von Programmgruppen sind, z. B. einer Analytics-Gruppe, die Sie zuvor über [!UICONTROL Analytics] > [!UICONTROL Admin Tools] verwaltet haben.

Wenn Sie diese Gruppen CX Enterprise-Gruppen zuordnen, müssen diese Benutzer ihre Anmeldeinformationen für das Programmkonto manuell mit ihrer Adobe ID verknüpfen.

Siehe [Verknüpfen von Konten in CX Enterprise](../administration/organizations.md)

>[!NOTE]
>
>Nach dem Zuordnen von Unternehmens- und Programmgruppen werden neue Benutzer automatisch verknüpft. (Lösungsanmeldedaten werden automatisch erstellt und mit ihrer Adobe ID verknüpft.)

In den folgenden Abschnitte wird die Modernisierung Ihrer Implementierung beschrieben. Die Modernisierung Ihrer Implementierung ermöglicht zentrale Services in CX Enterprise.

## Implementieren des [!UICONTROL CX Enterprise ID Service] {#section_3C9F6DF37C654D939625BB4D485E4354}

Die [!UICONTROL CX Enterprise ID Service] bietet eine gemeinsame ID für programmübergreifende Integrationen. Es bietet eine Domain-übergreifende Besucheridentifikation und einen Pfad für Geräte-/Browser-übergreifendes Targeting und die Personalisierung basierend auf CRM-Daten, die über [!DNL Customer Attributes] hochgeladen wurden.

Die einfachste Methode zur Aktivierung der CX Enterprise Core Services besteht darin, sie automatisch für Analytics und Adobe Target über die [CX Enterprise ID Service-Erweiterung](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/id-service/overview.html) in [!UICONTROL Experience Platform Launch] zu aktivieren.

Die vollständige Hilfe zum CX Enterprise ID Service (früher Besucher-ID) finden Sie [hier](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html#intro).

**Verwendet [!UICONTROL Experience Platform tags] nicht?**

Wenn Sie [!UICONTROL Experience Platform tags] nicht verwenden, implementieren Sie den ID-Service manuell über die JavaScript-Bereitstellung (`VisitorAPI.js`) wie folgt:

| Aufgabe | Beschreibung |
| -----------| ---------- |
| [Implementieren des CX Enterprise ID-Service für Analytics](https://experienceleague.adobe.com/docs/id-service/using/implementation/setup-analytics.html) | Adobe empfiehlt auch, zusätzliche [Kunden-IDs](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html) festzulegen. Diese IDs sind mit jedem Besucher verknüpft und ermöglichen aktuelle und zukünftige Funktionen in CX Enterprise. |
| Aktualisieren Sie Ihre vorhandene `s_code` auf die Version H.27.3 oder höher, oder Ihre vorhandene `AppMeasurement.js` auf Version 1.4 oder höher. | Diese Dateien können im [Code-Manager](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/code-manager-admin.html) in den Analytics Admin Tools heruntergeladen werden. (Das Handbuch für die [JavaScript-Implementierung](https://experienceleague.adobe.com/docs/analytics/implementation/js/overview.html#js) ist verfügbar, wenn Sie weitere Informationen zu `AppMeasurement.js` benötigen.) |

{style="table-layout:auto"}

### Analytics und Adobe Target – Synchronisieren der Kunden-ID {#section_AD473A6A21C1446498E700363F9A8437}

Adobe empfiehlt im Rahmen der Einrichtung des CX Enterprise ID-Service für Analytics und [!DNL Target] die Synchronisierung Ihrer [Kunden-IDs](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html) mit dem CX Enterprise.

In Adobe Target muss `mbox3rdpartyid` die Kunden-ID abrufen und an [!DNL Target] senden. (Siehe [Arbeiten mit Kundenattributen](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/working-with-customer-attributes.html?lang=de) in [!DNL Target].)

Wenn sich ein Besucher auf Ihrer Website authentifiziert oder sich auf andere Weise identifiziert, muss Ihre Implementierung die CRM-Kunden-ID dieser Person für die Seite oder App zur Verfügung stellen. Anschließend können Sie den entsprechenden Funktionsaufruf verwenden, um Ihre Kunden-ID mit CX Enterprise zu synchronisieren. Diese Synchronisierung speichert die CRM-Kunden-ID des Besuchers in CX Enterprise und aktiviert die Attribute dieses Kunden für die Verwendung in CX Enterprise.

Beispiel: Bob hat in Ihrem CRM-System die Kunden-ID `52mc210tr42`. Wenn sich Bob bei Ihrer Site authentifiziert, müssen Sie diese ID auf der Seite bereitstellen und die ID zur Synchronisierung auf eine der beiden folgenden Arten verwenden:

* Aufruf von `visitor.setCustomerIDs({"crm_id":"52mc210tr42"})` über den Besucher-ID-Dienst Oder
* Füllen Sie die *`Customer ID (52mc210tr42)`* in einer prop oder eVar.

Die Kunden-ID muss in jedem Aufruf an den [!DNL Analytics]-Server angegeben sein, auf dem die Kunden-ID bekannt ist.

#### Analytics: Synchronisieren der Kunden-ID mit der Data Warehouse-Aufstockungsmethode

Als Kundenattribute erstmals verfügbar wurden, hatten einige Kunden den CX Enterprise ID-Service noch nicht implementiert und konnten Kundenattribute nicht einfach nutzen. Um dieses Problem zu beheben, hat Adobe eine Möglichkeit zur Aufstockung von ID-Synchronisierungen mithilfe von Adobe Analytics Data Warehouse geschaffen. Diese Funktion wird als Data Warehouse-Aufstockung bezeichnet. Die Data Warehouse-Aufstockung ist jetzt im Allgemeinen nicht mehr erforderlich und ist daher seit Oktober 2022 nicht mehr verfügbar.


### Mobile SDKs

Im Abschnitt *CX Enterprise ID Service* finden Sie Syntaxbeispiele zum Festlegen zusätzlicher Kunden-IDs in [Android™](https://experienceleague.adobe.com/docs/mobile-services/android/overview.html?lang=de) und [iOS](https://experienceleague.adobe.com/docs/mobile-services/ios/overview.html?lang=de) Mobile Apps.

### Aktivieren von Attributen für historische Daten

Kundenattributdaten werden nach der Anmeldung durch die Besucher bereitgestellt. Wenn Sie den ID-Service noch nicht implementiert haben und Sie Kunden-IDs zuvor in einer Prop oder eVar verfolgt haben, können Sie einen Prozess anfordern, der historische Anmeldungen an CX Enterprise sendet. Auf diese Weise können Sie sofort mit der Verwendung von Kundenattributen beginnen.

Wenden Sie sich an die Kundenunterstützung, um historische Daten zu aktivieren.

## Report Suites einer CX Enterprise-Organisation zuordnen {#section_7B08516B01BA421681DF03D0E86CE3BA}

>[!NOTE]
>
>Die Funktion für die Report Suite-Zuweisung wurde im November 2020 eingestellt. Wenden Sie sich bei Fragen an den Support.

CX Enterprise-Services (z. B. CX Enterprise ID-Service) sind mit einer CX Enterprise-Organisation anstatt mit einer einzelnen Analytics-Report Suite verknüpft. Um sicherzustellen, dass diese Services ordnungsgemäß funktionieren, muss jede Analytics-Report Suite einer CX Enterprise-Organisation zugeordnet werden.

## Den Analytics-AppMeasurement-Code aktualisieren {#section_1798D9D0F05C47E29816AC4EEB9A0913}

Wenn Sie Erstanbieter-Cookies verwenden, finden Sie unter [CNAME und der CX Enterprise ID-Service](https://experienceleague.adobe.com/docs/id-service/using/reference/analytics-reference/cname.html?lang=de) Informationen zu CNAMEs für die Datenerfassung und zur domänenübergreifenden Verfolgung.

Adobe empfiehlt eine Modernisierung Ihrer Analytics-Implementierung durch Aktualisierung Ihrer JavaScript-Bibliotheken einschließlich der Besucher-API. Eine einfache Möglichkeit, dies zu erreichen, besteht darin, eine [Adobe Analytics-Erweiterung](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/analytics/overview.html) in der Experience Platform-Datenerfassung hinzuzufügen.

## Aktualisieren der Implementierung von Adobe Target {#section_C2F4493C7A36406DAE2266B429A4BD24}

* Es wird empfohlen, eine [Adobe Target-Erweiterung](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/target-v2/overview.html) in [!UICONTROL Experience Platform] Tags hinzuzufügen, damit der Bibliotheksabruf automatisch erfolgt. Sie können auch die [CX Enterprise ID Service-Erweiterung](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/adobe/id-service/overview.html) für Adobe Target (und andere Programme) mithilfe von [!UICONTROL Experience Platform] Tags einrichten. Die [!UICONTROL CX Enterprise ID Service] Aktualisierung **ist erforderlich** damit Adobe Target die People -Services verwenden kann.
* Wenn Sie keine [!UICONTROL Experience Platform] Tags verwenden, [&#x200B; Sie Ihre mbox-Bibliothek &#x200B;](https://experienceleague.adobe.com/docs/target/using/implement-target/client-side/implement-target-for-client-side-web.html).
* Fordern Sie Zugriff auf Adobe Analytics als Berichtsquelle für [!DNL Adobe Target] an. Daten von [!DNL Target] und [!DNL Analytics] werden während der Verarbeitung bei demselben Server-Aufruf zusammengeführt, damit Besucher programmübergreifend verknüpft werden. Siehe [Analytics for Target-Implementierung](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html).

  >[!IMPORTANT]
  >
  >Alle Analytics-Kunden sind bereits für zentrale Dienste wie Kundenattribute freigeschaltet. Wenn Sie kein Analytics-Kunde sind, wenden Sie sich an die Kundenunterstützung, um eine Freischaltung anzufordern.

## Überprüfen der Implementierung {#section_E641782A0F4F44AF8C9C91216BE330D5}

Verwenden Sie den folgenden Prozess, um sicherzustellen, dass der CX Enterprise ID-Service auf Ihrer Site korrekt implementiert ist.

1. Löschen Sie die Cookies für Ihre Site, damit Sie die Anfrage an den CX Enterprise ID-Service sehen können (die Anfrage erfolgt beim ersten Besuch und dann einmal pro Besucher und Woche).
1. Suchen Sie mit einem Paket-Sniffer oder dem Netzwerkbereich eines Webbrowser-Debuggers nach einer Anfrage für [!DNL dpm.demdex.net].
1. Überprüfen Sie, ob die Antwort `d_mid` und einen Wert enthält, z. B.: `_setMarketingCloudFields({"d_mid":"4235...`
1. Stellen Sie sicher, dass die Analytics-Anfrage den `mid` (die CX Enterprise ID) enthält. Während der Übergangsphase (sofern aktiviert) sollte auch ein `aid`-Parameter angezeigt werden (die Analytics-Besucher-ID).

Erwartete Antwort, die den CX Enterprise ID enthält:

![Erwartete Antwort mit CX Enterprise ID](../assets/mac_id_response.png)

Analytics-Bildanforderung mit enthaltener CX Enterprise ID (auch bekannt als `mid` oder _Besucher-ID_):

![Analytics-Bildanforderung mit CX Enterprise ID](../assets/mid.png)

CX Enterprise ID in der Mbox-Anfrage:

![CX Enterprise ID in der Mbox-Anfrage](../assets/mbox_request.png)

### Was ist die Übergangsphase?

Nach der Bereitstellung des CX Enterprise ID-Services erhalten neue Besucher keine Analytics CX Enterprise ID mehr von Ihrem Datenerfassungsserver. Wenn auf Ihrer Site für Bereiche der ID-Service noch nicht implementiert wurde und Besucher diese Bereiche aufrufen, wird die CX Enterprise ID nicht erkannt und den Besuchern wird eine alte Analytics-Besucher-ID zugewiesen. Dies kann zu potenziellen Problemen führen, einschließlich doppelten Besuchen und falscher Zuordnung.

Wenn beispielsweise der Supportbereich Ihrer Site in einem separaten CMS verwaltet wird, haben Sie möglicherweise eine andere Analytics-JavaScript-Datei für diesen Bereich. Wenn Sie CX Enterprise ID auf Ihrer Haupt-Site bereitstellen, bevor Sie den ID-Service auf der Support-Site bereitstellen, erhalten neue Besucher beim Besuch des Support-Abschnitts eine alte Analytics-ID. Besuche, die beide Site-Bereiche umfassen, werden als unterschiedliche Besuche gemeldet.

Die Bereitstellung des CX Enterprise ID-Service auf Sites, die mehrere JavaScript-Dateien oder andere Technologien (z. B. Flash) verwenden, kann Koordinierungsprobleme verursachen. Diese Probleme treten auf, da Sie den CX Enterprise ID-Service für alle Teile Ihrer Site gleichzeitig aktivieren müssen. Durch das Konfigurieren einer Übergangsphase können neue Besucher weiterhin eine Analytics-Besucher-ID vom ID-Service erhalten. Besucher können konsistent in Bereichen Ihrer Site identifiziert werden, die nicht für die Verwendung des Besucher-ID-Service aktualisiert wurden.

## Benutzer und Produkte verwalten {#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF}

Navigieren Sie nach der erfolgreichen Einrichtung zu [Admin Console](https://adminconsole.adobe.com/), wo Sie Benutzer und Produktprofile verwalten können.

![Zugriff auf Admin Console](../assets/menu-administration-shell.png)

### Kundenattribute

Benutzer, die der [!DNL Customer Attributes] hinzugefügt wurden, sehen auf der linken Seite von CX Enterprise das [!DNL Customer Attributes].

## Freigabe von Attributen und Zielgruppendaten beginnen {#section_960C06093623462E8EA247B3E97274A1}

Nutzen Sie die Vorteile folgender Funktionen.

### [!UICONTROL Customer Attributes]

Wenn Sie Unternehmens-Kundendaten in einer CRM-Datenbank (Customer Relationship Management) erfassen, können Sie diese Daten in eine Datenquelle für Kundenattribute in CX Enterprise hochladen. Verarbeiten Sie die Daten nach dem Hochladen mit [!DNL Adobe Analytics] und [!DNL Adobe Target].

Weitere Informationen finden [&#x200B; unter &#x200B;](customer-attributes/attributes.md)Kundenattribute“.

### [!UICONTROL People] > [!UICONTROL Audience Library]

CX Enterprise [!UICONTROL Audiences] ist die Benutzeroberfläche, über die Sie Zielgruppen erstellen, vorhandene Zielgruppen kombinieren können, um zusammengesetzte Zielgruppen zu erstellen, und alle freigegebenen Zielgruppen anzeigen können.

Weitere Informationen finden [&#x200B; unter &#x200B;](audiences/overview.md)Zielgruppen“.

## Datenspeicherung und Datenschutz

Wenn Sie die Profilerstellung für Zielgruppen in Echtzeit und andere zentrale Services in der Adobe [!DNL CX Enterprise] nutzen, kann die Verwendung dieser Dienste Auswirkungen darauf haben, in welchem Datenzentrum (und Land) sich Ihre Daten befinden. Da [!DNL CX Enterprise] Audience Manager verwendet, müssen sich im [!UICONTROL People]-Service verwendete Daten auf Audience Manager-Servern in den USA befinden.

Wenn Sie Services verwenden, die über den [!UICONTROL People]-Service zur Verfügung gestellt werden, lauten von anderen Adobe-Produkten an das Zielgruppen-Management gesendeten Datentypen wie folgt:

* Schlüssel-/Werte-Paare aus [!DNL Analytics] (Eigenschaften, eVars, Listenvariablen usw.). Standardmäßig enthalten die Protokollzeilen die IP-Adresse, inklusive des letzten Oktetts der IP (vorausgesetzt, die IP-Adresse wurde nicht durch Einstellungen zur IP-Verschleierung innerhalb von Adobe [!DNL Analytics] verändert).
* Merkmale und Segmente, für die sich Besucher auf der Grundlage der in Audience Manager festgelegten Regeln qualifizieren.
* (Optional) Eine oder mehrere Ihrer IDs. Je nach Implementierung des ID-Dienstes senden Sie möglicherweise auch eine oder mehrere Ihrer IDs, z. B. CRM-IDs oder Hash-E-Mail-Adressen. Werden diese Daten an Adobe [!DNL Analytics] gesendet, werden sie an das Adobe Zielgruppen-Management übergeben. Adobe empfiehlt, keine personenbezogenen Daten in Adobe [!DNL Analytics] bereitzustellen. Verwenden Sie stattdessen einen unidirektionalen Hash, um die Daten zu maskieren, bevor sie an Adobe gesendet werden.
* Segmente aus [!DNL Analytics] über die Back-End-Funktion zur Segmentfreigabe.
* Wenn Cookies von Drittanbietern nicht blockiert werden, wird das Cookie demdex.net gesetzt. Das `AMCV_###@AdobeOrg` Erstanbieter-Cookie wird immer mit dem CX Enterprise ID-Service festgelegt.

Alle diese Datenelemente werden in Form von Protokolldateien an Adobe Audience Manager gesendet. Audience Manager verarbeitet und speichert diese Daten in den USA. Audience Manager bietet keine Option zum Speichern oder Verarbeiten dieser Daten außerhalb der USA.
