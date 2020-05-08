---
title: Kundenattributunterstützung für California Consumer Privacy Act
description: Kundenattributunterstützung für California Consumer Privacy Act
translation-type: tm+mt
source-git-commit: 2e8c8aee39546a345e72cda2dad08ad866cd90f9
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 4%

---


# Kundenattributunterstützung für California Consumer Privacy Act


>[!IMPORTANT]
>
>Der Inhalt dieses Dokuments ist keine Rechtsberatung und soll keine Rechtsberatung ersetzen. Wenden Sie sich an Ihren Rechtsbeistand, um Ratschläge zum California Consumer Privacy Act zu erhalten.

Das California Consumer Privacy Act (CCPA) ist das neue kalifornische Datenschutzgesetz, das am 1. Januar 2020 in Kraft tritt. Die CCPA räumt den Einwohnern Kaliforniens neue Rechte in Bezug auf ihre personenbezogenen Daten ein und erlegt bestimmten Personen, die in Kalifornien Geschäfte tätigen, Datenschutzpflichten auf. CCPA bietet Verbrauchern das Recht, auf ihre personenbezogenen Daten zuzugreifen und sie zu löschen sowie das Recht auf Opt-out bestimmter Aktivitäten, die als &quot;Verkauf&quot; personenbezogener Daten an Dritte gelten.

Als Unternehmen bestimmen Sie die personenbezogenen Daten, die Adobe Experience Cloud in Ihrem Namen verarbeitet und speichert.

Als Dienstleister unterstützt Adobe Experience Cloud Ihr Unternehmen bei der Erfüllung seiner Verpflichtungen aus dem CCPA, die für die Verwendung von Experience Cloud-Produkten und -Diensten gelten, einschließlich der Verwaltung von Anforderungen zum Zugriff auf und Löschen personenbezogener Daten.

In diesem Dokument wird beschrieben, wie Kundenattribute die CCPA-Datenzugriff- und Löschungsrechte der betroffenen Personen mithilfe der API des Adobe Experience Platform Privacy Service und der Benutzeroberfläche des Datenschutzdienstes unterstützen.

Weitere Informationen zu den Datenschutzdiensten von Adobe für CCPA finden Sie im [Adobe Privacy Center](https://www.adobe.com/privacy/ccpa.html).

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

* &quot;Regulierung&quot;: **ccpa** (die Datenschutzverordnung, die für die Anforderung gilt)

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
