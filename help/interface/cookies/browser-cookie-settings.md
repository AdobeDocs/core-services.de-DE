---
description: Erfahren Sie, wie Sie die Datenschutzeinstellungen für Browser-Cookies aktivieren. Sie können Benutzer entfernen, die alle Cookies auf Desktopbrowsern und mobilen Browsern blockiert haben.
keywords: Cookies, Datenschutz
solution: Experience Cloud, Analytics, Target, Social
title: 'Datenschutzeinstellungen für Browser-Cookies '
uuid: f6a56e8b-b021-49db-8eb4-6c14af0c7243
feature: Cookies
topic: Administration
role: Administrator
level: Experienced
exl-id: 5d852e0e-4004-4f94-a6f7-3a14a96cd42f
source-git-commit: f720e37b693da2c657cb1efab45620c60bfa81a4
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 60%

---

# Datenschutzeinstellungen für Browser-Cookies aktivieren {#enable-privacy-settings-for-browser-cookies}

Sie können Benutzer entfernen, die alle Cookies auf Desktopbrowsern und mobilen Browsern blockiert haben. Bei dieser Funktion handelt es sich um eine Datenschutzeinstellung, bei der Benutzer ausgeschlossen werden, die sich von der Datenerfassung abmelden. So können Sie die Absicht eines Benutzers respektieren, die Analytics-Verarbeitung zu stoppen.

**Aktivieren der Datenschutzeinstellungen für Browser-Cookies**

1. Navigieren Sie zu **[!UICONTROL Admin Tools]** > **[!UICONTROL Report Suites]**.
1. Klicken Sie auf **[!UICONTROL Einstellungen bearbeiten]** > **[!UICONTROL Allgemein]** > **[!UICONTROL Datenschutzeinstellungen]**.
1. Aktivieren Sie **[!UICONTROL Datenschutzeinstellungen]** (für Desktopbrowser oder für mobile Browser).

>[!IMPORTANT]
>
>Viele mobile Apps (wie der In-App-Browser für Facebook oder Twitter) können als standardmäßiger mobiler Browser angezeigt werden, lassen jedoch nicht alle Cookies zu. Durch die Aktivierung dieser Funktion kann ein hoher Anteil des mobilen Traffics aus Analytics-Berichten ausgeschlossen werden.

**Über Datenschutzeinstellungen für Browser**

Gesetze und rechtliche Hinweise haben ergeben, dass die Aktion eines Benutzers zum Blockieren von Cookies mit dem Abwählen der Profilierung eines Benutzers übereinstimmt. Durch Aktivierung dieser Funktion werden Daten, die von Desktop-Browsern erfasst wurden, bei denen der Benutzer den Browser so eingestellt hat, dass alle Cookies blockiert werden, aus Analytics-Berichten ausgeschlossen. Wenn die Adobe den Webbrowser nicht erkennen kann, sind die Daten in [!DNL Analytics] -Berichten enthalten.

Sowohl in der Beratung als auch in der Abwicklung haben Gesetzgeber weltweit erklärt, dass Cookie-Browsereinstellungen ein Hinweis darauf sind, ob ein Benutzer die Profilierung abwählen möchte. Insbesondere haben diese Gesetzgeber erklärt, dass die Browsereinstellung zum Blockieren von Drittanbieter-Cookies eine Abwahlanforderung des Drittanbieter-Trackings (Site-übergreifend) darstellt. Das Blockieren aller Cookies ist eine Abwahlanforderung für das gesamte Tracking. Auch wenn serverseitige IDs (wie IP-Adressen oder Benutzeragenten) eine wünschenswerte Option sein können, die Cookie-Browsereinstellungen umgeht, sehen einige Gesetzgeber sie als Umgehung der Benutzerauswahl.
