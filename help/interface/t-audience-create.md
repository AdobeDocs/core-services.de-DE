---
description: Hier erfahren Sie, wie Sie in Adobe Experience Cloud mit Attributregeln eine Zielgruppe erstellen und eine gemischte Zielgruppe definieren.
keywords: Hauptdienste
solution: Experience Cloud
title: 'Erstellen einer Zielgruppe '
uuid: 7e622539-296e-4ff3-93b0-ec1c08b35429
feature: Zielgruppenbibliothek
topic: Administration
role: Admin
level: Experienced
exl-id: b65a12f5-fa89-400a-b279-13c381cd6c22
source-git-commit: 1fb1abc7311573f976f7e6b6ae67f60ada10a3e7
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 96%

---

# Erstellen einer Zielgruppe

Hier erfahren Sie, wie Sie in Experience Cloud mit Attributregeln eine Zielgruppe erstellen und eine gemischte Zielgruppe definieren.

In diesem Artikel lernen Sie Folgendes:

* Erstellen einer Zielgruppe
* Erstellen einer Regel
* Verwenden von Regeln zum Definieren einer gemischten Zielgruppe

Die folgende Grafik stellt zwei Regeln in einer gemischten Zielgruppe dar.

![](assets/audience_sharing.png)

Jeder Kreis steht für eine Regel, die die Mitgliedschaft in einer Zielgruppe definiert. Besucher, die sich in beiden Zielgruppenregeln qualifizieren, überschneiden sich und werden so zur gemischten, definierten Zielgruppe.

>[!NOTE]
>
>Die Zielgruppe ist erst nach Ablauf des für die Datenerfassung angegebenen Zeitraums vollständig definiert.

Das folgende Beispiel zeigt, wie die Regeln für eine gemischte Zielgruppe erstellt werden. Diese Zielgruppe umfasst Folgendes:

* Abschnitt „Home &amp; Garden“, der von Seitendaten oder Analyse-Rohdaten abgeleitet wurde.
* Chrome- und Safari-Benutzer, die einem [!DNL Adobe Analytics]-Segment entnommen wurden, das in der [!DNL Experience Cloud] [veröffentlicht](audience-library.md#task_32FEEFE0B32E4E388CD4D892D727282A) wurde.

   ![](assets/audience_create.png)

**Erstellen einer Zielgruppe**

1. Wählen Sie unter [!DNL Experience Cloud] unter [!DNL Experience Platform] **[!UICONTROL Personen]** > **[!UICONTROL Zielgruppenbibliothek].** aus.
1. Wählen Sie auf der Seite [!UICONTROL Zielgruppen] **[!UICONTROL Neu]**. ![](assets/add_icon_small.png) aus.

   ![Schritt Ergebnis](assets/audience_create_new.png)

1. Geben Sie auf der Seite [!UICONTROL Neue Zielgruppe erstellen] einen Titel und eine Beschreibung an.
1. Wählen Sie unter [!UICONTROL Regeln] eine Attributquelle aus:

   * **[!UICONTROL Daten von Real-Time Analytics:]** Hierbei handelt es sich um Attributdaten, die aus Bildanfragen in Real-Time Analytics gewonnen werden und Daten wie eVars und Ereignisse enthalten. Sie müssen bei Verwendung dieser Attributquelle eine Report Suite auswählen und die einzuschließende Dimension oder das einzuschließende Ereignis definieren. Diese Report Suite-Auswahl stellt die von der Report Suite verwendete Variablenstruktur bereit.
   >[!NOTE]
   >
   >Aufgrund der Caching-Funktion wird die Löschung von Report Suites in Analytics erst nach 12 Stunden durch Experience Cloud übernommen.

   * **[!UICONTROL Experience Cloud:]** Aus [!DNL Experience Cloud]-Quellen abgeleitete Attributdaten. Hierbei kann es sich z. B. um Daten aus Zielgruppensegmenten handeln, die Sie in [!DNL Analytics] erstellen, oder Daten aus [!DNL Audience Manager].

1. Definieren Sie Zielgruppenregeln und wählen Sie **[!UICONTROL Speichern].** aus.

>[!NOTE]
>
>Für die Erstellung von Zielgruppenregeln sollten Sie Ihre Implementierungsvariablen unbedingt kennen.

Definieren Sie unter [!UICONTROL Regeln] die *`Home & Garden`*-Attributauswahl:

* **[!UICONTROL Attributquelle:]** Analytics-Rohdaten
* **[!UICONTROL Report Suite:]** Report Suite 31
* Dimension = **[!UICONTROL Store (Merch) (v6)]** > **[!UICONTROL Entspricht]** > **[!UICONTROL Home &amp; Garden]**

![](assets/home_garden.png)

Die *Besucher von Chrome und Safari* sind ein in Analytics freigegebenes Zielgruppensegment:

* **[!UICONTROL Attributquelle:]** Experience Cloud
* **[!UICONTROL Dimension:]** Besucher von Chrome &amp; Safari

![](assets/chrome_safari.png)

Zum Vergleich können Sie eine *OR*-Regel hinzufügen, um alle Besucher eines Site-Bereichs wie „Patio &amp; Furniture“ anzuzeigen.

![](assets/audiences_rule_patio.png)

Die resultierende Regel ist eine definierte Zielgruppe mit Chrome &amp; Safari-Benutzern, die Home &amp; Garden besucht haben. Der Abschnitt „Patio &amp; Furniture“ bietet zusätzliche Einblicke in alle Besucher, die diesen Site-Abschnitt besuchen.

![](assets/defined_audience.png)

* **Historische Schätzdaten:** (Gepunkteter Kreis) Stellt Regeln dar, die basierend auf [!DNL Analytics]-Daten erstellt wurden.
* **Tatsächliche Zielgruppe:** (Durchgehender Kreis) Eine erstellte Regel, die 30 Tage lang Daten aus Audience Manager enthält. Wenn die Audience Manager-Daten 30 Tage erreichen, ist die Zeile durchgehend gefüllt und stellt die tatsächlichen Zahlen dar.

Nachdem die Datenerfassung für den angegebenen Zeitraum abgeschlossen wurde, werden die Kreise zu einer definierten Zielgruppe kombiniert.

Nach dem Speichern der Zielgruppe ist sie für andere Lösungen verfügbar. Sie können beispielsweise eine freigegebene Zielgruppe in eine Adobe Target-Aktivität aufnehmen.
