---
description: Hier erfahren Sie mehr über Adobe Analytics-Cookies in Adobe Experience Cloud.
solution: Analytics
title: Cookies in Adobe Analytics
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bc8ce894-f98c-4475-8a07-d74ae76f7451
source-git-commit: 5905644c2de154da77f33ae486818b5bede418df
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 16%

---

# Cookies in Adobe Analytics

Adobe Analytics verwendet Cookies, um Anforderungen von verschiedenen Browsern zu unterscheiden und nützliche Informationen zu speichern, die eine Anwendung später verwenden kann. Sie können auch verwendet werden, um Browserinformationen mit Kundendatensätzen zu verknüpfen.

Analytics verwendet Cookies, um anonym neue Besucher zu definieren, Clickstream-Daten zu analysieren und historische Aktivitäten auf der Website zu verfolgen, z. B. Reaktionen auf bestimmte Kampagnen oder die Dauer des Verkaufszyklus.

| Cookie-Name | Ablauf | Größe | Standort | Beschreibung |
| --- | --- | --- | --- | --- |
| **`s_ecid`** | 2 Jahre | 45 Byte | Erstanbieter | Speichert die Experience Cloud-ID (ECID) oder MID. Wird durch HTTP-Antwort festgelegt. Die MID wird im Format `s_ecid=MCMID` gespeichert. Wird eingestellt, nachdem der Client das AMCV-Cookie gesetzt hat. Sie ermöglicht ein beständiges Erstanbieter-ID-Tracking und wird als Referenz-ID verwendet, wenn das AMCV-Cookie abläuft. Dieses Cookie gilt nicht für Drittanbieter-Cookie-Implementierungen. `SameSite` ist auf &quot;Lax&quot;festgelegt. |
| **`s_cc`** | Session | 4 Byte | Erstanbieter | Bestimmt, ob Cookies aktiviert sind. Festgelegt von JavaScript. |
| **`s_sq`** | Session | 100-200 Byte | Erstanbieter | Wird von Activity Map verwendet. Er enthält Informationen zum vorherigen Link, auf den der Besucher geklickt hat. Festgelegt von JavaScript. |
| **`s_vi`** | 2 Jahre | 44 Byte | Erstanbieter oder `*.omtrdc.net` (Drittanbieter) | Speichert eine eindeutige Besucher-ID und einen Zeitstempel. Wird durch HTTP-Antwort festgelegt. Jede Besucher-ID ist einem Besucherprofil auf Adobe-Servern zugeordnet. Besucherprofile werden nach einem Jahr Inaktivität gelöscht, unabhängig vom Ablauf der Besucher-ID-Cookies. Das Flag `Secure` wird gesetzt, wenn `SameSite` &quot;Keine&quot;und die Verbindung HTTPS ist. `SameSite` ist bei Erstanbieter-Cookies standardmäßig &quot;Lax&quot;. `SameSite` ist &quot;Keine&quot;bei Verwendung von Drittanbieter-Cookies, z. B. bei `omtrdc.net` oder `2o7.net`. Setzen Sie `SameSite` bei Verwendung eines einzelnen CNAME zur Verfolgung mehrerer Domänen oder Eigenschaften auf &quot;Keine&quot;. |
| **`s_fid`** | 2 Jahre | 33 Byte | Erstanbieter | Speichert die Fallback-Unique Visitor-ID und den Zeitstempel. Wird von JavaScript gesetzt, wenn das standardmäßige `s_vi` -Cookie aufgrund von Beschränkungen für Drittanbieter-Cookies nicht gesetzt werden kann. Wird nicht für Erstanbieter-Cookie-Implementierungen verwendet. |
| **`s_ac`** | Unmittelbar | 1 Byte | Erstanbieter | Hilft bei der Bestimmung der richtigen Domäne für AppMeasurement-Cookies. Enthält den statischen Wert `"1"`. Sobald dieses Cookie gesetzt ist, wird es sofort gelöscht. |

{style="table-layout:auto"}

## Von Plug-ins eingestellte Cookies

Einige Implementierungen nutzen Plug-ins, bei denen es sich um Codefragmente handelt, die zusätzliche Funktionen für Analytics bieten. Diese Plug-ins können Cookies setzen, die oben nicht aufgeführt sind. Eine Liste der verfügbaren Plug-ins und der von ihnen gesetzten Cookies finden Sie unter [Übersicht über Analytics-Plug-ins](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/plugins/impl-plugins) .
