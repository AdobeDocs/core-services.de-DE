---
description: 'Hier erfahren Sie, wie Sie sich anmelden, und lernen mehr über die zentralen Komponenten der Benutzeroberfläche in Experience Cloud. Erfahren Sie mehr über die globale Suche, Ihre Kontovoreinstellungen und darüber, wie Sie in der Benutzeroberfläche navigieren und Hilfe erhalten. '
solution: Experience Cloud
title: 'Zentrale Komponenten der Experience Cloud-Benutzeroberfläche '
feature: Central Interface Components
topic: Administration
role: Admin, User
level: Beginner, Intermediate, Experienced
source-git-commit: 5281aededf07508cb49ecd4f3017ccec3d4851fb
workflow-type: ht
source-wordcount: '733'
ht-degree: 100%

---

# Hilfe zur Experience Cloud-Oberfläche

Die zentralen Komponenten der Benutzeroberfläche von Experience Cloud umfassen Funktionen, mit denen Sie:

* sich anmelden und auf Ihre Anwendungen und Dienste zugreifen können
* der globalen Suche nach Produkthilfe und Geschäftsobjekten suchen können
* Kontoeinstellungen verwalten können (Warnhinweise, Benachrichtigungen und Abonnements)

## Browser-Unterstützung in Experience Cloud {#browser}

Für eine optimale Leistung wurde Experience Cloud für die beliebtesten Browser optimiert, jeweils sowohl für deren neueste Version als auch für die beiden Vorgängerversionen.

* Chrome
* Edge
* Firefox
* Opera
* Safari

Wenn Ihr Browser nicht aufgeführt ist, wird er möglicherweise trotzdem unterstützt. Es wird jedoch empfohlen, einen der aufgelisteten Browser zu verwenden.

>[!NOTE]
>
>Nicht alle Anwendungen, die auf der Experience Cloud-Domain ausgeführt werden, unterstützen alle Browser. Wenn Sie sich nicht sicher sind, lesen Sie die Dokumentation zu einem bestimmten Programm.

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
* Spanisch
* Taiwanesisch

Obwohl sich alle Programm-Teams zur globalen Sprachunterstützung verpflichten, werden nicht alle Programme in allen oben genannten Sprachen angeboten. Wenn Ihre Primärsprache in einem Experience Cloud-Programm nicht unterstützt wird, können Sie auch eine sekundäre Sprache so einstellen, dass sie ggf. auf Standard gesetzt wird. Dies kann unter [Benutzervoreinstellungen für Experience Cloud](https://experience.adobe.com/preferences) durchgeführt werden.

## Melden Sie sich bei Experience Cloud an {#signin}

Melden Sie sich an und stellen Sie sicher, dass Sie sich in der richtigen [Organisation](organizations.md) befinden.

1. Navigieren Sie zur [Adobe Experience Cloud](https://experience.adobe.com).
1. Wählen Sie **[!UICONTROL Mit Adobe ID anmelden]** aus.
1. Stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden.

   ![Organisation überprüfen](assets/organizations-menu.png)

   Um sicherzustellen, dass Sie sich bei Ihrer richtigen [Organisation](organizations.md) angemeldet haben, klicken Sie auf Ihren Profilavatar, um den Organisationsnamen anzuzeigen. Wenn Sie Zugriff auf mehr als eine Organisation haben, können Sie rechts in der Kopfzeilenleiste auch eine andere Organisation anzeigen und zu dieser wechseln.

   Wenn Ihr Unternehmen Federated IDs verwendet, können Sie sich mit Experience Cloud beim Single Sign-on Ihres Unternehmens anmelden, ohne Ihre E-Mail-Adresse und Ihr Passwort eingeben zu müssen. Um diese Funktion zu verwenden, fügen Sie `#/sso:@domain` zur Experience Cloud-URL hinzu (`https://experience.adobe.com`).

   Setzen Sie beispielsweise für eine Organisation mit Federated IDs und der Domain `adobecustomer.com` Ihren URL-Link auf `https://experience.adobe.com/#/sso:@adobecustomer.com`. Sie können auch direkt zu einem bestimmten Programm gehen, indem Sie diese URL, an die der Programmpfad angehängt ist, als Lesezeichen speichern. (Beispiel für Adobe Analytics: `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Zugriff auf Experience Cloud-Anwendungen {#navigation}

Nach der Anmeldung bei Experience Cloud können Sie über den einheitlichen Header schnell auf alle Ihre Anwendungen, Dienste und Organisationen zugreifen.

Wählen Sie den Anwendungsselektor ![](assets/menu-icon.png) aus, um auf die von Ihnen verwalteten Experience Cloud-Services zuzugreifen.

![Zugriff auf Experience Cloud-Programme](assets/platform-core-services.png)

## Suche und Support in Experience Cloud {#search-support}

Mit der Experience Cloud-Suche können Sie nach Hilfe (Dokumentation, Tutorials und Kurse) auf [Experience League](https://experienceleague.adobe.com/?lang=de#home) suchen.

![Suche und Support in Experience Cloud](assets/search-menu.png)

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

Wählen Sie die Option **[!UICONTROL Voreinstellungen]** im Kontomenü ![](assets/preferences-icon-sm.png) aus, um die Voreinstellungen zu verwalten.

![Verwalten von Experience Cloud](assets/preferences-page.png)

Unter [!UICONTROL Experience Cloud-Einstellungen] können Sie die folgenden Funktionen konfigurieren:

| Funktion | Beschreibung |
|--- |--- |
| Standard [organisation](organizations.md) | Wählen Sie die Organisation aus, die beim Starten von Experience Cloud angezeigt werden soll. |
| [!UICONTROL Abonnements] | Wählen Sie die Produkte und Kategorien aus, die Sie abonnieren möchten. Benachrichtigungen im Pop-Over [!UICONTROL Benachrichtigungen] und in Ihren E-Mails. |
| [!UICONTROL Priorität] | Wählen Sie die Kategorien aus, die eine hohe Priorität erhalten sollen. Diese Kategorien sind mit dem Tag Hoch gekennzeichnet und können zur Zustellung wie Warnhinweise konfiguriert werden. |
| [!UICONTROL Warnhinweise] | Wählen Sie die Benachrichtigungen aus, für die Warnhinweise in Ihrem Browser angezeigt werden sollen. Warnhinweise werden einige Sekunden lang in der oberen rechten Ecke des Fensters angezeigt. |
| E-Mails | Geben Sie die Häufigkeit an, mit der Sie Benachrichtigungs-E-Mails erhalten möchten. (Nicht gesendet, unmittelbar, täglich oder wöchentlich) |

{style=&quot;table-layout:auto&quot;}

## Benachrichtigungen und Ankündigungen {#notifications}

Wählen Sie die Option **[!UICONTROL Benachrichtigungen]** aus, um für Sie wichtige Benachrichtigungen sowie Ankündigungen von Adobe anzuzeigen.

![Benachrichtigungen und Ankündigungen](assets/notifications-menu-small.png)

Sie können Benachrichtigungen unter [Experience Cloud-Einstellungen](#preferences) konfigurieren.
