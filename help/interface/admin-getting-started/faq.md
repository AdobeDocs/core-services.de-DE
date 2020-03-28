---
description: Fragen, die Administratoren der Experience Cloud häufig stellen, und Antworten darauf.
keywords: core services, Experience Cloud, Experience Platform, Analytics, Target, user management.
seo-description: Fragen, die Administratoren der Experience Cloud häufig stellen, und Antworten darauf.
seo-title: Häufig gestellte Fragen Informationen zu den Hauptdiensten der Experience Cloud.
solution: Adobe Experience Cloud
title: Häufig gestellte Fragen
index: true
translation-type: tm+mt
source-git-commit: 43de353155c640b3ddc519147c94d7e9ffcafe4e

---


# Häufig gestellte Fragen über Experience Cloud

Fragen, die Administratoren der Experience Cloud häufig stellen, und Antworten darauf.

## Wie finde ich heraus, ob für meine Lösungen Hauptdienste aktiviert sind?

Wenn Ihre Implementierung nicht für Hauptdienste bereitgestellt wurde, lesen Sie die den Abschnitt [Lösungen für Hauptdienste aktivieren](../core-services/core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C), in dem Folgendes beschrieben wird:

1. [Experience Cloud beitreten und Administrator werden](../core-services/core-services.md#section_2423F0BD3DF642658103310EE5EA6154)
1. [Implementieren Sie den Experience Cloud ID-Dienst mit Experience Platform Launch](https://docs.adobe.com/content/help/en/launch/using/intro/get-started/quick-start.html).
1. [Report Suites einer Experience Cloud-Organisation zuweisen](../core-services/core-services.md#concept_apg_zq2_rw)
1. [(Nur Analytics) Modernisierung Ihres Analytics-AppMeasurement-Codes](../core-services/core-services.md#section_1798D9D0F05C47E29816AC4EEB9A0913)
1. [(Nur Adobe-Zielgruppe) Modernisierung der Implementierung Ihrer Adobe-Zielgruppe](../core-services/core-services.md#section_C2F4493C7A36406DAE2266B429A4BD24)
1. [Überprüfen der Implementierung der Hauptdienste](../core-services/core-services.md#section_E641782A0F4F44AF8C9C91216BE330D5)
1. [Benutzer und Produkte verwalten](../core-services/core-services.md#section_B6E95F4E0E12483CB9DA99CBC0C5A4AF)
1. [Einführung in die Hauptdienste](../core-services/core-services.md#section_960C06093623462E8EA247B3E97274A1)

Weitere Hilfe erhalten Sie vom [Adobe-Support](https://helpx.adobe.com/marketing-cloud/contact-support.html).

## Stellt Adobe meinem Unternehmen den Zugriff auf die Experience Cloud in Rechnung?

Nein. Die Experience Cloud ist kostenlos im Preis inbegriffen. Bestimmte Kerndienste könnten jedoch zusätzliche Kosten verursachen.

## Weshalb muss sich mein Unternehmen über die Experience Cloud-Schnittstelle anmelden?

Die Funktionen der Experience Cloud-Oberfläche bieten Ihrem Unternehmen einen neuen Mehrwert. Es wird auch der Standardpfad für den Zugriff auf Lösungen sein, der in Zukunft verwendet wird und eventuell andere individuelle Lösungsanmeldevorgänge ersetzt. Die Anmeldung über die Experience Cloud erleichtert später eine reibungslosere Transition.

## Wie gehe ich auf die Bedenken ein, die mein Unternehmen gegenüber einer Migration hat?

[Wenden Sie sich an den Adobe Support](https://helpx.adobe.com/marketing-cloud/contact-support.html).

## Was ist _Bereitstellung?_

Bereitstellung im Sinne der Experience Cloud bedeutet:

* Ihre Benutzer können mit der Anmeldung bei der [!DNL Experience Cloud] und der Verknüpfung von Lösungen beginnen.
* Sie können mit der Verwendung der in der Experience Cloud verfügbaren Funktionen wie &quot;Personen&quot;beginnen.
* Sie können sich darauf einstellen, Ihren lösungsspezifischen Anmeldeprozess einzustellen.
* Sie können die Zugriffskontrolle zu Lösungen beibehalten.

## Wie verwalte ich Benutzer und Produktprofile?

* Hilfe finden Sie im [Administrationskonsole Benutzerhandbuch](https://helpx.adobe.com/enterprise/administering/user-guide.html) .

* Die Zuweisung von Benutzerrechten und die Produktverwaltung erfolgen über die [Adobe Admin Console](https://adminconsole.adobe.com/enterprise) (Produktlink).

* **Wichtig:** Analytics-Administratoren finden Informationen zur Migration von Benutzer-IDs aus den Analytics Admin Tools in die Admin-Konsole [unter Analytics-Benutzer](https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/user-management/migrate-users/c-migration-tool.html) verwalten.

## Was kann ich tun, wenn sich ein Benutzer nicht bei der Experience Cloud anmelden kann?

Administratoren der Admin-Konsole können Benutzern Zugriff gewähren. Benutzern werden E-Mails mit Anleitungen zum Anmelden gesendet.

You might need to [Contact Adobe Support](https://helpx.adobe.com/marketing-cloud/contact-support.html) to verify that your company has been fully provisioned.

## Wo können Benutzer die Kontoverknüpfung verwalten?

Einige Benutzer müssen unter Umständen ihr Lösungskonto (Analytics) mit der Adobe ID oder Enterprise ID verknüpfen.

See [Link a solution account to an Adobe ID](../admin-getting-started/organizations.md#task_FD389E78640848919E247AC5E95B8369).

## Wie verwalte ich Benutzerkontoprofile und Organisationen?

Siehe [Verwalten von Benutzerkonten](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1).

## Was ist eine Organisation?

Eine **-Organisation ist die Einheit, die es einem Administrator ermöglicht, Gruppen und Benutzer zu konfigurieren und das Single-Sign-on in der Experience Cloud zu steuern. Die Organisation agiert als zentrale Anmeldestelle, die sämtliche Experience Cloud-Produkte und -Lösungen umfasst. Normalerweise besitzt eine Organisation den Namen Ihres Unternehmens. Ein Unternehmen kann jedoch über mehrere Organisationen verfügen.

## Wo finde ich meine IMS-Organisations-ID?

Siehe [Suchen Ihrer Organisations-ID](organizations.md).

Die Organisations-ID wird auf der Landingpage der Experience Cloud und der [Landingpage der Admin Console](https://adminconsole.adobe.com) angezeigt.

Alternatively, administrators can log into the Admin console (Navigate to [https://adminconsole.adobe.com](https://adminconsole.adobe.com#)) for a specific organization, and you will be able to see your IMS org ID in the URL.

Beispielsweise in der folgenden URL:

`https://adminconsole.adobe.com/C538193582390300A495CC9@AdobeOrg/overview`

Hier lautet die ID:

`C538193582390300A495CC9@AdobeOrg`

## Was muss ich tun, wenn einer meiner Benutzer das Unternehmen verlässt?

Dessen Zugang muss direkt in der Lösung entfernt werden. Sie können nicht über die Experience Cloud oder die direkte Anmeldung auf das Produkt zugreifen. Sie sollten sie auch auf Experience Cloud-Ebene entfernen.

## Was ist eine Adobe ID?

Siehe [Identitätstypen](https://helpx.adobe.com/enterprise/help/identity.html).

## Kann ich für meine Benutzer Lösungskonten verknüpfen?

Nein. Benutzer müssen ihre eigenen Lösungen mit Benutzernamen und Kennwörtern verknüpfen.

## Warum wird mir Social angezeigt, wenn mein Unternehmen diesen Dienst gar nicht erworben hat?

Adobe Social ist ein Produkt, das mit Analytics verkauft werden kann. Wenn Sie Analytics verwenden, sehen Sie diese Lösung, haben aber keinen Zugriff, es sei denn, Sie haben sie gekauft.
