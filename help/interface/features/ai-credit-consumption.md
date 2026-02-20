---
title: Agent-Vorgänge und KI-Kreditverbrauch
description: Erfahren Sie mehr über Agentenaufträge und KI-Kreditverbrauchsraten in Experience Cloud-Programmen.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
source-git-commit: bb6adf13bed37d4a885b5baec28199efade592e1
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# Nutzung von Adobe Experience Platform-Agentenvorgängen und KI-Credits

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
| ------ |-----|------------------------|----------------------|----------------|
| Audience Agent | Zielgruppen-/Konto-Ideen | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 50 | <ul><li>Felder für wohlhabende Käufer anzeigen</li><li>Alle Felder für Kundeneinstellungen suchen</li></ul> |
| Audience Agent | Wissensbasierte Zielgruppe/Kontoerstellung | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 150 | <ul><li>Erstellen Sie eine Zielgruppe, die aus Personen besteht, die in Kalifornien leben</li><li>Erzeugt eine Audience von VIP-Mitgliedern, die in diesem Quartal mehr als 1000 USD ausgegeben haben</li><li>Eine Zielgruppe aus Benutzern erstellen, die Bekleidungsartikel gekauft, aber in den letzten 60 Tagen keinen Kauf getätigt haben</li></ul> |
| Audience Agent | Zielgruppen-/Kontoverwaltung | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li>Habe ich doppelte Zielgruppen?</li><li>Zeigen Sie mir meine 5 größten Audiences.</li><li>Anzeigen von Zielgruppen, die für kein Ziel aktiviert sind</li><li>Auflisten aller in Live-Journey verwendeten Zielgruppen</li></ul> |
| Audience Agent | Zielgruppen-/Kontoanalyse | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li>Welche Zielgruppen haben in der letzten Woche um mehr als 20 % zugenommen?</li><li>Wie stark hat sich das Publikum „Loyal Platinum“ im Vergleich zum Wert vor 30 Tagen verändert?</li><li>Welches ist mein am schnellsten wachsendes Publikum?</li></ul> |
| Audience Agent | Einkaufsgruppenidee | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li>Welche Konten geben die Absicht für diese Produkte an?</li><li>Zeigen Sie mir die wichtigsten Personen nach Produktabsicht für XYZ.</li><li>Welche Einkaufsgruppen haben mehr als 5 Mitglieder?</li></ul> |
| Data Insights Agent | Datenanalyse und -visualisierung | <ul><li>Customer Journey Analytics (B2C- und B2B-Editionen)</li></ul> | 25 | <ul><li>Trend der Bestellungen im Juli</li><li>Umsatz nach Region anzeigen.</li><li>Bestellungen nach Geschlecht anzeigen, von März bis Juni.</li><li>Was waren meine Top 10 SKUs mit Gewinn im Juni?</li><li>Anteil der Käufe nach Monat des Jahres</li><li>Umsatzanteil nach Produktkategorie</li></ul> |
| Journey Agent | Journey | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li>Erstellen Sie eine Journey für Whitespace-Konten mit dem Zweck für meine Lösung, mit Schwerpunkt auf Personen, die mit Inhalten auf der Website interagieren</li></ul> |
| Journey Agent | Journey-Erstellung | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> | 30 | <ul><li>Generieren einer Journey, um eine Erinnerung an Benutzende zu senden, die ihren ersten Kauf in den letzten sieben Tagen nicht abgeschlossen haben</li><li>Wenn Benutzer ihren ersten Kauf abschließen, senden Sie nach 3 Tagen per E-Mail eine SMS-Bestätigung und eine Erklärung der Folgevorteile</li></ul> |
| Journey Agent | Journey-Analyse | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> | 50 | <ul><li>Ich möchte den Fallout nach Knoten für das Journey der Kampagne vom 4. Juli analysieren.</li><li>Gibt es Planungskonflikte für Journey X?</li><li>Konflikte mit Zielgruppenüberschneidungen für Journey X anzeigen</li></ul> |
| Journey Agent | Journey-Verwaltung | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> | 25 | <ul><li>Wie viele lebende Journey habe ich?</li><li>Listen Sie alle Journey auf, die Audience X verwenden.</li><li>Auflisten aller Journey, die sich derzeit im Testmodus befinden</li></ul> |
| Produktsupport-Agent | Knowledge-based Troubleshooting | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C- und B2B-Editionen)</li><li>Customer Journey Analytics (B2C- und B2B-Editionen)</li></ul> | 0 | <ul><li>Warum unterscheidet sich die Anzahl meiner Profile im Lizenznutzungs-Dashboard und auf der Experience Platform-Startseite?</li><li>Was sind die Gründe dafür, dass eine Journey nicht ausgelöst wird?</li><li>Wie erstellt Adobe Experience Platform Echtzeit-Erlebnisse?</li><li>Wie werden Warnhinweise in Adobe Experience Platform konfiguriert und verwendet?</li><li>Wie hoch ist die Grenze für die durchschnittliche Profilreichhaltigkeit in Adobe Experience Platform Activation?</li></ul> |
| Produktsupport-Agent | Erstellung und Nachverfolgung von Support-Fällen | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li>Adobe Journey Optimizer (B2C- und B2B-Editionen)<li>Customer Journey Analytics (B2C- und B2B-Editionen)</li><li>Adobe Experience Manager</li></ul> | 10 | <ul><li>Erstellen Sie ein neues Support-Ticket für meinen fehlgeschlagenen Segmentierungsauftrag</li><li>Wie ist der Status von Ticket E-001772068?</li></ul> |
| Inhaltsratgeber-Agent | Inhaltserkennung | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 5 | <ul><li>Inhaltsfragmente zum Erstellen einer WKND-Angebotskampagne anzeigen.</li><li>Suchen Sie Produktverpackung PNG-Bilder.</li><li>Bilder mit Tag im Ordner „Office“ in WKND anzeigen.</li><li>Gibt es SVGs im Ordner WKND?</li><li>Alle Kreditantragsformulare anzeigen.</li><li>Ich suche Onboarding-Formulare für Mitarbeiter.</li></ul> |
| Inhaltsratgeber-Agent | <ul><li>Inhaltsaktualisierung</li><li>Inhaltsoptimierung</li><li>Forms-Erstellung</li></ul> | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 10 | <ul><li>Erstellen Sie eine Ausgabedarstellung von 2.000 Pixel als JPEG mit einer Qualität von 80 %.</li><li>Erstellen Sie eine Ausgabedarstellung für eine Instagram-Story.</li><li>Überlagern Sie das Bild mit 30 % Rabatt-Grafiken über dem Werbebanner und platzieren Sie es 100 Pixel von der Mitte entfernt.</li><li>Ändern Sie die Hintergrundfarbe des PNG in #ff8932.</li></ul> |
| Brand Experience Agent | <ul><li>Experience Support</li><li>Bereitstellungs-Support</li></ul> | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 5 | <ul><li>Fehlerbehebung bei fehlgeschlagener Pipeline</li><li>Meine fehlgeschlagenen Pipelines für das Hauptprogramm auflisten.</li><li>Analysieren Sie meine fehlgeschlagene Pipeline mit dem Namen „Entwicklungs-Pipeline“.</li><li>Fehlerbehebung bei der Pipeline-1234567</li></ul> |
| Brand Experience Agent | Site-Modernisierung | Adobe Experience Manager Cloud Services | 100 | <ul><li>Migrieren der Seite https://wknd-trendsetters.site</li></ul> |

>[!NOTE]
>
>Der tatsächliche KI-Kreditverbrauch kann je nach der Anzahl der ausgeführten Schritte und Iterationen pro Schritt variieren.

## Weitere Hilfe zu diesem Thema

* [Agent AI in Experience Cloud](/help/interface/features/agentic-ai.md)
* [Nutzungsgebundene Testversion für Adobe Experience Platform-Agenten](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)