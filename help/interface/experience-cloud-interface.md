---
description: Erfahren Sie, wie Sie sich anmelden, und lernen Sie die zentralen Komponenten der Benutzeroberfläche in CX Enterprise kennen. Erfahren Sie mehr über die globale Suche, Ihre Kontovoreinstellungen und darüber, wie Sie in der Benutzeroberfläche navigieren und Hilfe erhalten.
solution: Experience Cloud
title: Zentrale Komponenten der Experience Cloud-Benutzeroberfläche
feature: Central Interface Components
topic: Administration
role: Admin, User
level: Beginner, Intermediate, Experienced
source-git-commit: 1a77ef8d31211fb11c790152e78037a8c3b238a2
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 42%

---

# Zentrale Komponenten der CX Enterprise-Benutzeroberfläche

Die zentralen Komponenten der Benutzeroberfläche von CX Enterprise umfassen Funktionen, die Ihnen Folgendes ermöglichen:

* sich anmelden und auf Ihre Anwendungen und Dienste zugreifen können
* der globalen Suche nach Produkthilfe und Geschäftsobjekten suchen können
* Kontoeinstellungen verwalten können (Warnhinweise, Benachrichtigungen und Abonnements)

## Browser-Unterstützung in CX Enterprise

Um eine optimale Leistung zu erzielen, ist CX Enterprise für die beliebtesten Browser optimiert, einschließlich der neuesten Version sowie der beiden vorherigen Versionen.

* Chrome
* Edge
* Firefox
* Opera
* Safari

Wenn Ihr Browser nicht aufgeführt ist, wird er möglicherweise trotzdem unterstützt. Es wird jedoch empfohlen, einen der aufgelisteten Browser zu verwenden.

>[!NOTE]
>
>Nicht alle Anwendungen, die auf der CX Enterprise-Domain ausgeführt werden, unterstützen alle Browser. Wenn Sie sich nicht sicher sind, lesen Sie die Dokumentation zu einem bestimmten Programm.

## Sprachunterstützung in CX Enterprise

CX Enterprise unterstützt bevorzugte Sprachen für jeden Benutzer, wie in den Voreinstellungen Ihres Adobe-Benutzerkontos festgelegt. Derzeit werden folgende Sprachen unterstützt:

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

Obwohl sich alle Programm-Teams zur globalen Sprachunterstützung verpflichten, werden nicht alle Programme in allen oben genannten Sprachen angeboten. Wenn Ihre Primärsprache in einem CX Enterprise-Programm nicht unterstützt wird, können Sie auch eine sekundäre Sprache so einstellen, dass sie ggf. auf Standard gesetzt wird. Dies kann unter [Benutzereinstellungen für CX Enterprise erfolgen](https://experience.adobe.com/preferences).

## Bei CX Enterprise anmelden

Melden Sie sich an und stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden.

1. Navigieren Sie zu [Adobe CX Enterprise](https://experience.adobe.com).
1. Klicken Sie auf **[!UICONTROL Sign in with an Adobe ID]**.
1. Stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden.

   ![Organisation überprüfen](assets/organizations-menu.png)

   Um sicherzustellen, dass Sie sich bei Ihrer richtigen Organisation angemeldet haben, klicken Sie auf **[!UICONTROL Profile]**, um den Organisationsnamen anzuzeigen. Wenn Sie Zugriff auf mehr als eine Organisation haben, können Sie mit der **[!UICONTROL Organization]** auch eine andere Organisation anzeigen und zu ihr wechseln.

   Wenn Ihr Unternehmen Federated IDs verwendet, können Sie sich mit CX Enterprise beim Single Sign-on Ihres Unternehmens anmelden, ohne Ihre E-Mail-Adresse und Ihr Passwort eingeben zu müssen. Fügen Sie `#/sso:@domain` zur CX Enterprise-URL (`https://experience.adobe.com`) hinzu, um diese Aufgabe zu erfüllen.

   Setzen Sie beispielsweise für eine Organisation mit Federated IDs und der Domain `example.com` Ihren URL-Link auf `https://experience.adobe.com/#/sso:@example.com`. Sie können auch direkt zu einem bestimmten Programm gehen, indem Sie diese URL, an die der Programmpfad angehängt ist, als Lesezeichen speichern. (Beispiel für Adobe Analytics: `https://experience.adobe.com/#/sso:@example.com/analytics`.)

## Zugriff auf CX Enterprise-Programme

Nach der Anmeldung bei CX Enterprise können Sie über den einheitlichen Header schnell auf alle Ihre Programme, Services und Organisationen zugreifen.

Klicken Sie auf die Programmauswahl ![Menü](assets/menu-icon.png), um auf die von Ihnen verwalteten CX Enterprise-Services zuzugreifen.

![Zugriff auf CX Enterprise-Programme](assets/platform-core-services.png)

## Suche und Support in CX Enterprise

Mit der CX Enterprise-Suche können Sie nach Hilfe (Dokumentation, Tutorials und Kurse) in [Experience League suchen](https://experienceleague.adobe.com/de?lang=de#home).

![Suche und Support in CX Enterprise](assets/search-menu.png)

Das [!UICONTROL Help] Menü bietet außerdem Zugriff auf:

* **[!UICONTROL Support]:** Erstellen Sie ein Support-Ticket oder kontaktieren Sie [!UICONTROL Support] über Twitter.
* **[!UICONTROL Feedback]:** Kontaktieren Sie Adobe mithilfe von Feedback und teilen Sie uns Ihre Meinung mit.
* **[!UICONTROL Status]:** Navigieren Sie zu `https://status.adobe.com/de-de/experience_cloud` und überprüfen Sie den Betriebsstatus und die [!UICONTROL Manage Subscriptions] des Produkts.
* **[!UICONTROL Developer Connection]:** Navigation zum `adobe.io` und zur Entwicklerdokumentation.

## Kontoeinstellungen

Im Menü „Kontoeinstellungen“ haben Sie folgende Möglichkeiten:

* Festlegen eines dunklen Designs (nicht alle Anwendungen unterstützen dieses Design)
* Suchen nach Organisationen
* Abmelden
* [Einstellungen, Benachrichtigungen und Abonnements](#preferences) für das Konto konfigurieren

### Verwalten von CX Enterprise [!UICONTROL Preferences]

Zu den CX Enterprise-Voreinstellungen gehören Benachrichtigungen, Abonnements und Warnhinweise.

* Klicken Sie im Kontomenü ![Einstellungen](assets/preferences-icon-sm.png) auf **[!UICONTROL Preferences]** , um die Einstellungen zu verwalten.

![CX Enterprise verwalten](assets/preferences-page.png)

In [!UICONTROL CX Enterprise preferences] können Sie die folgenden Funktionen konfigurieren:

| Funktion | Beschreibung |
| --- | --- |
| Standardorganisation | Wählen Sie die Organisation aus, die beim Starten von CX Enterprise angezeigt werden soll. |
| [!UICONTROL Subscriptions] | Wählen Sie die Produkte und Kategorien aus, die Sie abonnieren möchten. Benachrichtigungen im Pop-up &quot;[!UICONTROL Notifications]&quot; und in Ihrer E-Mail. |
| [!UICONTROL Priority] | Wählen Sie die Kategorien aus, die eine hohe Priorität erhalten sollen. Diese Kategorien sind mit dem Tag Hoch gekennzeichnet und können zur Zustellung wie Warnhinweise konfiguriert werden. |
| [!UICONTROL Alerts] | Wählen Sie die Benachrichtigungen aus, für die Warnhinweise in Ihrem Browser angezeigt werden sollen. Warnhinweise werden einige Sekunden lang in der oberen rechten Ecke des Fensters angezeigt. |
| E-Mails | Geben Sie die Häufigkeit an, mit der Sie Benachrichtigungs-E-Mails erhalten möchten. (Nicht gesendet, unmittelbar, täglich oder wöchentlich) |

{style="table-layout:auto"}

## Benachrichtigungen und Ankündigungen

Klicken Sie auf **[!UICONTROL Notifications]** , um Benachrichtigungen, die für Sie wichtig sind, sowie Ankündigungen von Adobe anzuzeigen.

![Benachrichtigungen und Ankündigungen](assets/notifications-menu-small.png)

Sie können Benachrichtigungen in den [CX Enterprise-Voreinstellungen](#preferences) konfigurieren.
