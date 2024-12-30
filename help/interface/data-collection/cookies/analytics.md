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

Adobe Analytics verwendet Cookies, um Anforderungen von verschiedenen Browsern zu unterscheiden und nützliche Informationen zu speichern, die eine Anwendung später verwenden kann. Sie können auch verwendet werden, um Browserinformationen Kundendatensätzen zuzuordnen.

Analytics verwendet Cookies, um neue Besucher anonym zu definieren, Klickdaten zu analysieren und historische Aktivitäten auf der Website zu verfolgen, z. B. Reaktionen auf bestimmte Kampagnen oder die Länge des Verkaufszyklus.

| Cookie-Name | Ablauf | Größe | Standort | Beschreibung |
| --- | --- | --- | --- | --- |
| **`s_ecid`** | 2 Jahre | 45 Byte | Erstanbieter | Speichert die Experience Cloud-ID (ECID) oder MID. Durch HTTP-Antwort festgelegt. Die MID wird im `s_ecid=MCMID`-Format gespeichert. Wird festgelegt, nachdem der Client das AMCV-Cookie gesetzt hat. Sie ermöglicht ein persistentes First-Party-ID-Tracking und wird als Referenz-ID verwendet, wenn das AMCV-Cookie abläuft. Dieses Cookie gilt nicht für Drittanbieter-Cookie-Implementierungen. `SameSite` ist auf „Lax“ eingestellt. |
| **`s_cc`** | Session | 4 Byte | Erstanbieter | Bestimmt, ob Cookies aktiviert sind. Festgelegt durch JavaScript. |
| **`s_sq`** | Session | 100-200 Byte | Erstanbieter | Verwendet von Activity Map. Sie enthält Informationen zum vorherigen Link, auf den der Besucher geklickt hat. Festgelegt durch JavaScript. |
| **`s_vi`** | 2 Jahre | 44 Byte | Erstanbieter oder `*.omtrdc.net` (Drittanbieter) | Speichert eine Unique Visitor ID und einen Zeitstempel. Durch HTTP-Antwort festgelegt. Jede Besucher-ID ist einem Besucherprofil auf Adobe-Servern zugeordnet. Besucherprofile werden nach 1 Jahr Inaktivität gelöscht, unabhängig vom Ablauf von Besucher-ID-Cookies. Das `Secure`-Flag wird gesetzt, wenn `SameSite` „None“ und die Verbindung HTTPS ist. `SameSite` Erstanbieter-Cookies ist standardmäßig „Lax“. `SameSite` bei der Verwendung von Drittanbieter-Cookies, z. B. auf `omtrdc.net` oder `2o7.net`, ist „Keine“. Legen Sie `SameSite` auf „Keine“ fest, wenn Sie einen einzelnen CNAME verwenden, um mehrere Domains oder Eigenschaften zu verfolgen. |
| **`s_fid`** | 2 Jahre | 33 Byte | Erstanbieter | Speichert die Fallback-Unique-Visitor-ID und den Zeitstempel. Wird von JavaScript festgelegt, wenn das standardmäßige `s_vi`-Cookie aufgrund von Beschränkungen für Drittanbieter-Cookies nicht gesetzt werden kann. Wird nicht für Erstanbieter-Cookie-Implementierungen verwendet. |
| **`s_ac`** | Unmittelbar | 1 Byte | Erstanbieter | Hilft bei der Bestimmung der richtigen Domain für AppMeasurement-Cookies. Enthält den statischen Wert `"1"`. Sobald dieses Cookie gesetzt ist, wird es sofort gelöscht. |

{style="table-layout:auto"}

## Von Plug-ins eingestellte Cookies

Bei einigen Implementierungen werden Plug-ins verwendet, bei denen es sich um Code-Ausschnitte handelt, die zusätzliche Funktionen für Analytics bieten. Diese Plug-ins können Cookies setzen, die oben nicht aufgeführt sind. Unter [Übersicht über Analytics-Plug](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/plugins/impl-plugins) finden Sie eine Liste der verfügbaren Plug-ins und der von ihnen gesetzten Cookies.
