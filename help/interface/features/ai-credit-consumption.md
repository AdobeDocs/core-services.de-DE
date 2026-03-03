---
title: Agent-Vorgänge und KI-Kreditverbrauch
description: Erfahren Sie mehr über Agentenaufträge und KI-Kreditverbrauchsraten in Experience Cloud-Programmen.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
source-git-commit: d4734c4b43defedb20b7eb65556f56987dce02ae
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 3%

---

# Nutzung von Adobe Experience Platform-Agentenvorgängen und KI-Credits

Aktualisiert: **Mittwoch, 3. März 2026**

Erfahren Sie mehr über die Verwendung von agenten KI-Aufträgen und die Verwendung von KI-Krediten in Experience Cloud-Programmen. Informationen zur Aktivierung der Funktionen der agenten KI in bestehenden Experience Cloud-Programmen finden Sie unter [Agentische KI in Experience Cloud](agentic-ai.md#existing-apps).

## Agentenaufträge

Ein _Agentenauftrag_ ist eine Reihe von Aufgaben und Aktionen, die ein Agent ausführt, um ein bestimmtes Ergebnis zu erzielen, wie durch Kundeneingaben angewiesen.

Mithilfe natürlicher Eingabeaufforderungen über den KI-Assistenten können Sie Agenten bitten, bestimmte Aufträge auszuführen. Basierend auf diesen Eingaben koordiniert Agent Orchestrator die entsprechenden Agenten, um jeden Schritt in den entsprechenden Experience Cloud-Programmen auszuführen.

## KI-Credits

Ein _KI-_) ist eine nutzungsbasierte Metrik, die die Ausführung von Agentenvorgängen quantifiziert. KI-Credits gelten nicht für [KI-First-Anwendungen](/help/interface/features/agentic-ai.md).

## KI-Kreditnutzung

Die Verwendung von KI-Guthaben kann je nach Komplexität und Wert des ausgeführten Auftrags variieren:

* Einfache (oft einstufige) Aufgaben verbrauchen weniger Guthaben
* Komplexe (oft mehrstufige) Aufgaben verbrauchen mehr Guthaben
* Aufgaben mit erweitertem Argumentieren, Validierung, Koordination mit mehreren Agenten oder Integration verbrauchen mehr Credits

### Geschätzte KI-Kreditverbrauchsraten

| Agent | Job | Unterstützte Anwendungen | Geschätzte KI-Guthaben | Eingabeaufforderungen im Beispiel |
| ------ | ----- | ------------------------ | ----------------------- | ----------------- |
| Audience Agent | Zielgruppen-/Konto-Ideen | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 50 | <ul><li>_Felder für wohlhabende Käufer anzeigen_</li><li>_Ermitteln Sie alle Felder im Zusammenhang mit Kundenpräferenzen_</li></ul> |
| Audience Agent | Wissensbasierte Zielgruppe/Kontoerstellung | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 150 | <ul><li>_Erstellen Sie eine Zielgruppe aus Personen, die in Kalifornien leben_</li><li>_Generieren Sie eine Zielgruppe aus VIP-Mitgliedern, die in diesem Quartal mehr als 1.000 US-Dollar ausgegeben haben_</li><li>_Erstellen Sie eine Zielgruppe aus Benutzern, die Bekleidungsartikel gekauft, aber in den letzten 60 Tagen keinen Kauf getätigt haben_</li></ul> |
| Audience Agent | Zielgruppen-/Kontoverwaltung | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li>_Habe ich doppelte Zielgruppen?_</li><li>_Zeige mir meine 5 größten Audiences._</li><li>_Anzeigen von Zielgruppen, die für kein Ziel aktiviert sind_</li><li>_Listen Sie alle Zielgruppen auf, die in Live-Journey verwendet werden_</li></ul> |
| Audience Agent | Zielgruppen-/Kontoanalyse | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li>_Welche Zielgruppen haben in der letzten Woche um mehr als 20 % zugenommen?_</li><li>_Wie sehr hat sich das Publikum „Loyales Platin“ im Vergleich zum Wert vor 30 Tagen verändert?_</li><li>_Was ist mein am schnellsten wachsendes Publikum?_</li></ul> |
| Audience Agent | Einkaufsgruppenidee | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li>_Welche Konten geben die Absicht für diese Produkte an?_</li><li>_Zeigen Sie mir die wichtigsten Personen nach Produktabsicht für XYZ._</li><li>_Welche Einkaufsgruppen haben mehr als 5 Mitglieder?_</li></ul> |
| Data Insights Agent | Datenanalyse und -visualisierung | <ul><li>Customer Journey Analytics (B2C- und B2B-Editionen)</li></ul> | 25 | <ul><li>_Trend der Bestellungen im Juli_</li><li>_Umsatz nach Region anzeigen._</li><li>_Bestellungen nach Geschlecht anzeigen, von März bis Juni._</li><li>_Was waren meine Top 10 SKUs mit Gewinn im Juni_</li><li>_Anteil der Käufe nach Monat des Jahres_</li><li>_Umsatzanteil nach Produktkategorie_</li></ul> |
| Journey Agent | Journey | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li>_Erstellen Sie eine Journey für Whitespace-Konten mit dem Zweck für meine Lösung, mit Schwerpunkt auf Personen, die mit Inhalten auf der Website interagieren_</li></ul> |
| Journey Agent | Journey-Erstellung | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> | 30 | <ul><li>_Erstellen Sie eine Journey, um eine Erinnerung an Benutzende zu senden, die ihren ersten Kauf in den letzten sieben Tagen nicht abgeschlossen haben_</li><li>_Wenn Benutzer ihren ersten Kauf abschließen, senden Sie nach 3 Tagen per E-Mail eine SMS-Bestätigung und eine Erklärung der Folgevorteile_</li></ul> |
| Journey Agent | Journey-Analyse | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> | 50 | <ul><li>_Ich möchte den Fallout nach Knoten für das Journey am vierten Juli von Campaign analysieren._</li><li>_Gibt es Planungskonflikte für Journey X_</li><li>_Konflikte mit Zielgruppenüberschneidungen für Journey X anzeigen_</li></ul> |
| Journey Agent | Journey-Verwaltung | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> | 25 | <ul><li>_Wie viele lebende Journey habe ich?_</li><li>_Listen Sie alle Journey mit der Audience X auf._</li><li>_Listen Sie alle Journey auf, die sich derzeit im Testmodus befinden_</li></ul> |
| Produktsupport-Agent | Knowledge-based Troubleshooting | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C- und B2B-Editionen)</li><li>Customer Journey Analytics (B2C- und B2B-Editionen)</li></ul> | 0 | <ul><li>_Warum unterscheidet sich die Anzahl meiner Profile im Lizenznutzungs-Dashboard und auf der Experience Platform-Startseite?_</li><li>_Was sind die Gründe dafür, dass eine Journey nicht ausgelöst wird?_</li><li>_Wie erstellt Adobe Experience Platform Echtzeit-Erlebnisse?_</li><li>_Wie werden Warnhinweise in Adobe Experience Platform konfiguriert und verwendet?_</li><li>_Wie hoch ist die Grenze für die durchschnittliche Profilreichhaltigkeit in Adobe Experience Platform Activation?_</li></ul> |
| Produktsupport-Agent | Erstellung und Nachverfolgung von Support-Fällen | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li>Adobe Journey Optimizer (B2C- und B2B-Editionen)<li>Customer Journey Analytics (B2C- und B2B-Editionen)</li><li>Adobe Experience Manager</li></ul> | 10 | <ul><li>_Erstellen Sie ein neues Support-Ticket für meinen fehlgeschlagenen Segmentierungsauftrag_</li><li>_Wie ist der Status des Tickets E-001772068?_</li></ul> |
| Inhaltsratgeber-Agent | Inhaltserkennung | <ul><li>Adobe Experience Manager Assets</li></ul> | 5 | <ul><li>_Inhaltsfragmente zum Erstellen einer WKND-Angebotskampagne anzeigen._</li><li>_Produktverpackung finden PNG-Bilder._</li><li>_Bilder mit Tag in Office-Ordner anzeigen WKND._</li><li>_Gibt es SVGs im Ordner WKND?_</li><li>_Alle Kreditantragsformulare anzeigen._</li><li>_Ich suche Onboarding-Formulare für Mitarbeiter._</li></ul> |
| Inhaltsratgeber-Agent | <ul><li>Inhaltsoptimierung</li></ul> | <ul><li>Adobe Experience Manager Assets</li></ul> | 10 | <ul><li>_Erstellen Sie eine Ausgabedarstellung von 2.000 Pixel als JPEG mit 80 % Qualität._</li><li>_Erstellen Sie eine Ausgabedarstellung für eine Instagram-Story._</li><li>_Überlagern Sie das Bild mit 30 % Rabattgrafiken über dem Werbebanner und platzieren Sie es 100 Pixel von der Mitte entfernt._</li><li>_Ändern Sie die Hintergrundfarbe des PNG in #ff8932._</li></ul> |
| Brand Experience Agent | <ul><li>Inhaltsaktualisierung</li><li>Forms-Erstellung</li><li>Fehlerbehebung bei Pipelines</li></ul> | <ul><li>Adobe Experience Manager Cloud Services</li><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Forms</li></ul> | 50 | <ul><li>_Fehlerbehebung bei fehlgeschlagener Pipeline_</li><li>_Auflisten meiner fehlgeschlagenen Pipelines für das Hauptprogramm._</li><li>_Analysieren Sie meine fehlgeschlagene Pipeline mit dem Namen „Entwicklungs-Pipeline“_</li><li>_Fehlerbehebung bei der Pipeline-Ausführung 1234567_</li></ul> |
| Brand Experience Agent | Site-Modernisierung | Adobe Experience Manager Cloud Services | 100 | <ul><li>_Migrieren der`https://wknd-trendsetters.site`_</li></ul> |

>[!NOTE]
>
>Der tatsächliche KI-Kreditverbrauch kann je nach der Anzahl der ausgeführten Schritte und Iterationen pro Schritt variieren.

## Weitere Hilfe zu diesem Thema

* [Agent AI in Experience Cloud](/help/interface/features/agentic-ai.md)
* [Nutzungsgebundene Testversion für Adobe Experience Platform-Agenten](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)
