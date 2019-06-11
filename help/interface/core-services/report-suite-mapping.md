---
description: Erfahren Sie, wie Sie eine oder mehrere Report Suites einer Organisation zuweisen.
seo-description: Erfahren Sie, wie Sie eine oder mehrere Report Suites einer Organisation zuweisen.
seo-title: Report Suites einer Organisation zuweisen
title: Report Suites einer Organisation zuweisen
uuid: b 983 d 5 a 6-b 3 d 0-4137-ac 53-bc 5681 d 3 e 58 b
translation-type: tm+mt
source-git-commit: d9d6cebc0e9e14eac2471dc79b91276a154e35e0

---


# Report Suites einer Organisation zuweisen {#topic_7C4740559EAC4E0FA5F8DEF886B580DA}

Erfahren Sie, wie Sie eine oder mehrere Report Suites einer Organisation zuweisen.

Experience Cloud-Dienste (z. B. der Experience Cloud ID-Dienst und der People-Hauptdienst) sind einer Experience Cloud-Organisation zugeordnet und keiner einzelnen Report Suite. Damit sichergestellt ist, dass diese Dienste korrekt funktionieren, muss jede Analytics-Report Suite einer Organisation zugeordnet sein. Der Zuweisungsprozess:

* Legt eine Experience Cloud-Organisation als primäre Organisation für die Report Suite fest.
* hat keinen Einfluss darauf, wer auf die Report Suite zugreifen kann (der Zugriff wird nach wie vor über das Adobe Analytics-Anmeldekonto eines jeden Benutzers bestimmt) 


**Voraussetzungen**

Sie müssen Analytics-Administrator einer Unternehmensanmeldung sein, der Zugriff auf die zuzuweisende Report Suite hat. Außerdem muss dieses Konto [mit einer Experience Cloud-Organisation verknüpft](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1) sein, damit dieser Organisation Report Suites zugeordnet werden können.

Organisationen werden ausgegraut, wenn Sie in Analytics keine Administratorrechte für eine Unternehmensanmeldung einer Organisation haben, die über Zugriff auf die entsprechende Report Suite verfügt.

## Eine Report Suite einer Organisation zuordnen {#task_23993FE78DF6455FA8D7BE60686EA16C}

1. Klicken Sie auf **[!UICONTROL Experience Cloud]** &gt; **[!UICONTROL Administration]** &gt; **[!UICONTROL Report Suite Zuordnung]**

   Alternativ können Sie eine [direkte URL](https://audience.marketing.adobe.com/rsmapping/ui.html) verwenden.

1. Wenn Sie anzeigen möchten, welche Unternehmensanmeldungen Zugriff auf welche Report Suite haben, klicken Sie auf **[!UICONTROL Sichtbar für Unternehmensanmeldung]**.

   Mithilfe dieser Ansicht können Sie Entscheidungen über die Zuweisung einfacher treffen.

1. Klicken Sie auf das Dropdown-Menü in der Spalte **[!UICONTROL Zugeordnete Organisation]neben einer Report Suite und wählen Sie die Organisation aus, der Sie die Suite zuweisen möchten.**

   Tipps zum Auswählen einer Experience Cloud-Organisation finden Sie im nächsten Abschnitt.

## Mehrere Report Suites einer Organisation zuordnen {#task_94955B0D8ABA4CB1A38746ECF8E32711}

1. Klicken **[!UICONTROL Sie auf Experience Cloud]** &gt; **[!UICONTROL Administration]** &gt; **[!UICONTROL Report Suite Zuordnung]**.

   Alternativ können Sie eine [direkte URL](https://audience.marketing.adobe.com/rsmapping/ui.html) verwenden.

1. Wählen Sie die Report Suites aus, die Sie zuweisen möchten.

   ![](assets/rs-mapping-multiple.png)

1. Wählen Sie die Organisation aus (hier Outdoors Inc) und klicken Sie auf **[!UICONTROL Auswählen]**.

   Tipps zum Auswählen einer Experience Cloud-Organisation finden Sie im nächsten Abschnitt.

1. Klicken Sie auf **[!UICONTROL Zuordnung speichern]**.

## Tipps für die Auswahl einer Experience Cloud-Organisation {#mapping-tips}

In diesem Abschnitt finden Sie Tipps dazu, wie Sie die Experience Cloud-Organisation auswählen, der Sie eine Report Suite zuweisen sollten.

**Welche Organisation sollte ich auswählen?**

Wird der Experience Cloud ID-Dienst derzeit auf die Report Suite angewandt, müssen Sie sicherstellen, dass Sie im Zuordnungs-Tool für Report Suites die gleiche Organisation auswählen, die auch in der Datei [!DNL visitorAPI.js] auf Ihrer Site angegeben ist. Sie können die im Kapitel über das [Testen und Verifizieren des Experience Cloud ID-Dienstes](https://marketing.adobe.com/resources/help/en_US/mcvid/mcvid-test-verify.html) beschriebenen Schritte vornehmen, um die Organisations-ID zu ermitteln, die vom ID-Dienst genutzt wird.

Wird der Besucher-ID-Dienst bisher noch nicht auf Sites eingesetzt, auf denen die Report Suite Daten erfasst, muss die Bereitstellung der in der Report Suite-Zuweisung ausgewählten Organisation entsprechen, wenn der Experience Cloud-Besucher-ID-Dienst zu einem späteren Zeitpunkt verwendet wird.

**Warum sind einige Organisationen ausgegraut?**

Dieser Umstand zeigt an, dass Sie nicht über die für eine Zuweisung der ausgegrauten Report Suite notwendigen Zugriffsrechte verfügen. Siehe folgendes Beispiel:
![](assets/rs-mapping.png) In dieser Darstellung zeigt der blaue Schlüssel an, dass der Benutzer über Administratorrechte verfügt. Die graue Linie steht für die Sichtbarkeit.

Dieser Benutzer hat Zugriff auf zwei Experience Cloud-Organisationen. Er hat Folgendes unternommen:

* Er hat sein Administratorenkonto für die Analytics-Unternehmensanmeldung „chapek“ mit dem Experience Cloud-Organisationskonto der Chapek Corp verknüpft.
* Er hat sein Konto ohne Administratorrechte für die Analytics-Unternehmensanmeldung „doohan“ mit dem Experience Cloud-Organisationskonto der Chapek Corp verknüpft.
* Er hat sein Konto ohne Administratorrechte für die Analytics-Unternehmensanmeldung „nigel“ mit dem Experience Cloud-Organisationskonto der Nigel Inc verknüpft.

Im Folgenden wird beschrieben, welche Zuweisungen der Benutzer für die Report Suites vornehmen kann und welche nicht:

* Die Report Suite „chapek-prod“ kann der Organisation „Chapek Corp“ zugewiesen werden, da der Benutzer ein Administrator einer verknüpften Analytics-Unternehmensanmeldung (chapek) ist und sein Konto mit der Organisation verknüpft wurde.
* Die Report Suite „nigel-prod“ kann vom Benutzer nicht zugewiesen werden, da er kein Administrator einer Unternehmensanmeldung ist, für die die Report Suite sichtbar wäre.
* Die Report Suite „doohan-prod“ kann Chapek Corp zugewiesen werden, da der Benutzer Administrator einer Unternehmnsnameldung (chapek) ist, die mit der Experience Cloud-Organisation verknüpft wurde (beachten Sie, dass der Benutzer nicht Administrator der Analytics-Unternehmensanmeldung „doohan“ ist). Bedenken Sie, dass die Report Suite „doohan-prod“ auch der Experience Cloud-Organisation Nigel Inc zugewiesen werden kann, auch wenn der aktuell angemeldete Benutzer diese Zuweisung nicht vornehmen darf. In diesem Fall erscheinen beide Experience Cloud-Organisationen in der Liste, Nigel Inc wird jedoch ausgegraut. Vor der Zuordnung sollte sich der Benutzer mit einem Administrator der Unternehmensanmeldung „nigel“ in Verbindung setzen, um mit ihm zu besprechen, welche Organisation für die Zuweisung am besten geeignet ist. In der Benutzeroberfläche wird eine Warnmeldung über einen möglichen Konflikt angezeigt, wenn ein Benutzer eine Organisation auswählt, die nicht diejenige Organisation ist, unter der die Report Suite ursprünglich erstellt wurde.

## Häufig gestellte Fragen {#section_099E485805994C929FF9C9F75219BEE1}

**Warum werden mir nicht alle meine Report Suites angezeigt?**

Einige Ihrer Report Suites werden möglicherweise nur für eine andere Unternehmensanmeldung angezeigt. Die aktuelle Unternehmensanmeldung können Sie mithilfe des Dropdown-Menüs oben im Bildschirm ändern.

**Was passiert, wenn ich einige der im Dropdown-Menü einer meiner Report Suites aufgelisteten Organisationen nicht kenne?**

Die Liste zeigt Ihnen alle * möglichen * Organisationen, denen Ihre Report Suite zugeordnet werden könnte, auch wenn Sie nicht berechtigt sind, all diese Report Suites zuzuordnen. Wenn Sie nicht sicher sind, ob die Report Suite einer der ausgegrauten Report Suites in der Liste zugeordnet werden soll, wenden Sie sich an einen Experience Cloud-Administrator in Ihrer Organisation, um die am besten geeignete Option auszuwählen.

**Was ist, wenn ich einige der Unternehmensanmeldungen nicht kenne, die in der Spalte „Sichtbar für Unternehmensanmeldung“ einer Report Suite aufgezählt werden?**

In der Vergangenheit wurde die Report Suite für eine andere Unternehmensanmeldung freigegeben, die möglicherweise Teil einer anderen Experience Cloud-Organisation ist.

**Was bedeutet die Fehlermeldung über einen möglichen Konflikt bei einer Report Suite, die von einer anderen Organisation generiert wurde? Warum ist das für mich von Interesse?**

Diese Benachrichtigung unterstützt Sie dabei, bei der Zuordnung von Report Suites die richtige Entscheidung zu treffen. Wir möchten Sie darauf hinweisen, dass die Report Suite ursprünglich unter einer anderen Organisation erstellt wurde, da es möglich ist, dass sich diese Organisation für die Zuordnung der Report Suite besser eignet.

**Wie erkenne ich, ob eine Report Suite zugeordnet ist?**

Zugeordnete Report Suites werden als nicht bearbeitbar dargestellt. Sollten Sie eine Zuordnung ändern müssen, wenden Sie sich an die Kundenunterstützung.

**Was passiert, wenn ich nur die Organisations-ID meiner Experience Cloud-Organisation kenne? Wo kann ich den Namen meiner Organisations-ID nachschlagen?**

Den Namen Ihrer Organisation finden Sie unter [Organisationen und Kontoeinstellungen](https://marketing.adobe.com/resources/help/en_US/mcloud/?f=organizations).

**In der Spalte „Datum der Zuordnung“ ist ein Datum eingetragen. Wer hat diese Zuordnung vorgenommen?**

Im Report Suite-Änderungsprotokoll der Analytics-Oberfläche können Sie die ID des Benutzers nachschlagen, der die Änderung vorgenommen hat. Suchen Sie nach dem Ereignis „Suite associated to IMS Organization“.
