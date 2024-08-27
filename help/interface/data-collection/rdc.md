---
title: Regionale Datenerfassung
description: Erfahren Sie mehr über die regionale Datenerfassung in Experience Cloud.
exl-id: 295e9736-2a58-48a8-9968-5dfa33b70d95
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---

# Regionale Datenerfassung

Die Adobe Experience Cloud verwendet die regionale Datenerfassung (Regional Data Collection, RDC), damit Interaktionen zwischen Ihren Besuchern und Adobe so nahe wie möglich an Ihren Besuchern stattfinden. Lokal an einer Edge-Site erfasste Daten werden sicher zur Verarbeitung an eine Core-Site weitergeleitet. Nach der Verarbeitung sind die Daten für Adobe Experience Cloud-Produkte und -Dienste verfügbar.

Der regionale Datenerfassungs-Workflow bietet mehrere Vorteile:

* **Leistung**: Mit RDC stellen Ihre Besucher eine Verbindung zur nächsten Edge-Site her. Diese Optimierung bietet die schnellste Reaktionszeit, was zu genauerer Verfolgung und schnelleren Ladezeiten führt.
* **Redundanz**: Wenn die Kommunikation zwischen Edge-Sites und Core-Sites unterbrochen wird, speichert die Adobe-Infrastruktur Daten lokal und leitet sie bei der Wiederherstellung der Kommunikation an die Core-Site weiter. Adobe kann auch Traffic zu anderen Edge-Sites weiterleiten, wenn bei einem bestimmten Standort Unterbrechungen auftreten.

RDC umfasst derzeit die folgenden Speicherorte (kann geändert werden):

## Erstanbieter-Datenerfassung

| RDC-Typ | Datenerfassungszentren |
| --- | --- |
| Global (Standard) | Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |
| Global + China* | Peking*, Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |
| Nur Amerika | Oregon, Virginia |
| Nur Europa | Irland, Paris |
| Nur Asien | Mumbai, Singapur, Tokio, Sydney |
| Nur China* | Peking |

{style="table-layout:auto"}

_*China RDC erfordert das Add-On-Paket zur Leistungsoptimierung für China und gilt nur für Adobe Analytics, das die AppMeasurement-Datenerfassung verwendet. Andere Experience Cloud-Dienste und die Web SDK-Datenerfassung werden nicht unterstützt. Wenden Sie sich an Ihr Adobe Account-Team, um mehr über das Add-On-Paket zur Leistungsoptimierung für China zu erfahren._

## Datenerfassung von Drittanbietern

Die Datenerfassung von Drittanbietern umfasst Cookie-Domänen, die nicht mit Ihrer Website-Domäne übereinstimmen. Beispiele sind `adobedc.net`, `omtrdc.net` und `2o7.net`.

| RDC-Typ | Datenerfassungszentren |
| --- | --- |
| Standard | Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |
| Standard + China* | Peking*, Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |

{style="table-layout:auto"}
