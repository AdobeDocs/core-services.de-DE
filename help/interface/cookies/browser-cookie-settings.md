---
description: Entfernen von Benutzern, die alle Cookies auf Desktopbrowsern und mobilen Browsern blockiert haben. Diese Datenschutzeinstellung schließt Benutzer aus, die an der Analytics-Datenerfassung Opt-out.
keywords: cookies;privacy
seo-description: Entfernen von Benutzern, die alle Cookies auf Desktopbrowsern und mobilen Browsern blockiert haben. Diese Datenschutzeinstellung schließt Benutzer aus, die an der Analytics-Datenerfassung Opt-out.
seo-title: Datenschutzeinstellungen für Browser-Cookies aktivieren
solution: Marketing Cloud,Adobe Analytics,Adobe Target,Adobe Social
title: Datenschutzeinstellungen für Browser-Cookies aktivieren
uuid: f6a56e8b-b021-49db-8eb4-6c14af0c7243
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Datenschutzeinstellungen für Browser-Cookies aktivieren{#enable-privacy-settings-for-browser-cookies}

Sie können Benutzer entfernen, die alle Cookies in Desktop- und mobilen Browsern blockiert haben. Bei dieser Funktion handelt es sich um eine Datenschutzeinstellung, bei der Benutzer ausgeschlossen werden, die an der Datenerfassung Opt-out, sodass Sie die Absicht eines Benutzers respektieren können, die Verarbeitung von Analytics zu stoppen.

**So aktivieren Sie Datenschutzeinstellungen für Browser-Cookies**

1. Navigate to **[!UICONTROL Admin Tools]** > **[!UICONTROL Report Suites]**.
1. Click **[!UICONTROL Edit Settings]** > **[!UICONTROL General]** > **[!UICONTROL Privacy Settings]**.
1. Aktivieren Sie **[!UICONTROL Datenschutzeinstellungen]** (für Desktopbrowser oder für mobile Browser).

>[!IMPORTANT]
>
>Beachten Sie, dass viele mobile Apps (z. B. der In-App-Browser für Facebook oder Twitter) als Standard-Browser für Mobilgeräte angezeigt werden können, aber nicht alle Cookies zulassen. Durch Aktivierung dieser Funktion kann ein hoher Anteil des mobilen Traffics aus Analytics-Berichten ausgeschlossen werden.

**Datenschutzeinstellungen für Browser**

Gesetze und rechtliche Hinweise haben ergeben, dass die Aktion eines Benutzers zum Blockieren von Cookies mit der Opt-out des Profilings eines Benutzers übereinstimmt. Durch Aktivierung dieser Funktion werden Daten aus Desktop-Browsern, bei denen der Benutzer den Browser so eingestellt hat, dass alle Cookies blockiert werden, aus Analytics-Berichten ausgeschlossen. Wenn Adobe den Webbrowser nicht erkennen kann, werden Daten in Analytics-Berichte aufgenommen.

Sowohl in der Beratung als auch in der Abwicklung haben Gesetzgeber weltweit erklärt, dass Cookie-Browser-Einstellungen ein Hinweis auf die Benutzerpräferenz im Opt-out der Profilerstellung sind. Insbesondere haben diese Gesetzgeber erklärt, dass die Browsereinstellung zum Blockieren von Drittanbieter-Cookies eine Abmeldeanforderung von Drittanbieter-Tracking (Site-übergreifend) ist. Das Sperren aller Cookies ist eine Abmeldeanforderung für die gesamte Verfolgung. Auch wenn serverseitige IDs (wie IP-Adressen oder Benutzeragenten) eine wünschenswerte Option sein können, die Cookie-Browsereinstellungen umgeht, werden sie von einigen Gesetzgebern als Umgehung der Benutzerauswahl Ansicht.