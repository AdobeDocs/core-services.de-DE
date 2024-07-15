---
description: Erfahren Sie mehr über Adobe Advertising-Cookies für die Zuordnung von Anzeigeninteraktionsereignissen zu Konversionsereignissen und verwenden Sie diese Informationen möglicherweise zur Optimierung von Anzeigenangeboten.
title: Adobe Advertising-Cookies
uuid: 2eec48a3-3e81-488e-8e30-5fd62885de0b
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 6818edea-31b1-49fc-bca2-32828c7ca78d
source-git-commit: 4d2dc1e6126e26f61475efbd33efe98bd47153d5
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 13%

---

# Adobe Advertising-Cookies

Adobe Advertising (ehemals Adobe Advertising Cloud) verwendet Cookies, um Interaktionsereignisse von Anzeigen Konversionsereignissen zuzuordnen und diese Informationen möglicherweise zur Optimierung von Anzeigenangeboten zu verwenden.

>[!NOTE]
>
>Das JavaScript-Tag der Beta-Adobe Advertising, das den [Adobe Experience Cloud ID(ECID)-Dienst](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=de) verwendet, erstellt Erstanbieter-Cookies [Experience Cloud](experience-cloud.md) `s_ecid` und nicht Adobe Advertising-Cookies.

| Cookie-Name | Ablauf | Größe | Standort | Beschreibung |
| --- | --- | --- | --- | --- |
| **`_lcc`** | 15 Minuten | 52 Byte | `everesttech.net` | Speichert IDs und Zeitstempel von Anzeigeklicks. Bestimmt, ob ein Klickereignis für eine Display-Anzeige für einen Adobe Analytics-Treffer gilt. |
| **`_tmae`** | 1 Jahr | 1 KB | `everesttech.net` | Speichert kodierte IDs und Zeitstempel für Anzeigeninteraktionen mithilfe von DSP-Tracking. Enthält Benutzerinteraktion mit Anzeigen, z. B. zuletzt angezeigte Anzeige |
| **`_tmid`** | 1 Jahr | ~20 Byte | `everesttech.net` | Speichert die Adobe Advertising-Demand Side Platform-ID (DSP). Entspricht der Besucher-ID im Cookie `everest_g_v2` . |
| **`adcloud`** | 1 Jahr | 50-150 Byte | Erstanbieter | Die Zeitstempel des letzten Besuchs des Besuchers auf Ihrer Website und des letzten Suchklicks des Besuchers. Speichert auch den `ef_id` , der beim Klicken auf eine Anzeige durch den Besucher erstellt wurde. Verbindet die Besucher-ID mit relevanten Zielgruppensegmenten und Konversionen. Hilft, die Seitenladezeiten zu optimieren, indem unnötige Anforderungen an Adobe vermieden werden. |
| **`ev_sync_*`** |  | 8 Byte | `everesttech.net` | Das Datum, an dem die Synchronisierung im Format `yyymmdd` durchgeführt wird. Synchronisiert die Adobe Advertising-Besucher-ID mit der Partner-Anzeigenbörse. Sie wird für neue Besucher erstellt und sendet eine Synchronisierungsanforderung, wenn sie abgelaufen ist. Umfasst die Cookies `ev_sync_ax`, `ev_sync_bk`, `ev_sync_dd`, `ev_sync_fs`, `ev_sync_ix`, `ev_sync_nx`, `ev_sync_ox`, `ev_sync_pm`, `ev_sync_rc`, `ev_sync_tm` und `ev_sync_yh`. |
| **`everest_g_v2`** | 1 Jahr | ~27 Byte | `everesttech.net` | Speichert die Browser- und Besucher-ID. Wird erstellt, nachdem ein Benutzer anfänglich auf eine Anzeige geklickt hat. Wird verwendet, um die aktuellen und nachfolgenden Klicks anderen Ereignissen auf Ihrer Website zuzuordnen. |
| **`everest_session_v2`** | Session | ~16 Byte | `everesttech.net` | Speichert die aktuelle Sitzungs-ID. |
| **`id_adcloud`** | 91 Tage | 16 Byte | Erstanbieter | Speichert die Besucher-ID. |

{style="table-layout:auto"}
