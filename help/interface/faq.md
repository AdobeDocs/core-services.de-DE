---
description: Erfahren Sie mehr über Browser-Unterstützung und finden Sie Antworten für Administratoren auf häufig gestellte Fragen in Adobe Experience Cloud.
keywords: Zentrale Services, Experience Cloud, Experience Platform, Analytics, Target, Benutzerverwaltung.
solution: Experience Cloud
title: 'Häufig gestellte Fragen zu Experience Cloud '
index: true
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 062576da-328e-4b46-9e71-5a25733d607a
source-git-commit: 00a6aa791dd08c2907cd09c17b7e2a1e62b060c1
workflow-type: ht
source-wordcount: '775'
ht-degree: 100%

---

# Häufig gestellte Fragen zu Experience Cloud

Erfahren Sie mehr über Browser-Unterstützung und häufig gestellte Fragen und Antworten für Administratoren in Experience Cloud.

## Welche Browser werden in Experience Cloud unterstützt?

* Microsoft® Edge (aktuelle und die vorherigen zwei Versionen)
* Google Chrome (aktuelle und die vorherigen zwei Versionen)
* Mozilla Firefox (aktuelle und die vorherigen zwei Versionen)
* Safari (aktuelle und die vorherigen zwei Versionen)
* Opera (aktuelle und die vorherigen zwei Versionen)

## Wie finde ich heraus, ob meine Programme für zentrale Services aktiviert sind?

Wenn Ihre Implementierung nicht für zentrale Services bereitgestellt wurde, lesen Sie den Abschnitt [Aktivieren Ihrer Programme für zentrale Services](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C), in dem Folgendes beschrieben wird:

1. [Experience Cloud beitreten und Administrator werden](core-services.md#section_2423F0BD3DF642658103310EE5EA6154)
1. [Implementieren Sie den Experience Cloud ID-Dienst mit Experience Platform Launch](https://experienceleague.adobe.com/docs/experience-platform/tags/get-started/quick-start.html?lang=de).
1. [Report Suites einer Experience Cloud-Organisation zuweisen](core-services.md#concept_apg_zq2_rw)
1. [(nur Analytics) Modernisierung des Analytics-AppMeasurement-Codes](core-services.md#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [(nur Adobe Target) Modernisierung der Adobe Target-Implementierung](core-services.md#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [Überprüfen der Implementierung](core-services.md#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [Benutzer und Produkte verwalten](core-services.md#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [Einführung in die Hauptdienste](core-services.md#section_960C06093623462E8EA247B3E97274A1)

Wenden Sie sich für weitere Hilfe an den [Adobe-Support](https://experienceleague.adobe.com/?support-solution=General&amp;lang=de#support).

## Stellt Adobe meinem Unternehmen den Zugriff auf die Experience Cloud in Rechnung?

Nein. Die Experience Cloud ist ohne Zusatzkosten im Preis inbegriffen. Bestimmte zentrale Dienste könnten jedoch zusätzliche Kosten verursachen.

## Warum muss sich mein Unternehmen über die Experience Cloud-Oberfläche anmelden?

Die Funktionen der Experience Cloud-Oberfläche bieten Ihrem Unternehmen einen neuen Mehrwert. Dies wird künftig auch der Standardpfad für den Zugriff auf Programme sein und letztlich andere individuelle Programmanmeldevorgänge ersetzen. Das Anmelden über Experience Cloud erleichtert später eine reibungslosere Transition.

## Wie gehe ich auf die Bedenken ein, die mein Unternehmen gegenüber einer Migration hat?

[Wenden Sie sich an den Adobe Support](https://experienceleague.adobe.com/?support-solution=General&amp;lang=de#support).

## Wie kann [!DNL Adobe Support] auf meine Adobe-Cloud-Umgebung zugreifen, um ein Problem zu beheben?

[!DNL Adobe Support] können eine Identitätsanfrage einreichen, für die Sie eine E-Mail mit dem Adobe-Markenlogo erhalten (Beispiel unten), in der Ihre ausdrückliche Autorisierung angefordert wird. Der Zugriff wird für eine begrenzte Zeit gewährt. Nach der Gewährung können Sie den Zugriff jederzeit widerrufen. Adobe protokolliert alle von Adobe-Mitarbeitern getroffenen Maßnahmen.

![Adobe Support-Fall](assets/support-email.png)

## Was ist eine _Bereitstellung?_

Bereitstellung in Experience Cloud bedeutet:

* Ihre Benutzer können mit der Anmeldung bei [!DNL Experience Cloud] und der Verknüpfung von Programmen beginnen.
* Sie können mit der Verwendung der in Experience Cloud verfügbaren Funktionen beginnen, z. B. „Personen“.
* Sie können sich darauf vorbereiten, Ihren programmspezifischen Anmeldeprozess aufzugeben.
* Sie können die Zugangssteuerung für Programme beibehalten.

## Wie verwalte ich Benutzer und Produktprofile?

* Hilfe finden Sie im [Admin Console-Benutzerhandbuch](https://helpx.adobe.com/de/enterprise/admin-guide.html).

* Die Zuweisung von Benutzerrechten und die Produktverwaltung erfolgen über die [Adobe Admin Console](https://adminconsole.adobe.com/enterprise) (Produktlink).

* **Wichtig:** Analytics-Administratoren finden unter [Verwalten von Analytics-Benutzern in der Admin Console](https://experienceleague.adobe.com/docs/analytics/admin/user-product-management/migrate-users/c-migration-tool.html?lang=de) Informationen zur Migration von Benutzer-IDs aus den Analytics Admin-Tools in die Admin Console.

## Was kann ich tun, wenn sich ein Benutzer nicht bei der Experience Cloud anmelden kann?

Admin Console-Administratoren können Benutzern Zugriff gewähren. Benutzern werden E-Mails mit Anweisungen zum Anmelden gesendet.

Möglicherweise müssen Sie sich zunächst [an den Adobe-Support wenden](https://experienceleague.adobe.com/?support-solution=General&amp;lang=de#support), um zu bestätigen, dass Ihrem Unternehmen die entsprechenden Lösungen bereitgestellt wurden.

## Wo können Benutzer die Kontoverknüpfung verwalten?

Einige Benutzende müssen unter Umständen ihr Programmkonto (Analytics) mit der Adobe ID oder Enterprise ID verknüpfen.

Siehe [Verknüpfen von Programmkonten mit einer Adobe ID](organizations.md#task_FD389E78640848919E247AC5E95B8369).

## Wie verwalte ich Benutzerkontoprofile und Organisationen?

Siehe [Verwalten von Benutzerkonten](organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1).

## Was ist eine Organisation?

Eine [Organisation](organizations.md) ist die Einheit, die es einem Administrator ermöglicht, Gruppen und Benutzer zu konfigurieren und das Single-Sign-on in Experience Cloud zu steuern. Die Organisation funktioniert wie ein Unternehmen mit Anmeldung, das alle Experience Cloud-Produkte und -Programme umfasst. Normalerweise besitzt eine Organisation den Namen Ihres Unternehmens. Ein Unternehmen kann jedoch über mehrere Organisationen verfügen.

## Wo finde ich meine IMS-Organisations-ID?

Details hierzu finden Sie unter [Organisations-ID anzeigen](organizations.md).

## Was muss ich tun, wenn einer meiner Benutzer meine Organisation verlässt?

Dessen Zugang sollte direkt im Programm entfernt werden. Sie können nicht über die Experience Cloud oder die direkte Anmeldung auf das Produkt zugreifen. Sie sollten sie auch auf Ebene von Experience Cloud entfernen.

## Was ist eine Adobe ID?

Siehe [Identitätstypen](https://helpx.adobe.com/de/enterprise/using/identity.html).

## Kann ich für meine Benutzer Programmkonten verknüpfen?

Nein. Benutzer müssen ihre eigenen Programme mit ihren Benutzernamen und Kennwörtern verknüpfen.

## Warum wird mir Social angezeigt, wenn mein Unternehmen diesen Service gar nicht erworben hat?

Adobe Social ist ein Produkt, das mit Analytics verkauft werden kann. Daher sehen Sie dieses Programm, wenn Sie Analytics besitzen. Sie haben jedoch nur dann Zugriff darauf, wenn Sie es gekauft haben.
