---
title: Auswählen einer Datenerfassungs-Domain
description: Erfahren Sie mehr über die Domains, mit denen Sie Daten an Adobe senden können, und wie Sie die Mandanten-ID Ihres Unternehmens finden.
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
source-git-commit: e1185eeafc809b036b10955880536db7a576ca0b
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 3%
---
# Auswählen einer Datenerfassungsdomäne

Ihre Datenerfassungs-Domain ist der Host-Name, an den Ihre Implementierung Daten sendet. Alle Adobe CX Enterprise-Produkte, die die Adobe-Datenerfassung verwenden (z. B. Adobe Analytics, Customer Journey Analytics, Adobe Experience Platform, Adobe Target und Adobe Journey Optimizer), nutzen diese Domain.

## Optionen für Datenerfassungs-Domain

| Option | Implementierungs-Domain | Region-locked [RDC](rdc.md) | Zertifikatverwaltung |
| --- | --- | --- | --- |
| [Domain eines Drittanbieters](#third-party) | `example.data.adobedc.net` | Nicht unterstützt | Kein(e) |
| Erstanbieterdomäne mit einem von [Adobe verwalteten Zertifikat](adobe-managed-cert.md) | `data.example.com` | „Unterstützt“ | Keine (Adobe erneuert das Zertifikat automatisch) |
| Erstanbieterdomäne mit einem [vom Kunden verwalteten Zertifikat](customer-managed-cert.md) | `data.example.com` | „Unterstützt“ | Ihr Unternehmen erneuert das Zertifikat und stellt es Adobe zur Verfügung |
| [Content Delivery Network (CDN) mit Herkunft eines Drittanbieters](cdn.md#third-party-origin) | `data.example.com` | Nicht unterstützt | Kein(e) |
| [CDN mit First-Party-Herkunft](cdn.md#first-party-origin) | `data.example.com` | „Unterstützt“ | Ihr Unternehmen erneuert das Zertifikat und stellt es Adobe zur Verfügung |

## Datenerfassungs-Domain eines Drittanbieters {#third-party}

Wenn Sie keine Erstanbieter-Domain verwenden, senden Sie Daten an eine Subdomain von `data.adobedc.net`. Adobe empfiehlt, die (Mandanten[ID) Ihres Unternehmens &#x200B;](#tenant-id) Subdomain zu verwenden. Beispiel: `example.data.adobedc.net`. Diese Domain ist auch der empfohlene Ursprung, wenn Sie [Datenerfassung über ein CDN &#x200B;](cdn.md).

* Domänen von Drittanbietern verwenden immer den standardmäßigen [RDC-Typ](rdc.md#third-party-data-collection).
* Verwenden Sie keine Subdomains, die tiefer als `example.data.adobedc.net` liegen. `custom.example.data.adobedc.net` ist beispielsweise keine gültige Datenerfassungsdomäne.
* Bei älteren Implementierungen werden möglicherweise Domains wie `sc.omtrdc.net` oder `2o7.net` verwendet. Obwohl diese Domains immer noch gültig sind, empfiehlt Adobe, nach Möglichkeit `data.adobedc.net` zu verwenden.

### Mandanten-ID suchen {#tenant-id}

1. Melden Sie sich mit Ihren Adobe ID[&#128279;](https://experience.adobe.com)Anmeldeinformationen bei Adobe CX Enterprise an.
1. Drücken Sie an einer beliebigen Stelle in der CX Enterprise-Benutzeroberfläche `[Cmd]` + `[I]` (macOS) oder `[Ctrl]` + `[I]` (Windows).
1. Ein **[!UICONTROL User Data Debugger]** wird angezeigt. Wählen Sie die **[!UICONTROL Zugewiesene Organisationen]** aus.
1. Erweitern Sie die gewünschte IMS-Organisation.
1. Suchen Sie das Feld **[!UICONTROL Mandant]** . Dieser Wert ist Ihre Mandanten-ID.

Ihre Mandanten-ID unterscheidet sich von Ihrer IMS-Organisations-ID, die auf `@AdobeOrg` endet. Jede IMS-Organisation verfügt über eine Mandanten-ID. Wenn Ihr Unternehmen mehrere IMS-Organisationen verwendet, verfügt jede Organisation über eine eigene Mandanten-ID.

## Aktualisieren der Implementierung {#update-implementation}

Wenn Sie Ihre Datenerfassungs-Domain ändern, aktualisieren Sie jede Implementierung, die Daten an Adobe sendet:

* **Web-SDK-Tag** Erweiterung: Aktualisieren Sie das Feld [[!UICONTROL Edge]](https://experienceleague.adobe.com/de/docs/experience-platform/tags/extensions/client/web-sdk/configure/general)Domain“ beim Konfigurieren der Erweiterung.
* **Web SDK (Legierung)**: Aktualisieren Sie die [`edgeDomain`](https://experienceleague.adobe.com/de/docs/experience-platform/collection/js/commands/configure/edgedomain) Eigenschaft im `configure`.
* **Adobe Analytics-Erweiterung**: Aktualisieren Sie das Feld [[!UICONTROL SSL-Tracking]](https://experienceleague.adobe.com/de/docs/experience-platform/tags/extensions/client/analytics/overview)Server“, wenn Sie die Erweiterung konfigurieren. Stellen Sie sicher, dass Sie auch [&#x200B; Tag-Erweiterung „Visitor ID Service](https://experienceleague.adobe.com/de/docs/experience-platform/tags/extensions/client/id-service/overview) installiert haben. Weitere [&#x200B; finden Sie unter „Besucheridentifizierung mit der Tag](https://experienceleague.adobe.com/de/docs/analytics/implementation/id/analytics-extension)Erweiterung für Analytics“.
* **AppMeasurement**: Aktualisieren Sie die [`trackingServerSecure`](https://experienceleague.adobe.com/de/docs/analytics/implementation/vars/config-vars/trackingserversecure) Konfigurationsvariable. Stellen Sie sicher, dass Sie auch den [Besucher-ID-Service](https://experienceleague.adobe.com/de/docs/id-service/using/home) mit `VisitorAPI.js` implementiert haben. Weitere Informationen [&#x200B; Sie unter „Besucheridentifizierung mit &#x200B;](https://experienceleague.adobe.com/de/docs/analytics/implementation/id/appmeasurement)&quot;.
* **Andere Implementierungen**: Aktualisieren Sie die Datenerfassungs-Domain in jeder anderen Implementierung, die Daten an Adobe sendet, z. B. Mobile Apps oder serverseitige Implementierungen.

Wenn Ihre Implementierung weder den Besucher-ID-Service noch die Web-SDK verwendet, wird durch Ändern Ihrer Datenerfassungsdomäne die Domain der Besucher-Cookies geändert. Wiederkehrende Besucher können als neue Besucher gezählt werden.

Wenn Ihre Site mehrere Implementierungsmethoden verwendet und Sie nicht alle gleichzeitig aktualisieren können, sollten Sie eine Übergangsphase konfigurieren. Unter [Überlegungen zur Migration des Besucher-ID](https://experienceleague.adobe.com/de/docs/analytics/implementation/id/migration)Service finden Sie weitere Schritte, um zu verhindern, dass Besucher auf Ihrer Site als neue Besucher gezählt werden.
