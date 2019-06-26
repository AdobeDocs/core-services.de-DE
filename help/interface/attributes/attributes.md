---
description: Überblick und Voraussetzungen zum Hochladen von Kundenattributen in Experience Cloud.
keywords: Hauptdienste; Kundenattribute
seo-description: Überblick und Voraussetzungen zum Hochladen von Kundenattributen in Experience Cloud.
seo-title: Kundenattribute
solution: Experience Cloud
title: Kundenattribute
uuid: 1621402d-990f-46f9-981a-473280559069
translation-type: ht
source-git-commit: 979b2202a70e2a5362aa86a65a17d7c4279b3a1a

---


# Kundenattribute

## Übersicht

[!UICONTROL Die Kundenattributfunktion] in der Experience Cloud finden Sie hier.

**[!UICONTROL Personen]** &gt; **[!UICONTROL Kundenattribute]**

Wenn Sie Daten von Unternehmenskunden in einer CRM-Datenbank (Customer Relationship Management) erfassen, können Sie diese Daten in eine Datenquelle für Kundenattribute in die Experience Cloud hochladen. Nach dem Hochladen können die Daten mit [!DNL Adobe Analytics] und [!DNL Adobe Target] verarbeitet werden.

![](assets/custom_reports.png)

## Voraussetzungen für das Hochladen von Kundenattributen {#section_BD38693AFBF34926BA28E964963B4EA0}


* **Aktivierung der Lösung:**[Aktivieren Sie Ihre Lösungen für Hauptdienste](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C).

* **Gruppenmitgliedschaft:** Um Kundenattributdaten hochzuladen, müssen Benutzer Mitglieder der folgenden Gruppe sein:  [„Kundenattribute“](../admin-getting-started/admin-getting-started.md#task_3295A85536BF48899A1AB40D207E77E9). Sie müssen darüber hinaus einer Adobe Analytics-Gruppe oder einer Adobe Target-Gruppe angehören.

   Um herauszufinden, ob Ihr Unternehmen Zugang zu Kundenattributen hat, muss sich Ihr [!DNL Experience Cloud]-Administrator bei der [!DNL Experience Cloud] anmelden. Navigieren Sie zu **[!UICONTROL Administration]** &gt; **[!UICONTROL Admin Console starten]** &gt; **[!UICONTROL Gruppen]**. Falls *Kundenattribute* als eine der Gruppen angezeigt wird, können Sie beginnen.

   Benutzer, die der Gruppe „Kundenattribute“ hinzugefügt wurden, sehen auf der linken Seite der Experience Cloud-Benutzeroberfläche das Menüelement [!UICONTROL Kundenattribute].

* **Target-Mbox:** Für Kundenattribute ist mbox.js Version 58 oder höher erforderlich.


   Siehe [„mbox.js“-Implementation](https://marketing.adobe.com/resources/help/de_DE/target/ov/?f=t_mbox_download).

* **at.js:** Beliebige Version




## Was sind Enterprise-Kundendaten? {#section_6F34C29F11414842AA57D2B1248FA3C6}

Unternehmensdaten befinden sich auf anderen Systemen. Sie können komplex sein und für verschiedene Personen einen unterschiedlichen Stellenwert haben. Diese Daten können Informationen wie Mitgliedschaften, Loyalität, Alter, Geschlecht, erworbene Produkte, Interessen und Lebenszeitwert beinhalten.

Folgende Abbildung zeigt einen Ausschnitt aus einer Datendatei mit Produktabonnementdaten einschließlich Mitglieds-IDs, Produktberechtigungen, der am häufigsten gestarteten Produkte usw.

![](assets/01_crs_usecase.png)

Nach Erstellung der Datendatei können Sie sie in eine Kundenattributquelle hochladen, die Sie über **[!UICONTROL Experience Cloud]** &gt; **[!UICONTROL Kundenattribute]** erstellt haben.

Weitere Informationen zu diesem Arbeitsablauf finden Sie unter [Hochladen von Kundenattributdaten](../attributes/t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

## Anwendungsfälle für Lösungen {#section_4E77650F6CEE4C4ABCD0B3221A5AE5D9}

Nach dem Hochladen der Daten in die Experience Cloud können Sie sie anpassen und für Ihre Berichterstattungs-, Segmentierungs-, Aktivitäten- und Kampagnenlösungen freigeben.

Beispiel:

| Lösung | Vorzüge und Anwendungsfälle |
|--- |--- |
| Adobe Analytics | Marketingfachleute und Analysten gewinnen Einsichten in Folgendes:<ul><li>Die bezüglich der Gold-Kunden effektivsten Onlinekampagnen.</li><li>Die Produkte, die Gold-Kunden im Gegensatz zu Platin-Kunden suchen.</li><li>Die Frage, ob die Überarbeitung der Website für ältere Kunden positive Auswirkungen auf die Konversionsrate hat.</li><li>Nach welchen Produkten Kunden mit niedrigem Lebenszeitwert bevorzugt auf unserer Site suchen.</li></ul> |
| Adobe Target | Mit Attributdaten haben Target-Benutzer folgende Möglichkeiten:<ul><li>Besondere Angebote und Rabatte für Mitglieder des „Loyalty-Clubs“.</li><li>Empfehlungen von teureren Produkten für Kunden, die Luxusprodukte bevorzugen.</li><li>Anzeigen von Upsell-Angeboten für Kunden, die bereits E-Mails erhalten, an der normalerweise für E-Mail-Registrierungen reservierten Stelle.</li></ul> |
