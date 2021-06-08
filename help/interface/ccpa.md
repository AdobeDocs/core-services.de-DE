---
title: 'Unterstützung von Kundenattributen für den California Consumer Privacy Act '
description: Mehr über die Unterstützung von Kundenattributen für den California Consumer Privacy Act erfahren
feature: 'Kundenattribute '
topic: Administration
role: Administrator
level: Experienced
exl-id: 320defc7-2cd5-4481-955d-77cf6fbfef6d
source-git-commit: 40fd81f8a293dc5bca3b41e8f6e708d1be4bae5d
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 66%

---

# Unterstützung von Kundenattributen für den California Consumer Privacy Act

Auf dieser Seite wird die Unterstützung von [!UICONTROL Kundenattributen] für den California Consumer Privacy Act (CCPA) beschrieben.

>[!IMPORTANT]
>
>Der Inhalt dieses Dokuments ist keine Rechtsberatung und soll keine Rechtsberatung ersetzen. Wenden Sie sich an Ihren Rechtsbeistand, um Beratung zum CCPA zu erhalten.

Der CCPA ist das neue kalifornische Datenschutzgesetz, das am 1. Januar 2020 in Kraft tritt. Der CCPA räumt den Einwohnern Kaliforniens neue Rechte in Bezug auf ihre personenbezogenen Daten ein und erlegt Rechtspersönlichkeiten, die in Kalifornien Geschäfte tätigen, Datenschutzpflichten auf. Der CCPA bietet Verbrauchern das Recht, auf ihre personenbezogenen Daten zuzugreifen und diese zu löschen, sowie das Recht, bestimmte Aktivitäten, die als &quot;Verkauf&quot;personenbezogener Daten an Dritte gelten, abzuwählen.

Als Unternehmen legen Sie fest, welche personenbezogenen Daten Adobe Experience Cloud in Ihrem Namen verarbeitet und speichert.

Als Ihr Dienstleister unterstützt Adobe Experience Cloud Ihr Unternehmen bei der Erfüllung seiner CCPA-Verpflichtungen, die für die Verwendung von Experience Cloud-Produkten und -Dienstleistungen gelten. Diese Unterstützung umfasst die Verwaltung von Anfragen zum Zugriff auf und zur Löschung personenbezogener Daten.

In diesem Dokument wird beschrieben, wie [!UICONTROL Kundenattribute] die CCPA-Datenzugriffs- und -Löschungsrechte der betroffenen Personen mithilfe der Adobe Experience Platform Privacy Service-API und der Privacy Service-Benutzeroberfläche unterstützt.

Weitere Informationen zu den Datenschutzdiensten von Adobe für den CCPA finden Sie im [Adobe Privacy Center](https://www.adobe.com/privacy/ccpa.html).

## Erforderliche Einrichtung zum Senden von Anfragen für [!UICONTROL Kundenattribute]

Um Anfragen zum Zugreifen auf und Löschen von Daten für [!UICONTROL Kundenattribute] zu stellen, müssen Sie:

1. Sie benötigen:

   * Kennung der IMS-Organisation
   * Alias-ID der jeweiligen CRS-Datenquelle
   * CRM-ID des jeweiligen Profils

   Eine IMS-Organisations-ID ist eine 24-stellige alphanumerische Zeichenfolge, die an @AdobeOrg angehängt wird. Wenn Ihr Marketing-Team oder Ihr interner Adobe-Systemadministrator die IMS-Organisations-ID Ihres Unternehmens nicht kennen, wenden Sie sich an die Adobe-Kundenunterstützung unter gdprsupport@adobe.com. Sie benötigen die IMS-Organisations-ID, um Anfragen an die Datenschutz-API zu senden.

1. In [!UICONTROL Privacy Service] können Sie Zugriffs- und Löschanfragen an Kundenattribute senden und den Status vorhandener Anfragen überprüfen.

## Erforderliche Feldwerte in JSON-Anfragen für [!UICONTROL Kundenattribute]

&quot;company context&quot;:

* &quot;namespace&quot;: **imsOrgID**
* &quot;value&quot;: &lt;*IMS-Organisations-ID-Wert*>

&quot;users&quot;:

* &quot;key&quot;: &lt;*gewöhnlich der Name des Kunden*>

* &quot;action&quot;: entweder **Zugriff** (access) oder **Löschen** (delete)

* &quot;user IDs&quot;:

   * &quot;namespace&quot;: &lt;*Alias-ID der CRS-Datenquelle*>

   * &quot;type&quot;: **integrationCode**

   * &quot;value&quot;: &lt;*CRM-ID*>

* &quot;include&quot;: **CRS** (das Adobe-Produkt, auf das sich die Anfrage bezieht)

* &quot;regulation&quot;: **ccpa** (die Datenschutzverordnung, auf die sich die Anfrage bezieht)

## Beispiel für eine JSON-Anfrage

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

## Datenfelder, die für Zugriffsanfragen zurückgegeben werden

```
attributes:
{
"value”:<*value*>,
"key”:<*key*>,
"displayName”:<*displayName*>
}
```