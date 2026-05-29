---
title: Überwachung der Nutzung der Agent-KI
description: Erfahren Sie mehr über die Überwachung der KI-Nutzung in CX Enterprise. Verfolgen Sie die Akzeptanz, prüfen Sie Unterhaltungen und Feedback und verwalten Sie KI-Credits für Nutzung, Qualität und Sichtbarkeit der Kosten.
solution: Experience Cloud, Experience Platform
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
autotag-review: '2026-05-27T16:30:16.764Z'
TQID: 'https://experienceleague.adobe.com/J74yr0gGkFu1bzTmMvhrQ8TNaRX6nRjWY9WAwd3uydk'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
  - id: e1971122-7081-4556-9222-8a31bd71800c
feature_v2:
  - id: f84b2906-3ce9-4ef0-86f6-cda249273937
subfeature_v2:
  - id: cda95149-19e1-4cfa-a57e-751283a32378
topic_v2:
  - id: bbbea26f-9621-49eb-9ab8-e06fb3bbce8c
source-git-commit: 294e1638dc175d94fcd01927dbc6e6caafddf3f6
workflow-type: tm+mt
source-wordcount: 948
ht-degree: 2%

---

# Dashboard zur Überwachung der KI-Nutzung durch Agenten

CX Enterprise bietet zwei Dashboards zur Überwachung der Nutzung der Agent-KI in vorhandenen CX Enterprise-Anwendungen. Diese Dashboards helfen Ihnen, Akzeptanz, Interaktion, Feedback-Qualität und KI-Kreditnutzung für [!DNL Experience Platform Agents] zu verstehen, auf die Benutzer über [!DNL AI Assistant] und andere Gesprächsoberflächen zugreifen.

Die für die Nutzungsüberwachung verfügbaren Agenten werden unter [KI-Agenten in vorhandenen CX Enterprise-Apps](agentic-ai.md#existing-apps-table) in der Dokumentation [Agent-KI in Adobe CX Enterprise](agentic-ai.md) aufgeführt.

## Lizenznutzungs-Dashboard

Das Dashboard zur [!DNL Adobe Experience Platform] Lizenznutzung zeigt die Berechtigung für lizenzierte KI-Credits Ihres Unternehmens und die gesamten KI-Credits an, die verwendet werden, wenn Benutzer [!DNL Experience Platform Agents] ausführen.

Administratoren verwenden dieses Dashboard, um die Lizenznutzung im Vergleich zur Berechtigung zu verfolgen. Weitere Informationen über den Zugriff auf das Dashboard finden [&#x200B; unter „Lizenznutzungs](https://experienceleague.adobe.com/en/docs/experience-platform/dashboards/guides/license-usage)Dashboard“ in [!DNL Experience Platform] Dokumentation.

## Dashboard für die Überwachung der agenten KI

Das Überwachungs-Dashboard für die agentische KI bietet Mitgliedern des Kompetenzzentrums (Center of Excellence, COE) und anderen Governance-Stakeholdern Einblicke in die Nutzung und Akzeptanz der agentischen KI. Sie können Trends über einen Zeitraum von 7 oder 30 Tagen anzeigen, um zu sehen, wer [!DNL AI Assistant] oder andere Gesprächsoberflächen (z. B. [Adobe Marketing Agent for Microsoft 365 Copilot](https://experienceleague.adobe.com/de/docs/experience-cloud-ai/experience-cloud-ai/agents/ama-ms)) verwendet, um mit [!DNL Experience Platform Agents] zu interagieren, was sie bei diesen Interaktionen tun und welchen Wert sie erhalten.

Das Dashboard für die Überwachung der Agent-KI umfasst die folgenden Ansichten:

| Dashboard | Zweck |
| --- | --- |
| **Übersicht** | Aggregierte Metriken für Benutzer, Konversationen, Feedback und Kreditverbrauch |
| **Benutzer** | Nutzungshäufigkeit, Verteilung und Interaktion nach Benutzer |
| **Feedback** | Signale zur Reaktionsqualität und Benutzerzufriedenheit |
| **KI-Guthaben** | Entwicklung des Kreditverbrauchs und verbleibender Saldo |

Zusammen helfen diese Ansichten Ihnen, die Akzeptanz von Agenten mit Daten anstelle von Annahmen zu steuern.

## Übersichts-Dashboard

Das Übersichts-Dashboard ist der zentrale Ort für Akzeptanz- und Interaktionsmetriken in Ihrer gesamten Organisation. Er verbindet allgemeine Trends mit einer tieferen Analyse. Für jede Metrik können Sie einen Drilldown in einzelne Konversationen durchführen, um zu sehen, was die Zahlen antreibt.

### Metriken im Dashboard „Übersicht“

* **Eingabeaufforderungen im Zeitverlauf:** Gesamtnutzungswachstum und Akzeptanztrends.
* **Aktive Benutzer und Konversationen:** Anzahl der Benutzer, die mit [!DNL Experience Platform Agents] interagieren.
* **Durchschnittliche Eingabeaufforderungen pro Konversation:** Interaktionstiefe pro Konversation.
* **Feedback** Verteilung der Daumen hoch und Daumen runter Feedback von Benutzern (nur für [!DNL AI Assistant] Interaktionen).

### Unterhaltungswiederholung

Die Gesprächswiederholung zeigt individuelle Interaktionen, nicht nur Aggregate. Sie können Muster in vielen Unterhaltungen analysieren und von allgemeinen Trends zu einer bestimmten Unterhaltung wechseln.

* **Eingabeaufforderung und Antwortverlauf:** Die Eingabeaufforderung und die zugestellten Antworten des Benutzers.
* **Feedback-Signale:** Interactions-Benutzende, die mit einem Daumen nach oben oder unten gekennzeichnet sind, um Reibungs-, Blocker- oder Aktivierungsanforderungen zu identifizieren. Diese Informationen helfen Ihrem Unternehmen, die Relevanz der Anfragen schnell zu verbessern, und helfen Adobe, die Reaktionsqualität im Laufe der Zeit zu verbessern.

## Benutzer-Dashboard

Das Benutzer-Dashboard zeigt, wie sich die Akzeptanz und Interaktion von Agenten je nach Benutzer im Laufe der Zeit verändert. Sie können sehen, wer [!DNL Experience Platform Agents] aktiv nutzt, welche Oberfläche er nutzt und wie oft er damit interagiert. Admins und Code-Mitglieder können einen Drill-in in einzelne Benutzeraktivitäten und Konversationen durchführen, um Interaktionsmuster und Nutzungsverhalten zu verstehen.

### Metriken im Benutzer-Dashboard

* **Akzeptanz- und Interaktionstrends im Zeitverlauf:** Verfolgen Sie, wie sich Benutzersegmente im ausgewählten Zeitraum ändern. Benutzer werden klassifiziert als:
   * **Neu** Erste Aktivität im ausgewählten Zeitraum, ohne Aktivität in den letzten 12 Monaten.
   * **Wiederholen:** Aktivität sowohl im ausgewählten Zeitraum als auch im vorherigen Zeitraum.
   * **Zurück** Die Aktivität im ausgewählten Zeitraum, aber nicht im vorherigen Zeitraum.
   * **Inaktiv** Keine Aktivität im ausgewählten Zeitraum, aber Aktivität im vorherigen Zeitraum.
* **Benutzerinteraktionsmuster:** wie oft Benutzer mit Agenten interagieren und wie sich die Interaktion im Laufe der Zeit verändert.
* **Konversationsaktivität:** Anzahl der Konversationen und Eingabeaufforderungen pro Benutzer.
* **Top-aktive Benutzer:** Starke Interaktion zwischen Benutzern und Teams, die die Akzeptanz von Agenten fördert.

## Feedback-Dashboard

Das Feedback-Dashboard zeigt das Benutzer-Feedback an, das für Agenten-Interaktionen gesendet wurde. Sie können sehen, welche Konversationen Benutzer positiv oder negativ bewertet haben, und die Interaktionen hinter dem Feedback untersuchen. Zeigen Sie in Feedback-Zusammenfassungen einzelne Konversationen an, um Eingabeaufforderungen, Antworten, Argumentationsdetails und Feedback-Notizen zu überprüfen.

### Metriken im Feedback-Dashboard

* **Feedback-Trends im Zeitverlauf:** Wie sich das Benutzer-Feedback im Laufe der Zeit ändert.
* **Daumen hoch und Daumen runter Feedback:** positive und negative Interaktionssignale.
* **Feedback-Kategorien:** Rationale hinter jedem Daumen nach oben und Daumen nach unten.
* **Eingabeaufforderung und Antwortverlauf:** Benutzeraufforderungen und die Antworten, die mit gesendetem Feedback verknüpft sind.
* **Feedback-Details und -Hinweise** Zusätzlicher Kontext und Kommentare von Benutzern während der Übermittlung des Feedbacks.

## Dashboard für KI-Gutschriften

Das Dashboard „KI-Guthaben“ zeigt an, wie die Verwendung von [!DNL Experience Platform Agents] in Ihrem Unternehmen zur Nutzung von KI-Guthaben führt.

### Metriken im Dashboard für KI-Gutschriften

* **Insgesamt genutzte KI-Credits** Gesamte Agentennutzung in KI-Credits.
* **Tägliche und monatliche Trends** Spitzen, Tiefpunkte und Veränderungen der Konsummuster.
* **Verbleibende KI-Credits:** Restguthaben, damit Sie proaktiv planen und Überschüsse vermeiden können.

## Zugang und Governance

Dashboards zur Überwachung der Nutzung der agenten KI stellen die KI-Assistentenaktivität zur Verfügung, einschließlich Nutzungsmustern, Einblicken auf Konversationsebene, Feedback-Signalen und Betriebsmetriken. Einige dieser Informationen können sensible Geschäftskontexte, sofortige Aktivität oder Benutzerinteraktionsdaten umfassen.

Der Zugriff ist berechtigungsbasiert und nur für autorisierte Code-Administratoren und genehmigte Governance-Benutzer vorgesehen. Im folgenden Abschnitt wird beschrieben, wie Sie Dashboard-Berechtigungen erteilen.

## Dashboard-Berechtigungen aktivieren

Gewähren des Dashboard-Zugriffs in [!DNL Adobe Experience Platform] durch Aktualisieren des Produktprofils oder der Rolle für jeden autorisierten Benutzer.

1. Navigieren Sie zu [!DNL Experience Platform] **Administration** > **Berechtigungen**.

1. Öffnen Sie das Produktprofil oder die Rolle, das bzw. die Sie aktualisieren möchten.

   ![Dashboard-Berechtigungen aktivieren](../features/assets/dashboards-permissions.png)

1. Klicken Sie unter **[!UICONTROL AI Assistant]** Berechtigungen auf **[!UICONTROL Add Resource]** und dann auf **[!UICONTROL View AI Assistant usage dashboard]** aktivieren .

   Diese Berechtigung gewährt Zugriff auf die Dashboards zur Überwachung der Nutzung der Agent-KI.

1. Konfigurieren Sie unter **[!UICONTROL Dashboards]** Berechtigungen den Dashboard-Zugriff basierend auf den Zuständigkeiten der einzelnen Benutzer.

   ![Dashboard-Berechtigungen aktivieren](../features/assets/dashboards-add-resource.png)

   Empfohlene Berechtigungen für autorisierte Governance-Benutzer:

   * **[!UICONTROL View License Usage Dashboard]**
   * **[!UICONTROL View Standard Dashboards]**
   * **[!UICONTROL Export Dashboard Data]** (optional, nur für genehmigte Governance-Benutzer)

   Zusätzliche Berechtigungen, die Sie bei Bedarf erteilen können:

   * **[!UICONTROL Manage Custom Dashboards]**
   * **[!UICONTROL View Custom Dashboards]**
   * **[!UICONTROL Manage Standard Dashboards]**

## Weitere Hilfe zu diesem Thema

* [Agent-KI in Adobe CX Enterprise](agentic-ai.md)
* [Agent-Vorgänge und KI-Kreditverbrauch](ai-credit-consumption.md)
* [Lizenznutzungs-Dashboard](https://experienceleague.adobe.com/en/docs/experience-platform/dashboards/guides/license-usage) (Experience Platform)
