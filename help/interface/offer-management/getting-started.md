---
description: Eine Übersicht über die Angebotsverwaltung, den Zugriff darauf und die Erteilung von Benutzerberechtigungen.
seo-description: Eine Übersicht über die Angebotsverwaltung, den Zugriff darauf und die Erteilung von Benutzerberechtigungen.
seo-title: Erste Schritte
title: Erste Schritte
uuid: 28d83606-ee36-4bbf-b52d-bbe8b097f6d5
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 2f0c2eb70313c42da9e7ac1d75429ec768dea10d

---


# Adobe-Angebotsverwaltung {#section_07CBD4C01F4049A5A19781737D2DCD35}

[!UICONTROL Mithilfe der Angebotsverwaltung können Sie in Experience Cloud Angebote für alle Kanäle erstellen, verwalten und planen. ] Es dient als zentraler Angebotskatalog, in dem Sie mit jedem _Angebotsobjekt Berechtigungsregeln und mehrere Inhaltselemente verknüpfen können._ Sie können diese Angebote über Kanäle und Orte hinweg veröffentlichen und bei jeder Interaktion das beste Angebot für jeden Kunden bereitstellen. Diese Funktionen ermöglichen es Ihnen, Ihren Kunden das beste Angebot in einer konsistenten und abgestimmten Weise anzubieten.

Zu den Vorteilen zählen:

* Verbesserte E-Mail-Kampagnenleistung durch die Bereitstellung personalisierter Angebote in Ihren E-Mails.
* Verbesserter Arbeitsablauf: Anstatt mehrere Auslieferungen oder Kampagnen zu erstellen, können Marketingteams den Arbeitsablauf verbessern, indem sie eine einzige Auslieferung erstellen und die Angebote in verschiedenen Teilen der Vorlage variieren.
* Ermöglicht Ihnen das Erstellen, Verwalten und Genehmigen von Angeboten außerhalb des E-Mail-Kampagnen-Workflows von Adobe Campaign Standard.
* Steuern Sie, wie oft ein Angebot in E-Mail-Kampagnen und Kunden angezeigt wird.

## Zugreifen auf Angebote {#task_DEB6F6A4B6E04E15AD3E1817D700688E}

Erfahren Sie, wie Sie auf Angebotsverwaltung zugreifen.

1. Wenden Sie sich für die Bereitstellung an Adobe.

   Eine Experience Cloud-Organisation muss über eine Instanz von Campaign Standard verfügen. Adobe kann auch eine Funktion in Campaign aktivieren, mit der Sie Angebotsaktivitäten in E-Mails erstellen können.

1. Klicken Sie im Navigationsmenü der Experience Cloud auf die Lösungsauswahl und dann auf **[!UICONTROL Angebote]**.

   ![](assets/access-offers.png)

   Um auf Angebote in Campaign Standard zuzugreifen, klicken Sie in einer E-Mail-Vorlage auf das Symbol **[!UICONTROL Angebote]**.

   ![](assets/campaign-add-offer.png)

   Sobald Sie beide Elemente in der Marketing Cloud und in Ihrem Adobe Campaign-Konto sehen, wurden Sie mit den für den Einstieg erforderlichen Funktionen ausgestattet.

## Benutzer und Berechtigungen {#concept_81F0ABB07ACC49E099EDCD87AA0436E1}

Administratoren können Benutzer zur [!UICONTROL Angebotsverwaltung] in der Admin-Konsole hinzufügen. Dem neuen Benutzer wird eine E-Mail-Einladung mit Anweisungen zum Zugriff auf das Produkt gesendet. Nachdem ein Benutzer hinzugefügt wurde, können Sie seine Berechtigungen anpassen und ihm Zugriff auf verschiedene Funktionen in der gesamten [!UICONTROL Angebotsverwaltung]gewähren.

Weitere Informationen zur Verwendung der Admin-Konsole finden Sie in der Dokumentation[zur ](https://helpx.adobe.com/enterprise/help/aedash.html)HelpX Admin-Konsole.

In Campaign haben Standardbenutzer automatisch das Recht, Angebotsaktivitäten in eine E-Mail-Vorlage einzubetten.

>[!NOTE]
>
>Für Beta gibt es keine Berechtigungen. Jeder Benutzer, der zu Angeboten hinzugefügt wurde, hat vollen Zugriff auf alle Funktionen in der [!UICONTROL Angebotsverwaltung].

## Produktprofil für Angebotsverwaltung erstellen

Ein Produktprofil ist ein Satz von Berechtigungen, die kombiniert werden können, um eine Benutzerrolle innerhalb eines Produkts zu erstellen. Produktprofile müssen erstellt und anschließend Benutzern oder Gruppen zugewiesen werden.

1. Navigieren Sie zur Adobe [Admin-Konsole](https://adminconsole.adobe.com/).

1. Klicken Sie auf Ihren Prozess (z. B.**[!UICONTROL Angebote]**).

1. Klicken Sie auf der Seite [!UICONTROL Produktprofile] auf **[!UICONTROL Neues Profil]**.

1. Geben Sie einen Namen und eine Beschreibung für das Produktprofil ein und klicken Sie dann auf **[!UICONTROL Fertig]**.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

### Berechtigungen - Definitionen

Eine Beschreibung der [!UICONTROL Angebotsverwaltungsberechtigungen] , die für Produktprofile in der [!UICONTROL Admin-Konsole]verfügbar sind.

| Element | Beschreibung |
|--- |--- |
| Angebote erstellen und bearbeiten | Ermöglicht Benutzern den Zugriff auf das Erstellen und Bearbeiten von Angeboten in der [!UICONTROL Angebotsverwaltung]. Wenn ein Benutzer über diese Berechtigung verfügt, jedoch nicht über die Berechtigung zum _Genehmigen von Angeboten_ , kann er nur ein Angebot erstellen und zur Genehmigung senden. Es kann erst nach Genehmigung in einer Angebotsaktivität verwendet werden. |
| Angebote löschen | Ermöglicht Benutzern Zugriff auf das Löschen von Angeboten. |
| Angebote genehmigen | Bietet Benutzern die Möglichkeit, ein Angebot zu genehmigen. Benutzern mit dieser Berechtigung wird eine Benachrichtigung angezeigt, wenn sie sich bei der Angebotsverwaltung anmelden, wenn Angebote genehmigt werden müssen. Wenn ein Benutzer über diese Berechtigung und die Berechtigung zum _Erstellen und Bearbeiten von Angeboten_ verfügt, kann er Angebote in einem einzigen Arbeitsablauf erstellen und genehmigen. |
| Angebote archivieren | Bietet Benutzern die Möglichkeit, ein Angebot zu archivieren. |
| Erstellen von Bezeichnungen | Bietet Benutzern die Möglichkeit, Beschriftungen zu erstellen, sowohl auf der Registerkarte &quot;Bezeichnung&quot;als auch im Anzeigebereich &quot;Angebotserstellung&quot;. Ohne diese Berechtigung kann ein Benutzer beim Erstellen eines Angebots nur vordefinierte Angebote auswählen. |
| Beschriftungen bearbeiten | Ermöglicht Benutzern das Bearbeiten von Bezeichnungen auf der Registerkarte &quot;Bezeichnungen&quot;. |
| Beschriftungen löschen | Ermöglicht Benutzern das Löschen von Bezeichnungen auf der Registerkarte &quot;Bezeichnungen&quot;. |
| Erstellen von Platzierungen | Bietet Benutzern die Möglichkeit, Platzierungen auf der Registerkarte Platzierungen zu erstellen. |
| Bearbeiten von Platzierungen | Bietet Benutzern die Möglichkeit, Platzierungen auf der Registerkarte Platzierungen zu bearbeiten. |
| Platzierungen löschen | Ermöglicht dem Benutzer das Löschen von Platzierungen auf der Registerkarte &quot;Platzierungen&quot;. **** Hinweis: Nur Platzierungen, die nicht in einer Angebotstätigkeit verwendet werden, können gelöscht werden. |