---
title: Erstellen einer Zielgruppe in der Zielgruppenbibliothek
description: Erfahren Sie, wie Sie in der Zielgruppenbibliothek mithilfe von Attributregeln eine freigebbare Zielgruppe erstellen. Erfahren Sie, wie Sie eine Regel konfigurieren und eine gemischte Zielgruppe definieren.
solution: Experience Cloud
uuid: 7e622539-296e-4ff3-93b0-ec1c08b35429
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: b65a12f5-fa89-400a-b279-13c381cd6c22
source-git-commit: c98084e3960e40ae28e55050ce0727abce94ba0c
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 65%

---

# Erstellen einer Zielgruppe

In [!UICONTROL Zielgruppenbibliothek] können Sie Attributregeln verwenden, um eine Zielgruppe zu erstellen und eine gemischte Zielgruppe für die Freigabe in Experience Cloud-Programmen zu definieren.

In diesem Artikel lernen Sie Folgendes:

* Erstellen einer Zielgruppe
* Erstellen einer Regel
* Verwenden von Regeln zum Definieren einer gemischten Zielgruppe

Die folgende Grafik stellt zwei Regeln in einer gemischten Zielgruppe dar.

![Zwei Regeln in einer gemischten Zielgruppe](assets/audience_sharing.png)

Jeder Kreis steht für eine Regel, die die Zugehörigkeit zu einer Zielgruppe definiert. Besucher, die sich in beiden Zielgruppenregeln qualifizieren, überschneiden sich und werden so zur gemischten, definierten Zielgruppe.

>[!NOTE]
>
>Die Zielgruppe ist erst nach Ablauf des für die Datenerfassung angegebenen Zeitraums vollständig definiert.

Das folgende Beispiel zeigt, wie die Regeln für eine gemischte Zielgruppe erstellt werden. Diese Zielgruppe umfasst Folgendes:

* Abschnitt „Home &amp; Garden“, der von Seitendaten oder Analyse-Rohdaten abgeleitet wurde.
* Chrome- und Safari-Benutzer, die von einem [!DNL Adobe Analytics] Segment abgeleitet [veröffentlicht](overview.md) in [!DNL Experience Cloud].

  ![Erstellen der Regeln für eine gemischte Zielgruppe](assets/audience_create.png)

**Erstellen einer Zielgruppe**

1. Klicken Sie auf [!DNL Experience Cloud] Apps ![Apps-Symbol](assets/apps-icon.png) und dann auf **[!UICONTROL People]** > **[!UICONTROL Audience Library].**

1. Klicken Sie auf [!UICONTROL &#x200B; Seite &#x200B;]Zielgruppen **[!UICONTROL auf „Neu]**. ![Neue Zielgruppe](assets/add_icon_small.png)

   ![Erstellen einer Zielgruppe](assets/audience_create_new.png)

1. Füllen Sie auf [!UICONTROL &#x200B; Seite „Neue Zielgruppe &#x200B;]&quot; die Felder **[!UICONTROL Titel]** und **[!UICONTROL Beschreibung]** aus.
1. Wählen [!UICONTROL &#x200B; unter &#x200B;] eine Referenz-Report Suite und dann eine Attributquelle aus:

   * **[!UICONTROL Real-Time Analytics-Daten:]** (oder Rohdaten) Hierbei handelt es sich um Attributdaten, die aus Real-Time Analytics-Bildanforderungen abgeleitet wurden. Sie enthält eVars und Ereignisse. Sie müssen bei Verwendung dieser Attributquelle eine Report Suite auswählen und die einzuschließende Dimension oder das einzuschließende Ereignis definieren. Diese Report Suite-Auswahl stellt die von der Report Suite verwendete Variablenstruktur bereit.

   >[!NOTE]
   >
   >Aufgrund des Caching benötigen gelöschte Report Suites in Analytics 12 Stunden, bevor die Löschung in Experience Cloud angezeigt wird.

   * **[!UICONTROL Experience Cloud:]** Attributdaten werden aus [!DNL Experience Cloud] Quellen abgeleitet. Hierbei kann es sich z. B. um Daten aus Zielgruppensegmenten handeln, die Sie in [!DNL Analytics] erstellen, oder Daten aus [!DNL Audience Manager].

1. Definieren Sie Zielgruppenregeln und klicken Sie dann auf **[!UICONTROL Speichern].**

**Beispiel: Definieren von Regeln für eine gemischte Zielgruppe**

>[!NOTE]
>
>Für die Erstellung von Zielgruppenregeln sollten Sie Ihre Implementierungsvariablen unbedingt kennen.

Definieren Sie unter [!UICONTROL Regeln] die *`Home & Garden`*-Attributauswahl:

* **[!UICONTROL Attributquelle:]** Analytics-Rohdaten
* **[!UICONTROL Report Suite:]** Report Suite 31
* Dimension = **[!UICONTROL Store (Merch) (v6)]** > **[!UICONTROL Entspricht]** > **[!UICONTROL Home &amp; Garden]**

![Attributauswahlen in der Zielgruppenbibliothek](assets/home_garden.png)

Die *Besucher von Chrome und Safari* sind ein in Analytics freigegebenes Zielgruppensegment:

* **[!UICONTROL Attributquelle:]** Experience Cloud
* **[!UICONTROL Dimension:]** Besucher von Chrome &amp; Safari

![Besucher von Chrome und Safari](assets/chrome_safari.png)

Zum Vergleich können Sie eine *OR*-Regel hinzufügen, um alle Besucher eines Site-Bereichs wie „Terrasse &amp; Möbel“ anzuzeigen.

![ODER-Regel für eine Zielgruppe](assets/audiences_rule_patio.png)

Die resultierende Regel ist eine definierte Zielgruppe mit Chrome &amp; Safari-Benutzern, die Home &amp; Garden besucht haben. Der Abschnitt „Patio &amp; Furniture“ bietet zusätzliche Einblicke in alle Besucher, die diesen Site-Abschnitt besuchen.

![Definierte Zielgruppe in Experience Cloud](assets/defined_audience.png)

* **Historische Schätzdaten:** (Gepunkteter Kreis) Stellt Regeln dar, die basierend auf [!DNL Analytics]-Daten erstellt wurden.
* **Tatsächliche Zielgruppe:** (Durchgehender Kreis) Eine erstellte Regel, die 30 Tage lang Daten aus Audience Manager enthält. Wenn die Audience Manager-Daten 30 Tage erreichen, ist die Zeile durchgehend gefüllt und stellt die tatsächlichen Zahlen dar.

Nachdem die Datenerfassung für den angegebenen Zeitraum abgeschlossen wurde, werden die Kreise zu einer definierten Zielgruppe kombiniert.

Nachdem die Zielgruppe gespeichert wurde, ist sie für andere Experience Cloud-Programme verfügbar. Sie können beispielsweise eine freigegebene Zielgruppe in eine Adobe Target-Aktivität ([) ](https://experienceleague.adobe.com/de/docs/target/using/activities/activities).
