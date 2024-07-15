---
description: Erfahren Sie, wie Sie sichere Zertifikate für die Verwendung mit Erstanbieter-Cookies von Adobe Experience Cloud einrichten.
solution: Experience Cloud,Analytics
title: Adobe Managed Certificate Program
index: y
snippet: y
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
source-git-commit: 028b11dfbcfc0c5c9f6fd1c69350574f81f2846b
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 4%

---

# Adobe Managed Certificate Program

Das von Adobe verwaltete Zertifikatprogramm ist der empfohlene Prozess zum Einrichten von Erstanbieterzertifikaten, die für eine CNAME-Implementierung erforderlich sind. Das Programm ist vollständig automatisiert, sobald es konfiguriert wurde. Sie erneuert Zertifikate zeitnah, sodass die Datenerfassung aufgrund abgelaufener Zertifikate keine Auswirkungen hat. Das Programm ist kostenlos für Ihre ersten 100 CNAMEs.

Wenn Sie derzeit eigene Zertifikate verwalten, sind Sie für den Kauf, die Pflege und die Bereitstellung eines Zertifikats für die Adobe zur Verwendung von Erstanbieter-Cookies verantwortlich. Sie können sich an die Adobe-Kundenunterstützung wenden, um die Migration zum Adobe-verwalteten Zertifikatprogramm zu besprechen.

## Implementierung

Führen Sie die folgenden Schritte aus, um ein neues Zertifikat für die Erstanbieter-Datenerfassung zu implementieren:

1. Laden Sie das Anforderungsformular für die Domäne des Erstanbieters herunter und füllen Sie es aus ](cookies/assets/First_Party_Domain_Request_Form.xlsx)[

1. Öffnen Sie ein Ticket bei der Adobe-Kundenunterstützung, um die Datenerfassung von Erstanbietern im Adobe-verwalteten Zertifikatprogramm einzurichten.

1. Nach Erhalt des Tickets stellt Ihnen der Adobe-Support-Mitarbeiter einen CNAME-Eintrag zur Verfügung. Diese Datensätze müssen auf dem DNS-Server Ihres Unternehmens konfiguriert werden, bevor Adobe das Zertifikat in Ihrem Namen erwerben kann. Beispielsweise verweist der Hostname `data.example.com` auf `hiodsibxvip01.data.adobedc.net`.

1. Wenn der CNAME-Eintrag auf den Servern Ihres Unternehmens vorhanden ist, kauft und installiert Adobe gemeinsam mit DigiCert ein Zertifikat auf den Adobe-Datenerfassungsservern.

## Überprüfen der Hostnamenweiterleitung {#validate}

Nachdem das Zertifikat von Adobe installiert wurde, können Sie eine der folgenden Methoden verwenden, um zu überprüfen, ob es funktioniert.

+++**Browservalidierung**

Sie können jeden Browser verwenden, um zu überprüfen, ob ein Zertifikat ordnungsgemäß installiert ist. Geben Sie Ihren CNAME mit `_check` als Pfad in die Adressleiste ein. Beispiel:

`data.example.com/_check`

Wenn alles funktioniert, zeigt der Browser `SUCCESS` an. Wenn das Zertifikat nicht richtig installiert ist, wird Ihnen eine Sicherheitswarnung angezeigt.

+++

+++**Befehlszeile (`curl`)**

Die meisten modernen Betriebssysteme haben bereits [`curl`](https://curl.se) installiert.

Geben Sie Folgendes in die Befehlszeile ein:

```sh
curl data.example.com/_check
```

Wenn alles ordnungsgemäß funktioniert, gibt die Konsole `SUCCESS` zurück.

>[!TIP]
>
>Sie können das Flag `-k` verwenden, um die Sicherheitswarnung zu deaktivieren, um die Fehlerbehebung zu unterstützen.

+++

+++**Befehlszeile (`nslookup`)**

Geben Sie Folgendes in die Befehlszeile ein:

```sh
nslookup data.example.com
```

Wenn alles ordnungsgemäß funktioniert, werden Adobe-Datenerfassungsserver zurückgegeben:

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

* Aktualisieren Sie bei Adobe Analytics AppMeasurement-Implementierungen die Konfigurationsvariable [`trackingServer`](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/config-vars/trackingserver) . Wenn Sie über eine vorhandene Implementierung verfügen, finden Sie unter [Besuchermigration](https://experienceleague.adobe.com/en/docs/analytics/technotes/visitor-migration) weitere Schritte, um zu verhindern, dass vorhandene Besucher als neue Besucher gezählt werden.
* Aktualisieren Sie bei Web SDK-Implementierungen die Eigenschaft [`edgeDomain`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/edgedomain) innerhalb des Befehls [`configure`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/overview) .

## Instandhaltung und Erneuerung

Dreißig Tage vor Ablauf Ihres Erstanbieter-Zertifikats überprüft Adobe, ob der CNAME noch gültig ist und verwendet wird. Ist dies der Fall, geht Adobe davon aus, dass Sie den Dienst weiterhin verwenden möchten, und erneuert das Zertifikat automatisch in Ihrem Namen.

>[!IMPORTANT]
>
>Wenn der CNAME-Eintrag Ihres Unternehmens entfernt wird oder nicht mehr dem angegebenen sicheren Hostnamen des Adobe zugeordnet ist, kann Adobe das Zertifikat nicht verlängern. Der Eintrag im Adobe-System ist ohne weitere Mitteilung zum Entfernen markiert.

## Häufig gestellte Fragen

+++ Ist dieser Prozess sicher?

Ja. Das von Adobe verwaltete Zertifikatprogramm ist sicherer als das Unternehmen, das Adobe mit einem Zertifikat bereitstellt. Kein Zertifikat oder privater Schlüssel wechselt außerhalb von Adobe und der ausstellenden Zertifizierungsstelle.

+++

+++ Wie kann Adobe ein Zertifikat für unsere Domain erwerben?

Das Zertifikat kann nur erworben werden, wenn Sie mit dem angegebenen Hostnamen auf einen Hostnamen in Adobe verwiesen haben. Sie delegieren diesen Hostnamen im Wesentlichen an Adobe und gestatten Adobe, das Zertifikat in Ihrem Namen zu erwerben.

+++

++ + Kann ich die Sperrung des Zertifikats anfordern?

Ja. Als Inhaber der Domäne sind Sie berechtigt, die Sperrung des Zertifikats anzufordern. Wenden Sie sich an die Adobe-Kundenunterstützung , um diesen Vorgang zu starten.

+++

+++Welcher Verschlüsselungstyp wird verwendet?

Adobe arbeitet mit DigiCert zusammen, um ein SHA-2-Zertifikat auszustellen.

+++

++ Trifft dieses Programm zusätzliche Kosten auf?

Nein. Adobe bietet diesen Dienst allen Adobe Experience Cloud-Kunden kostenlos an.

+++

+++ Welche Sicherheitsstufen bietet Adobe?

Adobe bietet zwei Chiffre-Sicherheitsstufen, die den unterschiedlichen Kundenanforderungen an die Sicherheit bei der Erstanbieter-Datenerfassung gerecht werden. Diese Ebenen bestimmen, welche Verschlüsselungsalgorithmen für HTTPS-Verbindungen mit Adobe-Servern unterstützt werden. Adobe überprüft und aktualisiert regelmäßig den Satz der unterstützten Algorithmen anhand aktueller Sicherheitspraktiken. Wenden Sie sich an die Kundenunterstützung, wenn Sie die Sicherheitseinstellungen für die Chiffre ändern möchten.

* **Standard** erfordert TLS 1.2 oder höher und mindestens 128-Bit-Verschlüsselung. Es wurde entwickelt, um die größtmögliche Gerätekompatibilität zu gewährleisten und gleichzeitig eine sichere Verschlüsselung zu gewährleisten.
* **Hoch** Für die Verschlüsselungssicherheit ist TLS 1.2 oder höher erforderlich und entfernt die Unterstützung für schwächere Chiffren. Es wurde für Kunden entwickelt, die die strengste Verschlüsselung wünschen und sich nicht um die Unterstützung älterer Geräte sorgen.

Die folgenden Clients sind bekanntermaßen nicht in der Lage, eine Verbindung mit der Verschlüsselungssicherheit herzustellen, die auf **Hoch** festgelegt ist:

* Windows 8.1 und früher (zuletzt aktualisiert 2018)
* Windows Phone 8.1 und früher (zuletzt aktualisiert 2016)
* OS X 10.10 und früher (letzte Aktualisierung 2017)
* iOS 8.4 und früher (zuletzt aktualisiert 2015)

+++

++ Welche HTTPS-Zertifikatstypen werden unterstützt?

Adobe unterstützt sowohl RSA- als auch ECC-Zertifikatstypen, um unterschiedlichen Kundenanforderungen gerecht zu werden. RSA-Zertifikate werden für Clients häufiger unterstützt, ECC-Zertifikate verwenden jedoch weniger Verarbeitung auf Server- und Client-Seite. Für Adobe-verwaltete Zertifikate werden sowohl RSA als auch ECC bereitgestellt. Für kundenverwaltete Zertifikate ist RSA erforderlich und ECC wird empfohlen. Moderne Kunden unterstützen sowohl RSA als auch ECC. Die folgenden Clients unterstützen normalerweise nur RSA-Zertifikate:

* Windows Vista und früher (zuletzt aktualisiert 2012)
* Windows Phone 8.0 und früher (zuletzt aktualisiert 2014)
* OS X 10.8 und früher (letzte Aktualisierung 2013)
* iOS 5.1 und früher (zuletzt aktualisiert 2012)
* Android 4.3 und früher (zuletzt aktualisiert 2013)

+++
