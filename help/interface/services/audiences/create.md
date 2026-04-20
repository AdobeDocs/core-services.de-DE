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
TQID: https://experienceleague.adobe.com/xXhiBeGGEVpvdjZdpL2Q9-3eDn-gN58dynb56daQcig
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a42153ba5a885509e7735e7407e38586fcabb0ad
workflow-type: tm+mt
source-wordcount: 515
ht-degree: 60%

---

# Erstellen einer Zielgruppe

In [!UICONTROL Audience Library] können Sie Attributregeln verwenden, um eine Zielgruppe zu erstellen und eine gemischte Zielgruppe zu definieren, die in CX Enterprise-Programmen freigegeben werden kann.

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
* Chrome- und Safari-Benutzer, die von einem [!DNL Adobe Analytics] Segment abgeleitet [veröffentlicht](overview.md) in [!DNL CX Enterprise].

  ![Erstellen der Regeln für eine gemischte Zielgruppe](assets/audience_create.png)

**Erstellen einer Zielgruppe**

1. Klicken Sie auf [!DNL CX Enterprise] Apps ![Apps-Symbol](assets/apps-icon.png) und dann auf **[!UICONTROL People]** > **[!UICONTROL Audience Library].**

1. Klicken Sie auf der [!UICONTROL Audiences] Seite auf **[!UICONTROL New]**. ![Neue Zielgruppe](assets/add_icon_small.png)

   ![Erstellen einer Zielgruppe](assets/audience_create_new.png)

1. Füllen Sie auf der Seite [!UICONTROL Create New Audience] die Felder **[!UICONTROL Title]** und **[!UICONTROL Description]** aus.
1. Wählen Sie unter [!UICONTROL Rules] eine Referenz-Report Suite und dann eine Attributquelle aus:

   * **[!UICONTROL Real-Time Analytics Data:]** (oder Rohdaten) Hierbei handelt es sich um Attributdaten, die aus Real-Time Analytics-Bildanforderungen abgeleitet wurden. Sie enthält eVars und Ereignisse. Sie müssen bei Verwendung dieser Attributquelle eine Report Suite auswählen und die einzuschließende Dimension oder das einzuschließende Ereignis definieren. Diese Report Suite-Auswahl stellt die von der Report Suite verwendete Variablenstruktur bereit.

     >[!NOTE]
     >
     >Aufgrund des Caching benötigen gelöschte Report Suites in Analytics 12 Stunden, bevor die Löschung in CX Enterprise angezeigt wird.

   * **[!UICONTROL CX Enterprise:]** aus [!DNL CX Enterprise] Quellen abgeleitete Attributdaten. Hierbei kann es sich z. B. um Daten aus Zielgruppensegmenten handeln, die Sie in [!DNL Analytics] erstellen, oder Daten aus [!DNL Audience Manager].

1. Definieren Sie Zielgruppenregeln und klicken Sie dann auf **[!UICONTROL Save].**

**Beispiel: Definieren von Regeln für eine gemischte Zielgruppe**

>[!NOTE]
>
>Für die Erstellung von Zielgruppenregeln sollten Sie Ihre Implementierungsvariablen unbedingt kennen.

Definieren Sie unter [!UICONTROL Rules] die Auswahl der *`Home & Garden`* Attribute:

* **[!UICONTROL Attribute Source:]** von Analytics-Rohdaten
* Report Suite 31 **[!UICONTROL Report Suite:]**
* Dimension = **[!UICONTROL Store (Merch) (v6)]** > **[!UICONTROL Equals]** > **[!UICONTROL Home & Garden]**

![Attributauswahlen in der Zielgruppenbibliothek](assets/home_garden.png)

Die *Besucher von Chrome und Safari* sind ein in Analytics freigegebenes Zielgruppensegment:

* **[!UICONTROL Attribute Source:]** CX Enterprise
* Besuchende von Chrome und Safari **[!UICONTROL Dimension:]**

![Besucher von Chrome und Safari](assets/chrome_safari.png)

Zum Vergleich können Sie eine *OR*-Regel hinzufügen, um alle Besucher eines Site-Bereichs wie „Terrasse &amp; Möbel“ anzuzeigen.

![ODER-Regel für eine Zielgruppe](assets/audiences_rule_patio.png)

Die resultierende Regel ist eine definierte Zielgruppe mit Chrome &amp; Safari-Benutzern, die Home &amp; Garden besucht haben. Der Abschnitt „Patio &amp; Furniture“ bietet zusätzliche Einblicke in alle Besucher, die diesen Site-Abschnitt besuchen.

![Definierte Zielgruppe in CX Enterprise](assets/defined_audience.png)

* **Historische Schätzdaten:** (Gepunkteter Kreis) Stellt Regeln dar, die basierend auf [!DNL Analytics]-Daten erstellt wurden.
* **Tatsächliche Zielgruppe:** (Durchgehender Kreis) Eine erstellte Regel, die 30 Tage lang Daten aus Audience Manager enthält. Wenn die Audience Manager-Daten 30 Tage erreichen, ist die Zeile durchgehend gefüllt und stellt die tatsächlichen Zahlen dar.

Nachdem die Datenerfassung für den angegebenen Zeitraum abgeschlossen wurde, werden die Kreise zu einer definierten Zielgruppe kombiniert.

Nachdem die Zielgruppe gespeichert wurde, ist sie für andere CX Enterprise-Programme verfügbar. Sie können beispielsweise eine freigegebene Zielgruppe in eine Adobe Target-Aktivität ([) &#x200B;](https://experienceleague.adobe.com/de/docs/target/using/activities/activities).
