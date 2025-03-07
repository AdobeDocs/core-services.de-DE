---
description: Erfahren Sie mehr über zentrale Oberflächenkomponenten für Experience Cloud. Erhalten Sie Hilfe zur Benutzer- und Produktverwaltung in der Admin Console und aktivieren Sie Anwendungen für Experience Cloud-Services. Erhalten Sie Hilfe zur Zielgruppenbibliothek, zu Kundenattributen, zu Experience Cloud-Assets und mehr.
title: Benutzeroberfläche und Administration von Experience Cloud
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: dd4f3b5df4bb7f3775977049e8d9a67e21052f10
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 99%

---

# Benutzeroberfläche und Verwaltung von Experience Cloud

[Experience Cloud](https://experience.adobe.com) umfasst die Digital-Marketing-Programme, -Produkte und -Services von Adobe. Über die intuitive Benutzeroberfläche können Sie schnell auf Ihre Cloud-Programme, Produktfunktionen und Services zugreifen.

![Experience Cloud](assets/landing.png)

In der Kopfzeile von Experience Cloud haben Sie folgende Möglichkeiten:

* Zugriff auf alle Experience Cloud-Anwendungen und -Services
* Suchen Sie über das Menü „Hilfe“ nach Produktdokumentationen, Tutorials und Community-Beiträgen. Lassen Sie sich Ergebnisse in Experience League anzeigen.
* Suchen Sie global nach Geschäftsobjekten, indem Sie eine globale Suche (nur für Nutzerinnen und Nutzer der Experience Platform) im Feld „Suche“ verwenden.
* Verwalten der [Einstellungen](features/account-preferences.md) des Kontos (Warnhinweise, Benachrichtigungen und Abonnements)

## Melden Sie sich bei Experience Cloud an {#signin}

Melden Sie sich an und stellen Sie sicher, dass Sie sich in der richtigen [Organisation](administration/organizations.md) befinden.

1. Navigieren Sie zur [Adobe Experience Cloud](https://experience.adobe.com).
1. Geben Sie Ihre Adobe-E-Mail-Adresse ein und klicken Sie auf **[!UICONTROL Weiter]**.
1. Klicken Sie auf ein Konto.
1. Geben Sie Ihr Passwort ein.
1. Stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden.

   ![Stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden](assets/organizations-menu.png)

   **Organisation überprüfen**

   Die [Organisation](administration/organizations.md) wird in der Kopfzeile der Benutzeroberfläche angezeigt.

   Wenn Ihr Unternehmen Federated IDs verwendet, können Sie sich durch ein Single Sign-on Ihres Unternehmens bei Experience Cloud anmelden, ohne Ihre E-Mail-Adresse und Ihr Passwort eingeben zu müssen. Fügen Sie `#/sso:@domain` zur Experience Cloud-URL (`https://experience.adobe.com`) hinzu, um diese Aufgabe zu erfüllen.

   Setzen Sie beispielsweise für eine Organisation mit Federated IDs und der Domain `adobecustomer.com` Ihren URL-Link auf `https://experience.adobe.com/#/sso:@adobecustomer.com`. Sie können auch direkt zu einem bestimmten Programm gehen, indem Sie diese URL, an die der Programmpfad angehängt ist, als Lesezeichen speichern. (Beispiel für Adobe Analytics: `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Zugriff auf Experience Cloud-Anwendungen {#navigation}

Nach der Anmeldung bei Experience Cloud können Sie über den einheitlichen Header schnell auf alle Ihre Anwendungen, Dienste und Organisationen zugreifen.

Rufen Sie die das ![Menü](assets/apps-icon.png) der Programmauswahl auf, um auf die in Ihrem Unternehmen für Sie bereitgestellten Experience Cloud-Programme und -Services zuzugreifen.

![Zugriff auf Experience Cloud-Programme](assets/platform-core-services.png)

## Hilfe und Support {#support}

Greifen Sie über das **[!UICONTROL Hilfezentrum]** (![Asset](assets/help-icon.png)) in der Kopfzeile auf Lernmaterialien und Hilfe zu, einschließlich Hilfeinhalten (Dokumentation, Tutorials und Kurse) auf [Experience League](https://experienceleague.adobe.com/?lang=de#home) sowie zusätzlichen Ressourcen für einzelne Programme. Sie können auch ein unverbindliches Feedback senden und priorisierte Support-Tickets erstellen.

![Erhalten Sie Hilfe und Support](assets/search-menu.png)

Das Menü [!UICONTROL Hilfe] bietet Ihnen außerdem Zugriff auf:

* **[!UICONTROL Support]:** Erstellen Sie ein Support-Ticket oder kontaktieren Sie den [!UICONTROL Support] über Twitter.
* **[!UICONTROL Feedback]:** Teilen Sie Feedback zu Ihrem Experience Cloud-Erlebnis. Ihr Feedback wird verwendet, um die Produkte und Services von Adobe zu verbessern.
* **[!UICONTROL Status]:** Navigieren Sie zu `https://status.adobe.com/experience_cloud` und prüfen Sie den Betriebsstatus des Produkts und [!UICONTROL verwalten Sie Abonnements].
* **[!UICONTROL Developer Connection]:** Navigation zu `adobe.io` und Entwicklerdokumentation.

## Verwalten des Benutzerprofils

Im Menü [!UICONTROL Profil] haben Sie folgende Möglichkeiten:

* Festlegen eines dunklen Designs (nicht alle Anwendungen unterstützen dieses Design)
* Verwalten von Experience Cloud [-Einstellungen](features/account-preferences.md)
* Auswählen von oder Suchen nach [Organisationen](administration/organizations.md)
* Anzeigen von [!UICONTROL rechtlichen Hinweisen]
* Abmelden
* Einstellungen, Benachrichtigungen und Abonnements für das Konto konfigurieren

## Anzeigen von Benachrichtigungen und Ankündigungen im Produkt {#notifications}

Klicken Sie auf das Glockensymbol, um Benachrichtigungen und Ankündigungen anzuzeigen. Bei Ankündigungen kann es sich um relevante und umsetzbare Aktualisierungen handeln, einschließlich Produktversionen, Wartungshinweisen, freigegebenen Elementen und Genehmigungsanfragen.

![Benachrichtigungen und Ankündigungen](assets/notifications-menu-small.png)

Informationen zum Verwalten von Benachrichtigungen und Warnhinweisen finden Sie unter [Kontoeinstellungen und Benachrichtigungen](features/account-preferences.md).
