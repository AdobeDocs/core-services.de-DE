---
description: Erfahren Sie, wie Sie mit Attributregeln eine Zielgruppe erstellen und eine gemischte Zielgruppe in der Experience Cloud erstellen.
keywords: Hauptdienste
seo-description: Erfahren Sie, wie Sie mit Attributregeln eine Zielgruppe erstellen und eine gemischte Zielgruppe in der Experience Cloud erstellen.
seo-title: Erstellen einer Zielgruppe
solution: Experience Cloud
title: Erstellen einer Zielgruppe
uuid: 7 e 622539-296 e -4 ff 3-93 b 0-ec 1 c 08 b 35429
translation-type: tm+mt
source-git-commit: 979b2202a70e2a5362aa86a65a17d7c4279b3a1a

---


# Erstellen einer Zielgruppe

Erfahren Sie, wie Sie mit Attributregeln eine Zielgruppe erstellen und eine gemischte Zielgruppe in der Experience Cloud erstellen.

In diesem Abschnitt lernen Sie folgende Verfahren kennen:

* Erstellen einer Zielgruppe
* Erstellen von Regeln
* Verwenden von Regeln zum Definieren von zusammengefassten Zielgruppen


Nachfolgende Grafik stellt zwei Regeln einer zusammengefassten Zielgruppe dar.

![](assets/audience_sharing.png)

Beide Kreise stellen eine Regel dar, die die Mitglieder einer Zielgruppe definieren. Besucher, die sich nach beiden Regeln als Mitglieder der betreffenden Zielgruppe qualifizieren (also die Schnittmenge beider Regeln bilden), gehören zur zusammengefassten Zielgruppe.

>[!NOTE]
>
>Die Zielgruppe wird vollständig nach der Datenerfassung für den angegebenen Zeitraum definiert.
Nachfolgendes Beispiel zeigt, wie die Regeln für eine zusammengefasste Zielgruppe erstellt werden. Diese Zielgruppe besteht aus Folgendem:

* Home &amp; Garden-Abschnitt aus Seitendaten oder Analytics-Rohdaten
* Benutzer von Chrome und Safari, die aus einem [!DNL Adobe Analytics] in der Liste [veröffentlichten](../audience-library/audience-library.md#task_32FEEFE0B32E4E388CD4D892D727282A) Segment abgeleitet [!DNL Experience Cloud]wurden.


   ![](assets/audience_create.png)

1. Klicken [!DNL Experience Cloud]**[!UICONTROL Sie in &quot;Personen]** &quot; &gt; **[!UICONTROL &quot; Zielgruppenbibliothek]**«.
1. Klicken Sie auf der Seite [!UICONTROL „Zielgruppen“]**auf[!UICONTROL Neu]**. ![](assets/add_icon_small.png)

![Schrittergebnis](assets/audience_create_new.png)

1. Geben Sie auf der Seite [!UICONTROL „Neue Zielgruppe erstellen“] einen Titel und eine Beschreibung an.
1. Wählen Sie unter [!UICONTROL Regeln] eine Attributquelle aus:

* **[!UICONTROL Analytics-Echtzeitdaten (oder Rohdaten):]** Hierbei handelt es sich um Attributdaten, die aus Echtzeit-Bildanfragen an Analytics gewonnen werden und Daten wie eVars und Ereignisse enthalten. Wenn Sie diese Attributquelle verwenden, müssen eine Report Suite auswählen und die einbezogene Dimension oder das einbezogene Ereignis definieren. Die Auswahl dieser Report Suite stellt die Variablenstruktur bereit, die von der Report Suite verwendet wird.

   >[!NOTE]
   >
   >Aufgrund der Zwischenspeicherung müssen Report Suites in Analytics 12 Stunden vor dem Löschen in der Experience Cloud angezeigt werden.

* **[!UICONTROL Experience Cloud:]** Attributdaten aus den [!DNL Experience Cloud] Quellen. Hierbei kann es sich z. B. um Daten aus Zielgruppensegmenten handeln, die Sie in [!DNL Analytics] erstellen, oder Daten aus [!DNL Audience Manager].

1. Definieren Sie die Zielgruppenregeln.

>[!NOTE]
>
>Bei der Definition von Zielgruppenregeln sollten Sie Ihre Implementierungsvariablen kennen.

Definieren Sie unter [!UICONTROL Regeln]die *`Home & Garden`* Attributauswahl:

* **[!UICONTROL Attributquelle:]** Analytics-Rohdaten
* **[!UICONTROL Report Suite:]** Report Suite 31
* Dimension = **[!UICONTROL Store (Merch) (v 6)]** &gt; **[!UICONTROL Gleich]** &gt; **[!UICONTROL Home &amp; Garden]**

   ![](assets/home_garden.png)

   Die Besucher *von Chrome &amp; Safari* sind ein aus Analytics freigegebenes Zielgruppensegment:

* **[!UICONTROL Attributquelle:]** Experience Cloud
* **[!UICONTROL Dimension:]** Besucher von Chrome &amp; Safari

   ![](assets/chrome_safari.png)

   Zum Vergleich können Sie eine *OR* -Regel hinzufügen, um alle Besucher eines Site-Abschnitts wie Patio &amp; Furniture anzuzeigen.

   ![](assets/audiences_rule_patio.png)

1. Sehen Sie sich das Ergebnis an.

Die sich daraus ergebende Regel ist eine definierte Zielgruppe, die aus Besuchern von Chrome &amp; Safari besteht, die „Home &amp; Garden“ besucht haben. Das Segment „Patio &amp; Furniture“ bietet zusätzliche Einblicke zu allen Besuchern, die diesen Sitebereich besucht haben.

![](assets/defined_audience.png)

**Historische Schätzdaten:** (Gepunkteter Kreis) Stellt Regeln dar, die basierend auf [!DNL Analytics]-Daten erstellt wurden.

**Tatsächliche Zielgruppe:** (durchgehender Kreis) Jede erstellte Regel, die einen Datenzeitraum von 30 Tagen in Audience Manager umfasst. Wenn die Daten aus Audience Manager 30 Tage erreichen, wird die Linie durchgehend angezeigt und stellt tatsächliche Zahlen dar.

Nachdem die Datenerfassung für den angegebenen Zeitraum abgeschlossen wurde, werden die Kreise kombiniert, um eine definierte Zielgruppe anzuzeigen.

1. Klicken Sie nach der Definition der Regeln auf **[!UICONTROL Speichern]**.

Eine gespeicherte Zielgruppe steht auch anderen Lösungen zur Verfügung. Eine solchermaßen freigegebene Zielgruppe können Sie zum Beispiel auch in einer Target-Aktivität verwenden.
