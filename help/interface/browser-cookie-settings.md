---
description: Erfahren Sie, wie Sie die Datenschutzeinstellungen für Browser-Cookies aktivieren. Sie können Benutzer entfernen, die alle Cookies auf Desktopbrowsern und mobilen Browsern blockiert haben.
keywords: Cookies, Datenschutz
solution: Experience Cloud, Analytics, Target, Social
title: 'Datenschutzeinstellungen für Browser-Cookies '
uuid: f6a56e8b-b021-49db-8eb4-6c14af0c7243
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 5d852e0e-4004-4f94-a6f7-3a14a96cd42f
source-git-commit: 1fb1abc7311573f976f7e6b6ae67f60ada10a3e7
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 97%

---

# Datenschutzeinstellungen für Browser-Cookies aktivieren{#enable-privacy-settings-for-browser-cookies}

Sie können Benutzer entfernen, die alle Cookies auf Desktopbrowsern und mobilen Browsern blockiert haben. Bei dieser Funktion handelt es sich um eine Datenschutzeinstellung, bei der Benutzer ausgeschlossen werden, die die Datenerfassung abwählen. Dadurch können Sie die Absicht eines Benutzers respektieren, die Verarbeitung mit Analytics zu stoppen.

**Aktivieren der Datenschutzeinstellungen für Browser-Cookies**

1. Navigieren Sie zu **[!UICONTROL Admin Tools]** > **[!UICONTROL Report Suites]**.
1. Gehen Sie zu **[!UICONTROL Einstellungen bearbeiten]** > **[!UICONTROL Allgemein]** > **[!UICONTROL Datenschutzeinstellungen]**.
1. Aktivieren Sie **[!UICONTROL Datenschutzeinstellungen]** (für Desktopbrowser oder für mobile Browser).

>[!IMPORTANT]
>
>Beachten Sie, dass viele Mobile Apps (wie der In-App-Browser für Facebook oder Twitter) als mobile Standard-Browser angesehen werden können, jedoch nicht alle Cookies zulassen. Durch die Aktivierung dieser Funktion kann ein hoher Anteil des mobilen Traffics aus Analytics-Berichten ausgeschlossen werden.

**Über Datenschutzeinstellungen für Browser**

Gesetze und rechtliche Hinweise haben ergeben, dass die Aktion eines Benutzers zum Blockieren von Cookies mit dem Abwählen der Profilierung eines Benutzers übereinstimmt. Durch die Aktivierung dieser Funktion werden gesammelte Daten aus Desktop-Browsern, bei denen der Benutzer den Browser so eingestellt hat, dass alle Cookies blockiert werden, aus Analytics-Berichten ausgeschlossen. Wenn Adobe den Webbrowser nicht erkennen kann, werden Daten in [!DNL Analytics]-Berichte aufgenommen.

Sowohl in der Beratung als auch in der Abwicklung haben Gesetzgeber weltweit erklärt, dass Cookie-Browsereinstellungen ein Hinweis darauf sind, ob ein Benutzer die Profilierung abwählen möchte. Insbesondere haben diese Gesetzgeber erklärt, dass die Browsereinstellung zum Blockieren von Drittanbieter-Cookies eine Abwahlanforderung des Drittanbieter-Trackings (Site-übergreifend) darstellt. Das Blockieren aller Cookies ist eine Abwahlanforderung für das gesamte Tracking. Auch wenn serverseitige Kennungen (wie IP-Adressen oder Benutzeragent) eine wünschenswerte Option zur Umgehung der Cookie-Einstellungen des Browsers sein mögen, werden sie von einigen Gesetzgebern als Missachtung der Benutzerauswahl angesehen.
