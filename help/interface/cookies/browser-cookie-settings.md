---
description: Entfernen von Benutzern, die alle Cookies auf Desktopbrowsern und mobilen Browsern blockiert haben.
keywords: Cookies, Datenschutz
seo-description: Entfernen von Benutzern, die alle Cookies auf Desktopbrowsern und mobilen Browsern blockiert haben.
seo-title: Datenschutzeinstellungen für Browser-Cookies aktivieren
solution: Experience Cloud,Analytics,Target,Social
title: Datenschutzeinstellungen für Browser-Cookies aktivieren
uuid: f6a56e8b-b021-49db-8eb4-6c14af0c7243
translation-type: tm+mt
source-git-commit: 012283d79bda42f9dabb20b25903927b075f6d54

---


# Datenschutzeinstellungen für Browser-Cookies aktivieren{#enable-privacy-settings-for-browser-cookies}

Entfernen von Benutzern, die alle Cookies auf Desktopbrowsern und mobilen Browsern blockiert haben.

Mit dieser Einstellung können Sie die Intention von Benutzern respektieren, von einer Verarbeitung in Analytics ausgenommen zu werden, wenn diese alle Cookies in den Cookie-Einstellungen ihres Browsers blockiert haben.

1. Navigieren Sie zu **[!UICONTROL Admin Tools]** &gt; **[!UICONTROL Report Suites]**.
1. Klicken Sie auf **[!UICONTROL Einstellungen bearbeiten]** &gt; **[!UICONTROL Allgemein]** &gt; **[!UICONTROL Datenschutzeinstellungen]**.
1. Aktivieren Sie **[!UICONTROL Datenschutzeinstellungen]** (für Desktopbrowser oder für mobile Browser).

   Ist diese Funktion aktiviert, werden Daten, die über Desktopbrowser mit vollständig blockierten Cookies erfasst werden, aus den Analytics-Berichten ausgeschlossen. Wenn Adobe den Browser nicht erkennt, werden die Daten in die Analytics-Berichte einbezogen.

>[!IMPORTANT]
>
>Beachten Sie, dass viele mobile Apps (wie der In-App-Browser für Facebook oder Twitter) als mobile Standardbrowser angesehen werden können, jedoch nicht alle Cookies zulassen. Wenn Sie diese Funktion aktivieren, wird möglicherweise ein erheblicher Anteil des mobilen Datenverkehrs aus den Analytics-Berichten ausgeschlossen.

**Informationen über Datenschutzeinstellungen in Browsern**

In Gesetzen und behördlichen Auflagen wird darauf hingewiesen, dass das Blockieren von Cookies durch den Benutzer einer Anfrage zum Ausschluss von der Profilerstellung gleichkommt. Ist diese Funktion aktiviert, werden Daten, die über Desktopbrowser mit vollständig blockierten Cookies erfasst werden, aus den Analytics-Berichten ausgeschlossen. Wenn Adobe den Webbrowser nicht erkennt, werden die Daten in die Analytics-Berichte einbezogen.

Gesetzgeber auf der ganzen Welt haben (sowohl in Auflagen als auch in Vergleichen) erklärt, dass entsprechende Cookie-Browsereinstellungen eine Aufforderung seitens der Benutzer darstellen, von der Profilerstellung ausgenommen zu werden. Insbesondere haben diese Gesetzgeber erklärt, dass die Browsereinstellung zum Blockieren von Drittanbieter-Cookies eine Aufforderung darstellt, vom (siteübergreifenden) Drittanbieter-Tracking ausgenommen zu werden, und dass das Blockieren aller Cookies eine Aufforderung darstellt, von jeglichem Tracking ausgenommen zu werden. Zwar können serverseitige Kennungen (wie IP-Adresse oder Benutzeragent) als erstrebenswerte Alternative zur Umgehung von Cookie-Browsereinstellungen erscheinen, doch werden diese von manchen Gesetzgebern als Umgehung der vom Benutzer geäußerten Absicht gedeutet.