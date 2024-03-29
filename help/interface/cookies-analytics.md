---
description: Hier erfahren Sie mehr über Adobe Analytics-Cookies in Adobe Experience Cloud.
solution: Experience Cloud,Analytics,Target
title: Cookies in Analytics
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bc8ce894-f98c-4475-8a07-d74ae76f7451
source-git-commit: a20d51e6e7d5ec72d59e06e6a4951778a5828d9a
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 92%

---

# Cookies in Analytics{#analytics-cookies}

Adobe Analytics verwendet Cookies, um Anforderungen von verschiedenen Browsern zu unterscheiden und nützliche Informationen zu speichern, die eine Anwendung später verwenden kann. Sie können auch verwendet werden, um Browserinformationen Kundendatensätzen zuzuordnen.

Analytics verwendet Cookies vor allem, um anonym neue Besucher zu definieren, Klickdaten zu analysieren und historische Aktivitäten auf der Website zu verfolgen, z. B. Reaktionen auf bestimmte Kampagnen oder die Dauer des Verkaufszyklus.

* [Cookie-Name: s_ecid](cookies-mc.md#section-32fd753c3fa54452acd62b021434919a)
* [Cookie-Name: AMCV_###@AdobeOrg](cookies-mc.md#section-a12aa2a9296940ae82d8921b381b8fb0)
* [Cookie-Name: s_cc](cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [Cookie-Name: s_sq ](cookies-analytics.md#section-8abfff3a302d494f81a3cfb91e3b09ff)
* [Cookie-Name: s_vi](cookies-analytics.md#section-5d50a078de444d12b7d927d68ff3b679)
* [Cookie-Name: s_fid ](cookies-analytics.md#section-65e33f9bfc264959ac1513e2f4b10ac7)
* [Von Plug-ins eingestellte Cookies](cookies-analytics.md#section-a6b1cae8454945fab9eea5c7884c40fc)

Weitere Informationen finden Sie in der Analytics-Hilfe zu [Erstanbieter-Cookies](cookies-first-party.md).

## Cookie-Name: s_ecid {#section-32fd753c3fa54452acd62b021434919a}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Enthält eine Kopie der Experience Cloud ID (ECID) oder der MID. Die MID wird in einem Schlüssel-Wert-Paar gespeichert, das dieser Syntax folgt: s_ecid=MCMID | `<ECID>` |
| Ablauf | 2 Jahre |
| Nutzung | Dieses Cookie wird durch die Domain des Kunden gesetzt, nachdem das AMCV-Cookie vom Client gesetzt wurde. Dieses Cookie ermöglicht das durchgängige ID-Tracking als Erstanbieter und wird als Referenz-ID verwendet, wenn das AMCV-Cookie abgelaufen ist. Weitere Details zum AMCV-Cookie finden Sie hier. |
| Position | Nur CNAME-Kunden. Gilt nicht für Drittanbieter-Szenarien. Cookie wird in Ihrer Domain gespeichert; dieselbe Domain wie die von CNAME und Ihrer Analytics-Bildanforderung verwendete. |
| Größe | 45 Byte |

{style="table-layout:auto"}

## Cookie-Name: s_cc {#section-03aa90aa7e36427b8cb12dc4a0f0291e}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Dieses Cookie wird vom JavaScript-Code gesetzt und gelesen, um zu bestimmen, ob Cookies aktiviert (auf „True“ gesetzt) sind. |
| Ablauf | Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird |
| Nutzung | Nur ein Cookie für alle Konten |
| Position | Dieses Cookie wird in der Domain der Seite gespeichert. |
| Größe | 4 Byte |

{style="table-layout:auto"}

## Cookie-Name: s_sq {#section-8abfff3a302d494f81a3cfb91e3b09ff}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Dieses Cookie wird vom JavaScript-Code gesetzt und gelesen, wenn die ClickMap-Funktion oder die Activity Map-Funktion aktiviert ist. Es enthält Informationen zum vorherigen Link, der vom Benutzer ausgewählt wurde. |
| Ablauf | Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird |
| Nutzung | Nur ein Cookie für alle Konten |
| Position | Dieses Cookie wird in der Domain der Seite gespeichert. |
| Größe | Variiert je nach URL-Größe der Seite, normalerweise 100-200 Byte |

{style="table-layout:auto"}

## Cookie-Name: s_vi {#section-5d50a078de444d12b7d927d68ff3b679}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Datums-/Uhrzeitstempel der Unique-Visitor-ID. |
| Ablauf | 2 Jahre |
| Nutzung | Dieses Cookie wird zur Identifizierung eines Unique Visitor verwendet. |
| Position | Dieses Cookie wird in der Domain der Bildanforderung gespeichert. Dabei handelt es sich normalerweise um eine kundenspezifische Subdomäne unter 2o7.net oder omtrdc.net, wenn Sie Drittanbieter-Cookies verwenden oder wenn Ihre Domain Erstanbieter-Cookies verwendet. |
| Größe | 44 Byte |

{style="table-layout:auto"}

>[!NOTE]
>
>Jede Analytics-Besucher-ID ist einem Besucherprofil auf Adobe-Servern zugewiesen. Besucherprofile werden nach einem Jahr Inaktivität gelöscht, unabhängig vom Ablauf der Besucher-ID-Cookies.

## Cookie-Name: s_fid {#section-65e33f9bfc264959ac1513e2f4b10ac7}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Fallback-Datums-/Uhrzeitstempel der Unique-Visitor-ID. |
| Ablauf | 2 Jahre |
| Nutzung | Dieses Cookie wird verwendet, um einen Unique Visitor zu identifizieren, wenn die standardmäßige  `s_vi` aufgrund von Beschränkungen für Drittanbieter-Cookies nicht verfügbar ist. Es wird nicht für Implementierungen verwendet, die Erstanbieter-Cookies verwenden. |
| Position | Dieses Cookie wird als Erstanbieter-Cookie in Ihrer Domain gespeichert. |
| Größe | 33 Byte |

{style="table-layout:auto"}

## Cookie-Flags

In der folgenden Tabelle werden die Flags für Analytics-Cookies beschrieben:

| Cookie (gesetzt von) | httpOnly | Secure | SameSite |
|--- |--- |--- |--- |
| s_vi (http Response) | Nein | Ja, wenn SameSite „Keine“ lautet und die Verbindung HTTPS verwendet | Bei Verwendung von CNAME wird standardmäßig „Lax“ verwendet. „Keine“ bei Verwendung von 2o7.net oder omtrdc.net. |
| s_ecid (http-Antwort) | Nein | Nein | „Lax“ |
| s_fid (Javascript) | Nein | Nein | Löschen |
| s_cc (Javascript) | Nein | Nein | Löschen |
| s_sq (Javascript) | Nein | Nein | Löschen |

{style="table-layout:auto"}

>[!NOTE]
>
>Bei Verwendung eines einzelnen CNAME zur Verfolgung über mehrere Domains oder Eigenschaften hinweg sollte SameSite für `s_vi` auf „Keine“ festgelegt werden. Wenden Sie sich an die Kundenunterstützung, um Hilfe beim Ändern der Cookie-Einstellungen in Analytics zu erhalten.

## Von Plug-ins eingestellte Cookies {#section-a6b1cae8454945fab9eea5c7884c40fc}

{{plug-in}}

Zusätzliche Cookies können je nach Verwendung von Analytics-Plug-Ins gesetzt werden. Diese Cookies sind Codefragmente, die dem Client zur Verwendung in verschiedensten Situationen zur Verfügung stehen. Dazu gehören: Abrufen von Werten aus der URL; Verketten von Werten, die an Analytics übergeben werden sollen; Erfassen des Formularabbruchs usw. Beispiel: das Cookie [!DNL s_vh] wird mit den Plug-ins *Set Once Per* und *Set and Get Last Value* verwendet.

Konversionsvariablen (eVarX), die auf eine Bildanforderung ohne JavaScript hin weitergegeben werden, wie z. B. Code in einer E-Mail, werden nur dann richtig zugewiesen, wenn der E-Mail-Client und der Webbrowser denselben Cookie-Bereich nutzen.
