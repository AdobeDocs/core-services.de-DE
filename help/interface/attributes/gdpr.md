---
title: Unterstützung von Kundenattributen für die allgemeine Datenschutzverordnung
description: Unterstützung von Kundenattributen für die allgemeine Datenschutzverordnung
translation-type: tm+mt
source-git-commit: 3a86aed0794c3e35cc028e5bfde5dafcb2285fc8
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 5%

---


# Unterstützung von Kundenattributen für die allgemeine Datenschutzverordnung


>[!IMPORTANT]
>
>Der Inhalt dieses Dokuments ist keine Rechtsberatung und soll keine Rechtsberatung ersetzen. Wenden Sie sich an Ihren Rechtsbeistand, um Beratung zur allgemeinen Datenschutzverordnung zu erhalten.

Die am 25. Mai 2018 in Kraft getretene [Datenschutzverordnung](https://www.adobe.com/privacy/general-data-protection-regulation/what-is-gdpr.html) (GDPR) sieht vor, dass alle Personen (betroffene Personen) ihre personenbezogenen Daten innerhalb der Grenzen der Europäischen Vereinigung (EU) kontrollieren, und vereinfacht die Umgebung der Vorschriften für den internationalen Geschäftsverkehr. Dieses Gesetz gilt für alle Unternehmen (für die Verarbeitung von Daten verantwortliche Personen), die zum Zeitpunkt der Verarbeitung ihrer personenbezogenen Daten Waren oder Dienstleistungen an Personen innerhalb der Grenzen der Europäischen Union Angebot zur Überwachung des Verhaltens von Personen oder zur Erhebung personenbezogener Daten erbringen, unabhängig vom Standort des für die Verarbeitung Verantwortlichen.

Adobe Experience Cloud fungiert als Datenverarbeiter für alle persönlichen Daten, die es im Auftrag seiner Kunden empfängt und speichert. Als Datencontroller bestimmen Sie die personenbezogenen Daten, die Adobe Experience Cloud in Ihrem Namen verarbeitet und speichert.

In diesem Dokument wird beschrieben, wie Kundenattribute mithilfe der API und der Benutzeroberfläche des Datenschutzdienstes für Adobe Experience Platform die GDPR-Datenzugriff- und Löschungsrechte der betroffenen Personen unterstützen.

Weitere Informationen darüber, was GDPR für Ihr Unternehmen bedeutet, finden Sie unter [GDPR und Ihr Geschäft](https://www.adobe.com/de/privacy/general-data-protection-regulation.html).

## Erforderliche Einrichtung zum Senden von Anfragen für Kundenattribute

Um Anforderungen zum Zugriff auf Daten zu Kundenattributen und zum Löschen von Daten zu stellen, müssen Sie:

1. Identifizieren Sie Folgendes:

* Kennung der IMS-Organisation
* Alias-ID der CRS-Datenquelle, auf die Sie reagieren möchten
* CRM-ID des Profils, auf das Sie reagieren möchten

Eine IMS-Organisations-ID ist eine 24-stellige alphanumerische Zeichenfolge, die an @AdobeOrg angehängt wird. Wenn Ihr Marketingteam oder Ihr interner Adobe-Systemadministrator die IMS-Organisations-ID Ihres Unternehmens nicht kennen, wenden Sie sich an den Adobe-Kundendienst unter gdprsupport@adobe.com. Sie benötigen die IMS-Organisations-ID, um Anfragen an die Datenschutz-API zu senden.

2. Verwenden Sie die Benutzeroberfläche des Datenschutzdienstes, um Anforderungen an Kundenattribute zu senden und zu löschen und den Status vorhandener Anforderungen zu überprüfen.

## Erforderliche Feldwerte in JSON-Anforderungen zu Kundenattributen

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

## Für Zugriffsanforderungen zurückgegebene Datenfelder

```
attributes:
{
"value”:<*value*>,
"key”:<*key*>,
"displayName”:<*displayName*>
}
```
