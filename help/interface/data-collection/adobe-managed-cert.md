---
description: Erfahren Sie, wie Sie sichere Zertifikate für die Verwendung mit Adobe Experience Cloud-Erstanbieter-Cookies einrichten.
solution: Experience Cloud,Analytics
title: Adobe-Managed Certificate Program
index: y
snippet: y
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 4%

---

# Adobe Managed Certificate Program

Das Adobe-Managed Certificate Program (Programm für verwaltete Zertifikate) ist der empfohlene Prozess zum Einrichten von Erstanbieterzertifikaten, die für eine CNAME-Implementierung erforderlich sind. Das Programm ist nach der Konfiguration vollständig automatisiert. Zertifikate werden rechtzeitig erneuert, sodass sich die Datenerfassung aufgrund abgelaufener Zertifikate nicht auswirkt. Das Programm ist kostenlos für Ihre ersten 100 CNAMEs.

Wenn Sie derzeit Ihre eigenen Zertifikate verwalten, sind Sie dafür verantwortlich, ein Zertifikat für die Verwendung von Erstanbieter-Cookies zu erwerben, zu pflegen und dem Adobe bereitzustellen. Sie können sich an die Adobe-Kundenunterstützung wenden, um die Migration zum Adobe-verwalteten Zertifikatsprogramm zu besprechen.

## Implementierung

Führen Sie die folgenden Schritte aus, um ein neues Zertifikat für die Erstanbieter-Datenerfassung zu implementieren:

1. Laden Sie das Anforderungsformular für [-Domains herunter und füllen Sie es aus](cookies/assets/First_Party_Domain_Request_Form.xlsx)

1. Öffnen Sie ein Ticket bei der Adobe-Kundenunterstützung, um die Erstanbieter-Datenerfassung im Adobe-verwalteten Zertifikatsprogramm einzurichten.

1. Nach Erhalt des Tickets stellt Ihnen der Adobe-Repräsentant einen CNAME-Eintrag zur Verfügung. Diese Datensätze müssen auf dem DNS-Server Ihres Unternehmens konfiguriert werden, bevor Adobe das Zertifikat in Ihrem Namen erwerben kann. Beispielsweise verweist der Hostname-`data.example.com` auf `hiodsibxvip01.data.adobedc.net`.

1. Wenn der CNAME-Eintrag auf den Servern Ihres Unternehmens vorhanden ist, kauft und installiert Adobe gemeinsam mit DigiCert ein Zertifikat auf Adobe-Datenerfassungsservern.

## Überprüfen der Hostnamenweiterleitung {#validate}

Nachdem Adobe das Zertifikat installiert hat, können Sie eine der folgenden Methoden verwenden, um zu überprüfen, ob es funktioniert.

+++**Browser-Validierung**

Sie können jeden Browser verwenden, um zu überprüfen, ob ein Zertifikat korrekt installiert ist. Geben Sie Ihren CNAME mit `_check` als Pfad in die Adressleiste ein. z. B.:

`data.example.com/_check`

Wenn alles funktioniert, zeigt der Browser `SUCCESS` an. Wenn das Zertifikat nicht korrekt installiert ist, wird eine Sicherheitswarnung ausgegeben.

+++

+++**Befehlszeile (`curl`)**

Die meisten modernen Betriebssysteme [`curl`](https://curl.se) bereits installiert.

Geben Sie Folgendes in die Befehlszeile ein:

```sh
curl data.example.com/_check
```

Wenn alles ordnungsgemäß funktioniert, gibt die Konsole `SUCCESS` zurück.

>[!TIP]
>
>Sie können die `-k`-Markierung verwenden, um die Sicherheitswarnung zu deaktivieren und so die Fehlerbehebung zu erleichtern.

+++

+++**Befehlszeile (`nslookup`)**

Geben Sie Folgendes in die Befehlszeile ein:

```sh
nslookup data.example.com
```

Wenn alles ordnungsgemäß funktioniert, werden die Datenerfassungs-Server von Adobe zurückgegeben:

```text
Server: hiodsibxvip01.corp.adobe.com
Address: 10.50.112.247

Name: example.com.ssl.d1.sc.omtrdc.net
Addresses: 63.140.37.126
    63.140.37.206
    63.140.36.51
    63.140.36.145
Aliases: smetrics.example.com
```

+++

## Aktualisierung des Implementierungscodes {#update}

Nachdem Sie überprüft haben, ob Ihr Zertifikat ordnungsgemäß funktioniert, können Sie Ihre Adobe-Implementierung aktualisieren, um diese Werte zu verwenden.

* Aktualisieren Sie bei Adobe Analytics AppMeasurement-Implementierungen die [`trackingServer`](https://experienceleague.adobe.com/de/docs/analytics/implementation/vars/config-vars/trackingserver) Konfigurationsvariable . Wenn Sie über eine vorhandene Implementierung verfügen, finden Sie [Besuchermigration](https://experienceleague.adobe.com/de/docs/analytics/technotes/visitor-migration) weitere Schritte, um zu verhindern, dass vorhandene Besucher als neue Besucher gezählt werden.
* Bei Web-SDK-Implementierungen aktualisieren Sie die [`edgeDomain`](https://experienceleague.adobe.com/de/docs/experience-platform/web-sdk/commands/configure/edgedomain)-Eigenschaft im [`configure`](https://experienceleague.adobe.com/de/docs/experience-platform/web-sdk/commands/configure/overview).

## Wartung und Erneuerung

Adobe überprüft 30 Tage vor Ablauf Ihres Erstanbieterzertifikats, ob der CNAME noch gültig und in Verwendung ist. Wenn ja, geht Adobe davon aus, dass Sie den Service weiterhin verwenden möchten, und erneuert das Zertifikat automatisch in Ihrem Namen.

>[!IMPORTANT]
>
>Wenn der CNAME-Eintrag Ihres Unternehmens entfernt wurde oder nicht mehr dem bereitgestellten sicheren Adobe-Hostnamen zugeordnet ist, kann Adobe das Zertifikat nicht verlängern. Der Eintrag im Adobe-System wird ohne weitere Mitteilung zur Entfernung markiert.

## Häufig gestellte Fragen

+++Ist dieser Prozess sicher?

Ja. Das Adobe-verwaltete Zertifikatsprogramm ist sicherer als die Bereitstellung eines Zertifikats für Adobe durch Ihr Unternehmen. Außerhalb des Adobe und der ausstellenden Zertifizierungsstelle wechselt kein Zertifikat bzw. kein privater Schlüssel den Besitzer.

+++

+++Wie kann Adobe ein Zertifikat für unsere Domain erwerben?

Das Zertifikat kann nur erworben werden, wenn der angegebene Hostname auf einen Adobe-eigenen Hostnamen verweist. Sie delegieren diesen Hostnamen an Adobe und erlauben Adobe, das Zertifikat in Ihrem Namen zu erwerben.

+++

+++Kann ich beantragen, dass das Zertifikat widerrufen wird?

Ja. Als Eigentümer der Domain sind Sie berechtigt, den Widerruf des Zertifikats zu verlangen. Wenden Sie sich an die Adobe-Kundenunterstützung, um diesen Prozess zu starten.

+++

+++Welcher Verschlüsselungstyp wird verwendet?

Adobe arbeitet mit DigiCert zusammen, um ein SHA-2-Zertifikat auszustellen.

+++

+++Entstehen für dieses Programm zusätzliche Kosten?

Nein. Adobe bietet diesen Service allen Adobe Experience Cloud-Kunden kostenlos an.

+++

+++Welche Chiffrier-Sicherheitsstufen bietet Adobe?

Adobe bietet zwei Chiffrier-Sicherheitsstufen, die den unterschiedlichen Sicherheitsanforderungen bei der Erfassung von First-Party-Daten gerecht werden. Diese Stufen bestimmen, welche Verschlüsselungsalgorithmen für HTTPS-Verbindungen mit Adobe-Servern unterstützt werden. Adobe überprüft und aktualisiert regelmäßig die unterstützten Algorithmen auf der Grundlage aktueller Sicherheitspraktiken. Wenn Sie Ihre Chiffrier-Sicherheitseinstellungen ändern möchten, wenden Sie sich an die Kundenunterstützung.

* **Standard** erfordert TLS 1.2 oder höher und mindestens 128-Bit-Verschlüsselung. Es wurde entwickelt, um die größtmögliche Gerätekompatibilität bei gleichzeitiger Beibehaltung einer sicheren Verschlüsselung zu gewährleisten.
* **Hoch** Die Chiffrier-Sicherheitsstufe erfordert TLS 1.2 oder höher und entfernt die Unterstützung für schwächere Chiffren. Es wurde für Kunden entwickelt, die die stärkste Verschlüsselung wünschen und sich nicht um die Unterstützung älterer Geräte kümmern.

Es ist bekannt, dass die folgenden Clients keine Verbindung mit der auf „Hoch“ gesetzten **herstellen**:

* Windows 8.1 und niedriger (zuletzt aktualisiert 2018)
* Windows Phone 8.1 und niedriger (zuletzt aktualisiert 2016)
* OS X 10.10 und früher (zuletzt aktualisiert 2017)
* iOS 8.4 und niedriger (zuletzt aktualisiert 2015)

+++

+++Welche HTTPS-Zertifikatstypen werden unterstützt?

Adobe unterstützt sowohl RSA- als auch ECC-Zertifikatstypen, um unterschiedlichen Kundenanforderungen gerecht zu werden. RSA-Zertifikate werden für Clients häufiger unterstützt, aber ECC-Zertifikate verbrauchen sowohl auf Server- als auch auf Client-Seite weniger Verarbeitung. Für Adobe-verwaltete Zertifikate werden sowohl RSA als auch ECC bereitgestellt. Für kundenverwaltete Zertifikate ist eine RSA erforderlich, und es wird eine ECC empfohlen. Moderne Clients unterstützen sowohl RSA als auch ECC. Die folgenden Clients unterstützen in der Regel nur RSA-Zertifikate:

* Windows Vista und früher (zuletzt aktualisiert 2012)
* Windows Phone 8.0 und niedriger (zuletzt aktualisiert 2014)
* OS X 10.8 und niedriger (zuletzt aktualisiert 2013)
* iOS 5.1 und niedriger (zuletzt aktualisiert 2012)
* Android 4.3 und niedriger (zuletzt aktualisiert 2013)

+++
