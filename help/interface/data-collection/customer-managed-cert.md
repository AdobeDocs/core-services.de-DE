---
title: Vom Kunden verwaltete Zertifikate
description: Erfahren Sie, wann ein vom Kunden verwaltetes Zertifikat für die Erstanbieter-Datenerfassung verwendet werden sollte und welche Zuständigkeiten Ihr Unternehmen für die Erneuerung hat.
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
source-git-commit: 18fd590d6f0fd1800e3d5c62851453aa91d9db5f
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 1%
---
# Kundenverwaltete Zertifikate

Mit einem kundenverwalteten Zertifikat erhält Ihr Unternehmen das Zertifikat für den Hostnamen Ihrer Erstanbieter-Datenerfassung und stellt es Adobe zur Verfügung. Adobe hostet das Zertifikat auf seinen Datenerfassungsservern. Ihr Unternehmen ist für die Erneuerung des Zertifikats und die Bereitstellung jedes erneuerten Zertifikats an Adobe verantwortlich, bevor das aktuelle Zertifikat abläuft.

>[!TIP]
>
>Adobe empfiehlt für die meisten First-Party-Implementierungen ](adobe-managed-cert.md) von Adobe verwaltetes Zertifikatsprogramm . [Es ist sicherer und erneuert Zertifikate automatisch. Verwenden Sie ein vom Kunden verwaltetes Zertifikat nur, wenn Ihr Unternehmen es benötigt.

## Verwendung eines vom Kunden verwalteten Zertifikats

* **Sie leiten die Datenerfassung über ein CDN mit Erstanbieterherkunft**: Das von [Adobe verwaltete ](adobe-managed-cert.md) unterstützt keine CDN-Implementierungen. Siehe [Konfigurieren eines CDN mit Erstanbieterherkunft](cdn.md#first-party-origin).
* **Ihre Sicherheitsrichtlinie erfordert die direkte Kontrolle über das Zertifikat**: Beispielsweise muss Ihr Unternehmen in der Lage sein, das Zertifikat über seine eigene Zertifizierungsstelle zu widerrufen, anstatt einen Widerruf über die Adobe-Kundenunterstützung anzufordern.
* **Ihr Unternehmen benötigt eine bestimmte Zertifizierungsstelle oder einen bestimmten Zertifikatstyp**: Das Adobe-verwaltete Zertifikatsprogramm verwendet von DigiCert ausgestellte Zertifikate.

## Zertifikatmethoden vergleichen

| | Adobe-verwaltetes Zertifikat | Kundenverwaltetes Zertifikat |
| --- | --- | --- |
| **Wer erhält das Zertifikat** | Adobe über DigiCert | Ihre Organisation über eine kommerzielle Zertifizierungsstelle Ihrer Wahl |
| **Erneuerungen** | Adobe erneuert das Zertifikat automatisch | Ihr Unternehmen erneuert das Zertifikat und stellt es Adobe vor jedem Ablauf zur Verfügung |
| **Zertifikatstypen** | Adobe stellt sowohl RSA- als auch ECC-Zertifikate bereit | RSA ist erforderlich; ECC wird empfohlen |
| **Unterstützt mit einem CDN** | Nein | Ja, als First-Party-Herkunft |

## Einrichten eines vom Kunden verwalteten Zertifikats

1. Wenden Sie sich an die Adobe-Kundenunterstützung, um eine Erstanbieter-Datenerfassung mit einem kundenverwalteten Zertifikat anzufordern. Geben Sie Ihren Erstanbieter-Hostnamen an, z. B. `data.example.com`. Wenn Ihr Unternehmen Datenresidenz- oder Compliance-Anforderungen hat, geben Sie den gewünschten [RDC-Typ](rdc.md) in Ihrer Anfrage an.
1. Die Adobe-Kundenunterstützung stellt eine Certificate Signing Request (CSR) für Ihren Hostnamen bereit. Adobe generiert den privaten Schlüssel und speichert ihn, sodass Ihr Unternehmen den privaten Schlüssel nie verarbeitet. Adobe erfordert ein RSA-Zertifikat und empfiehlt ein ECC-Zertifikat. Für jeden Zertifikatstyp ist eine eigene CSR erforderlich. Wenn Sie also ein ECC-Zertifikat benötigen, wenden Sie sich an die Adobe-Kundenunterstützung, um eine ECC-CSR zu erhalten.
1. Senden Sie jede CSR an die gewünschte kommerzielle Zertifizierungsstelle, um ein signiertes Zertifikat zu erhalten. Kostenlose Zertifikatdienste werden nicht unterstützt. Stellen Sie Adobe die ausgestellten Zertifikate gemäß den Anweisungen der Kundenunterstützung zur Verfügung.
1. Sobald Adobe Ihr Zertifikat installiert hat, leiten Sie den Traffic für Ihren Hostnamen an Adobe weiter:
   * **Ohne CDN**: Aktualisieren Sie die DNS-Einträge Ihres Unternehmens, wie von der Adobe-Kundenunterstützung angewiesen.
   * **Mit einem CDN**: Legen Sie Ihren CDN-Ursprung auf Ihren Erstanbieter-Host-Namen fest. Siehe [Konfigurieren eines CDN mit Erstanbieterherkunft](cdn.md#first-party-origin).
1. Wenn Ihre Implementierung noch keine Daten an diesen Hostnamen sendet, aktualisieren [ Ihre Implementierung](collection-domain.md#update-implementation).

## Zertifikat verlängern {#renewals}

Ihr Unternehmen ist für die Erneuerung Ihres Zertifikats und die Bereitstellung des erneuerten Zertifikats an die Adobe-Kundenunterstützung verantwortlich, bevor das aktuelle Zertifikat abläuft.

Wenn das Zertifikat auf Adobe-Servern abläuft, lehnen Browser und CDNs Verbindungen zu Ihrem Hostnamen ab, sodass Daten aus diesen Anfragen verloren gehen. Ein CDN kann diese Daten verwerfen, ohne Sie zu benachrichtigen.

Die maximale Zertifikatlebensdauer nimmt ab, sodass Erneuerungen häufiger erfolgen. Weitere Informationen finden Sie unter [6.3.2 Certificate Operational Periods and Key Pair Usage Periods](https://cabforum.org/working-groups/server/baseline-requirements/requirements/#632-certificate-operational-periods-and-key-pair-usage-periods) in den CA/Browser Forum Server Certificate Baseline Requirements. So vermeiden Sie Lücken bei der Datenerfassung:

* Verfolgen Sie das Ablaufdatum jedes Zertifikats, das Sie Adobe bereitstellen.
* Weisen Sie einen Verantwortlichen für die Erneuerung zu und dokumentieren Sie den Erneuerungsprozess, damit er durch Mitarbeiteränderungen fortgesetzt wird.

Adobe prüft derzeit einen Prozess zur Erneuerung von Selbstbedienungszertifikaten.

## Beenden der Verwendung eines vom Kunden verwalteten Zertifikats

* **Um zum Adobe-verwalteten Zertifikatprogramm zu wechseln**: Wenden Sie sich an die Kundenunterstützung von Adobe. Für das Adobe-verwaltete Zertifikatsprogramm muss Ihr Hostname direkt auf Adobe verweisen und nicht auf ein CDN.
* **So verwenden Sie Ihren Erstanbieter-Hostnamen nicht mehr**: Aktualisieren Sie alle Implementierungen, die den Hostnamen verwenden, und wenden Sie sich dann an die Adobe-Kundenunterstützung, um das Zertifikat von den Adobe-Servern zu entfernen.
* **So wechseln Sie zu einem CDN mit Herkunft** Drittanbieters: Siehe [Verschieben einer vorhandenen Erstanbieterimplementierung in ein CDN](cdn.md#migrate).
