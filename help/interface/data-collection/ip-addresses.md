---
title: Von Experience Cloud verwendete IP-Adressen
description: Wenn die Firewall Ihres Unternehmens IP-Adressen blockiert, die von Adobe stammen, verwenden Sie diese Liste, um Ihre Firewall-Einstellungen zu aktualisieren.
exl-id: 1fca8d3b-ae8b-4095-96ef-d165f912b4c6
source-git-commit: 92f041f11cfa33c2e08e90c45e6fa46729447ac5
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 12%

---

# Von Experience Cloud verwendete IP-Adressen

Einige Firewall-Konfigurationen blockieren IP-Adressen, die von den Datenerfassungs-Servern oder -Servern von Adobe stammen, die für den Datenzugriff zuständig sind. Sie können diese Liste von Bereichen verwenden, um die Firewall-Einstellungen Ihrer Organisation zu ändern, um den Zugriff zu ermöglichen und Daten von innerhalb Ihrer Organisation zu senden. Diese Seite enthält sowohl eingehende Systeme (z. B. Datenerfassung) als auch ausgehende Systeme (z. B. Daten-Feeds in Adobe Analytics), die Adobe verwendet.

>[!IMPORTANT]
>
>Adobe setzt dieses Dokument nach besten Kräften auf dem neuesten Stand, kann jedoch nicht garantieren, dass die Liste der IP-Bereiche gleich bleibt. Mögliche Änderungen umfassen das Wachstum und die Erweiterung des Unternehmens, eine Internet-Registrierung erfordert Änderungen am IP-Adressbereich von Adobe oder ein Internet-Service-Provider funktioniert nicht mehr.

Zusätzlich zu den unten aufgeführten IP-Adressblöcken verfügen einzelne Adobe Experience Cloud-Produkte über eigene IP-Adressen, die sie verwenden:

* [Adobe Analytics](https://experienceleague.adobe.com/en/docs/analytics/technotes/ip-addresses)
* [Customer Journey Analytics](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/ip-addresses)
* [Marketo Engage](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started/initial-setup/configure-protocols-for-marketo#step-allowlist-marketo-ips)

## Alle Adobe IP-Adressblöcke

Die folgende Tabelle enthält alle IP-Adressen im Besitz von Adobe. Diese Tabelle enthält alle Adobe-Mitarbeiterbüros und Rechenzentren, die von Adobe global betrieben werden. Sie umfasst keine auf Public Clouds gehosteten Services.

| IP-Block (CIDR-Notation) |
| --- |
| `63.140.32.0/19` |
| `66.117.16.0/20` |
| `66.235.128.0/19` |
| `130.248.0.0/16` |
| `172.82.192.0/18` |
| `185.34.188.0/22` |
| `192.243.240.0/22` |

{style="table-layout:auto"}

## Adobe Experience Cloud-Datenerfassung und FTP-IP-Adressblöcke

Wenn Ihr Unternehmen bestimmte IP-Adressbereiche lieber zulässt, können Sie die folgende Tabelle heranziehen. Zu diesem Service gehören:

* Datenerfassungsserver für alle Experience Cloud-Produkte
* FTP-Server für alle Experience Cloud-Produkte

Alle IP-Bereiche in diesem Abschnitt sind in der obigen Tabelle enthalten.

| Standort | IP-Bereich (CIDR-Notation) |
| --- | --- |
| Australien | `63.140.55.0/24` |
| Australien | `63.140.56.0/23` |
| Kalifornien | `63.140.32.0/23` |
| Kalifornien | `63.140.34.0/24` |
| Frankreich | `63.140.62.0/23` |
| Indien | `66.117.22.0/23` |
| Japan | `130.248.169.0/23` |
| Japan | `63.140.50.0/23` |
| Japan | `66.117.31.0/24` |
| London | `66.235.156.0/24` |
| London | `185.34.188.0/22` |
| London | `130.248.152.0/22` |
| London | `130.248.244.0/23` |
| Ohio | `66.117.20.0/24` |
| Oregon | `66.235.132.0/22` |
| Oregon | `130.248.130.0/23` |
| Oregon | `130.248.150.0/24` |
| Oregon | `130.248.160.0/21` |
| Oregon | `192.243.242.0/24` |
| Singapur | `130.248.170.0/23` |
| Singapur | `130.248.240.0/24` |
| Singapur | `63.140.44.0/22` |
| Singapur | `63.140.48.0/23` |
| Singapur | `66.117.30.0/24` |
| Singapur | `172.82.240.8/29` |
| Singapur | `172.82.240.88/29` |
| Virginia | `63.140.38.0/23` |
| Virginia | `63.140.54.0/24` |
| Virginia | `67.202.5.244` |

{style="table-layout:auto"}

Der Adobe Experience Cloud unterstützt auch IPv6 in begrenzter Kapazität. Diese IP-Blöcke dienen ähnlichen Datenerfassungszwecken wie ihre IPv4-Gegenstücke oben, enthalten jedoch kein FTP.

| Standort | Host |
| --- | --- |
| Australien | `2406:da1c:406:1a00::/56` |
| Australien | `2406:da1c:ce5:b400::/56` |
| Kalifornien | `2600:1f1c:366:d900::/56` |
| Frankreich | `2a05:d012:706:d000::/56` |
| Indien | `2406:da1a:f34:6a00::/56` |
| Irland | `2a05:d018:309:600::/56` |
| Japan | `2406:da14:b07:ab00::/56` |
| Ohio | `2600:1f16:130f:7d00::/56` |
| Oregon | `2600:1f14:1eb:7d00::/56` |
| Oregon | `2600:1f14:9d3:2b00::/56` |
| Singapur | `2406:da18:6e8:1e00::/56` |
| Virginia | `2600:1f18:1a20:e800::/56` |
| Virginia | `2600:1f18:4fd:6000::/56` |
| Virginia | `2600:1f18:b00:e100::/56` |
| Virginia | `2600:1f18:d1f:bd00::/56` |

>[!TIP]
>
>FTP-Verbindungen für Adobe Analytics-Exportfunktionen (einschließlich Data Warehouse- und Daten-Feeds) stammen nur von IPv4-Adressen in London, Oregon und Singapur.
