---
title: Unterstützung von Kundenattributen für die allgemeine Datenschutzverordnung
description: Unterstützung von Kundenattributen für die allgemeine Datenschutzverordnung
translation-type: tm+mt
source-git-commit: 0bc7032d0052ba03beac1140dfbfd630e1802bfd
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 1%

---


# Unterstützung der Kundenattribute für die allgemeine Datenschutzverordnung

Auf dieser Seite wird beschrieben, wie Kundenattribute die Allgemeine Datenschutzverordnung (GDPR) unterstützen.

>[!IMPORTANT]
>
>Die Inhalte dieses Dokuments sind keine Rechtsberatung oder sollen Rechtsberatung ersetzen. Wenden Sie sich an Ihren Rechtsbeistand, um Beratung zu GDPR zu erhalten.

Die [Datenschutzverordnung](https://www.adobe.com/privacy/general-data-protection-regulation/what-is-gdpr.html), ein Gesetz vom 25. Mai 2018, gibt allen Personen (betroffenen Personen) die Kontrolle über ihre personenbezogenen Daten innerhalb der Grenzen der Europäischen Vereinigung (EU). Außerdem wird die regulatorische Umgebung für die internationale Wirtschaft vereinfacht. Dieses Gesetz gilt für alle Unternehmen (für die Verarbeitung von Daten verantwortliche Personen), die zum Zeitpunkt der Verarbeitung ihrer personenbezogenen Daten Waren oder Dienstleistungen an Personen innerhalb der Grenzen der Europäischen Union Angebot zur Überwachung des Verhaltens von Personen oder zur Erhebung personenbezogener Daten erbringen, unabhängig vom Standort des für die Verarbeitung Verantwortlichen.

Adobe Experience Cloud fungiert als Datenverarbeiter für alle persönlichen Daten, die es im Auftrag seiner Kunden empfängt und speichert. Als Datencontroller bestimmen Sie die personenbezogenen Daten, die Adobe Experience Cloud in Ihrem Namen verarbeitet und speichert.

In diesem Dokument wird beschrieben, wie [!UICONTROL Kundenattribute] die Zugriffsrechte auf und Löschung von GDPR-Daten Ihrer betroffenen Personen mithilfe der Adobe Experience Platform Privacy Service API und der Benutzeroberfläche des Datenschutzdienstes unterstützen.

Weitere Informationen darüber, was GDPR für Ihr Unternehmen bedeutet, finden Sie unter [GDPR und Ihr Geschäft](https://www.adobe.com/de/privacy/general-data-protection-regulation.html).

## Erforderliche Einrichtung zum Senden von Anforderungen für [!UICONTROL Kundenattribute]

Um Anforderungen zum Zugriff auf Daten zu [!UICONTROL Kundenattributen]und zum Löschen von Daten zu stellen, müssen Sie:

1. Identifizieren Sie Folgendes:

   * Kennung der IMS-Organisation
   * Alias-ID der CRS-Datenquelle, auf die Sie reagieren möchten
   * CRM-ID des Profils, auf das Sie reagieren möchten
   Eine IMS-Organisations-ID ist eine 24-stellige alphanumerische Zeichenfolge, die an @AdobeOrg angehängt wird. Wenn Ihr Marketingteam oder Ihr interner Adobe-Systemadministrator die IMS-Organisations-ID Ihres Unternehmens nicht kennen, wenden Sie sich an den Adobe-Kundendienst unter gdprsupport@adobe.com. Sie benötigen die IMS-Organisations-ID, um Anfragen an die Datenschutz-API zu senden.

1. Im [!UICONTROL Datenschutzdienst]können Sie Anforderungen zum Zugriff und Löschen an Kundenattribute senden und den Status vorhandener Anforderungen prüfen.

## Erforderliche Feldwerte in JSON-Anforderungen für [!UICONTROL Kundenattribute]

&quot;Kontext der Firma&quot;:

* &quot;Namensraum&quot;: **imsOrgID**
* &quot;value&quot;: &lt;*IMS-Organisations-ID-Wert*>

&quot;Benutzer&quot;:

* &quot;key&quot;: &lt;*gewöhnlich der Name des Kunden*>

* &quot;Aktion&quot;: entweder **Zugriff** oder **Löschen**

* &quot;Benutzer-IDs&quot;:

   * &quot;Namensraum&quot;: &lt;*Alias-ID der CRS-Datenquelle*>

   * &quot;type&quot;: **integrationCode**

   * &quot;value&quot;: &lt;*CRM-ID*>

* &quot;include&quot;: **CRS** (das Adobe-Produkt, das für die Anforderung gilt)

* &quot;Regulierung&quot;: **gdpr** (die Datenschutzverordnung, die für die Anforderung gilt)

## Beispiel für eine JSON-Anforderung

```
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "<IMS_ORG_ID>"
    }
  ],
  "users": [
    {
      "key": "<KEY>",
      "action": [
        "<access/delete>"
      ],
      "userIDs": [
        {
          "namespace": "<Alias ID of CRS Data Source>",
          "type": "integrationCode",
          "value": "<CRM ID>"
        }
      ]
    }
  ],
  "regulation": "<gdpr/ccpa/pdpa>",
  "include": [
    "CRS"
  ]
}
```

## Für Zugriffsanfragen zurückgegebene Datenfelder

```
attributes:
{
"value”:<*value*>,
"key”:<*key*>,
"displayName”:<*displayName*>
}
```
