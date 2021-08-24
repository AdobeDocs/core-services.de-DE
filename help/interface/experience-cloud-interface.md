---
description: 'Erfahren Sie, wie Sie sich anmelden und über die zentralen Komponenten der Benutzeroberfläche in Experience Cloud. Erfahren Sie mehr über die globale Suche, Ihre Kontovoreinstellungen und wie Sie in der Benutzeroberfläche navigieren und Hilfe erhalten. '
solution: Experience Cloud
title: 'Zentrale Komponenten der Experience Cloud-Benutzeroberfläche '
feature: „Zentrale Komponenten der Benutzeroberfläche“
topic: Administration.
role: Admin, User
level: Beginner, Intermediate, Experienced
source-git-commit: c9a6059b0af9c6229fd72580f997c1c6f2dfbbe4
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 50%

---

# Hilfe zur Experience Cloud-Oberfläche

Die zentralen Komponenten der Benutzeroberfläche von Experience Cloud umfassen Funktionen, mit denen Sie:

* sich anmelden und auf Ihre Anwendungen und Dienste zugreifen können
* der globalen Suche nach Produkthilfe und Geschäftsobjekten suchen können
* Kontoeinstellungen verwalten können (Warnhinweise, Benachrichtigungen und Abonnements)

## Browserunterstützung in Experience Cloud {#browser}

Für optimale Leistung wurde Experience Cloud für die beliebtesten Browser optimiert, einschließlich der neuesten Version und der beiden Vorgängerversionen.

* Chrome
* Edge
* Firefox
* Opera
* Safari

Wenn Ihr Browser nicht aufgeführt ist, wird er möglicherweise weiterhin unterstützt. Es wird jedoch empfohlen, einen der aufgelisteten Browser zu verwenden.

>[!NOTE]
>
>Nicht alle Anwendungen, die auf der Experience Cloud-Domäne ausgeführt werden, unterstützen alle Browser. Wenn Sie sich nicht sicher sind, lesen Sie die Dokumentation zu einer bestimmten Anwendung.

## Sprachunterstützung in Experience Cloud {#languages}

Experience Cloud unterstützt bevorzugte Sprachen für jeden Benutzer, wie in den Voreinstellungen Ihres Adobe-Benutzerkontos festgelegt. Derzeit werden folgende Sprachen unterstützt:

* Chinesisch
* Englisch
* Französisch
* Deutsch
* Italienisch
* Japanisch
* Koreanisch
* Portugiesisch
* spanisch
* Taiwanisch

Obwohl sich alle Anwendungsteams zur globalen Sprachunterstützung verpflichten, werden nicht alle Anwendungen in allen oben genannten Sprachen angeboten. Wenn Ihre Primärsprache in einer Experience Cloud App nicht unterstützt wird, können Sie auch eine sekundäre Sprache so einstellen, dass sie ggf. auf Standard gesetzt wird. Dies kann unter [Benutzereinstellungen für Experience Clouden](https://experience.adobe.com/preferences) durchgeführt werden.

## Melden Sie sich bei Experience Cloud an {#signin}

Melden Sie sich an und stellen Sie sicher, dass Sie sich in der richtigen [Organisation](organizations.md) befinden.

1. Navigieren Sie zur [Adobe Experience Cloud](https://experience.adobe.com).
1. Wählen Sie **[!UICONTROL Anmelden mit einer Adobe ID]** aus.
1. Stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden.

   ![](assets/organizations-menu.png)

   Um sicherzustellen, dass Sie sich bei Ihrer richtigen [Organisation](organizations.md) angemeldet haben, klicken Sie auf Ihren Profilavatar, um den Organisationsnamen anzuzeigen. Wenn Sie Zugriff auf mehr als eine Organisation haben, können Sie rechts in der Kopfzeilenleiste auch eine andere Organisation anzeigen und zu dieser wechseln.

   Wenn Ihr Unternehmen Federated IDs verwendet, können Sie sich mit Experience Cloud beim Single Sign-on Ihres Unternehmens anmelden, ohne Ihre E-Mail-Adresse und Ihr Passwort eingeben zu müssen. Fügen Sie dazu `#/sso:@domain` zur Experience Cloud-URL (`https://experience.adobe.com`) hinzu.

   Setzen Sie beispielsweise für eine Organisation mit Federated IDs und der Domäne `adobecustomer.com` Ihren URL-Link auf `https://experience.adobe.com/#/sso:@adobecustomer.com`. Sie können auch direkt zu einer bestimmten Anwendung gehen, indem Sie diese URL mit einem Lesezeichen versehen, das an den Anwendungspfad angehängt ist. (Beispiel: für Adobe Analytics `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Zugriff auf Experience Cloud-Anwendungen {#navigation}

Nach der Anmeldung bei Experience Cloud können Sie über den einheitlichen Header schnell auf alle Ihre Anwendungen, Dienste und Organisationen zugreifen.

Wählen Sie den Anwendungsselektor ![](assets/menu-icon.png) aus, um auf die von Ihnen verwalteten Experience Cloud-Dienste zuzugreifen.

![](assets/platform-core-services.png)

## Suche und Support in Experience Cloud {#search}

Mit der Experience Cloud-Suche können Sie nach Hilfe (Dokumentation, Tutorials und Kurse) auf [Experience League](https://experienceleague.adobe.com/?lang=de#home) suchen.

![](assets/search-menu.png)

Das Menü [!UICONTROL Hilfe] bietet Ihnen außerdem Zugriff auf:

* **[!UICONTROL Support]:** Erstellen Sie ein Support-Ticket oder kontaktieren Sie den [!UICONTROL Support] über Twitter.
* **[!UICONTROL Feedback]:** Kontaktieren Sie Adobe mithilfe von Feedback und teilen Sie uns Ihre Meinung mit.
* **[!UICONTROL Status]:** Navigieren Sie zu `https://status.adobe.com/experience_cloud` und prüfen Sie den Betriebsstatus des Produkts und [!UICONTROL verwalten Sie Abonnements].
* **[!UICONTROL Developer Connection]:** Navigation zu `adobe.io` und Entwicklerdokumentation.

## Kontoeinstellungen {#account-menu}

Im Menü „Kontoeinstellungen“ haben Sie folgende Möglichkeiten:

* Festlegen eines dunklen Designs (nicht alle Anwendungen unterstützen dieses Design)
* Suchen nach [Organisationen](organizations.md)
* Abmelden
* [Einstellungen, Benachrichtigungen und Abonnements](#preferences) für das Konto konfigurieren

### Experience Cloud [!UICONTROL -Einstellungen] verwalten {#preferences}

Zu den Einstellungen im Experience Cloud gehören Benachrichtigungen, Abonnements und Warnhinweise.

Wählen Sie **[!UICONTROL Voreinstellungen]** aus Ihrem Kontomenü ![](assets/preferences-icon-sm.png) aus, um die Voreinstellungen zu verwalten.

![](assets/preferences-page.png)

Unter [!UICONTROL Experience Cloud-Einstellungen] können Sie die folgenden Funktionen konfigurieren:

| Funktion | Beschreibung |
|--- |--- |
| Standard[organisation](organizations.md) | Wählen Sie die Organisation aus, die beim Starten von Experience Cloud angezeigt werden soll. |
| [!UICONTROL Abonnements] | Wählen Sie die Produkte und Kategorien aus, die Sie abonnieren möchten. Benachrichtigungen im Pop-Over [!UICONTROL Benachrichtigungen] und in Ihren E-Mails. |
| [!UICONTROL Priorität] | Wählen Sie die Kategorien aus, die eine hohe Priorität erhalten sollen. Diese Kategorien sind mit dem Tag Hoch gekennzeichnet und können zur Zustellung wie Warnhinweise konfiguriert werden. |
| [!UICONTROL Warnhinweise] | Wählen Sie die Benachrichtigungen aus, für die Warnhinweise in Ihrem Browser angezeigt werden sollen. Warnhinweise werden einige Sekunden lang in der oberen rechten Ecke des Fensters angezeigt. |
| E-Mails | Geben Sie die Häufigkeit an, mit der Sie Benachrichtigungs-E-Mails erhalten möchten. (Nicht gesendet, unmittelbar, täglich oder wöchentlich) |

{style=&quot;table-layout:auto&quot;}

## Benachrichtigungen und Ankündigungen {#notifications}

Wählen Sie **[!UICONTROL Benachrichtigungen]** aus, um Benachrichtigungen, die für Sie wichtig sind, sowie Mitteilungen aus Adobe anzuzeigen.

![](assets/notifications-menu-small.png)

Sie können Benachrichtigungen unter [Experience Cloud-Einstellungen](#preferences) konfigurieren.
