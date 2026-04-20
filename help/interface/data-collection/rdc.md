---
title: Regionale Datenerfassung
description: Erfahren Sie mehr über die regionale Datenerfassung in CX Enterprise.
exl-id: 295e9736-2a58-48a8-9968-5dfa33b70d95
TQID: https://experienceleague.adobe.com/hjHQDRoNOP2e6pKhKHB9DZaII2o8eJVzL5wjRzaMFwM
product_v2: id: e1971122-7081-4556-9222-8a31bd71800c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1id: d3cdead0-685a-4489-9250-4bb709942f66id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1a77ef8d31211fb11c790152e78037a8c3b238a2
workflow-type: tm+mt
source-wordcount: 299
ht-degree: 1%

---

# Regionale Datenerfassung

Die Adobe CX Enterprise verwendet regionale Datenerfassung (Regional Data Collection, RDC), damit die Interaktionen zwischen Ihren Besucherinnen und Besuchern und Adobe so nah wie möglich bei Ihren Besucherinnen und Besuchern stattfinden. Lokal an einer Edge-Site erfasste Daten werden zur Verarbeitung sicher an eine Core-Site weitergeleitet. Nach der Verarbeitung stehen die Daten für Adobe CX Enterprise-Produkte und -Services zur Verfügung.

Der Workflow für die regionale Datenerfassung bietet mehrere Vorteile:

* **Performance**: Mit RDC stellen Ihre Besucher eine Verbindung zur nächstgelegenen Edge-Site her. Diese Optimierung bietet die schnellste Reaktionszeit, was zu einer genaueren Verfolgung und schnelleren Ladezeiten führt.
* **Redundanz**: Wenn es zu einer Unterbrechung der Kommunikation zwischen einem Edge-Standort und einem Core-Standort kommt, speichert die Adobe-Infrastruktur die Daten lokal und leitet sie bei der Wiederherstellung der Kommunikation an den Core-Standort weiter. Adobe kann auch Traffic zu anderen Edge-Sites weiterleiten, wenn an einem bestimmten Ort Unterbrechungen auftreten.

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

_*Die regionale Datenerfassung für China erfordert das Add-on-Paket „China Performance Optimization“ und gilt nur für Adobe Analytics mithilfe der Datenerfassung von AppMeasurement. Andere CX Enterprise-Services und die Web-SDK-Datenerfassung werden nicht unterstützt. Wenden Sie sich an Ihr Adobe-Account-Team, um mehr über das Add-on-Paket zur Leistungsoptimierung für China zu erfahren._

## Datenerfassung durch Dritte

Die Datenerfassung durch Dritte umfasst Cookie-Domains, die nicht mit Ihrer Website-Domain übereinstimmen. Beispiele sind `adobedc.net`, `omtrdc.net` und `2o7.net`.

| RDC-Typ | Datenerfassungszentren |
| --- | --- |
| Standard | Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |
| Standard + China* | Peking*, Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |

{style="table-layout:auto"}

