---
description: Hier erfahren Sie, wie Sie den DNS-Vorabruf implementieren, um die Seitenladezeit bei verschiedenen Programmen und Services in Experience Cloud zu reduzieren.
solution: Experience Cloud
title: DNS-Vorabruf verwenden
uuid: 4220e223-e00e-46b1-8bde-52248913bea1
topic: Administration
role: Admin
level: Experienced
exl-id: caf2ff76-2076-436d-a5a7-aff531464480
source-git-commit: 9ee4d9b0e670dec35cda530892c49e36bf7cc107
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 90%

---

# DNS-Vorabruf verwenden

Implementieren Sie den DNS-Vorabruf, um die Seitenladezeiten verschiedener Programme und Services zu reduzieren.

## Vorstellung des DNS-Vorabrufs

Browser verwenden den DNS-Vorabruf, um Domänennamen, die auf einer Webseite mit ihren entsprechenden IP-Adressen verknüpft sind, automatisch aufzulösen. Der Vorabrufprozess beginnt, wenn der Browser eine Webseite lädt. Nehmen wir als Beispiel an, dass Ihre Seite einen anklickbaren Link zu `www.adobe.com` enthält. Lädt ein Browser diese Seite, nutzt er das [DNS-System](https://www.networksolutions.com/support/what-is-a-domain-name-server-dns-and-how-does-it-work/), um den verlinkten Domänennamen zu suchen und ihn in die zugehörige numerische IP-Adresse umzuwandeln. Der DNS-Vorabruf trägt zur Verbesserung der Seiten-Performance bei, da der Domänenname bereits in eine IP-Adresse aufgelöst wird, bevor ein Site-Besucher auf diesen Link oder diese Schaltfläche klickt. Der DNS-Vorabrufprozess ist für die Benutzer transparent.

## DNS-Vorabruf und Adobe Experience Cloud-Programme

Der DNS-Vorabruf funktioniert für statische, eingebettete Links auf einer Seite automatisch. Dies bedeutet auch, dass der automatische DNS-Vorabruf nicht mit verschiedenen [!UICONTROL Experience Cloud] Anwendungen und Dienste aus folgenden Gründen:

* Jedes Programm und jeder Service von Experience Cloud generiert beim Laden der Seite dynamisch DNS-Aufrufe.
* Der Browser kann Domain-Namen nicht in IP-Adressen auflösen, bevor diese Aufrufe durchgeführt werden.

Sie können jedoch den DNS-Vorabruf manuell in Ihre Experience Cloud-Programme implementieren. Fügen Sie hierzu das HTML`<dns-prefetch>`-Tag wie unten dargestellt in den Abschnitt `<head>` Ihres Seiten-Codes ein. Wurde der DNS-Vorabruf ordnungsgemäß implementiert, verkürzt er das Laden von Seiten unter Umständen um einige Millisekunden.

## Code-Beispiele für den DNS-Vorabruf

In den folgenden Beispielen wird dargestellt, wie Sie DNS-Vorabrufe an unterschiedliche Programme und Services von [!DNL Experience Cloud] tätigen können. Für einige Vorabrufe werden Ihre [!DNL Adobe]-Organisations-ID oder Tracking-Server-Daten benötigt. In den folgenden Beispielen steht der *kursive* Code für einen variablen Platzhalter. Diesen Code würden Sie durch Ihre eigene [!DNL Adobe]-Partner-ID, Kundennummer, Tracking-Server-Information usw. ersetzen.

* **Analytics:** `<link rel="dns-prefetch" href="//data.example.com">`.

  Fügen Sie jeden DNS-Namen einzeln ein, wenn Sie sichere und nicht sichere Tracking-Server nutzen.

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">`

* **Experience Cloud ID-Dienst:** `<link rel="dns-prefetch" href="//fast.examplepartnerid.demdex.net">`

* **Advertising Cloud:**

   * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`
   * `<link rel="dns-prefetch" href="//cm.everesttech.net">`

* **[!DNL Target]:** `<link rel="dns-prefetch" href="//example.tt.omtrdc.net">`

>[!MORELIKETHIS]
>
>* [DNS-Vorabruf](https://www.chromium.org/developers/design-documents/dns-prefetching) Chromium
