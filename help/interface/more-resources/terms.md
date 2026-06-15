---
description: Erfahren Sie, wie sich Produkt- und Schnittstellenbegriffe für Adobe in CX Enterprise, Experience Cloud-Lösungen, Creative Cloud, Experience League und anderen Support-Bereichen unterscheiden.
solution: Experience Cloud
title: Terminologie
feature-set: Experience Cloud Services
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: 3799f806-2794-43ab-9e70-06ee693871e7
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: bdea9bc8-5600-45db-b85e-d74bb59dfcff
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 50012e2564e88e1a6e16578e3331136c7df0cb21
workflow-type: tm+mt
source-wordcount: 692
ht-degree: 5%

---

# Terminologie

<!--
TQID: https://experienceleague.adobe.com/6wm7HcuAbaV1iV3AgN55dY5WR---BnMM7lJgN0HZDsk
-->

Verwenden Sie diese Tabelle, wenn dasselbe Wort in verschiedenen Adobe-Erlebnissen angezeigt wird (CX Enterprise, Marketing-Apps, Design-Apps oder Support-Sites). Es handelt sich nicht um ein vollständiges Glossar. Detaillierte Definitionen finden Sie in der produktspezifischen Hilfe [&#128279;](https://experienceleague.adobe.com/de) Experience League.

| Begriff | In CX Enterprise und dieses Handbuch | Andere gängige Verwendungszwecke von Adobe |
| --- | --- | --- |
| **Adobe CX Enterprise** | Das einheitliche Web-Erlebnis unter `experience.adobe.com`, in dem Sie Marketing-Programme öffnen, Voreinstellungen und Benachrichtigungen festlegen und freigegebene Benutzeroberflächen-Services (z. B. Kundenattribute und [Zielgruppenbibliothek](../services/audiences/overview.md)) erreichen. Zuvor *Adobe Experience Cloud*. | Nicht dasselbe Produkt wie **Adobe Experience Platform** (Kundendateninfrastruktur, Sandboxes, Datensätze). Nicht **Adobe Creative Cloud** (Design- und Medien-Apps). |
| **Adobe Experience Platform** | Wird angezeigt, wenn Sie Datenerfassungs-, Identitäts- oder Platform-Agenten mit Ihren Lösungen verbinden. Einige Navigationssuch- und KI-Funktionen sind Platform-gestützt. | Eine Daten- und Orchestrierungsplattform. Verwenden Sie &quot;Experience Platform&quot; nicht, wenn Sie die CX Enterprise-Shell oder Homepage meinen. |
| **Experience League** | Hier erhalten Sie Hilfe- und produktinterne Links zu **Dokumentation**, **Tutorials** Lernwiedergabelisten, Versionshinweisen und Community-Kontext für Adobe-Lösungen. Beginnen Sie bei [Experience League-Startseite](https://experienceleague.adobe.com/de). | Ergänzt das **[Adobe Help Center](https://helpx.adobe.com/de/support.html)**, das die Schwerpunkte **Account**, **Plan**, **Billing**, Downloads und produktübergreifende Fehlerbehebung für Einzelpersonen und Teams setzt. Verwenden Sie das Hilfe-Center für das Zurücksetzen von Passwörtern, Planänderungen und ähnliche Aufgaben; verwenden Sie Experience League für Anleitungsinhalte zu Produkten. |
| **KI-Assistent/Agent-KI** | Produktinterne Assistenten und koordinierte Agenten, die in den KI-Themen dieses Handbuchs beschrieben werden. Zugriff und Credits hängen von Produktberechtigungen ab. | Andere Adobe-Oberflächen (z. B. **Firefly** oder **Express**) verwenden „KI“-Funktionen mit unterschiedlichen Umfängen und Richtlinien. |
| **Organisation** | Ihre **IMS-Organisation**: die Grenze für Unternehmenslizenzierung, Benutzerverzeichnisse, SSO und Admin Console-Administration in CX Enterprise. Siehe [Organisationen und Kontoverknüpfung](../administration/organizations.md). | Keine Analytics *Report Suite*, keine Target *Eigenschaft* oder Experience Platform *Sandbox* (dies sind produktspezifische Container). |
| **Admin Console** | Enterprise Control Plane at `adminconsole.adobe.com` für Benutzer, Produktprofile und Identität; verknüpft mit CX Enterprise **Administration** Themen. Siehe [Benutzer- und Produktverwaltung](../administration/admin-console.md). | Anders als **Produktinterne Admin** innerhalb der einzelnen Apps (z. B. Analytics-Admin-Tools oder Journey Optimizer-Berechtigungsbildschirme). |
| **Produktprofil** | Ein Lizenzpaket in Admin Console, das Zugriff auf ein Produkt oder eine Funktion gewährt. Benutzer müssen einem Profil angehören, um eine Berechtigung zu erhalten. Siehe [Verwalten von Produkten und Profilen](https://helpx.adobe.com/de/enterprise/using/manage-products.html). | Nicht mit jedem produktinternen „Arbeitsbereich“, „Container“ oder „Eigenschaftsnamen“ austauschbar; diese variieren je nach Lösung. |
| **Kontoverknüpfung** | Verbinden eines Anwendungs-Logins (z. B. Analytics- oder Target-Anmeldedaten) mit Ihrer Adobe ID für das Unternehmen, damit Services einen Benutzer erkennen. Siehe [Organisationen und Kontoverknüpfung](../administration/organizations.md). | Nicht dasselbe wie **Ordnersynchronisierung**, **SSO** oder **Federation**-Setup (dies sind organisationsweite Identitätsentscheidungen in Admin Console). |
| **Experience Cloud ID Service/ECID** | Die in allen Lösungen verwendete persistente Besucherkennung, die häufig mit Tags oder Web-SDK bereitgestellt wird. Wird in älteren Analytics **Diskussionen immer noch häufig als** Experience Cloud-ID **oder** MID“ bezeichnet. Siehe [ID-Service - Übersicht](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=de). | Anders als der Name des veralteten Cookies einer einzelnen App oder von **Experience Platform** Identitätsdiagramm-Konzepten, obwohl sie in einer Implementierung verknüpft sein können. |
| **Kundenattribute** | CRM- oder Unternehmensattribute, die Sie hochladen und für die Verwendung in Analytics-, Target- und zugehörigen Workflows über den Personen-Service zuordnen. Siehe die [Kundenattribute](../services/customer-attributes/attributes.md) Themen. | Nicht mit **Audience Manager-Eigenschaften** allein oder mit jedem **Real-Time CDP**-Profilfeld gleichsetzen, ohne die Produktgrenze zu überprüfen. |
| **Zielgruppenbibliothek** | CX Enterprise-Benutzeroberfläche zum Erstellen und Freigeben von Audiences über integrierte Anwendungen hinweg. | **Audience Manager** und **Target** verwenden ebenfalls „Zielgruppen“, die Segmentierungsregeln und Ziele unterscheiden sich jedoch je nach Produkt. |
| **Segment** (Analytics) | Eine regelbasierte Zielgruppendefinition, die Sie in Adobe Analytics erstellen und bei Unterstützung für freigegebene Zielgruppen veröffentlichen können. | In **Audience Manager** kombinieren Segmente **Eigenschaften** Namensüberschneidungen, aber die Implementierung ist nicht identisch. In **Target** hat „Zielgruppen“ an vielen Stellen ältere „Segment“-Beschriftungen ersetzt. |
| **Assets (Experience Cloud Assets)** | Freigegebene Ordner und Dateien für die Zusammenarbeit zwischen CX Enterprise-Marketing-Workflows und genehmigten **Creative Cloud**-Benutzern. Siehe [Übersicht über Assets](../services/assets/experience-cloud-assets.md). | In **Creative Cloud** bedeutet „Assets“ normalerweise Designdateien (PSD, AI, INDD). Gleiches Wort, anderes Modell der Freigabe und Governance. |

{style="table-layout:auto"}

