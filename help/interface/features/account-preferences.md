---
title: Kontovoreinstellungen und Benachrichtigungen
description: Informationen zu Benutzerprofilen und Kontovoreinstellungen finden Sie unter Experience Cloud. Abonnieren Sie Produktbenachrichtigungen für E-Mails und  [!DNL Slack] und richten Sie Produktwarnungen ein.
solution: Experience Cloud
feature: Account Preferences, Notifications, Alerts
topic: Administration
role: Admin
level: Intermediate
exl-id: 1e34c6b2-a792-41c4-adb7-583de596237f
source-git-commit: e523471b6dd67cf8213ead3208347fd3aa32a164
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 8%

---

# Kontovoreinstellungen und Benachrichtigungen {#preferences}

Um Experience Cloud-Voreinstellungen zu finden, klicken Sie in der Kopfzeile auf **[!UICONTROL Profil]** ![Voreinstellungen](../assets/preferences-icon-sm.png) und dann auf **[!UICONTROL Voreinstellungen]**.

![Voreinstellungen](../assets/preferences-navigation.png){width="100" zoomable="yes"}

Auf der Seite [!UICONTROL Experience Cloud-Voreinstellungen] können Sie die folgenden Kontofunktionen verwalten:

| Funktion | Beschreibung |
|--- |--- |
| Profil | Aktualisieren Sie Ihr [Adobe-Kontoprofil](https://account.adobe.com/profile). <p>Ihr Profilfoto und Ihr Profilname werden angezeigt, wenn Sie sich bei Adobe.com, Adobe-Produkten und -Diensten und auf öffentlich zugänglichen Sites wie [!DNL Behance] anmelden. |
| Allgemein | Wählen Sie eine [Organisation](../administration/organizations.md) aus.<p>Diese Organisation wird standardmäßig bei der Anmeldung bei Experience Cloud verwendet. |
| [!UICONTROL Erfassung von Produktdaten] | Wählen Sie aus, welche Technologien Adobe verwenden kann, um Daten darüber zu sammeln, wie Sie Ihre Adobe-Produkte verwenden. |
| Benachrichtigungen | Konfigurieren Sie, wie und wann Sie Produkt-[Benachrichtigungen](#subscribe-to-notifications-in-experience-cloud) und Warnhinweise benötigen: <ul><li>Wählen Sie die Produkte aus, für die Sie Warnhinweise abonnieren möchten</li><li>Konfigurieren des Benachrichtigungstyps ([!UICONTROL in-app], [!UICONTROL email] oder [Slack](#slack-notifications))</li><li>Geben Sie die Häufigkeit an, mit der Sie Benachrichtigungs-E-Mails erhalten möchten. (Nicht gesendet, unmittelbar, täglich oder wöchentlich)</li><li>Bestimmen Sie die Priorität des Warnhinweises. In-App-Warnhinweise werden einige Sekunden oben rechts in Ihrem Fenster angezeigt. Sie können auch angeben, ob Warnhinweise angezeigt werden sollen, bis Sie sie schließen.</li></ul> |
| [!UICONTROL Personalisierte Empfehlungen und Angebote von Lerninhalten] | Wählen Sie aus, wo Sie [personalisierte Hilfe](personalized-learning.md) für Ihre Adobe-Produkte erhalten möchten. Diese Hilfe ist per E-Mail, im Produkt und in den Experience League Communities verfügbar. |

## Abonnieren von Benachrichtigungen in Experience Cloud {#notifications}

Sie können die Produkte und Kategorien auswählen, die Sie abonnieren möchten. Benachrichtigungen werden im Popup-Fenster [!UICONTROL Benachrichtigungen] (in der App), in Ihrer E-Mail oder in [Slack](#slack-notifications) (je nach Ihren Abonnements) angezeigt.

E-Mail- und Slack-Benachrichtigungen eignen sich für Situationen, in denen Sie nicht bei Experience Cloud angemeldet sind.

### In-App- und E-Mail-Benachrichtigungen abonnieren

1. Navigieren Sie zu Experience Cloud [Voreinstellungen](https://experience.adobe.com/preferences).

1. Aktivieren Sie unter **[!UICONTROL Benachrichtigungen]** die Option **[!UICONTROL In-App]** oder **[!UICONTROL E-Mail]**.

   Änderungen an Benachrichtigungen werden automatisch gespeichert.

### Anmelden für [!DNL Slack] -Benachrichtigungen {#slack}

Sie können Ihre Kontovoreinstellungen so konfigurieren, dass Experience Cloud-Benachrichtigungen an einen [!DNL Slack] -Kanal gesendet werden.

**Voraussetzungen**

* Sie müssen über ein Experience Cloud-Konto verfügen.
* Sie müssen über ein [!DNL Slack] -Konto verfügen. Ihr [!DNL Slack] -Administrator aktiviert die Experience Cloud-Integration mit [!DNL Slack].
* Sie müssen mindestens einem [!DNL Slack] -Arbeitsbereich angehören.

**Abonnieren von [!DNL Slack] Benachrichtigungen**

1. Navigieren Sie zu Experience Cloud [Voreinstellungen](https://experience.adobe.com/preferences).

1. Suchen Sie [!DNL Slack] und klicken Sie dann auf **[!UICONTROL Zu Slack hinzufügen]**.

   ![Zu Slack hinzufügen](../assets/add-to-slack.png)

   Wenn [!DNL Slack] installiert ist, wird die Anwendung geöffnet und eine Meldung mit einer Berechtigungsanforderung angezeigt. Wenn Slack nicht installiert ist, müssen Sie [die Berechtigung anfordern](#slack-troubleshoot).

1. Klicken Sie auf **[!UICONTROL Allow]**.

1. Aktivieren Sie unter **[!UICONTROL Benachrichtigungen]** die Option [!DNL Slack] Benachrichtigungen für Ihre gewünschten Produkte und Kategorien.

   ![Slack notifications](../assets/slack.png)

   Aktualisierungen der Benachrichtigungen werden automatisch gespeichert.

### Anforderungsberechtigung in [!DNL Slack] (Fehlerbehebung) {#slack-troubleshoot}

Wenn [!DNL Slack] nicht installiert ist, wird beim Öffnen der Slack nach dem Klicken auf **[!UICONTROL Zu Slack hinzufügen]** die Meldung _[!UICONTROL Installationsanfrage]_ angezeigt. Zum Beispiel:

![Slack-Integration anfordern](../assets/slack-workspace.png)

**So fordern Sie Berechtigungen in Slack** an

1. Wählen Sie in [!DNL Slack] den Arbeitsbereich aus dem Menü **[!UICONTROL Workspace]** (obere rechte Ecke) aus.

1. Um die Genehmigung des Antrags für den Arbeitsbereichsmanager [!DNL Slack] anzufordern, klicken Sie auf **[!UICONTROL Senden]**.

1. Sie erhalten eine Benachrichtigung in [!DNL Slack] , nachdem die Anwendungsanforderung genehmigt wurde.

1. Nachdem Sie die [!DNL Slack] -Genehmigung erhalten haben, kehren Sie zu Experience Cloud **[!UICONTROL Benachrichtigungen]** zurück und führen Sie die Schritte zum [Abonnieren von Slack](#slack-notifications) durch (siehe oben).

### Was Sie in [!DNL Slack] sehen werden

Nach erfolgreicher Integration von [!DNL Slack] zeigen die [!DNL Slack] -Benachrichtigungen die folgenden Informationen an:

* Die persönliche Nachricht wird vom Anwendungsnamen _Adobe[!DNL Experience Cloud]_ empfangen.
* Die Nachricht enthält das Produktlogo für die jeweilige Anwendung, z. B. Adobe [!DNL Experience Platform], Adobe [!DNL Experience Manager] usw.
* Ein Link zum Anzeigen aller Benachrichtigungen auf dem Experience Cloud.
* Ein Link zur Verwaltung von Benachrichtigungseinstellungen auf dem Experience Cloud.

## Anzeigen von [!UICONTROL Benachrichtigungen] und Mitteilungen in Experience Cloud {#view-notifications}

In der Kopfzeile [!DNL Experience Cloud] können Sie Benachrichtigungen anzeigen, für die Sie [angemeldet](#notifications) haben, sowie Ankündigungen anzeigen.

1. Klicken Sie auf das Glockensymbol in der Kopfzeile. ![Benachrichtigungen und Ankündigungen](../assets/bell-icon.png)

1. Klicken Sie auf **[!UICONTROL Benachrichtigungen]** oder **[!UICONTROL Mitteilungen]**.

   An diesem Ort erhalten Sie wichtige Informationen zu Produkten, Ihre Zusammenarbeit mit anderen Benutzern und andere relevante Updates. Zu den Aktualisierungen gehören Produktversionen, Wartungshinweise, freigegebene Elemente und Genehmigungsanfragen.
