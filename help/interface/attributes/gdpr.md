---
title: Unterstützung von Kundenattributen für die Datenschutz-Grundverordnung (DSGVO) | Adobe Experience Cloud
description: Informationen zur Unterstützung von Kundenattributen für die allgemeine Datenschutzverordnung
translation-type: tm+mt
source-git-commit: 4bea0c29afa580dc63b21535ce5c275cd649c9a5
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 97%

---


# Unterstützung von Kundenattributen für die Datenschutz-Grundverordnung (DSGVO)

Auf dieser Seite wird beschrieben, wie Kundenattribute die Datenschutz-Grundverordnung (DSGVO) unterstützen.

>[!IMPORTANT]
>
>Der Inhalt dieses Dokuments ist keine Rechtsberatung und soll keine Rechtsberatung ersetzen. Wenden Sie sich an Ihren Rechtsbeistand, um Beratung zur DSGVO zu erhalten.

Die [Datenschutz-Grundverordnung](https://www.adobe.com/de/privacy/general-data-protection-regulation/what-is-gdpr.html) ist am 25. Mai 2018 in Kraft getreten und bietet allen Personen (betroffenen Personen) innerhalb der Grenzen der Europäischen Union (EU) die Kontrolle über ihre personenbezogenen Daten. Außerdem wird das regulatorische Umfeld für internationale Geschäftsbeziehungen vereinfacht. Dieses Gesetz gilt für alle Unternehmen (Datenverantwortliche), die innerhalb der Grenzen der EU zum Zeitpunkt der Verarbeitung ihrer personenbezogenen Daten Waren oder Dienstleistungen anbieten, das Verhalten von Personen überwachen oder personenbezogene Daten von Personen sammeln, unabhängig davon, wo sich der Geschäftssitz des Datenverantwortlichen befindet.

Adobe Experience Cloud fungiert als Auftragsverarbeiter für alle personenbezogenen Daten, die es im Auftrag seiner Kunden empfängt und speichert. Als Datenverantwortlicher legen Sie fest, welche personenbezogenen Daten Adobe Experience Cloud in Ihrem Namen verarbeitet und speichert.

In diesem Dokument wird beschrieben, wie [!UICONTROL Kundenattribute] die DSGVO-Datenzugriffs- und -Löschungsrechte der betroffenen Personen mithilfe der Adobe Experience Platform Privacy Service-API und der Benutzeroberfläche von Privacy Service unterstützen.

Weitere Informationen darüber, was die DSGVO für Ihr Unternehmen bedeutet, finden Sie unter [DSGVO und Ihr Unternehmen](https://www.adobe.com/de/privacy/general-data-protection-regulation.html).

## Erforderliche Einrichtung zum Senden von Anfragen für [!UICONTROL Kundenattribute]

Um Anfragen zum Zugreifen auf und Löschen von Daten zu [!UICONTROL Kundenattributen] zu stellen, ist Folgendes erforderlich:

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

* &quot;action&quot;: entweder **Zugriff** oder **Löschen**

* &quot;user IDs&quot;:

   * &quot;namespace&quot;: &lt;*Alias-ID der CRS-Datenquelle*>

   * &quot;type&quot;: **integrationCode**

   * &quot;value&quot;: &lt;*CRM-ID*>

* &quot;include&quot;: **CRS** (das Adobe-Produkt, auf das sich die Anfrage bezieht)

* &quot;regulation&quot;: **dsgvo** (die Datenschutzverordnung, auf die sich die Anfrage bezieht)

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
