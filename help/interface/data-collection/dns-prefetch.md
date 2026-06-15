---
description: Erfahren Sie, wie Sie den DNS-Vorabruf implementieren, um die Seitenladezeiten bei verschiedenen Anwendungen und Services in CX Enterprise zu reduzieren.
solution: Experience Cloud
title: DNS-Vorabruf verwenden
uuid: 4220e223-e00e-46b1-8bde-52248913bea1
topic: Administration
role: Admin
level: Experienced
exl-id: caf2ff76-2076-436d-a5a7-aff531464480
TQID: https://experienceleague.adobe.com/oAe81mw-qFetDM0zky2eS6DNf-XZ67H68Qw-Sa8mk0Y
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: b75843fa-0a67-4a44-a6b1-cc627b0481dcid: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 352
ht-degree: 76%

---

# Verwenden des DNS-Vorabrufs

Implementieren Sie den DNS-Vorabruf, um die Seitenladezeiten verschiedener Programme und Services zu reduzieren.

## Vorstellung des DNS-Vorabrufs

Browser verwenden den DNS-Vorabruf, um Domänennamen, die auf einer Webseite mit ihren entsprechenden IP-Adressen verknüpft sind, automatisch aufzulösen. Der Vorabrufprozess beginnt, wenn der Browser eine Webseite lädt. Nehmen wir als Beispiel an, dass Ihre Seite einen anklickbaren Link zu `www.adobe.com` enthält. Lädt ein Browser diese Seite, nutzt er das _DNS-System_, um den verlinkten Domänennamen zu suchen und ihn in die zugehörige numerische IP-Adresse umzuwandeln. Der DNS-Vorabruf trägt zur Verbesserung der Seiten-Performance bei, da der Domänenname bereits in eine IP-Adresse aufgelöst wird, bevor ein Site-Besucher auf diesen Link oder diese Schaltfläche klickt. Der DNS-Vorabrufprozess ist für die Benutzer transparent.

## DNS-Vorabruf und Adobe CX Enterprise-Anwendungen

Der DNS-Vorabruf funktioniert für statische, eingebettete Links auf einer Seite automatisch. Dies bedeutet auch, dass der automatische DNS-Vorabruf nicht mit verschiedenen Anwendungen und Services [!UICONTROL CX Enterprise] funktioniert, da:

* Jedes Programm oder jeder Service von CX Enterprise generiert beim Laden der Seite dynamisch DNS-Aufrufe.
* Der Browser kann Domain-Namen nicht in IP-Adressen auflösen, bevor diese Aufrufe durchgeführt werden.

Sie können den DNS-Vorabruf jedoch manuell in Ihre CX Enterprise-Anwendungen implementieren. Fügen Sie hierzu das HTML`<dns-prefetch>`-Tag wie unten dargestellt in den Abschnitt `<head>` Ihres Seiten-Codes ein. Wurde der DNS-Vorabruf ordnungsgemäß implementiert, verkürzt er das Laden von Seiten unter Umständen um einige Millisekunden.

## Code-Beispiele für den DNS-Vorabruf

In den folgenden Beispielen wird dargestellt, wie Sie DNS-Vorabrufe an unterschiedliche Programme und Services von [!DNL CX Enterprise] tätigen können. Für einige Vorabrufe werden Ihre [!DNL Adobe]-Organisations-ID oder Tracking-Server-Daten benötigt. In den folgenden Beispielen steht der *kursive* Code für einen variablen Platzhalter. Diesen Code würden Sie durch Ihre eigene [!DNL Adobe]-Partner-ID, Kundennummer, Tracking-Server-Information usw. ersetzen.

* **Analytics:** `<link rel="dns-prefetch" href="//data.example.com">`.

  Fügen Sie jeden DNS-Namen einzeln ein, wenn Sie sichere und nicht sichere Tracking-Server nutzen.

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">`

* **CX Enterprise ID-Service:** `<link rel="dns-prefetch" href="//fast.examplepartnerid.demdex.net">`

* **Advertising Cloud:**

   * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`
   * `<link rel="dns-prefetch" href="//cm.everesttech.net">`

* **[!DNL Target]:** `<link rel="dns-prefetch" href="//example.tt.omtrdc.net">`

>[!MORELIKETHIS]
>
>* [DNS-Vorabruf](https://www.chromium.org/developers/design-documents/dns-prefetching) auf Chromium

