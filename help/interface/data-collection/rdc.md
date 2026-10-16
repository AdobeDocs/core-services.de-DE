---
title: Regionale Datenerfassung
description: Erfahren Sie mehr über die regionale Datenerfassung in CX Enterprise.
exl-id: 295e9736-2a58-48a8-9968-5dfa33b70d95
TQID: https://experienceleague.adobe.com/hjHQDRoNOP2e6pKhKHB9DZaII2o8eJVzL5wjRzaMFwM
product_v2:
  - id: e1971122-7081-4556-9222-8a31bd71800c
    internal-label: Experience Cloud Services
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
    internal-label: Optimization
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a714343bc3e17145e51fd99f64690e7d69ab4d9d
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 1%
---
# Regionale Datenerfassung

Adobe CX Enterprise verwendet regionale Datenerfassung (Regional Data Collection, RDC), damit die Interaktionen zwischen Ihren Besucherinnen und Besuchern und Adobe so nah wie möglich bei Ihren Besucherinnen und Besuchern stattfinden. Lokal an einer Edge-Site erfasste Daten werden zur Verarbeitung sicher an eine Core-Site weitergeleitet. Nach der Verarbeitung stehen die Daten für Adobe CX Enterprise-Produkte und -Services zur Verfügung.

Der Workflow für die regionale Datenerfassung bietet mehrere Vorteile:

* **Performance**: Mit RDC stellen Ihre Besucher eine Verbindung zur nächstgelegenen Edge-Site her. Diese Optimierung bietet die schnellste Reaktionszeit, was zu einer genaueren Verfolgung und schnelleren Ladezeiten führt.
* **Redundanz**: Wenn es zu einer Unterbrechung der Kommunikation zwischen einem Edge-Standort und einem Core-Standort kommt, speichert die Adobe-Infrastruktur die Daten lokal und leitet sie bei der Wiederherstellung der Kommunikation an den Core-Standort weiter. Adobe kann auch Traffic zu anderen Edge-Sites weiterleiten, wenn an einem bestimmten Ort Unterbrechungen auftreten.

## Erstanbieter-Datenerfassung

Die Erstanbieter-Datenerfassung verwendet eine CNAME-Implementierung, um Daten über Ihre eigene Domain an Adobe weiterzuleiten. Ihr RDC-Typ wird im Rahmen des Einrichtungsprozesses des [Adobe-Managed Certificate Program](adobe-managed-cert.md) ausgewählt. Um Ihren RDC-Typ zu überprüfen oder zu aktualisieren, wenden Sie sich an Ihr Adobe Account Team. Die folgenden RDC-Typen und zugehörigen Rechenzentren sind verfügbar:

| RDC-Typ | Datenerfassungszentren |
| --- | --- |
| Global (Standard) | Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |
| Global + China* | Peking*, Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |
| Nur Nord- und Südamerika | Oregon, Virginia |
| Nur Europa | Irland, Paris |
| Nur Asien/Pazifik | Mumbai, Singapur, Tokio, Sydney |
| Nur China* | Peking |

_*Die regionale Datenerfassung für China erfordert das Add-on-Paket „China Performance Optimization“ und gilt nur für Adobe Analytics mithilfe der Datenerfassung von AppMeasurement. Andere CX Enterprise-Services und die Web-SDK-Datenerfassung werden nicht unterstützt. Wenden Sie sich an Ihr Adobe-Account-Team, um mehr über das Add-on-Paket zur Leistungsoptimierung für China zu erfahren._

Wenn Sie [Datenerfassung über ein CDN &#x200B;](cdn.md)), benötigen regionsgesperrte RDC-Typen einen First-Party-Ursprung mit einem [kundenverwalteten Zertifikat](customer-managed-cert.md).

## Datenerfassung durch Dritte

Die Datenerfassung von Drittanbietern verwendet Cookie-Domains, die nicht mit Ihrer Website-Domain übereinstimmen. Beispiele sind `adobedc.net`, `omtrdc.net` und `2o7.net`.

| RDC-Typ | Datenerfassungszentren |
| --- | --- |
| Standard | Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |
| Standard + China* | Peking*, Oregon, Virginia, Irland, Paris, Mumbai, Singapur, Tokio, Sydney |

_*Erfordert das Zusatzpaket „China Performance Optimization“. Weitere Informationen finden Sie im Abschnitt Erstanbieter-Datenerfassung oben._

Daten, die über ein CDN an einen [-Ursprung weitergeleitet werden](cdn.md#third-party-origin) verwenden immer den standardmäßigen RDC-Typ.
