---
description: Erfahren Sie mehr über zentrale Oberflächenkomponenten für Experience Cloud. Erhalten Sie Hilfe zur Benutzer- und Produktverwaltung in der Admin Console und aktivieren Sie Anwendungen für Experience Cloud-Services. Erhalten Sie Hilfe zur Zielgruppenbibliothek, zu Kundenattributen, zu Experience Cloud-Assets und mehr.
title: Dokumentation zur Experience Cloud-Benutzeroberfläche
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: 5df8104d3d148cc7bda823b27bf96429ddb6018d
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 80%

---

# Übersicht über die zentrale Schnittstelle von Experience Cloud

[Experience Cloud](https://experience.adobe.com) umfasst die Digital-Marketing-Programme, -Produkte und -Services von Adobe. Über die intuitive Benutzeroberfläche können Sie schnell auf Ihre Cloud-Programme, Produktfunktionen und Services zugreifen.

![Experience Cloud](assets/landing.png)

In der Kopfzeile von Experience Cloud haben Sie folgende Möglichkeiten:

* Zugriff auf alle Experience Cloud-Anwendungen und -Dienste
* Suchen Sie über das Menü „Hilfe“ nach Produktdokumentationen, Tutorials und Community-Beiträgen. Lassen Sie sich Ergebnisse in Experience League anzeigen.
* Suchen Sie global nach Geschäftsobjekten, indem Sie eine globale Suche (nur für Nutzerinnen und Nutzer der Experience Platform) im Feld „Suche“ verwenden.
* Verwalten Sie Ihr Konto [Voreinstellungen](features/account-preferences.md) (Warnhinweise, Benachrichtigungen und Abonnements)

## Melden Sie sich bei Experience Cloud an {#signin}

Melden Sie sich an und stellen Sie sicher, dass Sie sich in der richtigen [Organisation](administration/organizations.md) befinden.

1. Navigieren Sie zur [Adobe Experience Cloud](https://experience.adobe.com).
1. Geben Sie Ihre Adobe-E-Mail-Adresse ein und wählen Sie **[!UICONTROL Weiter]**.
1. Wählen Sie ein Konto aus.
1. Geben Sie Ihr Passwort ein.
1. Stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden.

   ![Stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden](assets/organizations-menu.png)

   **Organisation überprüfen**

   Die [Organisation](administration/organizations.md) wird in der Kopfzeile der Benutzeroberfläche angezeigt.

   Wenn Ihr Unternehmen Federated IDs verwendet, können Sie sich durch ein Single Sign-on Ihres Unternehmens bei Experience Cloud anmelden, ohne Ihre E-Mail-Adresse und Ihr Passwort eingeben zu müssen. Fügen Sie `#/sso:@domain` zur Experience Cloud-URL (`https://experience.adobe.com`) hinzu, um diese Aufgabe zu erfüllen.

   Setzen Sie beispielsweise für eine Organisation mit Federated IDs und der Domain `adobecustomer.com` Ihren URL-Link auf `https://experience.adobe.com/#/sso:@adobecustomer.com`. Sie können auch direkt zu einem bestimmten Programm gehen, indem Sie diese URL, an die der Programmpfad angehängt ist, als Lesezeichen speichern. (Beispiel für Adobe Analytics: `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Zugriff auf Experience Cloud-Anwendungen {#navigation}

Nach der Anmeldung bei Experience Cloud können Sie über den einheitlichen Header schnell auf alle Ihre Anwendungen, Dienste und Organisationen zugreifen.

Rufen Sie die das ![Menü](assets/menu-icon.png) der Programmauswahl auf, um auf die in Ihrem Unternehmen für Sie bereitgestellten Experience Cloud-Programme und -Services zuzugreifen.

![Zugriff auf Experience Cloud-Programme](assets/platform-core-services.png)

## Erhalten Sie Hilfe und Support {#support}

Greifen Sie auf Lernmaterialien und Hilfe über das **[!UICONTROL Hilfezentrum]** (![Asset](assets/help-icon.png)) in der Kopfzeile zu, einschließlich Hilfeinhalten (Dokumentation, Tutorials und Kurse) auf [Experience League](https://experienceleague.adobe.com/?lang=de#home) sowie zusätzlichen Ressourcen für einzelne Anwendungen. Sie können auch ein unverbindliches Feedback senden und priorisierte Support-Tickets erstellen.

![Erhalten Sie Hilfe und Support](assets/search-menu.png)

Das Menü [!UICONTROL Hilfe] bietet Ihnen außerdem Zugriff auf:

* **[!UICONTROL Support]:** Erstellen Sie ein Support-Ticket oder kontaktieren Sie den [!UICONTROL Support] über Twitter.
* **[!UICONTROL Feedback]:** Teilen Sie Feedback zu Ihrem Experience Cloud-Erlebnis. Ihr Feedback wird verwendet, um die Produkte und Services von Adobe zu verbessern.
* **[!UICONTROL Status]:** Navigieren Sie zu `https://status.adobe.com/experience_cloud` und prüfen Sie den Betriebsstatus des Produkts und [!UICONTROL verwalten Sie Abonnements].
* **[!UICONTROL Developer Connection]:** Navigation zu `adobe.io` und Entwicklerdokumentation.

## Benutzerprofil verwalten

Im Menü [!UICONTROL Profil] haben Sie folgende Möglichkeiten:

* Festlegen eines dunklen Designs (nicht alle Anwendungen unterstützen dieses Design)
* Experience Cloud [-Einstellungen](features/account-preferences.md) verwalten
* Auswählen oder Suchen nach einer [Organisation](administration/organizations.md)
* Anzeigen von [!UICONTROL rechtlichen Hinweisen]
* Abmelden
* Einstellungen, Benachrichtigungen und Abonnements für das Konto konfigurieren

## Anzeigen von Benachrichtigungen und Mitteilungen innerhalb des Produkts {#notifications}

Klicken Sie auf das Glockensymbol, um Benachrichtigungen und Mitteilungen anzuzeigen. Mitteilungen können relevante und umsetzbare Aktualisierungen sein, einschließlich Produktversionen, Wartungshinweisen, freigegebenen Elementen und Genehmigungsanfragen.

![Benachrichtigungen und Ankündigungen](assets/notifications-menu-small.png)

Informationen zum Verwalten von Benachrichtigungen und Warnhinweisen finden Sie unter [Kontovoreinstellungen und Benachrichtigungen](features/account-preferences.md)


## Neuerungen

Erfahren Sie mehr über die neuesten Verbesserungen an den Komponenten der zentralen Experience Cloud-Benutzeroberfläche.

>[!BEGINTABS]

>[!TAB Slack-Integration mit Experience Cloud]

Sie können Ihre Kontovoreinstellungen so konfigurieren, dass Experience Cloud-Benachrichtigungen an einen [!DNL Slack] -Kanal gesendet werden.

[!BADGE Beta]{type=Informative url="https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences#notifications" tooltip="Informationen zum Slack"}


>[!TAB Neue Campaign Web-Benutzeroberfläche]

Erleben Sie die neue Adobe Campaign-Benutzeroberfläche. Moderner, intuitiver und dynamischer.

[![Bild](assets/do-not-localize/learn-more-button.svg)](start/campaign-ui.md#ac-web-ui)


>[!TAB Künftige Änderungen am Push-Kanal]

Einige wichtige Änderungen am FCM-Dienst (Android Firebase Cloud Messaging) werden 2024 veröffentlicht und können sich auf Ihre Implementierung von Adobe Campaign auswirken. Ihre Konfiguration der Anmeldedienste für Android-Push-Nachrichten muss möglicherweise aktualisiert werden, um diese Änderung zu unterstützen. Sie können dies bereits überprüfen und Maßnahmen ergreifen.

[![Bild](assets/do-not-localize/learn-more-button.svg)](../technotes/upgrades/push-technote.md)



>[!ENDTABS]

## Beginnen Sie mit den Grundlagen

<table style="table-layout:fixed">
  <tr style="border: 0;">
    <td>
    <a href="start/whats-new.md"><img src="assets/do-not-localize/start-capabilities.png"></a>
    <div><strong>Schlüsselfunktionen</strong><br/>Erfahren Sie mehr über die wichtigsten Funktionen von Adobe Campaign v8 für die kanalübergreifende Kampagnenverwaltung.</div>
    </td>
    <td>
    <a href="start/connect.md"><img src="assets/do-not-localize/start-connect.jpeg"></a>
    <div><strong>Herstellen einer Verbindung zu Campaign v8</strong><br/>Erfahren Sie, wie Sie eine Verbindung zu Adobe Campaign v8 herstellen und Ihre Kampagnenverwaltung durch die Installation und Konfiguration der Client-Konsole in Gang bringen.</div><br/>
    </td>
    <td>
    <a href="start/create-message.md"><img src="assets/do-not-localize/start-send.jpeg"></a>
    <div><strong>Nachrichten senden</strong><br/>Erfahren Sie, wie Sie Nachrichten über verschiedene Kanäle senden können, z. B. E-Mail, SMS oder Push-Benachrichtigungen.
    </div></td>
    <td>
    <a href="audiences/create-profiles.md"><img src="assets/do-not-localize/start-profiles.png"></a>
    <div><strong>Profile importieren</strong><br/>Das Erstellen von Profilen in der Datenbank von Adobe Campaign v8 ist unkompliziert. Fügen Sie Profile manuell oder durch Importe hinzu, verfeinern Sie Kundendaten und passen Sie Kampagnen mühelos an.</div>
    </td>
  </tr>
  <tr style="border: 0;">
    <td align="center"><a href="start/whats-new.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="start/connect.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="start/create-message.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    <td align="center"><a href="audiences/create-profiles.md"><img src="assets/do-not-localize/learn-more-button.svg"></a></td>
    </tr>
</table>

## Dokumentation

<table style="table-layout:auto">
  <tr style="border: 0;">
    <td>
      <img src="assets/do-not-localize/icon-start.svg" width="35px">
    <br/>
      <strong>Erste Schritte</strong><br/><a href="start/campaign-ui.md">Benutzeroberfläche</a> - <a href="start/ac-components.md">Komponenten und Prozesse</a> - <a href="start/v7-to-v8.md">Von Classic v7 zu v8</a> - <a href="start/campaign-faq.md">FAQs</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-experience.svg" width="35px">
    <br/>
      <strong>Kundenerlebnis</strong><br/><a href="../automation/workflow/about-workflows.md" target="_blank">Automatisieren mit Workflows</a> - <a href="../automation/campaigns/set-up-campaigns.md" target="_blank">Kampagnenorchestrierung</a> - <a href="interaction/interaction.md">Entscheidungs-Management</a> - <a href="send/personalize.md">Personalisierung</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-send.svg" width="35px">
    <br/>
      <strong>Nachrichten senden</strong><br/><a href="start/create-message.md">Erste Schritte</a> - <a href="send/preview-and-proof.md">Vorschau und Testsendungen</a> - <a href="send/predictive.md">Sendezeitoptimierung</a> - <a href="reporting/gs-reporting.md">Berichte und Analysen</a>
    </td>
  </tr>
  <tr style="border: 0;">
    <td>
      <img src="assets/do-not-localize/icon_profile-audience.svg" width="35px">
    <br/>
      <strong>Profile und Zielgruppen</strong><br/><a href="audiences/create-profiles.md">Profile hinzufügen</a> - <a href="audiences/create-audiences.md">Zielgruppen erstellen</a> - <a href="start/subscriptions.md">Abonnements verwalten</a> - <a href="start/privacy.md">Datenschutz</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-configure.svg" width="35px">
    <br/>
      <strong>Architektur und Konfiguration</strong><br/><a href="architecture/architecture.md">Architektur</a> - <a href="start/implement.md">Implementierung von Campaign v8</a> - <a href="connect/integration.md">Verbinden mit anderen Lösungen</a> - <a href="start/gs-permissions.md">Benutzende und Berechtigungen</a>
    </td>
    <td>
      <img src="assets/do-not-localize/icon-dev.svg" width="35px">
    <br/>
      <strong>Entwicklerressourcen</strong><br/><a href="dev/datamodel.md">Datenmodell von Campaign v8</a> - <a href="dev/schemas.md">Schemas</a> - <a href="dev/api.md">APIs</a>
    </td>
  </tr>
</table>

## Zusätzliche Ressourcen

[Adobe Campaign v8-Produktbeschreibung](https://helpx.adobe.com/de/legal/product-descriptions/adobe-campaign-managed-cloud-services.html){target="_blank"} – [Dokumentation der Web-Benutzeroberfläche von Adobe Campaign](https://experienceleague.adobe.com/docs/campaign-web/v8/campaign-web-home.html?lang=de){target="_blank"} – [Tutorials](https://experienceleague.adobe.com/docs/campaign-learn/tutorials/overview.html?lang=de){target="_blank"} - [[!DNL Adobe Campaign] Automatisierungshandbuch](https://experienceleague.adobe.com/docs/campaign/automation/home.html?lang=de){target="_blank"} - [Control Panel für Campaign v8](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/key-features.html?lang=de){target="_blank"}

