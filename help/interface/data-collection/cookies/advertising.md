---
description: Erfahren Sie mehr über Adobe Advertising-Cookies für die Zuordnung von Anzeigeninteraktionsereignissen zu Konversionsereignissen und verwenden Sie diese Informationen möglicherweise, um Anzeigengebote zu optimieren.
title: Cookies in Adobe Advertising
uuid: 2eec48a3-3e81-488e-8e30-5fd62885de0b
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 6818edea-31b1-49fc-bca2-32828c7ca78d
TQID: 'https://experienceleague.adobe.com/jr9RwaF63elDUN-XewIdrPNsGb6T5wo98vktP5U6jIM'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: dab36b01-8bfa-48f3-8392-626455a058e6
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: eb7e29b9-c5e9-4ed0-8e4b-6465dabb3cb1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9c2010694b8bb32c3922dd65f846375e43b2caac
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 15%

---

# Adobe Advertising-Cookies

Adobe Advertising (früher Adobe Advertising Cloud) verwendet Cookies, um Ereignisse von Anzeigeninteraktionen Konversionsereignissen zuzuordnen und diese Informationen ggf. zur Optimierung der Anzeigengebote zu verwenden.

>[!NOTE]
>
>Das JavaScript-Tag der Beta-Adobe Advertising, das den [Adobe CX Enterprise ID (ECID) Service verwendet](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=de) erstellt `s_ecid`-Cookies von Erstanbieter-[CX](experience-cloud.md), nicht von Adobe Advertising-Cookies.

| Cookie-Name | Ablauf | Größe | Standort | Beschreibung |
| --- | --- | --- | --- | --- |
| **`_lcc`** | 15 Minuten | 52 Byte | `everesttech.net` | Speichert IDs und Zeitstempel von Anzeigeklicks. Bestimmt, ob ein Klickereignis auf einer Display-Anzeige für einen Adobe Analytics-Treffer gilt. |
| **`_tmae`** | 1 Jahr | 1 KB | `everesttech.net` | Speichert kodierte IDs und Zeitstempel für Anzeigeninteraktionen mit dem DSP-Tracking. Umfasst die Benutzerinteraktion mit Anzeigen, z. B. zuletzt angezeigte Anzeigen |
| **`_tmid`** | 1 Jahr | ~20 Byte | `everesttech.net` | Speichert die Adobe Advertising Demand Side Platform (DSP) ID. Entspricht der Besucher-ID im `everest_g_v2`-Cookie. |
| **`adcloud`** | 1 Jahr | 50-150 Byte | Erstanbieter | Der Zeitstempel des letzten Besuchs der Besucherin oder des Besuchers auf Ihrer Website und der letzte Suchklick der Besucherin oder des Besuchers. speichert auch die `ef_id`, die erstellt wurden, als der Besucher auf eine Anzeige geklickt hat. verknüpft die Besucher-ID mit relevanten Zielgruppensegmenten und Konversionen. Hilft bei der Optimierung der Seitenladezeiten, indem unnötige Anfragen an Adobe vermieden werden. |
| **`ev_sync_*`** |  | 8 Byte | `everesttech.net` | Das Datum, an dem die Synchronisierung `yyymmdd` Format durchgeführt wird. Synchronisiert die Adobe Advertising-Besucher-ID mit dem Partner-Ad-Exchange. Sie wird für neue Besucher erstellt und sendet bei Ablauf eine Synchronisierungsanfrage. Umfasst die Cookies `ev_sync_ax`, `ev_sync_bk`, `ev_sync_dd`, `ev_sync_fs`, `ev_sync_ix`, `ev_sync_nx`, `ev_sync_ox`, `ev_sync_pm`, `ev_sync_rc`, `ev_sync_tm` und `ev_sync_yh`. |
| **`everest_g_v2`** | 1 Jahr | ~27 Byte | `everesttech.net` | Speichert den Browser und die Besucher-ID Erstellt, nachdem ein Benutzer anfänglich auf eine Anzeige geklickt hat. Wird verwendet, um aktuelle und nachfolgende Klicks anderen Ereignissen auf Ihrer Website zuzuordnen. |
| **`everest_session_v2`** | Session | ~16 Byte | `everesttech.net` | Speichert die aktuelle Sitzungs-ID |
| **`id_adcloud`** | 91 Tage | 16 Byte | Erstanbieter | Speichert die Besucher-ID. |

{style="table-layout:auto"}

