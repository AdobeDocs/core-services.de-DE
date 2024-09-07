---
title: Kontovoreinstellungen und Benachrichtigungen
description: Informationen zu Benutzerprofilen und Kontovoreinstellungen finden Sie unter Experience Cloud. Abonnieren Sie Produktbenachrichtigungen für E-Mails und  [!DNL Slack] und richten Sie Produktwarnungen ein.
solution: Experience Cloud
feature: Account Preferences, Notifications, Alerts
topic: Administration
role: Admin
level: Intermediate
exl-id: 1e34c6b2-a792-41c4-adb7-583de596237f
source-git-commit: b79d6c6fb7bb165fdd5d47061da16f65f6fc7579
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 21%

---

# Kontovoreinstellungen und Benachrichtigungen {#preferences}

Zu den Experience Cloud [Voreinstellungen](https://experience.adobe.com/preferences) gehören Benachrichtigungen (In-App, E-Mail und [!DNL Slack]), Abonnements und Warnungen.

In den Voreinstellungen haben Sie folgende Möglichkeiten:

* Suchen nach [Organisationen](../administration/organizations.md)
* Geben Sie ein dunkles Design an (nicht alle Anwendungen unterstützen dieses Design).
* Konfigurieren Sie Benutzereinstellungen, Benachrichtigungen und Abonnements.
* Melden Sie sich von der Experience Cloud ab.

## Verwalten von Voreinstellungen

Um die Voreinstellungen zu verwalten, wählen Sie die Option **[!UICONTROL Voreinstellungen]** im Menü ![Voreinstellungen](../assets/preferences-icon-sm.png) Ihres Kontos aus.

Unter [!UICONTROL Experience Cloud-Einstellungen] können Sie die folgenden Funktionen konfigurieren:

| Funktion | Beschreibung |
|--- |--- |
| Standard [organisation](../administration/organizations.md) | Wählen Sie die Organisation aus, die beim Starten von Experience Cloud angezeigt werden soll. |
| [!UICONTROL Erfassung von Produktdaten] | Wählen Sie aus, welche Technologien Adobe verwenden kann, um Daten darüber zu sammeln, wie Sie Ihre Adobe-Produkte verwenden. |
| [Benachrichtigungen](#notifications-and-announcements) | Aktivieren Sie die Benachrichtigungen für [!UICONTROL In-App], [!UICONTROL E-Mail] oder [Slack](#slack-notifications). |
| [!UICONTROL Personalisierte Empfehlungen und Angebote von Lerninhalten] | Wählen Sie aus, wo Sie [personalisierte Hilfe](personalized-learning.md) für Ihre Adobe-Produkte erhalten möchten. Diese Hilfe ist per E-Mail, im Produkt und in den Experience League Communities verfügbar. |
| [!UICONTROL Abonnements] | Wählen Sie die Produkte und Kategorien aus, die Sie abonnieren möchten. Benachrichtigungen im Popup-Fenster [!UICONTROL Benachrichtigungen] und in Ihrer E-Mail. |
| [!UICONTROL Priorität] | Wählen Sie die Kategorien aus, die eine hohe Priorität erhalten sollen. Diese Kategorien sind mit dem Tag [!UICONTROL Hoch] markiert und können für Sendungen wie Warnungen konfiguriert werden. |
| [!UICONTROL Warnhinweise] | Wählen Sie die Benachrichtigungen aus, für die Warnhinweise in Ihrem Browser angezeigt werden sollen. Warnhinweise werden einige Sekunden lang in der oberen rechten Ecke des Fensters angezeigt. |
| E-Mails | Geben Sie die Häufigkeit an, mit der Sie Benachrichtigungs-E-Mails erhalten möchten. (Nicht gesendet, unmittelbar, täglich oder wöchentlich) |

## Abonnieren von Benachrichtigungen in Experience Cloud {#notifications}

Sie können die Produkte und Kategorien auswählen, die Sie abonnieren möchten. Benachrichtigungen werden im Popup-Fenster [!UICONTROL Benachrichtigungen] (in der App), in Ihrer E-Mail oder in [Slack](#slack-notifications) (je nach Ihren Abonnements) angezeigt.

E-Mail- und Slack-Benachrichtigungen eignen sich für Situationen, in denen Sie nicht bei Experience Cloud angemeldet sind.

### In-App- und E-Mail-Benachrichtigungen abonnieren

1. Navigieren Sie zu Experience Cloud [Voreinstellungen](https://experience.adobe.com/preferences).

1. Aktivieren Sie unter **[!UICONTROL Benachrichtigungen]** die Option **[!UICONTROL In-App]** oder **[!UICONTROL E-Mail]**.

   Änderungen an Benachrichtigungen werden automatisch gespeichert.

### Anmelden für [!DNL Slack] -Benachrichtigungen {#slack}

>[!NOTE]
>
>Slack-Benachrichtigungen werden veröffentlicht: **11. September 2024**


Sie können Ihre Kontovoreinstellungen so konfigurieren, dass Experience Cloud-Benachrichtigungen an einen [!DNL Slack] -Kanal gesendet werden.

**Voraussetzungen**

* Sie müssen über ein Experience Cloud-Konto verfügen.
* Sie müssen über ein [!DNL Slack] -Konto verfügen. Ihr Slack-Administrator aktiviert die Experience Cloud-Integration mit Slack.
* Sie müssen mindestens einem [!DNL Slack] -Arbeitsbereich angehören.

**Abonnieren von Slack-Benachrichtigungen**

1. Navigieren Sie zu Experience Cloud [Voreinstellungen](https://experience.adobe.com/preferences).

1. Suchen Sie [!DNL Slack] und klicken Sie dann auf **[!UICONTROL Zu Slack hinzufügen]**.

   ![Zu Slack hinzufügen](../assets/add-to-slack.png)

   Wenn [!DNL Slack] installiert ist, wird die Anwendung geöffnet und eine Meldung mit einer Berechtigungsanforderung angezeigt. Wenn Slack nicht installiert ist, müssen Sie [die Berechtigung anfordern](#slack-troubleshoot).

1. Klicken Sie auf **[!UICONTROL Allow]**.

1. Aktivieren Sie unter **[!UICONTROL Benachrichtigungen]** die Option [!DNL Slack] Benachrichtigungen für Ihre gewünschten Produkte und Kategorien.

   ![Slack notifications](../assets/slack.png)

   Aktualisierungen der Benachrichtigungen werden automatisch gespeichert.

### Anfrageberechtigung in Slack {#slack-troubleshoot}

Wenn [!DNL Slack] nicht installiert ist, wird beim Öffnen der Slack nach dem Klicken auf **[!UICONTROL Zu Slack hinzufügen]** die Meldung _[!UICONTROL Installationsanfrage]_ angezeigt.

![Slack-Integration anfordern](../assets/slack-request.png)

**So fordern Sie Berechtigungen in Slack** an

1. Wählen Sie unter Slack den Arbeitsbereich oben rechts im Programm aus.

1. Um die Anwendungsgenehmigung für den Slack Workspace-Manager anzufordern, klicken Sie auf **[!UICONTROL Senden]**.

1. Sie erhalten eine Benachrichtigung in [!DNL Slack] , nachdem die Anwendungsanforderung genehmigt wurde.

1. Nachdem Sie die [!DNL Slack]-Genehmigung erhalten haben, kehren Sie zu Experience Cloud **[!UICONTROL Benachrichtigungen]** und [Abonnieren Sie Slack](#slack-notifications) zurück (siehe oben).

### Was Sie in [!DNL Slack] sehen werden

Nach erfolgreicher Integration von Slack zeigen die Slack-Benachrichtigungen die folgenden Informationen an:

* Die persönliche Nachricht wird vom Anwendungsnamen _Adobe Experience Cloud_ empfangen.
* Die Nachricht enthält das Produktlogo für die jeweilige Anwendung, z. B. Adobe Experience Platform, Adobe Experience Manager usw.
* Ein Link zum Anzeigen aller Benachrichtigungen auf dem Experience Cloud.
* Ein Link zur Verwaltung von Benachrichtigungseinstellungen auf dem Experience Cloud.

## Anzeigen von [!UICONTROL Benachrichtigungen] und Mitteilungen in Experience Cloud {#view-notifications}

In der Experience Cloud-Kopfzeile können Sie Benachrichtigungen anzeigen, für die Sie [Abonnement](#notifications) abgeschlossen haben, sowie Ankündigungen anzeigen.

1. Klicken Sie auf das Glockensymbol in der Kopfzeile. ![Benachrichtigungen und Ankündigungen](../assets/bell-icon.png)

1. Klicken Sie auf **[!UICONTROL Benachrichtigungen]** oder **[!UICONTROL Mitteilungen]**.

   An diesem Ort erhalten Sie wichtige Informationen zu Produkten, Ihre Zusammenarbeit mit anderen Benutzern und andere relevante Updates. Zu den Aktualisierungen gehören Produktversionen, Wartungshinweise, freigegebene Elemente und Genehmigungsanfragen.