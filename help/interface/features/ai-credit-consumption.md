---
title: Agent-Vorgänge und KI-Kreditverbrauch
description: Erfahren Sie mehr über Agentenaufträge und KI-Kreditverbrauchsraten in Experience Cloud-Programmen.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
source-git-commit: 6a7cd999ec96967084c67d059cb2efd6a3235235
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 3%

---

# Nutzung von Adobe Experience Platform-Agentenvorgängen und KI-Credits

Aktualisiert: **Freitag, 5. März 2026**

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
| Audience Agent | Zielgruppen-/Konto-Ideen | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 50 | <ul><li><em>Felder für wohlhabende Käufer anzeigen</em></li><li><em>Ermitteln Sie alle Felder im Zusammenhang mit Kundenpräferenzen</em></li></ul> |
| Audience Agent | Wissensbasierte Zielgruppe/Kontoerstellung | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 150 | <ul><li><em>Erstellen Sie eine Zielgruppe aus Personen, die in Kalifornien leben</em></li><li><em>Generieren Sie eine Zielgruppe aus VIP-Mitgliedern, die in diesem Quartal mehr als 1.000 US-Dollar ausgegeben haben</em></li><li><em>Erstellen Sie eine Zielgruppe aus Benutzern, die Bekleidungsartikel gekauft, aber in den letzten 60 Tagen keinen Kauf getätigt haben</em></li></ul> |
| Audience Agent | Zielgruppen-/Kontoverwaltung | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li><em>Habe ich doppelte Zielgruppen?</em></li><li><em>Zeige mir meine 5 größten Audiences.</em></li><li><em>Anzeigen von Zielgruppen, die für kein Ziel aktiviert sind</em></li><li><em>Listen Sie alle Zielgruppen auf, die in Live-Journey verwendet werden</em></li></ul> |
| Audience Agent | Zielgruppen-/Kontoanalyse | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li><em>Welche Zielgruppen haben in der letzten Woche um mehr als 20 % zugenommen?</em></li><li><em>Wie sehr hat sich das Publikum „Loyales Platin“ im Vergleich zum Wert vor 30 Tagen verändert?</em></li><li><em>Was ist mein am schnellsten wachsendes Publikum?</em></li></ul> |
| Audience Agent | Einkaufsgruppenidee | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li><em>Welche Konten geben die Absicht für diese Produkte an?</em></li><li><em>Zeigen Sie mir die wichtigsten Personen nach Produktabsicht für XYZ.</em></li><li><em>Welche Einkaufsgruppen haben mehr als 5 Mitglieder?</em></li></ul> |
| Data Insights Agent | Datenanalyse und -visualisierung | <ul><li>Customer Journey Analytics (B2C- und B2B-Editionen)</li></ul> | 25 | <ul><li><em>Trend der Bestellungen im Juli</em></li><li><em>Umsatz nach Region anzeigen.</em></li><li><em>Bestellungen nach Geschlecht anzeigen, von März bis Juni.</em></li><li><em>Was waren meine Top 10 SKUs mit Gewinn im Juni</em></li><li><em>Anteil der Käufe nach Monat des Jahres</em></li><li><em>Umsatzanteil nach Produktkategorie</em></li></ul> |
| Journey Agent | Journey | <ul><li>Adobe Journey Optimizer (B2B edition)</li></ul> | 25 | <ul><li><em>Erstellen Sie eine Journey für Whitespace-Konten mit dem Zweck für meine Lösung, mit Schwerpunkt auf Personen, die mit Inhalten auf der Website interagieren</em></li></ul> |
| Journey Agent | Journey-Erstellung | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> | 30 | <ul><li><em>Erstellen Sie eine Journey, um eine Erinnerung an Benutzende zu senden, die ihren ersten Kauf in den letzten sieben Tagen nicht abgeschlossen haben</em></li><li><em>Wenn Benutzer ihren ersten Kauf abschließen, senden Sie nach 3 Tagen per E-Mail eine SMS-Bestätigung und eine Erklärung der Folgevorteile</em></li></ul> |
| Journey Agent | Journey-Analyse | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> | 50 | <ul><li><em>Ich möchte den Fallout nach Knoten für das Journey am vierten Juli von Campaign analysieren.</em></li><li><em>Gibt es Planungskonflikte für Journey X</em></li><li><em>Konflikte mit Zielgruppenüberschneidungen für Journey X anzeigen</em></li></ul> |
| Journey Agent | Journey-Verwaltung | <ul><li>Adobe Journey Optimizer (B2B- und B2C-Editionen)</li></ul> | 25 | <ul><li><em>Wie viele lebende Journey habe ich?</em></li><li><em>Listen Sie alle Journey mit der Audience X auf.</em></li><li><em>Listen Sie alle Journey auf, die sich derzeit im Testmodus befinden</em></li></ul> |
| Produktsupport-Agent | Knowledge-based Troubleshooting | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C- und B2B-Editionen)</li><li>Customer Journey Analytics (B2C- und B2B-Editionen)</li></ul> | 0 | <ul><li><em>Warum unterscheidet sich die Anzahl meiner Profile im Lizenznutzungs-Dashboard und auf der Experience Platform-Startseite?</em></li><li><em>Was sind die Gründe dafür, dass eine Journey nicht ausgelöst wird?</em></li><li><em>Wie erstellt Adobe Experience Platform Echtzeit-Erlebnisse?</em></li><li><em>Wie werden Warnhinweise in Adobe Experience Platform konfiguriert und verwendet?</em></li><li><em>Wie hoch ist die Grenze für die durchschnittliche Profilreichhaltigkeit in Adobe Experience Platform Activation?</em></li></ul> |
| Produktsupport-Agent | Erstellung und Nachverfolgung von Support-Fällen | <ul><li>Real-Time CDP (B2B-, B2C- und B2P-Editionen)</li><li>Adobe Journey Optimizer (B2C- und B2B-Editionen)</li><li>Customer Journey Analytics (B2C- und B2B-Editionen)</li><li>Adobe Experience Manager</li></ul> | 10 | <ul><li><em>Erstellen Sie ein neues Support-Ticket für meinen fehlgeschlagenen Segmentierungsauftrag</em></li><li><em>Wie ist der Status des Tickets E-001772068?</em></li></ul> |
| Inhaltsratgeber-Agent | Inhaltserkennung | <ul><li>Adobe Experience Manager</li></ul> | 5 | <ul><li><em>Inhaltsfragmente zum Erstellen einer WKND-Angebotskampagne anzeigen.</em></li><li><em>Produktverpackung finden PNG-Bilder.</em></li><li><em>Bilder mit Tag in Office-Ordner anzeigen WKND.</em></li><li><em>Gibt es SVGs im Ordner WKND?</em></li><li><em>Alle Kreditantragsformulare anzeigen.</em></li><li><em>Ich suche Onboarding-Formulare für Mitarbeiter.</em></li></ul> |
| Inhaltsratgeber-Agent | <ul><li>Inhaltsoptimierung</li></ul> | <ul><li>Adobe Experience Manager Assets und Dynamic Media</li></ul> | 10 | <ul><li><em>Erstellen Sie eine Ausgabedarstellung von 2.000 Pixel als JPEG mit 80 % Qualität.</em></li><li><em>Erstellen Sie eine Ausgabedarstellung für eine Instagram-Story.</em></li><li><em>Überlagern Sie das Bild mit 30 % Rabattgrafiken über dem Werbebanner und platzieren Sie es 100 Pixel von der Mitte entfernt.</em></li><li><em>Ändern Sie die Hintergrundfarbe des PNG in #ff8932.</em></li></ul> |
| Brand Governance Agent | <ul><li>Prüfungen der Markenrichtlinien</li></ul><ul><li>Berechtigungen mit Content Hub</li></ul><ul><li>Asset-Ablauf</li></ul> | <ul><li>Adobe Experience Manager Sites (Markenrichtlinien)</li></ul><ul><li>Adobe Experience Manager Assets</li></ul> | 25 | <ul><li><em>Ist diese Seite mit meiner Marke abgestimmt? `https://www.website/en.html`</em></li><li><em>Alle vorhandenen Content Hub ABAC-Regeln anzeigen</em></li><li><em>Laufen einige meiner Assets bald aus?</em></li></ul> |
| Brand Experience Agent | <ul><li>Inhaltsaktualisierung</li><li>Forms-Erstellung</li><li>Fehlerbehebung bei Pipelines</li></ul> | <ul><li>Adobe Experience Manager Cloud Services</li><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Forms</li></ul> | 50 | <ul><li><em>Aktualisieren Sie am `URL` die Überschrift auf Hello world</em></li><li><em>Erstellen Sie ein Kontaktformular mit den Feldern Name, E-Mail und Nachricht</em></li><li><em>Fehlerbehebung bei fehlgeschlagener Pipeline</em></li><li><em>Auflisten meiner fehlgeschlagenen Pipelines für das Hauptprogramm.</em></li></ul> |
| Brand Experience Agent | Site-Modernisierung | Adobe Experience Manager Cloud Services | 100 | <ul><li><em>Migrieren der `https://wknd-trendsetters.site`</em></li></ul> |

>[!NOTE]
>
>Der tatsächliche KI-Kreditverbrauch kann je nach der Anzahl der ausgeführten Schritte und Iterationen pro Schritt variieren.

## Weitere Hilfe zu diesem Thema

* [GenAI in Experience Cloud](/help/interface/features/generative-ai.md)
* [Agent AI in Experience Cloud](/help/interface/features/agentic-ai.md)
* [Nutzungsgebundene Testversion für Adobe Experience Platform-Agenten](https://experienceleague.adobe.com/de/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)
