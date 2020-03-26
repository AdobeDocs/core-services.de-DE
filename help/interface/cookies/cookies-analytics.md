---
description: Adobe Analytics verwendet Cookies, um Anforderungen von verschiedenen Browsern zu unterscheiden und nützliche Informationen zu speichern, die eine Anwendung später verwenden kann. Sie können auch verwendet werden, um Browserinformationen Kundendatensätzen zuzuordnen.
keywords: cookies;privacy
seo-description: Adobe Analytics verwendet Cookies, um Anforderungen von verschiedenen Browsern zu unterscheiden und nützliche Informationen zu speichern, die eine Anwendung später verwenden kann. Sie können auch verwendet werden, um Browserinformationen Kundendatensätzen zuzuordnen.
seo-title: Analytics-Cookies
solution: Marketing Cloud,Analytics,Adobe Target,Adobe Social
title: Analytics-Cookies
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Cookiesin Analytics{#analytics-cookies}

Adobe Analytics verwendet Cookies, um Anforderungen von verschiedenen Browsern zu unterscheiden und nützliche Informationen zu speichern, die eine Anwendung später verwenden kann. Sie können auch verwendet werden, um Browserinformationen Kundendatensätzen zuzuordnen.

Analytics verwendet Cookies vor allem, um anonym neue Besucher zu definieren, Clickstream-Daten zu analysieren und historische Aktivitäten auf der Website zu verfolgen, z. B. Antworten auf bestimmte Kampagnen oder die Dauer des Verkaufszyklus.

* [Cookie-Name: s_ecid](../cookies/cookies-mc.md#section-32fd753c3fa54452acd62b021434919a)
* [Cookie-Name: AMCV_###@AdobeOrg](../cookies/cookies-mc.md#section-a12aa2a9296940ae82d8921b381b8fb0)
* [Cookie-Name: s_cc](../cookies/cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [Cookie-Name: s_cc](../cookies/cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [Cookie-Name: s_sq ](../cookies/cookies-analytics.md#section-8abfff3a302d494f81a3cfb91e3b09ff)
* [Cookie-Name: s_vi](../cookies/cookies-analytics.md#section-5d50a078de444d12b7d927d68ff3b679)
* [Cookie-Name: s_fid ](../cookies/cookies-analytics.md#section-65e33f9bfc264959ac1513e2f4b10ac7)
* [Von Plug-ins eingestellte Cookies ](../cookies/cookies-analytics.md#section-a6b1cae8454945fab9eea5c7884c40fc)

Weitere Informationen finden Sie in der Analytics-Hilfe zu [Erstanbieter-Cookies](/help/interface/cookies/cookies-first-party.md).

## Cookie-Name: s_ecid {#section-32fd753c3fa54452acd62b021434919a}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Enthält eine Kopie der Experience Cloud ID (ECID) oder der MID. Die MID wird in einem Schlüssel-Wert-Paar gespeichert, das dieser Syntax folgt: s_ecid=MCMID | `<ECID>` |
| Ablauf | 2 Jahre |
| Nutzung | Dieses Cookie wird durch die Domäne des Kunden festgelegt, nachdem das AMCV-Cookie vom Client festgelegt wurde. Dieses Cookie ermöglicht das durchgängige ID-Tracking als Erstanbieter und wird als Referenz-ID verwendet, wenn das AMCV-Cookie abgelaufen ist. Weitere Details zum AMCV-Cookie finden Sie hier. |
| Position | Nur CNAME-Kunden. Gilt nicht für Drittanbieter-Szenarien. Cookie wird in Ihrer Domäne gespeichert; dieselbe Domäne wie die von CNAME und Ihrer Analytics-Bildanforderung verwendete. |
| Größe | 45 Byte |

## Cookie-Name: s_cc {#section-03aa90aa7e36427b8cb12dc4a0f0291e}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Dieses Cookie wird vom JavaScript-Code eingestellt und gelesen, um festzustellen, ob Cookies aktiviert sind (einfach auf &quot;True&quot;setzen) |
| Ablauf | Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird |
| Nutzung | Nur ein Cookie für alle Konten |
| Position | Dieses Cookie wird in der Domäne der Seite gespeichert |
| Größe | 4 Byte |

## Cookie-Name: s_sq  {#section-8abfff3a302d494f81a3cfb91e3b09ff}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Dieses Cookie wird vom JavaScript-Code gesetzt und gelesen, wenn die ClickMap-Funktion oder die Aktivität Map-Funktion aktiviert ist. enthält Informationen zum vorherigen Link, auf den der Benutzer geklickt hat |
| Ablauf | Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird |
| Nutzung | Nur ein Cookie für alle Konten |
| Position | Dieses Cookie wird in der Domäne der Seite gespeichert |
| Größe | Variiert je nach URL-Größe der Seite, normalerweise 100-200 Byte |

## Cookie-Name: s_vi {#section-5d50a078de444d12b7d927d68ff3b679}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Eindeutiger Besucher-ID-Datums-/Uhrzeitstempel |
| Ablauf | 2 Jahre |
| Nutzung | Dieses Cookie wird zur Identifizierung eines Unique Visitor verwendet  |
| Position | Dieses Cookie wird in der Domäne der Bildanforderung gespeichert - normalerweise eine kundenspezifische Subdomäne unter 2o7.net oder omtrdc.net, wenn Sie Drittanbieter-Cookies verwenden oder wenn Ihre Domäne Erstanbieter-Cookies verwendet. |
| Größe | 44 Byte |

>[!NOTE]
>
>Jede Analytics-Besucher-ID ist einem Besucherprofil auf Adobe-Servern zugewiesen. Besucherprofile werden nach einem Jahr Inaktivität gelöscht, unabhängig vom Ablauf der Besucher-ID-Cookies.

## Cookie-Name: s_fid  {#section-65e33f9bfc264959ac1513e2f4b10ac7}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Zeitstempel/Datumsstempel für eindeutige Besucher-ID |
| Ablauf | 2 Jahre |
| Nutzung | Dieses Cookie wird zur Identifizierung eines Unique Visitor verwendet  if the standard  `s_vi` cookie is unavailable due to third-party cookie restrictions. Nicht für Implementierungen verwendet, die Erstanbieter-Cookies verwenden. |
| Position | Dieses Cookie wird als Erstanbieter-Cookie in Ihrer Domäne gespeichert. |
| Größe | 33 Byte |

## Cookie-Flags

In der folgenden Tabelle werden die Flags für Analytics-Cookies beschrieben:

| Cookie (gesetzt von) | httpOnly | Secure | SameSite |
|--- |--- |--- |--- |
| s_vi (http Response) | Nein | Ja, wenn dieselbe Site &quot;Keine&quot;ist und die Verbindung HTTPS verwendet | Bei Verwendung von CNAME wird standardmäßig &quot;Lax&quot;verwendet. &quot;Keine&quot;bei Verwendung von 2o7.net oder omtrdc.net. |
| s_ecid (http Response) | Nein | Nein | &quot;Nicht streng&quot; |
| s_fid (Javascript) | Nein | Nein | Ungestellt |
| s_cc (Javascript) | Nein | Nein | Ungestellt |
| s_sq (Javascript) | Nein | Nein | Ungestellt |

>[!NOTE] Wenn ein einziger CNAME zur Verfolgung über mehrere Domänen oder Eigenschaften hinweg verwendet wird, sollte für SameSite für `s_vi`die Verfolgung auf &quot;Keine&quot;eingestellt werden. Wenden Sie sich an den Kundendienst, um Hilfe beim Ändern der Cookie-Einstellungen in Analytics zu erhalten.

## Von Plug-ins eingestellte Cookies  {#section-a6b1cae8454945fab9eea5c7884c40fc}

Zusätzliche Cookies können je nach Verwendung von Analytics-Plug-Ins eingestellt werden. Diese Cookies sind Codefragmente, die dem Client zur Verwendung in verschiedensten Situationen zur Verfügung stehen. Dazu gehören: Abrufen von Werten aus der URL; Verketten von Werten, die an Analytics übergeben werden sollen; Erfassen des Formularabbruchs usw. Weitere Informationen zu Cookies, die von jedem Plug-in gesetzt werden, erhalten Sie von der Kundenunterstützung. Beispiel: das Cookie [!DNL s_vh] wird mit den Plug-ins *Set Once Per* und *Set and Get Last Value* verwendet.

Konversionsvariablen (eVarX), die auf eine Bildanforderung ohne JavaScript hin weitergegeben werden, wie z. B. Code in einer E-Mail, werden nur dann richtig zugewiesen, wenn der E-Mail-Client und der Webbrowser denselben Cookie-Bereich nutzen.
