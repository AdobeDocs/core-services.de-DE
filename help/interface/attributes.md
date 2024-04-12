---
title: "[!DNL Customer Attributes]"
description: Informationen zu [!DNL Customer Attributes] in Experience Cloud. Erfahren Sie, wie Sie Kundenattributdaten für die Verwendung in Adobe Analytics und Adobe Target hochladen.
solution: Experience Cloud,Target,Analytics
feature: Customer Attributes
role: Admin
topic: Administration
level: Experienced
exl-id: fe8ad013-76da-49f8-aa51-dc5f6c1b1d79
source-git-commit: 06c51428244c67fdb871d4039888aa2517048d2b
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 74%

---

# [!DNL Customer Attributes] in Experience Cloud

[!DNL Customer Attributes] in Experience Cloud ermöglicht Ihnen das Hochladen Ihrer erfassten Unternehmensdaten aus einer CRM-Datenbank (Customer Relationship Management). Sie können die Daten in eine Kundenattribut-Datenquelle in Experience Cloud hochladen und dann die Daten in [!DNL Adobe Analytics] und [!DNL Adobe Target].

## Suchen Sie die [!DNL Customer Attributes] Funktion

1. Melden Sie sich bei Experience Cloud an.

1. Navigieren Sie zu **[!DNL Experience Platform]** > **[!UICONTROL Personen]** > **[!UICONTROL Kundenattribute]**.

![Übersicht über Kundenattribute](assets/custom_reports.png)

## Voraussetzungen für das Hochladen [!DNL Customer Attributes] {#section_BD38693AFBF34926BA28E964963B4EA0}

* **Aktivierung der Lösung:** [Aktivieren Sie Ihre Lösungen für Experience Platform-Dienste](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C).

* **Gruppenmitgliedschaft:** Um Kundenattributdaten hochzuladen, müssen Benutzer Mitglieder der [Kundenattributgruppe](admin-getting-started.md#task_3295A85536BF48899A1AB40D207E77E9) sein. Sie müssen auch einer Adobe Analytics-Gruppe oder einer Adobe Target-Gruppe angehören.

  Um herauszufinden, ob Ihr Unternehmen Zugang zu Kundenattributen hat, muss sich Ihr [!DNL Experience Cloud]-Administrator bei [Experience Cloud](https://experience.adobe.com) anmelden. Navigieren Sie zu **[!UICONTROL Administration]** > **[!UICONTROL Admin Console]** > **[!UICONTROL Produkte]**. Wenn *[!DNL Customer Attributes]* wird als einer der [!UICONTROL Produktprofile], können Sie beginnen.

  Benutzer, die zu [!DNL Customer Attributes] die [!UICONTROL Kundenattribute] -Menüpunkt auf der linken Seite der Experience Cloud-Oberfläche.

* **Adobe Target** `at.js` (beliebige Version) oder `mbox.js` Version 58 oder höher ist für Kundenattribute erforderlich.

  Siehe [Bereitstellen von at.js](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/overview.html?lang=de).

## Was sind Enterprise-Kundendaten? {#section_6F34C29F11414842AA57D2B1248FA3C6}

Enterprise-Daten befinden sich in anderen Systemen. Sie können komplex sein und verschiedene Bedeutungen für verschiedene Personen haben. Diese Daten können Informationen wie Mitgliedschaften, Treueebene, Alter, Geschlecht, eigene Produkte, Interessen und Lebenszeitwert beinhalten.

Das folgende Bild ist ein Beispiel für eine Datendatei mit Abonnentendaten zu Produkten, einschließlich Mitglieds-IDs, Produkten mit Berechtigung, den am häufigsten gestarteten Produkten usw.

![Was sind Unternehmens-Kundendaten?](assets/01_crs_usecase.png)

Nach Erstellung der Datendatei können Sie sie in eine Kundenattributquelle hochladen, die Sie unter **[!UICONTROL Experience Cloud]** > **[!UICONTROL Kundenattribute]** erstellen.

Weitere Informationen zu diesem Workflow finden Sie unter [Hochladen von Kundenattributdaten](t-crs-usecase.md#task_BCC327B2A0EF4A1BBB2934013AB92B78).

## Beispiele für Kundenattribute in Analytics und Target {#section_4E77650F6CEE4C4ABCD0B3221A5AE5D9}

Nachdem sich die Daten im Experience Cloud befinden, können Sie sie anpassen und für Berichterstellungs-, Segmentierungs-, Aktivitäts- und Kampagnenlösungen freigeben.

Beispiel:

| Lösung | Vorteile und Anwendungsfälle |
|--- |--- |
| Adobe Analytics | Marketing-Experten und Analysten können Folgendes nachvollziehen:<ul><li>Die Online-Kampagnen, die bei Ihren Gold-Kunden am effektivsten sind.</li><li>Die Produkte, nach denen Gold-Kunden suchen, im Vergleich zu Produkten, nach denen Platin-Kunden suchen.</li><li>Ob Ihre Site-Neugestaltung positive Auswirkungen auf die Konversionsraten älterer Kunden hat.</li><li>Die Produkte, nach denen Kunden mit einem niedrigem Lifetime Value auf meiner Seite suchen.</li></ul> |
| Adobe Target | Attributdaten ermöglichen Benutzern von Adobe Target Folgendes:<ul><li>Anzeigen von Sonderrabatten und -angeboten für Treueclub-Mitglieder.</li><li>Senden von Empfehlungen teurerer Produkte an Luxuskunden.</li><li>Anzeigen von Up-Sell-Angeboten für Kunden, die bereits E-Mails erhalten, an der Stelle, die normalerweise für E-Mail-Anmeldungen reserviert ist.</li></ul> |

{style="table-layout:auto"}
