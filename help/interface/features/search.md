---
description: Erfahren Sie mehr über die Funktion „Einheitliche Suche“ für bestimmte Anwendungen in Experience Cloud.
solution: Experience Cloud
title: Experience Cloud – Einheitliche Suche
index: true
feature: Central Interface Components
topic: Administration
role: Admin
level: Beginner
exl-id: 70586f18-6f84-4308-bab3-1da7fab823d6
source-git-commit: c39672f0d8a0fd353b275b2ecd095ada1e2bf744
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 100%

---

# [!UICONTROL Einheitliche Suche] nach Objekten und Entitäten {#globally-search}

Die [!UICONTROL einheitliche Suche] ermöglicht es Ihnen, durchsuchbare Geschäftsobjekte oder Entitäten in einem nahtlosen, konsistenten Erlebnis mit einem Mausklick zu finden. Diese Suche zeigt auch die Objekte an, auf die Sie zuletzt zugegriffen haben.

![Globale Suche nach Objekten und Entitäten](../assets/platform-search.png)

## Zugriff auf die einheitliche Suche

Die einheitliche Suche ist auf jeder Seite von Experience Cloud in der Kopfzeile am oberen Seitenrand verfügbar. Sie können auch den Tastaturbefehl `command /` oder `ctrl /` verwenden, um auf die Suche zuzugreifen.

Diese Funktion ist nur für unterstützte Produkte verfügbar – derzeit die folgenden:

* Experience Platform (AEP)
* Journey Optimizer (AJO)

In dem Maße, in dem mehr Inhalte indiziert werden, wird diese Funktion zu den entsprechenden Programmen hinzugefügt.

## Durchsuchbare Objekte und Felder

Während der Eingabe werden die passenden Ergebnisse aus den Objekten, auf die Sie Zugriff haben, angezeigt.

Die Suchalgorithmen zeigen zuerst die relevantesten Einträge an. Die Reihenfolge der Ergebnisse hängt von verschiedenen Faktoren ab, z. B.:

Ihre Möglichkeiten und Objektberechtigungen
Übereinstimmung in Prozent
Ob es eine genaue Übereinstimmung gibt

![Einheitliche Suche in Experience Cloud](../assets/unified-search-results.png)

Zu den durchsuchbaren Geschäftsobjekten gehören:

* Segmente (Name, Beschreibung, ID)
* Schema (Name, Beschreibung, ID)
* Datensätze (Name, Beschreibung, ID)
* Quellen (Name, Beschreibung, ID)
* Ziele (Name, Beschreibung, ID)
* Abfragen (Name, Beschreibung, ID)
* Nachrichten (Name, Beschreibung, ID)
* Angebote (Name, Beschreibung, ID)
* Komponenten (Name, Beschreibung, ID)
* Journeys (Name, Beschreibung, ID)

Wenn ein Keyword zu einer Navigationsseite passt, können Sie einen Schnellzugriffs-Link zu den Beispieldatensätzen der Navigationsseite erhalten. Der Abschnitt Top-Ergebnisse zeigt die 30 besten Ergebnisse.

Sie finden die Hilfeartikel auch in Experience League und Communities. Abfragen in natürlicher Sprache werden unterstützt.

So liefert z. B. _Wie man ein Schema erstellt_ Ergebnisse von Experience League unter _[!UICONTROL Lernen]_:

![Einheitliche Suche in der Experience Cloud-Hilfe](../assets/unified-search-learning.png)

Suchalgorithmen zeigen zuerst die relevantesten Datensätze an. Die Reihenfolge der Ergebnisse hängt von verschiedenen Faktoren ab, z. B.:

* Benutzerberechtigungen für den Zugriff auf Objekte
* Prozentsatz der Übereinstimmung
* Exakte Übereinstimmungen
* Der Abschnitt _[!UICONTROL Top-Ergebnisse]_ zeigt die 30 besten Ergebnisse.

Um die Suche zu verfeinern, klicken Sie auf eine der folgenden Optionen:

* **[!UICONTROL Alle Lerninhalte]**: Öffnet die Suche in Experience League.
* **[!UICONTROL Alle anzeigen...]**: Ermöglicht die weitere Verfeinerung und Filterung der Ergebnisse.

## Funktionen der einheitlichen Suche

Die folgenden Funktionen sind in der einheitlichen Suche verfügbar.

| Funktion | Beschreibung |
| ------- | ------- |
| Globale Sprachunterstützung | Die globale Suche versteht Abfragen und liefert Ergebnisse für Deutsch, Spanisch, Französisch, Italienisch, Japanisch, Koreanisch, Portugiesisch und Chinesisch. |
| Automatische Tippfehler-Korrektur | Die einheitliche Suche korrigiert Tippfehler unter Verwendung erweiterter Algorithmen automatisch. Diese Algorithmen berechnen Bearbeitungen und liefern passende Ergebnisse. |
| Hervorhebung | In der Suchanfrage wird das Übereinstimmungs-Keyword hervorgehoben, sodass Sie den Abschnitt und die Wörter, die Ihrer Abfrage entsprechen, einfach finden können. Die Hervorhebung funktioniert auch bei falsch geschriebenen Wörtern. |
| Snippets | In der Suchantwort sehen Sie ein Snippet, einen Ausschnitt des Ergebnisses. Snippets geben die übereinstimmenden Wörter und einige Inhalte rund um die Übereinstimmungs-Keywords zurück. |
| Stoppwörter | Einige im Englischen häufig verwendete Wörter werden als _Stoppwörter_ definiert. Wenn Stoppwörter in der Suchabfrage enthalten sind, wird ihnen weniger Gewicht zugemessen. <br>Stoppwörter beinhalten: _a, an, and, are, as, at, be, but, by, for, if, in, into, is, it, no, not, of, on, or, such, that, the, their, then, there, these, they, this, to, was, will, with_. <br>Stoppwörter werden in anderen globalen Sprachen nicht unterstützt. |
| Natürliche Sprachabfragen | Wenn Sie in Experience League Communitys nach einem Hilfeartikel oder einer Diskussion suchen, können Sie Ihre Frage in natürlicher Sprache eingeben und die Antwort erhalten. Beispielsuche: „Wie erstelle ich ein Schema?“ |
| Exakte Suche in Anführungszeichen | Mithilfe von Anführungszeichen in der Abfrage können Sie eine exakte Suche durchführen. Bei Abfragen mit exakter Übereinstimmung wird keine Korrektur von Tippfehlern vorgenommen. Beispiel: „Luma Journey 2022“. |
| Filter | Im Popup-Fenster mit den vollständigen Suchergebnissen können Sie Filter wie _Objekttyp_ und andere objektspezifische Filter anwenden. Wenn Sie die Eingabetaste drücken, nachdem Sie die Suchabfrage eingegeben haben, wird ein ganzseitiges Popup-Fenster geöffnet, das die Filter enthält. |

{style="table-layout:auto"}

## Es wird nicht gefunden?

Probieren Sie die folgenden Tipps aus:

* Geben Sie einen spezifischeren Suchbegriff ein
* Prüfen Sie die Rechtschreibung
* Versuchen Sie, den vollständigen Suchbegriff zu schreiben
* Vergewissern Sie sich, dass Sie über Berechtigungen für Objekte verfügen, nach denen Sie suchen
