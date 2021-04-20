---
description: Erfahren Sie, wie Sie den DNS-Vorabruf implementieren, um die Seitenladezeit bei verschiedenen Lösungen und Diensten in Experience Cloud zu reduzieren.
solution: Experience Cloud
title: 'Verwendung des DNS-Vorabrufs für verschiedene Lösungen und Dienste '
uuid: 4220e223-e00e-46b1-8bde-52248913bea1
feature: Customer Attributes
topic: Administration
role: Administrator
level: Experienced
translation-type: tm+mt
source-git-commit: ea8f36313940d7c5c12d753084a4fb8d0a4379bc
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 100%

---


# Verwendung des DNS-Vorabrufs für verschiedene Lösungen und Dienste

Implementieren Sie den DNS-Vorabruf, um die Seitenladezeiten verschiedener Lösungen und Dienste zu reduzieren.

## Vorstellung des DNS-Vorabrufs {#section_772BF9CB7C4141DE9B0355146E2CD962}

Browser verwenden den DNS-Vorabruf, um Domänennamen, die auf einer Webseite mit ihren entsprechenden IP-Adressen verknüpft sind, automatisch aufzulösen. Der Vorabrufprozess beginnt, wenn der Browser eine Webseite lädt. Nehmen wir als Beispiel an, dass Ihre Seite einen anklickbaren Link zu `www.adobe.com` enthält. Lädt ein Browser diese Seite, nutzt er das [DNS-System](https://www.networksolutions.com/support/what-is-a-domain-name-server-dns-and-how-does-it-work/), um den verlinkten Domänennamen zu suchen und ihn in die zugehörige numerische IP-Adresse umzuwandeln. Der DNS-Vorabruf trägt zur Verbesserung der Seitenleistung bei, da der Domänenname bereits in eine IP-Adresse aufgelöst wird, bevor ein Site-Besucher auf diesen Link oder diese Schaltfläche klickt. Der DNS-Vorabrufprozess ist für die Benutzer transparent.

## DNS-Vorabruf und Adobe Experience Cloud-Lösungen {#section_202A07F9F79F4ABDA44B98BA1DDCD516}

Der DNS-Vorabruf funktioniert für statische, eingebettete Links auf einer Seite automatisch. Dies bedeutet auch, dass der automatische DNS-Vorabruf nicht mit verschiedenen [!UICONTROL Experience Cloud]-Lösungen und -Diensten funktioniert, weil:

* Jede Experience Cloud-Lösung oder jeder Experience Cloud-Dienst generiert beim Laden der Seite dynamisch DNS-Aufrufe.
* Der Browser kann Domänennamen nicht in IP-Adressen auflösen, bevor diese Aufrufe durchgeführt werden.

Sie können jedoch den DNS-Vorabruf manuell in Ihre Experience Cloud-Lösungen implementieren. Fügen Sie hierzu das HTML`<dns-prefetch>`-Tag wie unten dargestellt in den Abschnitt `<head>` Ihres Seiten-Codes ein. Wurde der DNS-Vorabruf ordnungsgemäß implementiert, verkürzt er das Laden von Seiten unter Umständen um einige Millisekunden.

## Code-Beispiele für den DNS-Vorabruf {#section_E886F7B2861E48BA9EF3D8B3CE32B345}

In den folgenden Beispielen ist dargestellt, wie Sie DNS-Vorabrufe an unterschiedliche Lösungen und Dienste der [!DNL Experience Cloud] tätigen können. Für einige Vorabrufe werden Ihre [!DNL Adobe]-Organisations-ID oder Tracking-Server-Daten benötigt. In den folgenden Beispielen steht der *kursive* Code für einen variablen Platzhalter. Diesen würden Sie durch Ihre eigene [!DNL Adobe]-Partner-ID, Kundennummer, Tracking-Server-Daten usw. ersetzen.

* **Analytics:** `<link rel="dns-prefetch" href="//insert tracking server name here">`.

   Fügen Sie jeden DNS-Namen einzeln ein, wenn Sie sichere und nicht sichere Tracking-Server nutzen.

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">`

* **Experience Cloud ID-Dienst:** `<link rel="dns-prefetch" href="//fast. *`hier Partner-ID einfügen`*.demdex.net">`

* **Dynamischer Tag-Manager** (DTM): nicht erforderlich. DTM-Links sind verfügbar, sobald die Seite lädt.

* **Media Optimizer (Ad Cloud):**

   * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`
   * `<link rel="dns-prefetch" href="//cm.everesttechnet">`


* **[!DNL Target]:** `<link rel="dns-prefetch" href="//insert customer code here.tt.omtrdc.net">`

>[!MORELIKETHIS]
>
>* [DNS-Vorabruf](https://www.chromium.org/developers/design-documents/dns-prefetching)

