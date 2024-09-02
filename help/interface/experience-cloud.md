---
description: Erfahren Sie mehr über zentrale Oberflächenkomponenten für Experience Cloud. Erhalten Sie Hilfe zur Benutzer- und Produktverwaltung in der Admin Console und aktivieren Sie Anwendungen für Experience Cloud-Services. Erhalten Sie Hilfe zur Zielgruppenbibliothek, zu Kundenattributen, zu Experience Cloud-Assets und mehr.
title: Dokumentation zur Experience Cloud-Benutzeroberfläche
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: 2a80851c0a7d4ef7dbcc2565177b239f3e063164
workflow-type: ht
source-wordcount: '714'
ht-degree: 100%

---

# Übersicht über die zentrale Schnittstelle von Experience Cloud

[Experience Cloud](https://experience.adobe.com) umfasst die Digital-Marketing-Programme, -Produkte und -Services von Adobe. Über die intuitive Benutzeroberfläche können Sie schnell auf Ihre Cloud-Programme, Produktfunktionen und Services zugreifen.

![Experience Cloud](assets/landing.png)

In der Kopfzeile von Experience Cloud haben Sie folgende Möglichkeiten:

* Greifen Sie auf Ihre Programme und Services zu
* Suchen Sie über das Menü „Hilfe“ nach Produktdokumentationen, Tutorials und Community-Beiträgen. Lassen Sie sich Ergebnisse in Experience League anzeigen.
* Suchen Sie global nach Geschäftsobjekten, indem Sie eine globale Suche (nur für Nutzerinnen und Nutzer der Experience Platform) im Feld „Suche“ verwenden.
* Kontoeinstellungen verwalten können (Warnhinweise, Benachrichtigungen und Abonnements)

## Melden Sie sich bei Experience Cloud an {#signin}

Melden Sie sich an und stellen Sie sicher, dass Sie sich in der richtigen [Organisation](administration/organizations.md) befinden.

1. Navigieren Sie zur [Adobe Experience Cloud](https://experience.adobe.com).
1. Geben Sie Ihre Adobe-E-Mail-Adresse ein und wählen Sie **[!UICONTROL Weiter]**.
1. Wählen Sie ein Konto aus.
1. Geben Sie Ihr Passwort ein.
1. Stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden.

   ![Stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden](assets/organizations-menu.png)

   **Organisation überprüfen**

   Um sicherzustellen, dass Sie sich bei Ihrer richtigen [Organisation](administration/organizations.md) angemeldet haben, klicken Sie auf Ihren Profilavatar, um den Organisationsnamen anzuzeigen. Wenn Sie Zugriff auf mehr als eine Organisation haben, können Sie rechts in der Kopfzeilenleiste auch eine andere Organisation anzeigen und zu dieser wechseln.

   Wenn Ihr Unternehmen Federated IDs verwendet, können Sie sich durch ein Single Sign-on Ihres Unternehmens bei Experience Cloud anmelden, ohne Ihre E-Mail-Adresse und Ihr Passwort eingeben zu müssen. Fügen Sie `#/sso:@domain` zur Experience Cloud-URL (`https://experience.adobe.com`) hinzu, um diese Aufgabe zu erfüllen.

   Setzen Sie beispielsweise für eine Organisation mit Federated IDs und der Domain `adobecustomer.com` Ihren URL-Link auf `https://experience.adobe.com/#/sso:@adobecustomer.com`. Sie können auch direkt zu einem bestimmten Programm gehen, indem Sie diese URL, an die der Programmpfad angehängt ist, als Lesezeichen speichern. (Beispiel für Adobe Analytics: `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Zugriff auf Experience Cloud-Anwendungen {#navigation}

Nach der Anmeldung bei Experience Cloud können Sie über den einheitlichen Header schnell auf alle Ihre Anwendungen, Dienste und Organisationen zugreifen.

Rufen Sie die das ![Menü](assets/menu-icon.png) der Programmauswahl auf, um auf die in Ihrem Unternehmen für Sie bereitgestellten Experience Cloud-Programme und -Services zuzugreifen.

![Zugriff auf Experience Cloud-Programme](assets/platform-core-services.png)

## Erhalten Sie Hilfe und Support {#support}

Greifen Sie mithilfe des Hilfesymbols (![asset](assets/help-icon.png)) in der Kopfzeile auf Lernmaterialien und Hilfe zu, einschließlich Hilfeinhalten (Dokumentation, Tutorials und Kurse) zu [Experience League](https://experienceleague.adobe.com/?lang=de#home) sowie zusätzlichen Ressourcen für einzelne Programme. Sie können auch ein unverbindliches Feedback senden und priorisierte Support-Tickets erstellen.

![Erhalten Sie Hilfe und Support](assets/search-menu.png)

Das Menü [!UICONTROL Hilfe] bietet Ihnen außerdem Zugriff auf:

* **[!UICONTROL Support]:** Erstellen Sie ein Support-Ticket oder kontaktieren Sie den [!UICONTROL Support] über Twitter.
* **[!UICONTROL Feedback]:** Teilen Sie Feedback zu Ihrem Experience Cloud-Erlebnis. Ihr Feedback wird verwendet, um die Produkte und Services von Adobe zu verbessern.
* **[!UICONTROL Status]:** Navigieren Sie zu `https://status.adobe.com/experience_cloud` und prüfen Sie den Betriebsstatus des Produkts und [!UICONTROL verwalten Sie Abonnements].
* **[!UICONTROL Developer Connection]:** Navigation zu `adobe.io` und Entwicklerdokumentation.

## Benutzerprofil- und Kontovoreinstellungen {#preferences}

Zu den Einstellungen im Experience Cloud gehören Benachrichtigungen, Abonnements und Warnhinweise. Im Menü „Kontoeinstellungen“ haben Sie folgende Möglichkeiten:

* Festlegen eines dunklen Designs (nicht alle Anwendungen unterstützen dieses Design)
* Suchen nach [Organisationen](administration/organizations.md)
* Abmelden
* Einstellungen, Benachrichtigungen und Abonnements für das Konto konfigurieren

Um die Voreinstellungen zu verwalten, wählen Sie die Option **[!UICONTROL Voreinstellungen]** im Menü ![Voreinstellungen](assets/preferences-icon-sm.png) Ihres Kontos aus.

![Benutzerprofil- und Kontovoreinstellungen](assets/preferences-page.png)

Unter [!UICONTROL Experience Cloud-Einstellungen] können Sie die folgenden Funktionen konfigurieren:

| Funktion | Beschreibung |
|--- |--- |
| Standard [organisation](administration/organizations.md) | Wählen Sie die Organisation aus, die beim Starten von Experience Cloud angezeigt werden soll. |
| [!UICONTROL Erfassung von Produktdaten] | Wählen Sie aus, welche Technologien Adobe verwenden kann, um Daten darüber zu sammeln, wie Sie Ihre Adobe-Produkte verwenden. |
| [!UICONTROL Personalisierte Empfehlungen und Angebote von Lerninhalten] | Wählen Sie aus, wo Sie personalisierte Hilfe für Ihr(e) Adobe-Produkt(e) erhalten möchten. Diese Hilfe ist per E-Mail, innerhalb des Produktes und in den Experience League Communities verfügbar. [Weitere Informationen.](features/personalized-learning.md) |
| [!UICONTROL Abonnements] | Wählen Sie die Produkte und Kategorien aus, die Sie abonnieren möchten. Benachrichtigungen im Pop-Over [!UICONTROL Benachrichtigungen] und in Ihren E-Mails. |
| [!UICONTROL Priorität] | Wählen Sie die Kategorien aus, die eine hohe Priorität erhalten sollen. Diese Kategorien sind mit dem Tag Hoch gekennzeichnet und können zur Zustellung wie Warnhinweise konfiguriert werden. |
| [!UICONTROL Warnhinweise] | Wählen Sie die Benachrichtigungen aus, für die Warnhinweise in Ihrem Browser angezeigt werden sollen. Warnhinweise werden einige Sekunden lang in der oberen rechten Ecke des Fensters angezeigt. |
| E-Mails | Geben Sie die Häufigkeit an, mit der Sie Benachrichtigungs-E-Mails erhalten möchten. (Nicht gesendet, unmittelbar, täglich oder wöchentlich) |

{style="table-layout:auto"}

## Benachrichtigungen und Ankündigungen {#notifications}

Wählen Sie die Option **[!UICONTROL Benachrichtigungen]** aus, um über relevante und ausführbare Aktualisierungen, einschließlich Produktversionen, Wartungshinweise, freigegebene Elemente und Genehmigungsanfragen, informiert zu werden.

![Benachrichtigungen und Ankündigungen](assets/notifications-menu-small.png)
