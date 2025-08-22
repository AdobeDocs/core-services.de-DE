---
title: '[!DNL Customer attributes]'
description: Weitere Informationen zu  [!DNL customer attributes]  in Experience Cloud. Erfahren Sie, wie Sie Kundenattributdaten für die Verwendung in Adobe Analytics und Adobe Target hochladen.
solution: Experience Cloud,Target,Analytics
feature: Customer Attributes
role: Admin
topic: Administration
level: Experienced
exl-id: fe8ad013-76da-49f8-aa51-dc5f6c1b1d79
source-git-commit: 3043cd913d5165c58fb84f3342b05a00a690d6a6
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 78%

---

# [!DNL Customer attributes] in Experience Cloud

Mit [!DNL Customer attributes] in Experience Cloud können Sie Ihre erfassten Unternehmensdaten aus einer CRM-Datenbank (Customer Relationship Management) hochladen. Sie können die Daten in eine Datenquelle für Kundenattribute in Experience Cloud hochladen und dann die Daten in [!DNL Adobe Analytics] und [!DNL Adobe Target] verwenden.

## Suchen Sie die Funktion [!DNL customer attributes]

1. Melden Sie sich bei [!DNL Experience Cloud] an und wählen Sie das Symbol ![Menü](assets/menu-icon.png) aus.

1. Wählen Sie **[!UICONTROL Kundenattribute]** aus.

![Übersicht über Kundenattribute](assets/custom_reports.png)

## Voraussetzungen zum Hochladen von [!DNL customer attributes] {#prerequisites}

* **Gruppenmitgliedschaft:** Um Kundenattributdaten hochzuladen, müssen Benutzer Mitglieder der Gruppe „Kundenattribute“ sein. Sie müssen auch einer Adobe Analytics-Gruppe oder einer Adobe Target-Gruppe angehören.

  Um herauszufinden, ob Ihr Unternehmen Zugriff auf Kundenattribute hat, muss sich Ihr [!DNL Experience Cloud]-Administrator bei der [Experience Cloud](https://experience.adobe.com) anmelden. Navigieren Sie zu **[!UICONTROL Admin Console]** > **[!UICONTROL Produkte]**. Wenn *[!DNL Customer Attributes]* als eines der [!UICONTROL Produktprofile] angezeigt wird, können Sie beginnen.

  Benutzerinnen und Benutzer, die den [!DNL Customer Attributes] hinzugefügt wurden, sehen auf der linken Seite der Experience Cloud-Benutzeroberfläche das Menüelement [!UICONTROL Kundenattribute].

* **Adobe Target** `at.js` (beliebige Version) oder `mbox.js` Version 58 oder höher ist für Kundenattribute erforderlich.

  Siehe [Bereitstellen von at.js](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/overview.html?lang=de).

## Was sind Enterprise-Kundendaten? {#enterprise_data}

Enterprise-Daten befinden sich in anderen Systemen. Sie können komplex sein und verschiedene Bedeutungen für verschiedene Personen haben. Diese Daten können Informationen wie Zugehörigkeiten, Treueebene, Alter, Geschlecht, eigene Produkte, Interessen und Lebenszeitwert beinhalten.

Das folgende Bild ist ein Beispiel für eine Datendatei mit Abonnentendaten zu Produkten, einschließlich Mitglieds-IDs, Produkten mit Berechtigung, den am häufigsten gestarteten Produkten usw.

![Was sind Unternehmens-Kundendaten?](assets/01_crs_usecase.png)

Nachdem Sie die Datendatei erstellt haben, können Sie sie in die Kundenattributquelle hochladen, die Sie unter **[!UICONTROL Experience Cloud]** > **[!UICONTROL Kundenattribute]** erstellen.

Weitere [ zu diesem Workflow finden Sie unter ](t-crs-usecase.md) von Kundenattributdaten hochladen .

## Beispiele für Kundenattribute in Analytics und Target {#examples}

Nachdem sich die Daten in Experience Cloud befinden, können Sie sie anpassen und für Lösungen für Berichte, Segmentierung, Aktivitäten und Kampagnen freigeben.

Beispiel:

| Lösung | Vorteile und Anwendungsfälle |
|--- |--- |
| Adobe Analytics | Marketing-Experten und Analysten können Folgendes nachvollziehen:<ul><li>Die Online-Kampagnen, die bei Ihren Gold-Kunden am effektivsten sind.</li><li>Die Produkte, nach denen Gold-Kunden suchen, im Vergleich zu Produkten, nach denen Platin-Kunden suchen.</li><li>Ob Ihre Site-Neugestaltung positive Auswirkungen auf die Konversionsraten älterer Kunden hat.</li><li>Die Produkte, nach denen Kunden mit einem niedrigem Lifetime Value auf meiner Seite suchen.</li></ul> |
| Adobe Target | Attributdaten ermöglichen Benutzern von Adobe Target Folgendes:<ul><li>Anzeigen von Sonderrabatten und -angeboten für Treueclub-Mitglieder.</li><li>Senden von Empfehlungen teurerer Produkte an Luxuskunden.</li><li>Anzeigen von Up-Sell-Angeboten für Kunden, die bereits E-Mails erhalten, an der Stelle, die normalerweise für E-Mail-Anmeldungen reserviert ist.</li></ul> |

{style="table-layout:auto"}
