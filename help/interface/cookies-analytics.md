---
description: Hier erfahren Sie mehr über Adobe Analytics-Cookies in Adobe Experience Cloud.
keywords: Cookies, Datenschutz
solution: Experience Cloud,Analytics,Target
title: 'Analytics-Cookies '
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
feature: Cookies
topic: Administration
role: Administrator
level: Experienced
exl-id: bc8ce894-f98c-4475-8a07-d74ae76f7451
source-git-commit: 93f5eda7229990e3645b54efa2a172d7b57dcb9b
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 79%

---

# Analytics-Cookies{#analytics-cookies}

Adobe Analytics verwendet Cookies, um Anforderungen von verschiedenen Browsern zu unterscheiden und nützliche Informationen zu speichern, die eine Anwendung später verwenden kann. Sie können auch verwendet werden, um Browserinformationen Kundendatensätzen zuzuordnen.

Analytics verwendet Cookies, um anonym neue Besucher zu definieren, Clickstream-Daten zu analysieren und historische Aktivitäten auf der Website zu verfolgen, z. B. Reaktionen auf bestimmte Kampagnen oder die Dauer des Verkaufszyklus.

* [Cookie-Name: s_ecid](cookies-mc.md#section-32fd753c3fa54452acd62b021434919a)
* [Cookie-Name: AMCV_###@AdobeOrg](cookies-mc.md#section-a12aa2a9296940ae82d8921b381b8fb0)
* [Cookie-Name: s_cc](cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
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
| Nutzung | Dieses Cookie wird durch die Domäne des Kunden festgelegt, nachdem das AMCV-Cookie vom Client festgelegt wurde. Dieses Cookie ermöglicht das durchgängige ID-Tracking als Erstanbieter und wird als Referenz-ID verwendet, wenn das AMCV-Cookie abgelaufen ist. Weitere Details zum AMCV-Cookie finden Sie hier. |
| Position | Nur CNAME-Kunden. Gilt nicht für Drittanbieter-Szenarien. Cookie wird in Ihrer Domäne gespeichert; dieselbe Domäne wie die von CNAME und Ihrer Analytics-Bildanforderung verwendete. |
| Größe | 45 Byte |

{style=&quot;table-layout:auto&quot;}

## Cookie-Name: s_cc {#section-03aa90aa7e36427b8cb12dc4a0f0291e}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Dieses Cookie wird vom JavaScript-Code gesetzt und gelesen, um zu bestimmen, ob Cookies aktiviert sind (auf &quot;True&quot;eingestellt). |
| Ablauf | Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird |
| Nutzung | Nur ein Cookie für alle Konten |
| Position | Dieses Cookie wird in der Domäne der Seite gespeichert. |
| Größe | 4 Byte |

{style=&quot;table-layout:auto&quot;}

## Cookie-Name: s_sq {#section-8abfff3a302d494f81a3cfb91e3b09ff}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Dieses Cookie wird vom JavaScript-Code gesetzt und gelesen, wenn die SelectMap-Funktion oder die Activity Map-Funktion aktiviert sind. Es enthält Informationen zum vorherigen Link, der vom Benutzer ausgewählt wurde. |
| Ablauf | Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird |
| Nutzung | Nur ein Cookie für alle Konten |
| Position | Dieses Cookie wird in der Domäne der Seite gespeichert. |
| Größe | Variiert je nach URL-Größe der Seite, normalerweise 100-200 Byte |

{style=&quot;table-layout:auto&quot;}

## Cookie-Name: s_vi {#section-5d50a078de444d12b7d927d68ff3b679}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Datums-/Uhrzeitstempel der Unique-Visitor-ID. |
| Ablauf | 2 Jahre |
| Nutzung | Dieses Cookie wird zur Identifizierung eines Unique Visitor verwendet. |
| Position | Dieses Cookie wird in der Domäne der Bildanforderung gespeichert. Dabei handelt es sich normalerweise um eine kundenspezifische Subdomäne unter 2o7.net oder omtrdc.net, wenn Sie Drittanbieter-Cookies verwenden oder wenn Ihre Domäne Erstanbieter-Cookies verwendet. |
| Größe | 44 Byte |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>Jede Analytics-Besucher-ID ist einem Besucherprofil auf Adobe-Servern zugewiesen. Besucherprofile werden nach einem Jahr Inaktivität gelöscht, unabhängig vom Ablauf der Besucher-ID-Cookies.

## Cookie-Name: s_fid {#section-65e33f9bfc264959ac1513e2f4b10ac7}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Fallback-Datums-/Uhrzeitstempel der Unique-Visitor-ID. |
| Ablauf | 2 Jahre |
| Nutzung | Dieses Cookie wird zur Identifizierung eines Unique Visitor verwendet. wenn das standardmäßige `s_vi`-Cookie aufgrund von Beschränkungen für Drittanbieter-Cookies nicht verfügbar ist. Es wird nicht für Implementierungen verwendet, die Erstanbieter-Cookies verwenden. |
| Position | Dieses Cookie wird als Erstanbieter-Cookie in Ihrer Domäne gespeichert. |
| Größe | 33 Byte |

{style=&quot;table-layout:auto&quot;}

## Cookie-Flags

In der folgenden Tabelle werden die Flags für Analytics-Cookies beschrieben:

| Cookie (gesetzt von) | httpOnly | Secure | SameSite |
|--- |--- |--- |--- |
| s_vi (http Response) | Nein | Ja, wenn SameSite „Keine“ lautet und die Verbindung HTTPS verwendet | Bei Verwendung von CNAME wird standardmäßig „Lax“ verwendet. „Keine“ bei Verwendung von 2o7.net oder omtrdc.net. |
| s_ecid (http-Antwort) | Nein | Nein | „Lax“ |
| s_fid (Javascript) | Nein | Nein | Löschen |
| s_cc (Javascript) | Nein | Nein | Löschen |
| s_sq (Javascript) | Nein | Nein | Löschen |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>Bei Verwendung eines einzelnen CNAME zur Verfolgung über mehrere Domänen oder Eigenschaften hinweg sollte SameSite für `s_vi` auf „Keine“ festgelegt werden. Hilfe beim Ändern der Analytics-Cookie-Einstellungen erhalten Sie bei der Kundenunterstützung.

## Von Plug-ins eingestellte Cookies {#section-a6b1cae8454945fab9eea5c7884c40fc}

Zusätzliche Cookies können je nach Verwendung von Analytics-Plug-Ins gesetzt werden. Diese Cookies sind Codefragmente, die dem Client zur Verwendung unter verschiedenen Umständen zur Verfügung stehen. Dazu gehören: Abrufen von Werten aus der URL; Verketten von Werten, die an Analytics übergeben werden sollen; Erfassen des Formularabbruchs usw. Weitere Informationen zu Cookies, die von jedem Plug-in gesetzt werden, erhalten Sie von der Kundenunterstützung. Beispiel: das Cookie [!DNL s_vh] wird mit den Plug-ins *Set Once Per* und *Set and Get Last Value* verwendet.

Konversionsvariablen (eVarX), die in einer Bildanforderung ohne JavaScript übergeben werden (z. B. Code in einer E-Mail), werden nur dann richtig zugeordnet, wenn der E-Mail-Client und der Webbrowser Cookie-Speicherplatz gemeinsam nutzen.
