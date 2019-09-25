---
description: Erfahren Sie, wie Sie mit Attributregeln eine Zielgruppe erstellen und eine gemischte Zielgruppe in der Experience Cloud definieren.
keywords: Hauptdienste
seo-description: Erfahren Sie, wie Sie mit Attributregeln eine Zielgruppe erstellen und eine gemischte Zielgruppe in der Experience Cloud definieren.
seo-title: Erstellen einer Zielgruppe
solution: Experience Cloud
title: Erstellen einer Zielgruppe
uuid: 7e622539-296e-4ff3-93b0-ec1c08b35429
translation-type: ht
source-git-commit: f8b48077d936e289d66c1a93a96fe9ebaa4f0136

---


# Erstellen einer Zielgruppe

Erfahren Sie, wie Sie mit Attributregeln eine Zielgruppe erstellen und eine gemischte Zielgruppe in der Experience Cloud definieren.

In diesem Abschnitt lernen Sie folgende Verfahren kennen:

* Erstellen einer Zielgruppe
* Erstellen von Regeln
* Verwenden von Regeln zum Definieren von zusammengefassten Zielgruppen


Nachfolgende Grafik stellt zwei Regeln einer zusammengefassten Zielgruppe dar.

![](assets/audience_sharing.png)

Beide Kreise stellen eine Regel dar, die die Mitglieder einer Zielgruppe definieren. Besucher, die sich nach beiden Regeln als Mitglieder der betreffenden Zielgruppe qualifizieren (also die Schnittmenge beider Regeln bilden), gehören zur zusammengefassten Zielgruppe.

>[!NOTE]
>
>Die Zielgruppe ist erst nach Ablauf des für die Datenerfassung angegebenen Zeitraums vollständig definiert.
Nachfolgendes Beispiel zeigt, wie die Regeln für eine zusammengefasste Zielgruppe erstellt werden. Diese Zielgruppe besteht aus Folgendem:

* Home &amp; Garden-Abschnitt aus Seitendaten oder Analytics-Rohdaten
* Chrome- und Safari-Benutzer, die einem [!DNL Adobe Analytics]-Segment entnommen wurden, das in der [!DNL Experience Cloud] [veröffentlicht](../audience-library/audience-library.md#task_32FEEFE0B32E4E388CD4D892D727282A) wurde.


   ![](assets/audience_create.png)

1. Klicken Sie in der [!DNL Experience Cloud] unter [!DNL Experience Platform] auf **[!UICONTROL Personen]** &gt; **[!UICONTROL Zielgruppenbibliothek]**.
1. Klicken Sie auf der Seite [!UICONTROL „Zielgruppen“] auf **[!UICONTROL Neu]**. ![](assets/add_icon_small.png)

![Schritt Ergebnis](assets/audience_create_new.png)

1. Geben Sie auf der Seite [!UICONTROL Neue Zielgruppe erstellen] einen Titel und eine Beschreibung an.
1. Wählen Sie unter [!UICONTROL Regeln] eine Attributquelle aus:

* **[!UICONTROL Analytics-Echtzeitdaten (oder Rohdaten):]** Hierbei handelt es sich um Attributdaten, die aus Echtzeit-Bildanfragen an Analytics gewonnen werden und Daten wie eVars und Ereignisse enthalten. Wenn Sie diese Attributquelle verwenden, müssen eine Report Suite auswählen und die einbezogene Dimension oder das einbezogene Ereignis definieren. Die Auswahl dieser Report Suite stellt die Variablenstruktur bereit, die von der Report Suite verwendet wird.

   >[!NOTE]
   >
   >Aufgrund der Caching-Funktion wird die Löschung von Report Suites in Analytics erst nach 12 Stunden durch Experience Cloud übernommen.

* **[!UICONTROL Experience Cloud:]** Aus [!DNL Experience Cloud]-Quellen abgeleitete Attributdaten. Hierbei kann es sich z. B. um Daten aus Zielgruppensegmenten handeln, die Sie in [!DNL Analytics] erstellen, oder Daten aus [!DNL Audience Manager].

1. Definieren Sie die Zielgruppenregeln.

>[!NOTE]
>
>Für die Erstellung von Zielgruppenregeln sollten Sie Ihre Implementierungsvariablen unbedingt kennen.

Definieren Sie unter [!UICONTROL Regeln] die *`Home & Garden`*-Attributauswahl:

* **[!UICONTROL Attributquelle:]** Analytics-Rohdaten
* **[!UICONTROL Report Suite:]** Report Suite 31
* Dimension = **[!UICONTROL Store (Merch) (v6)]** &gt; **[!UICONTROL Entspricht]** &gt; **[!UICONTROL Home &amp; Garden]**

   ![](assets/home_garden.png)

   Die *Besucher von Chrome und Safari* sind ein in Analytics freigegebenes Zielgruppensegment:

* **[!UICONTROL Attributquelle:]** Experience Cloud
* **[!UICONTROL Dimension:]** Besucher von Chrome &amp; Safari

   ![](assets/chrome_safari.png)

   Zum Vergleich können Sie eine *OR*-Regel hinzufügen, um alle Besucher eines Site-Bereichs wie „Patio &amp; Furniture“ anzuzeigen.

   ![](assets/audiences_rule_patio.png)

1. Sehen Sie sich das Ergebnis an.

Die sich daraus ergebende Regel ist eine definierte Zielgruppe, die aus Besuchern von Chrome &amp; Safari besteht, die „Home &amp; Garden“ besucht haben. Das Segment „Patio &amp; Furniture“ bietet zusätzliche Einblicke zu allen Besuchern, die diesen Sitebereich besucht haben.

![](assets/defined_audience.png)

**Historische Schätzdaten:** (Gepunkteter Kreis) Stellt Regeln dar, die basierend auf [!DNL Analytics]-Daten erstellt wurden.

**Tatsächliche Zielgruppe:** (durchgehender Kreis) Jede erstellte Regel, die einen Datenzeitraum von 30 Tagen in Audience Manager umfasst. Wenn die Daten aus Audience Manager 30 Tage erreichen, wird die Linie durchgehend angezeigt und stellt tatsächliche Zahlen dar.

Nachdem die Datenerfassung für den angegebenen Zeitraum abgeschlossen wurde, werden die Kreise kombiniert, um eine definierte Zielgruppe anzuzeigen.

1. Klicken Sie nach der Definition der Regeln auf **[!UICONTROL Speichern]**.

Eine gespeicherte Zielgruppe steht auch anderen Lösungen zur Verfügung. Eine solchermaßen freigegebene Zielgruppe können Sie zum Beispiel auch in einer Target-Aktivität verwenden.
