---
description: Eine Übersicht über die Verwaltung von Angeboten, den Zugriff darauf und das Gewähren von Benutzerberechtigungen.
seo-description: Eine Übersicht über die Verwaltung von Angeboten, den Zugriff darauf und das Gewähren von Benutzerberechtigungen.
seo-title: Erste Schritte
title: Erste Schritte
uuid: 28d83606-ee36-4bbf-b52d-bbe8b097f6d5
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e

---


# Adobe Angebot Management {#section_07CBD4C01F4049A5A19781737D2DCD35}

[!UICONTROL Angebot Management] bietet Angebot-Erstellung, -Verwaltung und -Entscheidungsfindung für alle Kanal in der Experience Cloud. Es dient als zentraler Angebotskatalog, in dem Sie Eignungsregeln und mehrere Inhaltselemente mit jedem Angebot- _Objekt verknüpfen können._ Sie können diese Angebot über Kanal und Orte hinweg veröffentlichen und bei jeder Interaktion das beste Angebot für jeden Kunden bereitstellen. Diese Funktionen ermöglichen es Ihnen, Ihren Kunden stets das beste Angebot in einer konsistenten und konsistenten Form und in koordinierter Form bereitzustellen.

Zu den Vorteilen zählen:

* Verbesserte E-Mail-Kampagne durch die Bereitstellung personalisierter Angebot in Ihren E-Mails.
* Verbesserter Arbeitsablauf: Anstatt mehrere Versand oder Kampagnen zu erstellen, können Marketingteams den Arbeitsablauf verbessern, indem sie einen einzigen Versand erstellen und die Angebot in verschiedenen Vorlagenteilen variieren.
* Ermöglicht das Erstellen, Verwalten und Genehmigen von Angeboten außerhalb des E-Mail-Kampagnen-Workflows von Adobe Campaign Standard.
* Steuern Sie, wie oft ein Angebot in E-Mail-Kampagnen und Kunden angezeigt wird.

## Zugreifen auf Angebot {#task_DEB6F6A4B6E04E15AD3E1817D700688E}

Erfahren Sie, wie Sie auf Angebot-Management zugreifen können.

1. Wenden Sie sich für die Bereitstellung an Adobe.

   Eine Experience Cloud-Organisation muss über eine Instanz von Campaign Standard verfügen. Adobe kann auch eine Funktion in der Kampagne aktivieren, mit der Sie Angebot-Aktivitäten in E-Mails erstellen können.

1. Klicken Sie im Experience Cloud-Navigationsmenü auf die Lösungsauswahl und dann auf **[!UICONTROL Angebot]**.

   ![](assets/access-offers.png)

   Um auf Angebot in Campaign Standard zuzugreifen, klicken Sie auf das Symbol &quot; **[!UICONTROL Angebot]** &quot;in einer E-Mail-Vorlage.

   ![](assets/campaign-add-offer.png)

   Sobald Sie beide Elemente in der Marketing Cloud und in Ihrem Adobe Campaign-Konto sehen, wurden Sie mit den für den Einstieg erforderlichen Funktionen eingerichtet.

## Users and Permissions {#concept_81F0ABB07ACC49E099EDCD87AA0436E1}

Administratoren können Benutzer zur [!UICONTROL Angebot-Verwaltung] in der Admin-Konsole hinzufügen. Dem neuen Benutzer wird eine E-Mail-Einladung mit Anweisungen zum Zugriff auf das Produkt gesendet. Nachdem ein Benutzer hinzugefügt wurde, können Sie seine Berechtigungen anpassen und ihm Zugriff auf verschiedene Funktionen in der gesamten [!UICONTROL Angebot-Verwaltung]gewähren.

Weitere Informationen zur Verwendung der Admin-Konsole finden Sie in der Dokumentation [zur](https://helpx.adobe.com/enterprise/help/aedash.html)HelpX Admin-Konsole.

In Kampagne haben Standardbenutzer automatisch das Recht, Angebot-Aktivitäten in eine E-Mail-Vorlage einzubetten.

>[!NOTE]
>
>Für Beta gibt es keine Berechtigungen. Jeder Benutzer, der zu Angeboten hinzugefügt wurde, hat vollen Zugriff auf alle Funktionen in der [!UICONTROL Angebot-Verwaltung].

## Profil für Angebot-Management erstellen

Ein Profil ist ein Satz von Berechtigungen, die kombiniert werden können, um eine Benutzerrolle innerhalb eines Produkts zu erstellen. Produktgruppen müssen erstellt und Profil oder Gruppen zugewiesen werden.

1. Navigieren Sie zur Adobe [Admin-Konsole](https://adminconsole.adobe.com/).

1. Klicken Sie auf Ihren Prozess (z. B.**[!UICONTROL Angebote]**).

1. Klicken Sie auf der Seite [!UICONTROL Product Profils] auf **[!UICONTROL New Profil]**.

1. Geben Sie einen Namen und eine Beschreibung für das Profil ein und klicken Sie dann auf **[!UICONTROL Fertig]**.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

### Berechtigungen - Definitionen

Eine Beschreibung der [!UICONTROL Angebot-Management] -Berechtigungen, die für Produkt-Profil in der [!UICONTROL Admin-Konsole]verfügbar sind.

| Element | Beschreibung |
|--- |--- |
| Angebote erstellen und bearbeiten | Ermöglicht Benutzern Zugriff auf das Erstellen und Bearbeiten von Angeboten in der [!UICONTROL Angebot-Verwaltung]. Wenn ein Benutzer über diese Berechtigung, jedoch nicht über die Berechtigung &quot;Angebot _genehmigen_ &quot;verfügt, kann er nur ein Angebot erstellen und zur Genehmigung senden. Es kann erst nach Genehmigung in einer Angebot-Aktivität verwendet werden. |
| Angebote löschen | Ermöglicht Benutzern Zugriff auf das Löschen von Angeboten. |
| Validierung von Angeboten | Gibt Benutzern die Möglichkeit, ein Angebot zu genehmigen. Benutzern mit dieser Berechtigung wird beim Anmelden bei Angebot Management eine Benachrichtigung angezeigt, wenn Angebote genehmigt werden müssen. Wenn ein Benutzer sowohl über diese Berechtigung als auch über die Berechtigung zum _Erstellen und Bearbeiten von Angeboten_ verfügt, kann er Angebot in einem einzigen Arbeitsablauf erstellen und genehmigen. |
| Angebote archivieren | Bietet Benutzern die Möglichkeit, ein Angebot zu archivieren. |
| Erstellen von Bezeichnungen | Ermöglicht Benutzern das Erstellen von Beschriftungen, sowohl auf der Registerkarte &quot;Bezeichnung&quot;als auch im Anzeigebereich &quot;Angebot-Erstellung&quot;. Ohne diese Berechtigung kann ein Benutzer beim Erstellen eines Angebots nur vordefinierte Angebot auswählen. |
| Bezeichnungen bearbeiten | Ermöglicht Benutzern das Bearbeiten von Bezeichnungen auf der Registerkarte &quot;Bezeichnungen&quot;. |
| Beschriftungen löschen | Ermöglicht dem Benutzer das Löschen von Bezeichnungen auf der Registerkarte &quot;Bezeichnungen&quot;. |
| Erstellen von Platzierungen | Bietet Benutzern die Möglichkeit, Platzierungen auf der Registerkarte Platzierungen zu erstellen. |
| Bearbeiten von Platzierungen | Bietet Benutzern die Möglichkeit, Platzierungen auf der Registerkarte Platzierungen zu bearbeiten. |
| Platzierungen löschen | Ermöglicht dem Benutzer das Löschen von Platzierungen auf der Registerkarte &quot;Platzierungen&quot;. **Hinweis:** Nur Platzierungen, die nicht in einer Angebot-Aktivität verwendet werden, können gelöscht werden. |