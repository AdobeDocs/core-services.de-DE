---
title: 'Unterstützung von Kundenattributen für die Datenschutz-Grundverordnung (DSGVO) '
description: Unterstützung von Kundenattributen für die Datenschutz-Grundverordnung (DSGVO)
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 02417c0c-6780-4699-9470-f1685c3cd25d
source-git-commit: 55c81003b94b7e033cddb6854b5c1f1c1ffa199c
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 91%

---

# Unterstützung von Kundenattributen für die Datenschutz-Grundverordnung (DSGVO)

Auf dieser Seite wird beschrieben, wie [!UICONTROL Kundenattribute] die Datenschutz-Grundverordnung (DSGVO) unterstützen.

>[!IMPORTANT]
>
>Der Inhalt dieses Dokuments ist keine Rechtsberatung und soll keine Rechtsberatung ersetzen. Wenden Sie sich an Ihren Rechtsbeistand, um Beratung zur DSGVO zu erhalten.

Die [Datenschutz-Grundverordnung](https://business.adobe.com/de/privacy/general-data-protection-regulation.html) ist am 25. Mai 2018 in Kraft getreten und bietet allen Personen (betroffenen Personen) innerhalb der Grenzen der Europäischen Union (EU) die Kontrolle über ihre personenbezogenen Daten. Außerdem wird das regulatorische Umfeld für internationale Geschäftsbeziehungen vereinfacht. Dieses Gesetz gilt für alle Unternehmen (Datenverantwortliche), die innerhalb der Grenzen der EU zum Zeitpunkt der Verarbeitung ihrer personenbezogenen Daten Waren oder Dienstleistungen anbieten, das Verhalten von Personen überwachen oder personenbezogene Daten von Personen sammeln, unabhängig davon, wo sich der Geschäftssitz des Datenverantwortlichen befindet.

Adobe Experience Cloud fungiert als Auftragsverarbeiter für alle personenbezogenen Daten, die es im Auftrag seiner Kunden empfängt und speichert. Als Datenverantwortlicher legen Sie fest, welche personenbezogenen Daten Adobe Experience Cloud in Ihrem Namen verarbeitet und speichert.

In diesem Dokument wird beschrieben, wie [!UICONTROL Kundenattribute] die DSGVO-Datenzugriffs- und -Löschungsrechte der betroffenen Personen mithilfe der Adobe Experience Platform Privacy Service-API und der Benutzeroberfläche von Privacy Service unterstützen.

Weitere Informationen darüber, was die DSGVO für Ihr Unternehmen bedeutet, finden Sie unter [DSGVO und Ihr Unternehmen](https://business.adobe.com/privacy/general-data-protection-regulation.html).

## Erforderliche Einrichtung zum Senden von Anfragen für [!UICONTROL Kundenattribute]

Um Anfragen zum Zugreifen auf und Löschen von Daten zu [!UICONTROL Kundenattributen] zu stellen, ist Folgendes erforderlich:

1. Sie benötigen:

   * [Organisations-ID](#organizations.md)
   * Alias-ID der jeweiligen CRS-Datenquelle
   * CRM-ID des jeweiligen Profils

   Ihre [Organisations-ID](#organizations.md) ist eine 24-stellige alphanumerische Zeichenfolge, die an @AdobeOrg angehängt wird. Sie benötigen die Kennung des Unternehmens, um Anfragen an die Datenschutz-API zu senden. Wenden Sie sich an die Kundenunterstützung von Adobe unter `gdprsupport@adobe.com` , wenn Sie die ID nicht finden können.

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
