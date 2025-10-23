---
title: Kontovoreinstellungen und Benachrichtigungen
description: Erfahren Sie mehr über Benutzerprofile, Kontovoreinstellungen und Produktnutzungsdaten in Experience Cloud. Abonnieren Sie Produktbenachrichtigungen für E-Mail und  [!DNL Slack] und richten Sie Produktbenachrichtigungen ein.
solution: Experience Cloud
feature: Account Preferences, Notifications, Alerts
topic: Administration
role: Admin
level: Intermediate
exl-id: 1e34c6b2-a792-41c4-adb7-583de596237f
source-git-commit: c447723f4d6c57bdccad6c4a8996693aec4a56fe
workflow-type: tm+mt
source-wordcount: '788'
ht-degree: 6%

---

# Kontovoreinstellungen und Benachrichtigungen

Um die Experience Cloud-Voreinstellungen zu finden, klicken Sie **[!UICONTROL Profile]** ![Voreinstellungen](../assets/preferences-icon-sm.png) in der Kopfzeile und dann auf **[!UICONTROL Preferences]**.

![Voreinstellungen](../assets/preferences-navigation.png){width="100" zoomable="yes"}

Auf der Seite [!UICONTROL Experience Cloud preferences] können Sie die folgenden Kontofunktionen verwalten:

| Funktion | Beschreibung |
|--- |--- |
| [!UICONTROL Profile] | Aktualisieren Sie Ihr [Adobe-Kontoprofil](https://account.adobe.com/profile). <p>Ihr Profilbild und Ihr Name werden angezeigt, wenn Sie sich bei Adobe.com, Adobe-Produkten und -Services und auf öffentlich zugänglichen Sites wie [!DNL Behance] anmelden. |
| [!UICONTROL General] | Wählen Sie eine [Organisation](../administration/organizations.md) aus.<p>Diese Organisation wird standardmäßig bei der Anmeldung bei Experience Cloud verwendet. |
| [!UICONTROL Product usage data] | Sie können steuern, welche Produktnutzungsdaten mit Adobe freigegeben werden, wenn Sie Experience Cloud-Programme verwenden. Hierbei handelt es sich um Daten darüber, wie Sie unsere Produkte verwenden, nicht um die Inhalte oder Daten Ihres Unternehmens selbst. Adobe verwendet diese Informationen, um Sie bei der Verbesserung unserer Produkte zu unterstützen, Ihnen einen erweiterten produktinternen Support bereitzustellen und Ihre Erfahrungen und Mitteilungen von uns zu personalisieren. <p>Weitere Informationen finden Sie [Produktnutzungsdaten](#product-usage-data) (auf dieser Seite). |
| [!UICONTROL Notifications] | Konfigurieren Sie, wie und wann Sie Produkt[Benachrichtigungen &#x200B;](#subscribe-to-notifications-in-experience-cloud) Warnhinweise wünschen: <ul><li>Wählen Sie die Produkte aus, die Sie für Warnhinweise abonnieren möchten</li><li>Benachrichtigungstyp konfigurieren ([!UICONTROL in-app], [!UICONTROL email] oder [Slack](#slack-notifications))</li><li>Geben Sie die Häufigkeit an, mit der Sie Benachrichtigungs-E-Mails erhalten möchten. (Nicht gesendet, unmittelbar, täglich oder wöchentlich)</li><li>Bestimmen Sie die Warnhinweispriorität. In-App-Warnhinweise werden einige Sekunden lang in der oberen rechten Ecke des Fensters angezeigt. Sie können auch festlegen, ob Warnhinweise angezeigt werden sollen, bis Sie sie schließen.</li></ul> |

## [!UICONTROL Product usage data]

Produktverwendungsdaten, die Sie für Adobe freigeben, enthalten die folgenden Arten von Informationen darüber, wie Sie Adobe-Programme verwenden und mit ihnen interagieren:

* Browser- und Geräteinformationen wie Gerätemodell und Betriebssystem, Software- und Hardwareinformationen, Browser- und Geräteeinstellungen, eindeutige Kennungen (wie IP-Adresse, Cookie-ID oder Geräte-ID), installierter Arbeitsspeicher, Spracheinstellungen und Bildschirmauflösung;
* Interaktion mit Adobe Experience Cloud-Programmen, einschließlich der von Ihnen verwendeten Funktionen und der von Ihnen ausgewählten Optionen;
* Adobe-Produktinformationen wie Versionsnummer;
* Informationen über Ihre Inhalte und Dokumente, wie z. B. die Anzahl der Seiten und eindeutige Kennungen, aber nicht den Inhalt selbst;
* Informationen zur Inhaltsnutzung, wie oft Sie auf Inhalte zugreifen und wie Sie mit Ihren Inhalten in der App interagieren;
* Absturz- und Fehlerprotokolle.

Adobe verwendet diese Informationen, um Sie bei der Verbesserung unserer Produkte zu unterstützen, Ihnen sowohl im Produkt als auch über die Kundenunterstützung Unterstützung zu bieten und Ihre Erfahrungen und Mitteilungen von uns zu personalisieren. Weitere Informationen über [personalisierte Erlebnisse](personalized-learning.md).

## Abonnieren von Benachrichtigungen in Experience Cloud

Sie können die Produkte und Kategorien auswählen, die Sie abonnieren möchten. Benachrichtigungen werden im [!UICONTROL Notifications]-Popover (in-App), in Ihrer E-Mail oder in [Slack](#slack-notifications) angezeigt (je nach Ihren Abonnements).

E-Mail- und Slack-Benachrichtigungen sind nützlich in Situationen, in denen Sie nicht bei Experience Cloud angemeldet sind.

### Abonnieren von In-App- und E-Mail-Benachrichtigungen

1. Navigieren Sie zu Experience Cloud [Einstellungen](https://experience.adobe.com/preferences).

1. Aktivieren Sie unter **[!UICONTROL Notifications]** die Option **[!UICONTROL In-app]** oder **[!UICONTROL Email]**.

   Änderungen an Benachrichtigungen werden automatisch gespeichert.

### [!DNL Slack] abonnieren

Sie können Ihre Kontovoreinstellungen so konfigurieren, dass Experience Cloud-Benachrichtigungen an einen [!DNL Slack] gesendet werden.

**Voraussetzungen**

* Sie benötigen ein Experience Cloud-Konto.
* Sie müssen über ein [!DNL Slack] Konto verfügen. Ihr [!DNL Slack] ermöglicht die Integration von Experience Cloud mit [!DNL Slack].
* Sie müssen Teil von mindestens einem [!DNL Slack] Arbeitsbereich sein.

**So abonnieren Sie [!DNL Slack] Benachrichtigungen**

1. Navigieren Sie zu Experience Cloud [Voreinstellungen](https://experience.adobe.com/preferences).

1. Suchen Sie nach [!DNL Slack] und klicken Sie dann auf **[!UICONTROL Add to Slack]**.

   ![Zu Slack hinzufügen](../assets/add-to-slack.png)

   Wenn [!DNL Slack] installiert ist, wird die Anwendung geöffnet und eine Meldung über eine Berechtigungsanfrage wird angezeigt. Wenn Slack nicht installiert ist, müssen Sie [Berechtigung anfordern](#slack-troubleshoot).

1. Klicken Sie auf **[!UICONTROL Allow]**.

1. Aktivieren Sie unter **[!UICONTROL Notifications]** die Option [!DNL Slack] Benachrichtigungen für Ihre gewünschten Produkte und Kategorien.

   ![Slack-Benachrichtigungen](../assets/slack.png)

   Aktualisierungen der Benachrichtigungen werden automatisch gespeichert.

### Berechtigung in [!DNL Slack] anfordern (Fehlerbehebung)

Wenn [!DNL Slack] nicht installiert ist, wird beim Öffnen von Slack nach dem Klicken auf _[!UICONTROL Request to install]_&#x200B;eine **[!UICONTROL Add to Slack]**&#x200B;angezeigt. Beispiel:

![Slack-Integration anfordern](../assets/slack-workspace.png)

**So fordern Sie Berechtigungen in Slack an**

1. Wählen Sie in [!DNL Slack] den Arbeitsbereich aus dem Menü **[!UICONTROL Workspace]** (obere rechte Ecke).

1. Um die Genehmigung des Programms für den [!DNL Slack] Workspace Manager anzufordern, klicken Sie auf **[!UICONTROL Submit]**.

1. Sie erhalten eine Benachrichtigung in [!DNL Slack], nachdem die Antragsanforderung genehmigt wurde.

1. Nachdem Sie [!DNL Slack] Genehmigung erhalten haben, kehren Sie zu Experience Cloud **[!UICONTROL Notifications]** zurück und führen Sie die Schritte [Abonnieren von Slack](#slack-notifications) (oben beschrieben) aus.

### Was Sie in [!DNL Slack] sehen werden

Nach erfolgreicher Integration von [!DNL Slack] zeigen die [!DNL Slack]-Benachrichtigungen die folgenden Informationen an:

* Die persönliche Nachricht wird vom App-Namen _Adobe[!DNL Experience Cloud]_ empfangen.
* Die Nachricht enthält das Produktlogo für die jeweilige Anwendung, z. B. Adobe [!DNL Experience Platform], Adobe [!DNL Experience Manager] usw.
* Ein Link, um alle Benachrichtigungen auf Experience Cloud anzuzeigen.
* Ein Link zum Verwalten der Benachrichtigungseinstellungen auf Experience Cloud.

## Anzeigen von [!UICONTROL notifications] und Ankündigungen in Experience Cloud

In der [!DNL Experience Cloud] können Sie Benachrichtigungen, die Sie [abonniert](#notifications) sowie Ankündigungen anzeigen.

1. Klicken Sie auf das Glockensymbol in der Kopfzeile. ![Benachrichtigungen und Ankündigungen](../assets/bell-icon.png)

1. Klicken Sie auf **[!UICONTROL Notifications]** oder **[!UICONTROL Announcements]**.

   Hier erhalten Sie wichtige Informationen über Produkte, Ihre Zusammenarbeit mit anderen Benutzern und andere relevante Updates. Zu den Aktualisierungen gehören Produktversionen, Wartungshinweise, freigegebene Elemente und Genehmigungsanfragen.
