---
description: Implementieren Sie den DNS-Vorabruf, um die Seitenladezeiten verschiedener Lösungen und Dienste zu reduzieren.
seo-description: Implementieren Sie den DNS-Vorabruf, um die Seitenladezeiten verschiedener Lösungen und Dienste zu reduzieren.
seo-title: Verwenden von DNS-Vorab-Lösungen mit verschiedenen Lösungen und Diensten
solution: Experience Cloud
title: Verwenden von DNS-Vorab-Lösungen mit verschiedenen Lösungen und Diensten
uuid: 4220 e 223-e 00 e -46 b 1-8 bde -52248913 bea 1
translation-type: tm+mt
source-git-commit: af5339fe58ce884345804574c209907d6504a483

---


# Verwenden von DNS-Vorab-Lösungen mit verschiedenen Lösungen und Diensten

Implementieren Sie den DNS-Vorabruf, um die Seitenladezeiten verschiedener Lösungen und Dienste zu reduzieren.

## DNS-Vorab-Abruf {#section_772BF9CB7C4141DE9B0355146E2CD962}

Mithilfe des DNS-Vorabrufs können Browser auf Webseiten verlinkte Domänennamen automatisch in die zugehörigen IP-Adressen umwandeln. Der Vorabruf beginnt, sobald in Ihrem Browser eine Webseite geladen wird. Beispiel: Ihre Seite enthält einen anklickbaren Link zu `www.adobe.com`. Lädt ein Browser diese Seite, nutzt dieser das [DNS-System](https://www.networksolutions.com/support/what-is-a-domain-name-server-dns-and-how-does-it-work/), um den verlinkten Domänennamen nachzuschlagen und ihn in die zugehörige, numerische IP-Adresse umzuwandeln. Mithilfe des DNS-Vorabrufs lässt sich die Leistung einer Seite verbessern, da der Domännename bereits in eine IP-Adresse umgewandelt wurde, bevor ein Besucher auf den Link oder die zugehörige Schaltfläche klickt. Der DNS-Vorabruf ist für Benutzer vollständig transparent.

## DNS-Prefetch und Adobe Experience Cloud-Lösungen {#section_202A07F9F79F4ABDA44B98BA1DDCD516}

Der DNS-Vorabruf kann automatisch für statische, eingebettete Links auf einer Seite verwendet werden. Das bedeutet, dass der DNS-Vorabruf aus folgenden Gründen nicht für unterschiedliche Lösungen und Dienste der [!UICONTROL Experience Cloud] eingesetzt werden kann:

* Jede Lösung und jeder Dienst der Experience Cloud generiert beim Laden einer Seite dynamisch DNS-Aufrufe.
* Der Browser ist nicht in der Lage, Domänennamen in IP-Adressen umzuwandeln, bevor diese Aufrufe getätigt werden.

Sie können jedoch manuell einen DNS-Vorabruf in Ihre Experience Cloud-Lösungen einbetten. Fügen Sie das HTML `<dns-prefetch>` -Tag dem `<head>` Abschnitt Ihres Seitencodes wie unten gezeigt hinzu. Wurde der DNS-Vorabruf ordnungsgemäß implementiert, verkürzt er das Laden von Seiten unter Umständen um einige Millisekunden.

## DNS-Vorabrufen von Codebeispielen {#section_E886F7B2861E48BA9EF3D8B3CE32B345}

In den folgenden Beispielen ist dargestellt, wie Sie DNS-Vorabrufe an unterschiedliche Lösungen und Dienste der [!DNL Experience Cloud] tätigen können. Für einige Vorabrufe werden Ihre [!DNL Adobe]-Organisations-ID oder Tracking-Server-Daten benötigt. In den folgenden Beispielen steht der *kursive* Code für einen variablen Platzhalter. Diesen würden Sie durch Ihre eigene [!DNL Adobe]-Partner-ID, Kundennummer, Tracking-Server-Daten usw. ersetzen.

* **Analytics:** `<link rel="dns-prefetch" href="//insert tracking server name here">`.

   Fügen Sie jeden DNS-Namen einzeln ein, wenn Sie sichere und nicht sichere Tracking-Server nutzen.

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">`

* **Experience Cloud ID-Dienst:**`<link rel="dns-prefetch" href="//fast. *`hier Partner-ID einfügen`*.demdex.net">`

* **Dynamischer Tag-Manager** (DTM): Nicht erforderlich. DTM-Links sind verfügbar, sobald die Seite lädt.

* **Media Optimizer (Ad Cloud):**

   * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`
   * `<link rel="dns-prefetch" href="//cm.everesttechnet">`


* **Target:** `<link rel="dns-prefetch" href="//insert customer code here.tt.omtrdc.net">`

>[!MORE_ LIKE_ THIS]
>
>* [DNS-Vorabruf](https://www.chromium.org/developers/design-documents/dns-prefetching)

