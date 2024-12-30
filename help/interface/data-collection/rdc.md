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

Die Adobe Experience Cloud verwendet regionale Datenerfassung (Regional Data Collection, RDC), damit die Interaktionen zwischen Ihren Besuchern und dem Adobe so nah wie möglich bei Ihren Besuchern stattfinden. Lokal an einer Edge-Site erfasste Daten werden zur Verarbeitung sicher an eine Core-Site weitergeleitet. Nach der Verarbeitung stehen die Daten für Adobe Experience Cloud-Produkte und -Services zur Verfügung.

Der Workflow für die regionale Datenerfassung bietet mehrere Vorteile:

* **Performance**: Mit RDC stellen Ihre Besucher eine Verbindung zur nächstgelegenen Edge-Site her. Diese Optimierung bietet die schnellste Reaktionszeit, was zu einer genaueren Verfolgung und schnelleren Ladezeiten führt.
* **Redundanz**: Bei einer Unterbrechung der Kommunikation zwischen einem Edge-Standort und einem Core-Standort speichert die Adobe-Infrastruktur die Daten lokal und leitet sie bei der Wiederherstellung der Kommunikation an den Core-Standort weiter. Adobe kann auch Traffic zu anderen Edge-Standorten leiten, wenn an einem bestimmten Standort Unterbrechungen auftreten.

RDC umfasst derzeit die folgenden Speicherorte (kann sich ändern):

## Erstanbieter-Datenerfassung

| RDC-Typ | Datenerfassungszentren |
| --- | --- |
| Global (Standard) | Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |
| Global + China* | Peking*, Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |
| Nur Nord- und Südamerika | Oregon, Virginia |
| Nur Europa | Irland, Paris |
| Nur Asien/Pazifik | Mumbai, Singapur, Tokio, Sydney |
| Nur China* | Peking |

{style="table-layout:auto"}

_*Die regionale Datenerfassung für China erfordert das Add-on-Paket „Leistungsoptimierung für China“ und gilt nur für Adobe Analytics mithilfe der AppMeasurement-Datenerfassung. Andere Experience Cloud-Services und die Web SDK-Datenerfassung werden nicht unterstützt. Wenden Sie sich an Ihr Adobe-Account-Team, um mehr über das Add-on-Paket zur Leistungsoptimierung für China zu erfahren._

## Datenerfassung durch Dritte

Die Datenerfassung durch Dritte umfasst Cookie-Domains, die nicht mit Ihrer Website-Domain übereinstimmen. Beispiele sind `adobedc.net`, `omtrdc.net` und `2o7.net`.

| RDC-Typ | Datenerfassungszentren |
| --- | --- |
| Standard | Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |
| Standard + China* | Peking*, Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |

{style="table-layout:auto"}
