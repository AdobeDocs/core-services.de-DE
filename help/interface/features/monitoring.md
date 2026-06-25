---
title: Überwachung der Nutzung der Agent-KI
description: Erfahren Sie mehr über Dashboards zur Überwachung der KI-Nutzung in CX Enterprise. Verfolgen Sie die Akzeptanz, prüfen Sie Unterhaltungen und Feedback und verwalten Sie KI-Credits für Nutzung, Qualität und Sichtbarkeit der Kosten.
solution: Experience Cloud, Experience Platform
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
autotag-review: '2026-05-27T16:30:16.764Z'
TQID: 'https://experienceleague.adobe.com/J74yr0gGkFu1bzTmMvhrQ8TNaRX6nRjWY9WAwd3uydk'
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87id: e1971122-7081-4556-9222-8a31bd71800c
feature_v2: id: f84b2906-3ce9-4ef0-86f6-cda249273937
subfeature_v2: id: cda95149-19e1-4cfa-a57e-751283a32378
topic_v2: id: bbbea26f-9621-49eb-9ab8-e06fb3bbce8c
source-git-commit: 5c3f20052f8c0a847cd0c56f02697c1d749c040c
workflow-type: tm+mt
source-wordcount: 917
ht-degree: 2%

---

# Dashboards zur Überwachung der agenten KI

Das Überwachungs-Dashboard für die agentische KI bietet Mitgliedern des Kompetenzzentrums (Center of Excellence, COE) und anderen Governance-Stakeholdern Einblicke in die Nutzung und Akzeptanz der agentischen KI. Sie können Trends über einen Zeitraum von 7 oder 30 Tagen anzeigen, um zu sehen, wer [!DNL AI Assistant] oder andere Gesprächsoberflächen (z. B. [Adobe Marketing Agent for Microsoft 365 Copilot](https://experienceleague.adobe.com/de/docs/experience-cloud-ai/experience-cloud-ai/agents/ama-ms)) verwendet, um mit [!DNL Experience Platform Agents] zu interagieren, was sie bei diesen Interaktionen tun und welchen Wert sie erhalten. Zusammen helfen diese Ansichten Ihnen, die Akzeptanz von Agenten mit Daten anstelle von Annahmen zu steuern.

**Verfügbarkeit**

* Derzeit kann jedes Konto mit einer Lizenz für mindestens ein natives Experience Platform-Programm (Customer Journey Analytics, Journey Optimizer oder Real-Time CDP) auf dieses Dashboard zugreifen
* Nutzungs- und Akzeptanzmetriken für [KI-First](agentic-ai.md#ai-first-cx-enterprise-applications)Anwendungen wie Experimentation Accelerator, LLM Optimizer, Sites Optimizer usw. sind für dieses Dashboard nicht verfügbar

Das [!UICONTROL Monitoring]-Dashboard enthält die folgenden Ansichten:

| Dashboard | Zweck |
| --- | --- |
| **Übersicht** | Aggregierte Metriken für Benutzer, Konversationen, Feedback und Kreditverbrauch |
| **Benutzer** | Nutzungshäufigkeit, Verteilung und Interaktion nach Benutzer |
| **Feedback** | Signale zur Reaktionsqualität und Benutzerzufriedenheit |
| **KI-Guthaben** | Entwicklung des Kreditverbrauchs und verbleibender Saldo |

Die für die Nutzungsüberwachung verfügbaren Agenten werden unter [KI-Agenten in vorhandenen CX Enterprise-Apps](agentic-ai.md#existing-apps-table) in der Dokumentation [Agent-KI in Adobe CX Enterprise](agentic-ai.md) aufgeführt.

>[!VIDEO](https://video.tv.adobe.com/v/3491864?learn=on)

## Dashboard-Berechtigungen aktivieren {#permissions}

Gewähren des Dashboard-Zugriffs in [!DNL Adobe Experience Platform] durch Aktualisieren des Produktprofils oder der Rolle für jeden autorisierten Benutzer. Die [!UICONTROL Monitoring]-Funktion wird Benutzern auf der Startseite von CX Enterprise angezeigt, nachdem die Berechtigungen aktiviert wurden.

1. Navigieren Sie zu [!DNL Experience Platform] **Administration** > **Berechtigungen**.

1. Öffnen Sie das Produktprofil oder die Rolle, das bzw. die Sie aktualisieren möchten.

   ![Dashboard-Berechtigungen aktivieren](../features/assets/dashboards-permissions.png)

1. Klicken Sie unter **[!UICONTROL KI]** Assistent) auf **[!UICONTROL Ressource hinzufügen]** und aktivieren Sie dann **[!UICONTROL Nutzungsdashboard des KI-Assistenten anzeigen]**.

   Diese Berechtigung gewährt Zugriff auf die Dashboards zur Überwachung der Nutzung der Agent-KI.

1. Konfigurieren **[!UICONTROL unter &quot;]**&quot; den Dashboard-Zugriff basierend auf den Verantwortlichkeiten der einzelnen Benutzer.

   ![Dashboard-Berechtigungen aktivieren](../features/assets/dashboards-add-resource.png)

   Empfohlene Berechtigungen für autorisierte Governance-Benutzer:

   * **[!UICONTROL Anzeigen des Dashboards zur Lizenznutzung]**
   * **[!UICONTROL Standard-Dashboards anzeigen]**
   * **[!UICONTROL Dashboard-Daten exportieren]** (optional, nur für genehmigte Governance-Benutzer)

   Zusätzliche Berechtigungen, die Sie bei Bedarf erteilen können:

   * **[!UICONTROL Benutzerdefinierte Dashboards verwalten]**
   * **[!UICONTROL Benutzerdefinierte Dashboards anzeigen]**
   * **[!UICONTROL Standard-Dashboards verwalten]**

1. Um Dashboards anzuzeigen, kehren Sie zur Startseite von CX Enterprise zurück und klicken Sie auf **[!UICONTROL Monitoring]**.

   ![Dashboard für die Überwachung der agenten KI](../features/assets/monitoring.png)

## Übersichts-Dashboard

Das Übersichts-Dashboard ist der zentrale Ort für Akzeptanz- und Interaktionsmetriken in Ihrer gesamten Organisation. Er verbindet allgemeine Trends mit einer tieferen Analyse. Für jede Metrik können Sie einen Drilldown in einzelne Konversationen durchführen, um zu sehen, was die Zahlen antreibt.

### Metriken im Dashboard „Übersicht“

* **Eingabeaufforderungen im Zeitverlauf:** Gesamtnutzungswachstum und Akzeptanztrends.
* **Aktive Benutzer und Konversationen:** Anzahl der Benutzer, die mit [!DNL Experience Platform Agents] interagieren.
* **Durchschnittliche Eingabeaufforderungen pro Konversation:** Interaktionstiefe pro Konversation.
* **Feedback** Verteilung der Daumen hoch und Daumen runter Feedback von Benutzern (nur für [!DNL AI Assistant] Interaktionen).

>[!VIDEO](https://video.tv.adobe.com/v/3491865?learn=on)

### Unterhaltungswiederholung

Die Gesprächswiederholung zeigt individuelle Interaktionen, nicht nur Aggregate. Sie können Muster in vielen Unterhaltungen analysieren und von allgemeinen Trends zu einer bestimmten Unterhaltung wechseln.

* **Eingabeaufforderung und Antwortverlauf:** Die Eingabeaufforderung und die zugestellten Antworten des Benutzers.
* **Feedback-Signale:** Interactions-Benutzende, die mit einem Daumen nach oben oder unten gekennzeichnet sind, um Reibungs-, Blocker- oder Aktivierungsanforderungen zu identifizieren. Diese Informationen helfen Ihrem Unternehmen, die Relevanz der Anfragen schnell zu verbessern, und helfen Adobe, die Reaktionsqualität im Laufe der Zeit zu verbessern.

>[!VIDEO](https://video.tv.adobe.com/v/3491866?learn=on)

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

>[!VIDEO](https://video.tv.adobe.com/v/3491868?learn=on)

## Feedback-Dashboard

Das Feedback-Dashboard zeigt das Benutzer-Feedback an, das für Agenten-Interaktionen gesendet wurde. Sie können sehen, welche Konversationen Benutzer positiv oder negativ bewertet haben, und die Interaktionen hinter dem Feedback untersuchen. Zeigen Sie in Feedback-Zusammenfassungen einzelne Konversationen an, um Eingabeaufforderungen, Antworten, Argumentationsdetails und Feedback-Notizen zu überprüfen.

### Metriken im Feedback-Dashboard

* **Feedback-Trends im Zeitverlauf:** Wie sich das Benutzer-Feedback im Laufe der Zeit ändert.
* **Daumen hoch und Daumen runter Feedback:** positive und negative Interaktionssignale.
* **Feedback-Kategorien:** Rationale hinter jedem Daumen nach oben und Daumen nach unten.
* **Eingabeaufforderung und Antwortverlauf:** Benutzeraufforderungen und die Antworten, die mit gesendetem Feedback verknüpft sind.
* **Feedback-Details und -Hinweise** Zusätzlicher Kontext und Kommentare von Benutzern während der Übermittlung des Feedbacks.

>[!VIDEO](https://video.tv.adobe.com/v/3491878?learn=on)

## Dashboard für KI-Gutschriften

Das Dashboard „KI-Guthaben“ zeigt an, wie die Verwendung von [!DNL Experience Platform Agents] in Ihrem Unternehmen zur Nutzung von KI-Guthaben führt.

### Metriken im Dashboard für KI-Gutschriften

* **Insgesamt genutzte KI-Credits** Gesamte Agentennutzung in KI-Credits.
* **Tägliche und monatliche Trends** Spitzen, Tiefpunkte und Veränderungen der Konsummuster.
* **Verbleibende KI-Credits:** Restguthaben, damit Sie proaktiv planen und Überschüsse vermeiden können.

>[!VIDEO](https://video.tv.adobe.com/v/3491867?learn=on)

## Weitere Hilfe zu diesem Thema

* [Lizenznutzungs-Dashboard](https://experienceleague.adobe.com/en/docs/experience-platform/dashboards/guides/license-usage) in [!DNL Experience Platform]
* [Agent-KI in Adobe CX Enterprise](agentic-ai.md)
* [Agent-Vorgänge und KI-Kreditverbrauch](ai-credit-consumption.md)
* [Lizenznutzungs-Dashboard](https://experienceleague.adobe.com/en/docs/experience-platform/dashboards/guides/license-usage) (Experience Platform)
