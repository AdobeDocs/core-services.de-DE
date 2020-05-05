---
description: Erfahren Sie, wie Sie eine oder mehrere Report Suites einer Organisation zuweisen.
seo-description: Erfahren Sie, wie Sie eine oder mehrere Report Suites einer Organisation zuweisen.
seo-title: Report Suites einer Organisation zuweisen
title: Report Suites einer Organisation zuweisen
uuid: b983d5a6-b3d0-4137-ac53-bc5681d3e58b
translation-type: tm+mt
source-git-commit: 08e8e5fea4e4e64a195ebe25ae3ef19e849cabc5

---


# Report Suites einer Organisation zuweisen {#topic_7C4740559EAC4E0FA5F8DEF886B580DA}

Erfahren Sie, wie Sie eine oder mehrere Report Suites einer Organisation zuweisen.

<!-- May 5 2020: This feature will likely be deprecated in Nov 2020. Any users with outstanding report suites that are not mapped will have 6 months to map their RS. -->

Experience Cloud services (such as Experience Cloud ID Service and [!UICONTROL People]) are associated with an organization instead of an individual report suite. Um sicherzustellen, dass diese Dienste ordnungsgemäß funktionieren, muss jede Analytics Report Suite einer Organisation zugeordnet werden. Der Zuordnungsprozess:

* Legt eine Experience Cloud-Organisation als primäre Organisation für die Report Suite fest.
* hat keinen Einfluss darauf, wer auf die Report Suite zugreifen kann (der Zugriff wird nach wie vor über das Adobe Analytics-Anmeldekonto eines jeden Benutzers bestimmt)

## Anforderungen

Sie müssen Analytics-Administrator einer Anmelde-Firma sein, die Zugriff auf die Report Suite hat, die Sie zuordnen möchten. Außerdem muss dieses Konto mit einer Experience Cloud-Organisation [](../admin-getting-started/organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1) verknüpft sein, um Report Suites dieser Organisation zuzuordnen.

Organisationen werden ausgegraut, wenn Sie in Analytics keine Administratorrechte für eine Unternehmensanmeldung einer Organisation haben, die über Zugriff auf die entsprechende Report Suite verfügt.

## Report Suite einer Organisation zuweisen{#task_23993FE78DF6455FA8D7BE60686EA16C}

1. Click **[!UICONTROL Experience Cloud]** > **[!UICONTROL Administration]** > **[!UICONTROL Report Suite Mapping]**

1. Wenn Sie anzeigen möchten, welche Unternehmensanmeldungen Zugriff auf welche Report Suite haben, klicken Sie auf **[!UICONTROL Sichtbar für Unternehmensanmeldung]**.

   Mithilfe dieser Ansicht können Sie Entscheidungen über die Zuweisung einfacher treffen.

1. Klicken Sie auf das Dropdown-Menü in der Spalte **[!UICONTROL Zugeordnete Organisation]** neben einer Report Suite und wählen Sie die Organisation aus, der Sie die Suite zuweisen möchten.

   Tipps zum Auswählen einer Experience Cloud-Organisation finden Sie im nächsten Abschnitt.

## Mehrere Report Suites einer Organisation zuweisen {#task_94955B0D8ABA4CB1A38746ECF8E32711}

1. Click **[!UICONTROL Experience Cloud]** > **[!UICONTROL Administration]** > **[!UICONTROL Report Suite Mapping]**.

1. Wählen Sie die Report Suites aus, die Sie zuweisen möchten.

   ![](assets/rs-mapping-multiple.png)

1. Wählen Sie die Organisation aus (hier Outdoors Inc) und klicken Sie auf **[!UICONTROL Auswählen]**.

   Tipps zum Auswählen einer Experience Cloud-Organisation finden Sie im nächsten Abschnitt.

1. Klicken Sie auf **[!UICONTROL Zuordnung speichern]**.

## Tipps für die Auswahl einer Experience Cloud-Organisation {#mapping-tips}

Dieser Abschnitt enthält Tipps zur Auswahl der Experience Cloud-Organisation, der Sie eine Report Suite zuordnen sollten.

### Welche Einrichtung sollte ich wählen?

If the Experience Cloud ID Service is currently deployed on the report suite, ensure the organization you select in the Report Suite Mapping tool is the same organization specified in the [!DNL visitorAPI.js] file on your site. You can use the instructions in [Test and Verify the Experience Cloud ID Service](https://docs.adobe.com/content/help/en/id-service/using/implementation-guides/test-verify.html) to find the org ID that is being used by the Visitor ID service.

Wird der Besucher-ID-Dienst bisher noch nicht auf Sites eingesetzt, auf denen die Report Suite Daten erfasst, muss die Implementierung der in der Report Suite-Zuweisung ausgewählten Organisation entsprechen, wenn der Experience Cloud-Besucher-ID-Dienst zu einem späteren Zeitpunkt verwendet wird.

### Warum sind einige Organisationen ausgegraut?

Dies weist darauf hin, dass Sie nicht über ausreichende Berechtigungen verfügen, um der ausgegrauten Report Suite zuzuordnen. Siehe folgendes Beispiel:


![](assets/rs-mapping.png)

 In dieser Darstellung zeigt der blaue Schlüssel an, dass der Benutzer über Administratorrechte verfügt. Die grauen Linien zeigen die Sichtbarkeit an.

Dieser Benutzer hat Zugriff auf zwei Experience Cloud-Organisationen. Er hat Folgendes ausgeführt:

* Verknüpfte sein Admin-Konto in der [!UICONTROL chapek] Analytics-Anmelde-Firma mit seinem [!UICONTROL Chapek] Corp Experience Cloud-Organisationskonto.
* Verknüpfte sein Nicht-Admin-Konto in der [!UICONTROL Analytics-Anmelde-Firma von Adobe] mit seinem [!UICONTROL Chapek] Corp Experience Cloud-Organisationskonto.
* Verknüpfte sein Nicht-Admin-Konto in der nigel Analytics-Anmelde-Firma mit seinem Nigel Inc Experience Cloud-Organisationskonto.

Mit den folgenden Punkten werden die Zuordnungsaktionen Liste, die dieser Benutzer in Bezug auf diese Report Suites ausführen kann und kann:

* [!UICONTROL Die Chapek-prod] Report Suite kann [!UICONTROL Chapek] Corp Org zugeordnet werden, da dieser Benutzer Administrator einer verknüpften Analytics-Anmelde-Firma ([!UICONTROL chapek]) ist und sein Konto mit dieser Organisation verknüpft ist.
* [!UICONTROL Nigel-prod] Report Suite kann von diesem Benutzer nicht verknüpft werden, da er in keiner der Anmelde-Firmen, auf die diese Report Suite angezeigt wird, Administrator ist.
* [!UICONTROL Doohan-prod] Report Suite kann [!UICONTROL Chapek Corp] zugeordnet werden, da dieser Benutzer Administrator einer Anmelde-Firma ([!UICONTROL chapek]) ist, die mit der Experience Cloud-Organisation verknüpft ist (beachten Sie, dass er kein Administrator der Analytics-Anmelde-Firma ist). Beachten Sie, dass die [!UICONTROL doohan-prod] Report Suite auch für die Zuordnung zum Nigel Inc Experience Cloud-Org geeignet ist, auch wenn dieser Benutzer diese Zuordnung nicht durchführen kann. In diesem Fall werden beide Experience Cloud-Organisationen in der Liste angezeigt, [!UICONTROL Nigel Inc] ist jedoch grau ausgeblendet. Vor der Zuordnung sollte sich der Benutzer mit einem Administrator der nigel-Login-Firma beraten, um zu ermitteln, welches Org für die Zuordnung am besten geeignet ist. In der Benutzeroberfläche wird eine Warnung zu möglichen Konflikten angezeigt, wenn Sie eine Organisation auswählen, die sich von der Organisation unterscheidet, unter der die Report Suite ursprünglich erstellt wurde.

## Häufig gestellte Fragen {#section_099E485805994C929FF9C9F75219BEE1}

### Warum werden nicht alle meine Report Suites angezeigt?

Einige Ihrer Report Suites können unter einer anderen Firma angezeigt werden. Sie können die aktuelle Firma der Anmeldung über die Dropdown-Liste oben im Bildschirm ändern.

### Was geschieht, wenn ich einige der in der Dropdown-Liste für eine meiner Report Suites aufgelisteten Organisationen nicht kenne?

The list shows you all the *possible* organizations your report suite could be mapped to, even you don’t have permission to map to all those report suites. Wenn Sie sich nicht sicher sind, ob die Report Suite einer der grau ausgeblendeten Report Suites in der Liste zugeordnet werden soll, wenden Sie sich an einen Experience Cloud-Administrator in Ihrem Unternehmen, um die beste Auswahl zu ermitteln.

### Was geschieht, wenn ich einige der Firmen für die Anmeldung, die für eine Report Suite in der Spalte &quot;Sichtbare Firmen bei der Anmeldung&quot;aufgeführt sind, nicht erkenne?

Irgendwann wurde diese Report Suite für eine andere Firma freigegeben, die möglicherweise Teil eines anderen Experience Cloud-Unternehmens ist.

### Was bedeutet die Fehlermeldung über einen möglichen Konflikt bei einer Report Suite, die von einer anderen Organisation generiert wurde? Warum ist das wichtig?

Dies ist eine Benachrichtigung, die Sie bei einer informierten Entscheidung über die Zuordnung Ihrer Report Suite unterstützt. Wir möchten Sie darauf hinweisen, dass die Report Suite ursprünglich unter einer anderen Organisation erstellt wurde, falls diese Organisation für diese Report Suite geeigneter sein sollte.

### Woher weiß ich, ob eine Report Suite zugeordnet ist?

Zugeordnete Report Suites werden in einem nicht bearbeitbaren Format angezeigt. Wenn Sie eine Zuordnung ändern müssen, wenden Sie sich bitte an den Kundendienst.

### Was geschieht, wenn ich die Organisations-ID für mein Experience Cloud-Unternehmen kenne? Wo kann ich den Namen meiner Organisations-ID nachschlagen?

Sie finden Ihren Firmennamen in [Organisationen und Kontoeinstellungen](https://docs.adobe.com/content/help/de-DE/core-services/interface/manage-users-and-products/organizations.html).

### In der Spalte „Datum der Zuordnung“ ist ein Datum eingetragen. Wer hat diese Zuordnung gemacht?

Sie können das Report Suite-Änderungsprotokoll in der Benutzeroberfläche von Analytics verwenden, um die Benutzer-ID zu überprüfen, die die Änderung vorgenommen hat. Suchen Sie nach dem Ereignis &quot;Suite in Verbindung mit IMS-Organisation&quot;.
