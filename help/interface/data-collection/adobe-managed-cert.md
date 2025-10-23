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
source-git-commit: c447723f4d6c57bdccad6c4a8996693aec4a56fe
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 3%

---

# Adobe Managed Certificate Program

Das Adobe-verwaltete Zertifikatsprogramm ist der empfohlene Prozess zum Einrichten von Erstanbieterzertifikaten, die für eine CNAME-Implementierung erforderlich sind. Das Programm ist nach der Konfiguration vollständig automatisiert. Zertifikate werden rechtzeitig erneuert, sodass sich die Datenerfassung aufgrund abgelaufener Zertifikate nicht auswirkt. Das Programm ist kostenlos für Ihre ersten 100 CNAMEs.

Wenn Sie derzeit Ihre eigenen Zertifikate verwalten, sind Sie für den Kauf, die Verwaltung und die Bereitstellung eines Zertifikats für Adobe zur Verwendung von Erstanbieter-Cookies verantwortlich. Sie können sich an die Adobe-Kundenunterstützung wenden, um die Migration zum Adobe-verwalteten Zertifikatprogramm zu besprechen.

## Implementierung

Führen Sie die folgenden Schritte aus, um ein neues Zertifikat für die Erstanbieter-Datenerfassung zu implementieren:

1. Laden Sie das Anforderungsformular für [-Domains herunter und füllen Sie es aus](cookies/assets/First_Party_Domain_Request_Form.xlsx)
1. Öffnen Sie ein Ticket bei der Adobe-Kundenunterstützung, um die Erstanbieter-Datenerfassung für das von Adobe verwaltete Zertifikatsprogramm einzurichten.
1. Nach Erhalt des Tickets stellt Ihnen der Adobe-Support einen CNAME-Datensatz zur Verfügung. Diese Einträge müssen auf dem DNS-Server Ihres Unternehmens konfiguriert werden, bevor Adobe das Zertifikat in Ihrem Namen erwerben kann. Beispielsweise verweist der Hostname-`data.example.com` auf `hiodsibxvip01.data.adobedc.net`.
1. Wenn der CNAME-Eintrag auf den Servern Ihres Unternehmens vorhanden ist, kauft und installiert Adobe gemeinsam mit DigiCert ein Zertifikat auf den Datenerfassungsservern von Adobe.

## Überprüfen der Hostnamenweiterleitung

Nachdem Adobe das Zertifikat installiert hat, können Sie eine der folgenden Methoden verwenden, um zu überprüfen, ob es funktioniert.

+++**Browser-Validierung**

Sie können jeden Browser verwenden, um zu überprüfen, ob ein Zertifikat korrekt installiert ist. Geben Sie Ihren CNAME mit `_check` als Pfad in die Adressleiste ein. Beispiel:

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

## Aktualisierung des Implementierungscodes

Nachdem Sie überprüft haben, ob Ihr Zertifikat ordnungsgemäß funktioniert, können Sie Ihre Adobe-Implementierung aktualisieren, um diese Werte zu verwenden.

* **Web SDK-Tag** Erweiterung: Aktualisieren Sie das Feld [[!UICONTROL Edge domain]](https://experienceleague.adobe.com/de/docs/experience-platform/tags/extensions/client/web-sdk/web-sdk-extension-configuration) beim Konfigurieren der Erweiterung.
* **Web SDK (Legierung)**: Aktualisieren Sie die [`edgeDomain`](https://experienceleague.adobe.com/de/docs/experience-platform/web-sdk/commands/configure/edgedomain) Eigenschaft im [`configure`](https://experienceleague.adobe.com/de/docs/experience-platform/web-sdk/commands/configure/overview).
* **Adobe Analytics-Erweiterung**: Aktualisieren Sie das Feld &quot;[[!UICONTROL SSL Tracking Server]](https://experienceleague.adobe.com/de/docs/experience-platform/tags/extensions/client/analytics/overview)&quot;, wenn Sie die Erweiterung konfigurieren. Stellen Sie sicher, dass Sie auch [&#x200B; Tag-Erweiterung „Visitor ID Service](https://experienceleague.adobe.com/de/docs/experience-platform/tags/extensions/client/id-service/overview) installiert haben. Weitere [&#x200B; finden Sie unter „Besucheridentifizierung mit der Tag](https://experienceleague.adobe.com/de/docs/analytics/implementation/id/analytics-extension)Erweiterung für Analytics“.
* **AppMeasurement**: Aktualisieren Sie die [`trackingServerSecure`](https://experienceleague.adobe.com/de/docs/analytics/implementation/vars/config-vars/trackingserversecure) Konfigurationsvariable. Stellen Sie sicher, dass Sie auch den [Besucher-ID-Service](https://experienceleague.adobe.com/de/docs/id-service/using/home) mit `VisitorAPI.js` implementiert haben. AppMeasurement Weitere Informationen [&#x200B; Sie unter „Besucheridentifizierung mit &#x200B;](https://experienceleague.adobe.com/de/docs/analytics/implementation/id/analytics-extension)&quot;.

Wenn Ihre Site mehrere Implementierungsmethoden verwendet und Sie nicht alle gleichzeitig aktualisieren können, sollten Sie eine Übergangsphase konfigurieren. Unter [Überlegungen zur Migration des Besucher-ID](https://experienceleague.adobe.com/de/docs/analytics/implementation/id/migration)Service finden Sie weitere Schritte, um zu verhindern, dass Besucher auf Ihrer Site als neue Besucher gezählt werden.

## Wartung und Erneuerung

Dreißig Tage vor Ablauf Ihres Erstanbieterzertifikats überprüft Adobe, ob der CNAME noch gültig und in Verwendung ist. Wenn ja, geht Adobe davon aus, dass Sie den Service weiterhin verwenden möchten, und erneuert das Zertifikat automatisch in Ihrem Namen.

>[!IMPORTANT]
>
>Wenn der CNAME-Eintrag Ihres Unternehmens entfernt wurde oder nicht mehr dem bereitgestellten sicheren Adobe-Hostnamen zugeordnet ist, kann Adobe das Zertifikat nicht verlängern. Der Eintrag im System von Adobe wird ohne weitere Mitteilung zur Entfernung markiert.

## Häufig gestellte Fragen

+++Ist dieser Prozess sicher?

Ja. Das von Adobe verwaltete Zertifikatsprogramm ist sicherer als die Bereitstellung eines Zertifikats für Adobe durch Ihr Unternehmen. Außerhalb von Adobe und der ausstellenden Zertifizierungsstelle ändert sich kein Zertifikat oder privater Schlüssel.

+++

+++Wie kann Adobe ein Zertifikat für unsere Domain erwerben?

Das Zertifikat kann nur erworben werden, wenn der angegebene Hostname auf einen Adobe-eigenen Hostnamen verweist. Sie delegieren diesen Hostnamen an Adobe und erlauben Adobe, das Zertifikat in Ihrem Namen zu erwerben.

+++

+++Kann ich beantragen, dass das Zertifikat widerrufen wird?

Ja. Als Eigentümer der Domain sind Sie berechtigt, den Widerruf des Zertifikats zu verlangen. Wenden Sie sich an die Adobe-Kundenunterstützung, um diesen Prozess zu starten.

+++

+++Welcher Verschlüsselungstyp wird verwendet?

Adobe stellt in Zusammenarbeit mit DigiCert ein SHA-2-Zertifikat aus.

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

Adobe unterstützt sowohl RSA- als auch ECC-Zertifikatstypen, um unterschiedlichen Kundenanforderungen gerecht zu werden. RSA-Zertifikate werden für Clients häufiger unterstützt, aber ECC-Zertifikate verbrauchen sowohl auf Server- als auch auf Client-Seite weniger Verarbeitung. Für von Adobe verwaltete Zertifikate werden sowohl RSA als auch ECC bereitgestellt. Für kundenverwaltete Zertifikate ist eine RSA erforderlich, und es wird eine ECC empfohlen. Moderne Clients unterstützen sowohl RSA als auch ECC. Die folgenden Clients unterstützen in der Regel nur RSA-Zertifikate:

* Windows Vista und früher (zuletzt aktualisiert 2012)
* Windows Phone 8.0 und niedriger (zuletzt aktualisiert 2014)
* OS X 10.8 und niedriger (zuletzt aktualisiert 2013)
* iOS 5.1 und niedriger (zuletzt aktualisiert 2012)
* Android 4.3 und niedriger (zuletzt aktualisiert 2013)

+++

+++Kann ich stattdessen meine eigenen Zertifikate verwalten?

Ja. Wenn Sie jedoch Ihre eigenen Zertifikate verwalten, sind Sie für die Erneuerung Ihrer Zertifikate und deren Bereitstellung für Adobe bei jeder Erneuerung verantwortlich. Dieser Prozess ist weniger sicher und kann zu Datenverlust führen, wenn Ihr Unternehmen vergisst, ein Zertifikat rechtzeitig zu erneuern. Adobe empfiehlt, das verwaltete Zertifikatprogramm zu verwenden, anstatt Zertifikate selbst zu verwalten, insbesondere aufgrund der Verkürzung der maximalen Lebensdauer von TLS-Zertifikaten. Weitere Informationen finden Sie unter [6.3.1 Archivierung &#x200B;](https://cabforum.org/working-groups/server/baseline-requirements/requirements/#632-certificate-operational-periods-and-key-pair-usage-periods) öffentlichen Schlüssels) in den Grundanforderungen für Zertifikate des CA/Browser-Forums.
+++
