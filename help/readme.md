---
source-git-commit: 58ccef353b492b1c2adfbb8c2471e1f92263e6e4
translation-type: tm+mt

---
# Anleitung

**Hinweis: Diese Seite (und jede andere „readme.md“-Seite) wird nicht in der Kundendokumentation veröffentlicht**

## Inhaltsverzeichnis

+ `TOC.md` steht am Anfang des Benutzerhandbuchs und ermöglicht die Organisation der Themen, die im Handbuch für diese Lösung enthalten sind.
+ Jedes Benutzerhandbuch verfügt über ein eigenes `TOC.md`, in dem Sie alle Seiten/Themen nach Bedarf sortieren können.
+ Die erste Seite aller Benutzerhandbücher ist `overview.md`.

## Benutzerhandbuch

+ Die Einführung in das Benutzerhandbuch finden Sie in der `overview.md`
+ Jedes Thema im Benutzerhandbuch verfügt über ein eigenes Verzeichnis.
   + Wenn im Handbuch ein Thema namens *Implementierung* vorhanden ist, lautet auch der entsprechende Ordner `/implementation`.
+ Alle Bild-Assets befinden sich in `/assets` im Stammordner des Benutzerhandbuchs.
   + Alle Bilder im `/assets`-Ordner werden übersetzt.
   + Bilder im `/no-localize`-Ordner werden nicht übersetzt. Damit kann sichergestellt werden, dass bestimmte Assets nicht unnötig reproduziert werden.

## Metadaten auf Benutzerhandbuchebene

+ Metadaten, die das Benutzerhandbuch beschreiben, werden im Abschnitt `TOC.md` gespeichert. Dazu gehören:
   + product – Name des Produkts/der Funktion.
   + cloud – Cloud, zu der dieses Produkt gehört.
   + audience – Zielgruppe des Handbuchs.
   + user-guide – Name des Benutzerhandbuchs.

## Metadaten auf Seitenebene

+ Die zur Beschreibung eines Dokuments erforderlichen Metadaten werden als Teil jeder einzelnen Seite gespeichert. Dazu gehören:
   + title – Titel der Seite.
   + description – Beschreibung der Seite.
   + seo-title – Seo-Alternativtitel.
   + seo-description – Alternativer Titel für SEO-Zwecke.
   + short-title – (Optionales Feld).
   + index – ja/nein – Wird die Seite durch die Suchplattform von Adobe indexiert?
   + translate – ja/nein – Wird diese Seite übersetzt?
   + version – Hauptsächlich für AEM und Campaign verwendet, um die Produktversion zu kennzeichnen.
   + private-feature-pack – Hauptsächlich für AEM verwendet.
   + beta – Ist dieses Produkt in der Beta-Phase?
   + redirect – Kann verwendet werden, um bei Bedarf eine Referenz zu einer neuen Seite zu erstellen.
   + doc-type: reference (Standard)/troubleshooting/developer/tutorial/kb/whitepaper.

## Weitere Informationen

Weitere Veröffentlichungsanweisungen, Stilhandbücher, Beispiele und andere Ressourcen finden Sie in [Kollaboratives Dokumentationsverzeichnis](https://git.corp.adobe.com/AdobeDocs/collaborative-doc-instructions)
