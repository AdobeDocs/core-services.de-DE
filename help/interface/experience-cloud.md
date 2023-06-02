---
description: Erfahren Sie mehr über zentrale Oberflächenkomponenten für Experience Cloud. Diese Hilfe enthält Benutzer- und Produktverwaltung in der Admin Console, die Aktivierung von Programmen für Experience Cloud-Services sowie Hilfe zur Zielgruppenbibliothek, zu Kundenattributen, Experience Cloud-Elementen und mehr.
solution: Experience Cloud
title: Hilfe und Dokumentation zur Experience Cloud-Oberfläche
uuid: aec6f689-e617-4876-ae6c-e961cfcb991a
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: aedad5cb-3282-4a97-8e7e-6d65f7b75ba9
source-git-commit: 657d7e665ac3d20b80bdb26db0e3e62e421218bf
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 97%

---

# Handbuch für Komponenten der Experience Cloud Zentrale Schnittstelle

[Experience Cloud](https://experience.adobe.com) umfasst die Digital-Marketing-Programme, -Produkte und -Services von Adobe. Über die intuitive Benutzeroberfläche können Sie schnell auf Ihre Cloud-Programme, Produktfunktionen und Services zugreifen.

![Experience Cloud](assets/landing.png)

In der Kopfzeile von Experience Cloud haben Sie folgende Möglichkeiten:

* Greifen Sie auf Ihre Programme und Services zu
* Suchen Sie im Hilfemenü nach Produktdokumentation, Tutorials und Community-Posts. Ergebnisse in Experience League anzeigen.
* Globale Suche nach Geschäftsobjekten mithilfe einer globalen Suche (nur Experience Platform-Benutzer) im Suchfeld.
* Kontoeinstellungen verwalten können (Warnhinweise, Benachrichtigungen und Abonnements)

## Melden Sie sich bei Experience Cloud an {#signin}

Melden Sie sich an und stellen Sie sicher, dass Sie sich in der richtigen [Organisation](organizations.md) befinden.

1. Navigieren Sie zur [Adobe Experience Cloud](https://experience.adobe.com).
1. Geben Sie Ihre Adobe-E-Mail-Adresse ein und wählen Sie **[!UICONTROL Weiter]**.

   Als Administrator finden Sie unter [Experience Cloud-Benutzerauthentifizierung](admin-getting-started.md#migration) Informationen zu wichtigen Aktualisierungen bei den Identitätstypen (Business ID).

1. Wählen Sie ein Konto aus.
1. Geben Sie Ihr Passwort ein.
1. Stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden.

   ![Stellen Sie sicher, dass Sie sich in der richtigen Organisation befinden](assets/organizations-menu.png)

   **Organisation überprüfen**

   Um sicherzustellen, dass Sie sich bei Ihrer richtigen [Organisation](organizations.md) angemeldet haben, klicken Sie auf Ihren Profilavatar, um den Organisationsnamen anzuzeigen. Wenn Sie Zugriff auf mehr als eine Organisation haben, können Sie rechts in der Kopfzeilenleiste auch eine andere Organisation anzeigen und zu dieser wechseln.

   Wenn Ihr Unternehmen Federated IDs verwendet, können Sie sich durch ein Single Sign-on Ihres Unternehmens bei Experience Cloud anmelden, ohne Ihre E-Mail-Adresse und Ihr Passwort eingeben zu müssen. Fügen Sie `#/sso:@domain` zur Experience Cloud-URL (`https://experience.adobe.com`) hinzu, um diese Aufgabe zu erfüllen.

   Setzen Sie beispielsweise für eine Organisation mit Federated IDs und der Domain `adobecustomer.com` Ihren URL-Link auf `https://experience.adobe.com/#/sso:@adobecustomer.com`. Sie können auch direkt zu einem bestimmten Programm gehen, indem Sie diese URL, an die der Programmpfad angehängt ist, als Lesezeichen speichern. (Beispiel für Adobe Analytics: `https://experience.adobe.com/#/sso:@adobecustomer.com/analytics`.)

## Zugriff auf Experience Cloud-Anwendungen {#navigation}

Nach der Anmeldung bei Experience Cloud können Sie über den einheitlichen Header schnell auf alle Ihre Anwendungen, Dienste und Organisationen zugreifen.

Rufen Sie die das ![Menü](assets/menu-icon.png) der Programmauswahl auf, um auf die in Ihrem Unternehmen für Sie bereitgestellten Experience Cloud-Programme und -Services zuzugreifen.

![Zugriff auf Experience Cloud-Programme](assets/platform-core-services.png)

## Browser-Unterstützung in Experience Cloud {#browser}

Für eine optimale Leistung wurde Experience Cloud für die beliebtesten Browser optimiert, jeweils sowohl für deren neueste Version als auch für die beiden Vorgängerversionen.

* Chrome
* Edge
* Firefox
* Opera
* Safari

Wenn Ihr Browser nicht aufgeführt ist, wird er möglicherweise trotzdem unterstützt. Es wird jedoch empfohlen, einen der aufgelisteten Browser zu verwenden.

>[!NOTE]
>
>Nicht alle Anwendungen, die auf der Experience Cloud-Domain ausgeführt werden, unterstützen alle Browser. Wenn Sie sich nicht sicher sind, lesen Sie die Dokumentation zu einem bestimmten Programm.

## Sprachunterstützung in Experience Cloud {#languages}

Experience Cloud unterstützt bevorzugte Sprachen für jeden Benutzer, wie in den Voreinstellungen Ihres Adobe-Benutzerkontos festgelegt. Derzeit werden folgende Sprachen unterstützt:

* Chinesisch
* Englisch
* Französisch
* Deutsch
* Italienisch
* Japanisch
* Koreanisch
* Portugiesisch
* Spanisch
* Taiwanesisch

Obwohl sich alle Programm-Teams zur globalen Sprachunterstützung verpflichten, werden nicht alle Programme in allen oben genannten Sprachen angeboten. Wenn Ihre Primärsprache in einem Experience Cloud-Programm nicht unterstützt wird, können Sie auch eine sekundäre Sprache so einstellen, dass sie ggf. auf Standard gesetzt wird. Dies kann unter [Benutzervoreinstellungen für Experience Cloud](https://experience.adobe.com/preferences) durchgeführt werden.

## Erhalten Sie Hilfe und Support {#support}

Greifen Sie mithilfe des Hilfesymbols (![asset](assets/help-icon.png)) in der Kopfzeile auf Lernmaterialien und Hilfe zu, einschließlich Hilfeinhalten (Dokumentation, Tutorials und Kurse) zu [Experience League](https://experienceleague.adobe.com/?lang=de#home) sowie zusätzlichen Ressourcen für einzelne Programme. Sie können auch ein unverbindliches Feedback senden und priorisierte Support-Tickets erstellen.

![Erhalten Sie Hilfe und Support](assets/search-menu.png)

Das Menü [!UICONTROL Hilfe] bietet Ihnen außerdem Zugriff auf:

* **[!UICONTROL Support]:** Erstellen Sie ein Support-Ticket oder kontaktieren Sie den [!UICONTROL Support] über Twitter.
* **[!UICONTROL Feedback]:** Teilen Sie Feedback zu Ihrem Experience Cloud-Erlebnis. Ihr Feedback wird verwendet, um die Produkte und Services von Adobe zu verbessern.
* **[!UICONTROL Status]:** Navigieren Sie zu `https://status.adobe.com/experience_cloud` und prüfen Sie den Betriebsstatus des Produkts und [!UICONTROL verwalten Sie Abonnements].
* **[!UICONTROL Developer Connection]:** Navigation zu `adobe.io` und Entwicklerdokumentation.

## Benutzerprofil- und Kontovoreinstellungen {#preferences}

Zu den Einstellungen im Experience Cloud gehören Benachrichtigungen, Abonnements und Warnhinweise. Im Menü „Kontoeinstellungen“ haben Sie folgende Möglichkeiten:

* Festlegen eines dunklen Designs (nicht alle Anwendungen unterstützen dieses Design)
* Suchen nach [Organisationen](organizations.md)
* Abmelden
* Einstellungen, Benachrichtigungen und Abonnements für das Konto konfigurieren

Um die Voreinstellungen zu verwalten, wählen Sie die Option **[!UICONTROL Voreinstellungen]** im Menü ![Voreinstellungen](assets/preferences-icon-sm.png) Ihres Kontos aus.

![Benutzerprofil- und Kontovoreinstellungen](assets/preferences-page.png)

Unter [!UICONTROL Experience Cloud-Einstellungen] können Sie die folgenden Funktionen konfigurieren:

| Funktion | Beschreibung |
|--- |--- |
| Standard [organisation](organizations.md) | Wählen Sie die Organisation aus, die beim Starten von Experience Cloud angezeigt werden soll. |
| [!UICONTROL Erfassung von Produktdaten] | Wählen Sie aus, welche Technologien Adobe verwenden kann, um Daten darüber zu sammeln, wie Sie Ihre Adobe-Produkte verwenden. |
| [!UICONTROL Personalisierte Empfehlungen und Angebote von Lerninhalten] | Wählen Sie aus, wo Sie personalisierte Hilfe für Ihr(e) Adobe-Produkt(e) erhalten möchten. Diese Hilfe ist per E-Mail, innerhalb des Produktes und in den Experience League Communities verfügbar. [Weitere Informationen.](personalized-learning-preferences.md) |
| [!UICONTROL Abonnements] | Wählen Sie die Produkte und Kategorien aus, die Sie abonnieren möchten. Benachrichtigungen im Pop-Over [!UICONTROL Benachrichtigungen] und in Ihren E-Mails. |
| [!UICONTROL Priorität] | Wählen Sie die Kategorien aus, die eine hohe Priorität erhalten sollen. Diese Kategorien sind mit dem Tag Hoch gekennzeichnet und können zur Zustellung wie Warnhinweise konfiguriert werden. |
| [!UICONTROL Warnhinweise] | Wählen Sie die Benachrichtigungen aus, für die Warnhinweise in Ihrem Browser angezeigt werden sollen. Warnhinweise werden einige Sekunden lang in der oberen rechten Ecke des Fensters angezeigt. |
| E-Mails | Geben Sie die Häufigkeit an, mit der Sie Benachrichtigungs-E-Mails erhalten möchten. (Nicht gesendet, unmittelbar, täglich oder wöchentlich) |

{style="table-layout:auto"}

## Benachrichtigungen und Ankündigungen {#notifications}

Wählen Sie die Option **[!UICONTROL Benachrichtigungen]** aus, um über relevante und ausführbare Aktualisierungen, einschließlich Produktversionen, Wartungshinweise, freigegebene Elemente und Genehmigungsanfragen, informiert zu werden.

![Benachrichtigungen und Ankündigungen](assets/notifications-menu-small.png)

## Experience Cloud-Domains {#domains}

Experience Cloud verwendet die folgenden Hosts, um das Programm bereitzustellen, die Leistung zu verbessern und das Produkterlebnis zu verbessern. Adobe empfiehlt, diese Domains zur Zulassungsliste Ihrer Firewall hinzuzufügen, um ein optimales Erlebnis zu gewährleisten. Zusätzliche Domains können auch für bestimmte Experience Cloud-Programme wie Adobe Analytics verwendet werden. Weitere Informationen finden Sie in der Dokumentation für diese Programme.

| Technologie | Domains |
|--- |--- |
| Adobe Experience Cloud-Domains | `adobe.com`, `adobe.net`, `adobe.io` |
| Adobe Identity Management Service (IMS) | `adobelogin.com` |
| Experience Cloud-Schriftarten | `typekit.net` |
| Datenerfassung in Adobe (für Produktanleitungen und -hilfe) | `adobedtm.com` |
| Gainsight (für Produktanleitungen und Hilfe) | `esp.aptrinsic.com` |

## Hilfe zu Administrations- und programmübergreifenden Services

Dieses Handbuch bietet Hilfe zur Verwaltung von Experience Cloud-Benutzern und -Produkten in Admin Console, wodurch Programme Platform-Services nutzen können. Sie können auch auf die Hilfe über die Zielgruppenbibliothek, Kundenattribute, Experience Cloud-Kreativelemente und mehr zugreifen:

* [[!UICONTROL Zielgruppenbibliothek]](audience-library.md)
* [[!UICONTROL Kundenattribute]](attributes.md)
* [[!UICONTROL Triggers]](triggers.md)
* [Experience Cloud-[!UICONTROL Assets]](experience-cloud-assets.md)
* [Cookies in Experience Cloud](cookies-privacy.md)
* [Benutzer- und Produktverwaltung](admin-getting-started.md) (Admin Console)
* [Aktivieren Ihrer Programme für zentrale Services](core-services.md)
* [Häufig gestellte Fragen](admin-getting-started.md)
* [Organisationen und Kontoverknüpfung](organizations.md)
* [Integrationen](marketing-cloud-integrations.md)
* [Integrieren von Adobe Target in Experience Cloud](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html?lang=de)
* [Überblick über den Datenschutz und Sicherheitsmaßnahmen in Experience Cloud](assets/Adobe-Marketing-Cloud-Privacy-and-Security-Overview.pdf)
* [DNS-Vorabruf](admin-getting-started.md#concept_6BC8C6856E3644F8956D7AD0A96383B7)

## Handbücher

Weitere Experience Cloud-Handbücher:

* [Adobe Mobile](https://experienceleague.adobe.com/docs/mobile-services/using/home.html?lang=de)
* [Experience Platform Co-op Graph](https://experienceleague.adobe.com/docs/device-co-op/using/home.html?lang=de)
* [Exchange](https://exchange.adobe.com/experiencecloud)
* [Experience Cloud ID-Dienst](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=de)
* [ Experience Platform-Datenerfassung/Launch](https://experienceleague.adobe.com/docs/launch.html?lang=de)
* [Experience Cloud Debugger](https://experienceleague.adobe.com/docs/debugger/using/experience-cloud-debugger.html?lang=de)
* [[!UICONTROL Dynamic Tag Management]](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html?lang=de)

## Tutorials

Nutzen Sie die Vorteile von Selbsthilfe-Tutorials und Schnellanleitungen in Experience League:

* [Alle Tutorials in Experience League](https://experienceleague.adobe.com/?lang=de#quick-how-tos)
* [Experience Platform-Tutorials](https://experienceleague.adobe.com/docs/platform-learn/data-collection/overview.html?lang=de)
* [Real-time Customer Data Platform](https://experienceleague.adobe.com/docs/platform-learn/tutorials/application-services/rtcdp/understanding-the-real-time-customer-data-platform.html?lang=de)

## Versionshinweise und zugehörige Experience Cloud-Hilfe

* [Versionshinweise für alle Experience Cloud-Programme](https://experienceleague.adobe.com/docs/home.html?lang=de) – Suchen Sie nach Hilfe unter „Experience Cloud Learn &amp; Support“
* [Versionshinweise und Produktupdates](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=de) – Neue Funktionen in der Experience Cloud und Abonnieren von Updates
* [Übungen zur Implementierung der zentralen Dienste](https://experienceleague.adobe.com/docs/platform-learn/data-collection/overview.html?lang=de) – Videos und Übungen zu den zentralen Diensten
* [Expertenhilfe bei Experience League](https://experienceleague.adobe.com/?lang=de) – Lernen Sie von Experten und der Community
* [Ausbildung und Schulung](https://helpx.adobe.com/de/learning.html?promoid=KAUDK) – Wenden Sie sich an Adobe, um sicherzustellen, dass Sie die Produkte von Adobe optimal nutzen
* [Customer Experience-Blog](https://blog.adobe.com/de/topics/digital-transformation) – Lesen Sie den Experience Cloud-Blog
* [Kundenunterstützung](https://experienceleague.adobe.com/?support-solution=General&amp;lang=de#support) – Wenden Sie sich an die Adobe-Kundenunterstützung
