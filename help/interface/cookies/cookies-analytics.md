---
description: Adobe Analytics verwendet Cookies, um Anforderungen von verschiedenen Browsern zu unterscheiden und nützliche Informationen, die von einer Anwendung später genutzt werden können, zu speichern. Cookies können auch eingesetzt werden, um Browserinformationen Kundendatensätzen zuzuordnen.
keywords: Cookies; Datenschutz
seo-description: Adobe Analytics verwendet Cookies, um Anforderungen von verschiedenen Browsern zu unterscheiden und nützliche Informationen, die von einer Anwendung später genutzt werden können, zu speichern. Cookies können auch eingesetzt werden, um Browserinformationen Kundendatensätzen zuzuordnen.
seo-title: Analytics-Cookies
solution: Marketing Cloud, Analytics, Target, Social
title: Analytics-Cookies
uuid: e 2 d 3 d 61 d -2708-48 b 2-a 7 e 6-2331 f 2 aed 8 e 0
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: f59badcd3423ada51a3fe0c605158a009d5b1d64

---


# Analytics-Cookies{#analytics-cookies}

Adobe Analytics verwendet Cookies, um Anforderungen von verschiedenen Browsern zu unterscheiden und nützliche Informationen, die von einer Anwendung später genutzt werden können, zu speichern. Cookies können auch eingesetzt werden, um Browserinformationen Kundendatensätzen zuzuordnen.

Analytics verwendet Cookies vor allem, um anonym neue Besucher zu definieren, Clickstreamdaten zu analysieren und historische Aktivitäten auf der Website zu verfolgen, wie die Reaktion auf bestimmte Kampagnen oder die Länge des Verkaufszyklus.

* [Cookie-Name: s_ ecid](../cookies/cookies-mc.md#section-32fd753c3fa54452acd62b021434919a)
* [Cookie-Name: AMCV_###@AdobeOrg](../cookies/cookies-mc.md#section-a12aa2a9296940ae82d8921b381b8fb0)
* [Cookie-Name: s_cc](../cookies/cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [Cookie-Name: s_cc](../cookies/cookies-analytics.md#section-03aa90aa7e36427b8cb12dc4a0f0291e)
* [Cookie-Name: s_sq](../cookies/cookies-analytics.md#section-8abfff3a302d494f81a3cfb91e3b09ff)
* [Cookie-Name: s_vi](../cookies/cookies-analytics.md#section-5d50a078de444d12b7d927d68ff3b679)
* [Cookie-Name: s_fid](../cookies/cookies-analytics.md#section-65e33f9bfc264959ac1513e2f4b10ac7)
* [Von Plug-ins eingestellte Cookies](../cookies/cookies-analytics.md#section-a6b1cae8454945fab9eea5c7884c40fc)

Weitere Informationen finden Sie in der Analytics-Hilfe zu [Erstanbieter-Cookies](/help/interface/cookies/cookies-first-party.md).

## Cookie-Name: s_ ecid {#section-32fd753c3fa54452acd62b021434919a}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Enthält eine Kopie der Experience Cloud ID (ECID) oder MID. Die MID wird in einem Schlüssel-Wert-Paar gespeichert, das auf diese Syntax folgt, s_ ecid = MCMID. | <ECID> |
| Ablauf | 2 Jahre |
| Nutzung | Dieses Cookie wird durch die Domäne des Kunden festgelegt, nachdem das AMCV-Cookie vom Client festgelegt wurde. Dieses Cookie soll die dauerhafte ID-Verfolgung im Status 1 ^ st ^ Party zulassen und wird als Referenz-ID verwendet, wenn das AMCV-Cookie abgelaufen ist. Weitere Details finden Sie im AMCV-Cookie. |
| Position | Nur CNAME-Kunden. Gilt nicht für Drittanbieterszenarien. Cookie wird in Ihrer Domäne gespeichert, dieselbe Domäne wie CNAME und Ihre Analytics-Bildanforderung. |
| Größe | 45 Byte |

## Cookie-Name: s_cc {#section-03aa90aa7e36427b8cb12dc4a0f0291e}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Dieses Cookie wurde vom JavaScript-Code eingestellt und gelesen, um festzustellen, ob Cookies aktiviert wurden (einfach auf „True“ einstellen) |
| Ablauf | Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird |
| Nutzung | Nur ein Cookie für alle Konten |
| Position | Dieses Cookie wird in der Domäne der Seite gespeichert |
| Größe | 4 Byte |

## Cookie-Name: s_sq {#section-8abfff3a302d494f81a3cfb91e3b09ff}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Dieses Cookie wird vom JavaScript-Code gesetzt und gelesen, wenn die ClickMap-Funktion und die Activity Map-Funktion aktiviert sind. Es enthält Informationen über den vorherigen Link, der vom Benutzer angeklickt wurde. |
| Ablauf | Dieses Cookie ist ein Sitzungs-Cookie und läuft ab, wenn der Browser geschlossen wird |
| Nutzung | Nur ein Cookie für alle Konten |
| Position | Dieses Cookie wird in der Domäne der Seite gespeichert |
| Größe | Variiert je nach URL-Größe der Seite, normalerweise 100-200 Byte |

## Cookie-Name: s_vi {#section-5d50a078de444d12b7d927d68ff3b679}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Unique Visitor-ID, Zeit-/Datumsstempel |
| Ablauf | 2 Jahre |
| Nutzung | Dieses Cookie wird zur Identifizierung eines Unique Visitor verwendet |
| Position | Dieses Cookie wird unter der Domäne der Bildanforderung gespeichert – üblicherweise 2O7.net, wenn Sie Drittanbieter-Cookies verwenden, oder Ihre Domäne, wenn Sie Erstanbieter-Cookies verwenden. |
| Größe | 44 Byte |

>[!NOTE]
>
>Jede Analytics-Besucher-ID ist mit einem Besucherprofil auf Adobe-Servern verknüpft. Besucherprofile werden nach einem Jahr Inaktivität gelöscht, unabhängig vom Ablauf der Besucher-ID-Cookies.

## Cookie-Name: s_fid {#section-65e33f9bfc264959ac1513e2f4b10ac7}

| Attribut | Beschreibung |
|--- |--- |
| Gespeicherte Informationen | Unique Visitor-ID, Zeit-/Datumsstempel (Fallback) |
| Ablauf | 5 Jahre |
| Nutzung | Dieses Cookie wird zur Identifizierung eines Unique Visitor verwendet wenn das standardmäßig eingesetzte Cookie s_vi aufgrund von Beschränkungen für Drittanbieter-Cookies nicht verfügbar ist. Wird nicht für Implementierungen eingesetzt, die Erstanbieter-Cookies verwenden. |
| Position | Dieses Cookie wird als Erstanbieter-Cookie in Ihrer Domäne gespeichert. |
| Größe | 33 Byte |

## Von Plug-ins eingestellte Cookies {#section-a6b1cae8454945fab9eea5c7884c40fc}

Zusätzliche Cookies können je nach Verwendung von Analytics-Plug-ins gesetzt werden. Diese Cookies sind Codefragmente, die dem Client zur Verwendung in verschiedensten Situationen zur Verfügung stehen. Zu diesen Situationen zählen: Abrufen von Werten aus der URL, Verknüpfen von Werten zur Weitergabe an Analytics, Erfassen von Formularabbrüchen usw. Weitere Informationen zu Cookies, die von jedem Plug-in eingestellt werden, erhalten Sie bei ClientCare. Beispiel: das Cookie [!DNL s_vh] wird mit den Plug-ins *Set Once Per* und *Set and Get Last Value* verwendet.

Umrechnungs- bzw. Konversionsvariablen (eVarX), die auf eine Bildanforderung ohne JavaScript hin weitergegeben werden, wie z. B. Code in einer E-Mail, werden nur dann richtig zugewiesen, wenn der E-Mail-Client und der Webbrowser denselben Cookie-Bereich nutzen.
