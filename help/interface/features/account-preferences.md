---
title: Kontovoreinstellungen und Benachrichtigungen
description: Erfahren Sie mehr über Voreinstellungen zu Benutzerprofilen und Konten in Experience Cloud. Abonnieren Sie Produktbenachrichtigungen für E-Mail und  [!DNL Slack] und richten Sie Produktbenachrichtigungen ein.
solution: Experience Cloud
feature: Account Preferences, Notifications, Alerts
topic: Administration
role: Admin
level: Intermediate
exl-id: 1e34c6b2-a792-41c4-adb7-583de596237f
source-git-commit: e523471b6dd67cf8213ead3208347fd3aa32a164
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 10%

---

# Kontovoreinstellungen und Benachrichtigungen {#preferences}

Um Experience Cloud-Voreinstellungen zu finden, klicken Sie **[!UICONTROL Profil]** ![Voreinstellungen](../assets/preferences-icon-sm.png) in der Kopfzeile und anschließend auf **[!UICONTROL Voreinstellungen]**.

![Voreinstellungen](../assets/preferences-navigation.png){width="100" zoomable="yes"}

Auf der Seite [!UICONTROL Experience Cloud]Einstellungen können Sie die folgenden Kontofunktionen verwalten:

| Funktion | Beschreibung |
|--- |--- |
| Profil | [Adobe-Kontoprofil aktualisieren](https://account.adobe.com/profile). <p>Ihr Profilbild und Ihr Name werden angezeigt, wenn Sie sich bei Adobe.com, Adobe-Produkten und -Services und auf öffentlich zugänglichen Websites wie [!DNL Behance] anmelden. |
| Allgemein | Wählen Sie eine [Organisation](../administration/organizations.md) aus.<p>Diese Organisation wird standardmäßig verwendet, wenn Sie sich bei Experience Cloud anmelden. |
| [!UICONTROL Erfassung von Produktdaten] | Wählen Sie aus, welche Technologien Adobe verwenden kann, um Daten darüber zu sammeln, wie Sie Ihre Adobe-Produkte verwenden. |
| Benachrichtigungen | Konfigurieren Sie, wie und wann Sie Produkt[Benachrichtigungen ](#subscribe-to-notifications-in-experience-cloud) Warnhinweise wünschen: <ul><li>Wählen Sie die Produkte aus, die Sie für Warnhinweise abonnieren möchten</li><li>Benachrichtigungstyp konfigurieren ([!UICONTROL In-App], [!UICONTROL Email] oder [Slack](#slack-notifications))</li><li>Geben Sie die Häufigkeit an, mit der Sie Benachrichtigungs-E-Mails erhalten möchten. (Nicht gesendet, unmittelbar, täglich oder wöchentlich)</li><li>Bestimmen Sie die Warnhinweispriorität. In-App-Warnhinweise werden einige Sekunden lang in der oberen rechten Ecke des Fensters angezeigt. Sie können auch festlegen, ob Warnhinweise angezeigt werden sollen, bis Sie sie schließen.</li></ul> |
| [!UICONTROL Personalisierte Empfehlungen und Angebote von Lerninhalten] | Wählen Sie aus, wo Sie [personalisierte Hilfe](personalized-learning.md) für Ihre Adobe-Produkte erhalten möchten. Diese Hilfe ist per E-Mail, innerhalb des Produkts und in den Experience League Communities verfügbar. |

## Abonnieren von Benachrichtigungen auf Experience Cloud {#notifications}

Sie können die Produkte und Kategorien auswählen, die Sie abonnieren möchten. Benachrichtigungen werden im [!UICONTROL Benachrichtigungen]-Popover (in-App), in Ihrer E-Mail oder in [Slack](#slack-notifications) angezeigt (je nach Ihren Abonnements).

E-Mail- und Slack-Benachrichtigungen sind nützlich, wenn Sie nicht beim Experience Cloud angemeldet sind.

### Abonnieren von In-App- und E-Mail-Benachrichtigungen

1. Navigieren Sie zu Experience Cloud [Einstellungen](https://experience.adobe.com/preferences).

1. Aktivieren **[!UICONTROL unter &quot;]** Benachrichtigungen“ **[!UICONTROL In-App]** oder **[!UICONTROL E-Mail]**.

   Änderungen an Benachrichtigungen werden automatisch gespeichert.

### [!DNL Slack] abonnieren {#slack}

Sie können Ihre Kontovoreinstellungen so konfigurieren, dass Experience Cloud-Benachrichtigungen an einen [!DNL Slack] gesendet werden.

**Voraussetzungen**

* Sie benötigen ein Experience Cloud-Konto.
* Sie müssen über ein [!DNL Slack] Konto verfügen. Ihr [!DNL Slack] ermöglicht die Integration von Experience Cloud mit [!DNL Slack].
* Sie müssen Teil von mindestens einem [!DNL Slack] Arbeitsbereich sein.

**So abonnieren Sie [!DNL Slack] Benachrichtigungen**

1. Navigieren Sie zu Experience Cloud [Voreinstellungen](https://experience.adobe.com/preferences).

1. Suchen Sie nach [!DNL Slack] und klicken Sie dann auf **[!UICONTROL Zu Slack hinzufügen]**.

   ![Zu Slack hinzufügen](../assets/add-to-slack.png)

   Wenn [!DNL Slack] installiert ist, wird die Anwendung geöffnet und eine Meldung über eine Berechtigungsanfrage wird angezeigt. Wenn Slack nicht installiert ist, müssen Sie [Erlaubnis anfordern](#slack-troubleshoot).

1. Klicken Sie **[!UICONTROL Zulassen]**.

1. Aktivieren **[!UICONTROL unter]** Benachrichtigungen“ [!DNL Slack] Benachrichtigungen für Ihre gewünschten Produkte und Kategorien.

   ![Slack-Benachrichtigungen](../assets/slack.png)

   Aktualisierungen der Benachrichtigungen werden automatisch gespeichert.

### Berechtigung in [!DNL Slack] anfordern (Fehlerbehebung) {#slack-troubleshoot}

Wenn [!DNL Slack] nicht installiert ist, wird die Meldung _[!UICONTROL Installationsanfrage]_ angezeigt, wenn der Slack geöffnet wird, nachdem auf **[!UICONTROL Zu Slack hinzufügen]** geklickt wurde. z. B.:

![Integration von Slack anfordern](../assets/slack-workspace.png)

**So fordern Sie Berechtigungen auf Slack an**

1. Wählen Sie in [!DNL Slack] den Arbeitsbereich aus dem Menü **[!UICONTROL Workspace]** (oben rechts).

1. Um die Genehmigung des Antrags für den [!DNL Slack] Workspace Manager anzufordern, klicken Sie auf **[!UICONTROL Senden]**.

1. Sie erhalten eine Benachrichtigung in [!DNL Slack], nachdem die Antragsanforderung genehmigt wurde.

1. Nachdem Sie [!DNL Slack] Genehmigung erhalten haben, kehren Sie zu Experience Cloud **[!UICONTROL Benachrichtigungen]** zurück und führen Sie die Schritte zum [Abonnieren von Slack](#slack-notifications) (oben beschrieben) aus.

### Was Sie in [!DNL Slack] sehen werden

Nach erfolgreicher Integration von [!DNL Slack] zeigen die [!DNL Slack]-Benachrichtigungen die folgenden Informationen an:

* Die persönliche Nachricht wird vom Anwendungsnamen _Adobe[!DNL Experience Cloud]_ empfangen.
* Die Nachricht enthält das Produktlogo für die jeweilige Anwendung, z. B. Adobe [!DNL Experience Platform], Adobe [!DNL Experience Manager] usw.
* Ein Link, um alle Benachrichtigungen auf Experience Cloud anzuzeigen.
* Ein Link zum Verwalten der Benachrichtigungseinstellungen auf Experience Cloud.

## Anzeigen [!UICONTROL Benachrichtigungen] und Ankündigungen auf Experience Cloud {#view-notifications}

In der [!DNL Experience Cloud] können Sie Benachrichtigungen, die Sie [abonniert](#notifications) sowie Ankündigungen anzeigen.

1. Klicken Sie auf das Glockensymbol in der Kopfzeile. ![Benachrichtigungen und Ankündigungen](../assets/bell-icon.png)

1. Klicken Sie **[!UICONTROL Benachrichtigungen]** oder **[!UICONTROL Ankündigungen]**.

   Hier erhalten Sie wichtige Informationen über Produkte, Ihre Zusammenarbeit mit anderen Benutzern und andere relevante Updates. Zu den Aktualisierungen gehören Produktversionen, Wartungshinweise, freigegebene Elemente und Genehmigungsanfragen.
