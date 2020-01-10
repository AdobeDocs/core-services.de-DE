---
description: Erfahren Sie mehr über den Workflow der Angebotsverwaltung auf hoher Ebene, einschließlich der Erstellung von Platzierungen und Angeboten, des Einfügen von Angebotsaktivitäten und des Anzeigen von Berichten.
seo-description: Erfahren Sie mehr über den Workflow der Angebotsverwaltung auf hoher Ebene, einschließlich der Erstellung von Platzierungen und Angeboten, des Einfügen von Angebotsaktivitäten und des Anzeigen von Berichten.
seo-title: Arbeitsablauf der Angebotsverwaltung
title: Arbeitsablauf der Angebotsverwaltung
uuid: c95ec474-88de-4e6e-92bf-f49f3a7b32c5
index: y
internal: n
snippet: y
translation-type: tm+mt
source-git-commit: 2f0c2eb70313c42da9e7ac1d75429ec768dea10d

---


# Arbeitsablauf der Angebotsverwaltung{#offer-management-workflow}

Erfahren Sie mehr über den Arbeitsablauf auf hoher Ebene im Bereich [!UICONTROL Angebotsverwaltung], einschließlich Platzierung und Angebotserstellung, Einfügen von Angebotsaktivitäten und Anzeigen von Berichten.

## Schritt 1 - Bestimmen Sie, wo in Ihren E-Mail-Vorlagen personalisierte Angebote erforderlich sind {#section_F184E589428B403EA8EB921BF230CF87}

Identifizieren Sie, in welche E-Mail-Kampagnen Sie personalisierte Angebote einfügen möchten. Legen Sie von dort die Orte in Ihrer E-Mail-Vorlage fest, an denen diese Angebote eingefügt werden sollen. Sie können beispielsweise das Produktangebot auf Grundlage der Branche oder der Person des Kunden ändern, die Nachricht auf der Grundlage derselben Kriterien ändern und das Bild je nach der geografischen Lage des Kunden variieren.

![](assets/workflow1.png)

## Schritt 2: Bestimmen Sie, welche Attribute aus der Kampagne Sie als Ziel auswählen und für das Angebotsmanagement freigeben möchten {#section_1461F1FAC0B943E5BBDED6B3B00E9D5C}

Beim Erstellen eines Angebots in der [!UICONTROL Angebotsverwaltung]können Sie Berechtigungsregeln festlegen, die beschränken, welche Profile bestimmte Angebote erhalten können. Diese Berechtigungsregeln können auf Grundlage von Attributen (oder Feldern) festgelegt werden, die in Adobe Campaign vorhanden sind. Diese Felder müssen von einem Benutzer auf Administratorebene in Kampagne freigegeben werden, bevor sie im Regelaufbau für die [!UICONTROL Angebotsverwaltung] angezeigt werden.

Informationen zum Freigeben dieser Attribute finden Sie unter [Freigeben von Attributen von Kampagne zu Angebotsverwaltung](campaign.md#task_4DFA9A20D7B04E1F9AFF4774D67B6EBC).

## Schritt 3: Erforderliche Platzierungen in der [!UICONTROL Angebotsverwaltung] eingeben {#section_71619756A86F4DB58B8200D8A1CE1B87}

Eine Platzierung hilft sicherzustellen, dass der richtige Angebotsinhalt an der richtigen Stelle in Ihrer E-Mail-Vorlage angezeigt wird. Wenn Sie einem Angebot Inhalte hinzufügen, werden Sie aufgefordert, eine Platzierung auszuwählen, an der der Inhalt angezeigt werden kann.

Sie können mehrere Orte mit derselben Platzierung haben. Im folgenden Beispiel gibt es zwei Platzierungen für zwei Bilder unterschiedlicher Größe und eine Platzierung für den Text, der oben und unten in der Vorlage angezeigt wird.

Nachdem Sie die benötigten Platzierungen festgelegt haben, können Sie sie der Registerkarte &quot; [!UICONTROL Platzierung] &quot;hinzufügen.

![](assets/workflow2.png)

## Schritt 4: Erstellen Ihrer Angebote {#section_C4F9732B0596425EB0BD5AE76E4BA6EF}

Erstellen Sie die Angebote, die Sie in Ihrer E-Mail-Kampagne verwenden werden. Es gibt Daten und Inhalte, die dem Angebot hinzugefügt werden können, um das beste Angebot für die Bereitstellung zu ermitteln und festzulegen, welche Inhalte angezeigt werden sollen. Wenn Sie eine Inhaltsdarstellung erstellen, verknüpfen Sie sie mit einer der unter [Platzierungen](placements.md)definierten Platzierungen. Nachdem Sie ein Angebot erstellt und übermittelt haben, kann es in einer Angebotsaktivität verwendet werden.

![](assets/workflow3.png)

## Schritt 5: Erstellen Sie Ihre E-Mail-Kampagne und fügen Sie eine Angebotsaktivität ein {#section_6FD36404759B4C6E9FD3A65ACABB26C8}

Nachdem Sie Ihre Angebote erstellt haben, können Sie sie in einer E-Mail-Kampagne verwenden. Im Content Editor können Sie einen Block auswählen und eine Angebotsaktivität einfügen. Mit einer Angebotsaktivität können Sie eine Angebotsgruppe aus Ihrem Angebotsbestand auswählen, aus der die Entscheidungsmaschine das beste Angebot für jeden Benutzer ermittelt.

![](assets/workflow4.png)

## Schritt 6: Vorbereitung und Senden Ihrer E-Mail-Kampagne {#section_EDD8EA4696664130A678D7C4483DA806}

Wenn Sie nun Ihre E-Mail-Kampagne vorbereiten, bestimmt die [!UICONTROL Angebotsverwaltung] anhand des aktuellen Datums, der Profilattribute und der Priorität das beste Angebot für jeden Besucher. Es wird auch bestimmt, ob eine Inhaltsdarstellung für die Platzierung dieses Orts verfügbar ist.

Im folgenden Beispiel nehmen Sie an, dass Sie eine E-Mail-Kampagne mit einer Angebotsaktivität eingerichtet haben, die 3 Angebote enthält (A, B, C). Sie können festlegen, welches Angebot an einer der Orte in unserer E-Mail bereitgestellt werden soll. Zur Vorbereitung wird [!UICONTROL Angebotsverwaltung] :

1. Analysieren Sie das aktuelle Datum, die Profildaten der einzelnen Benutzer und die Priorität.
1. Vergleichen Sie diese Informationen mit den Daten in den Angeboten.
1. Legen Sie das beste Angebot fest, das bereitgestellt werden soll.

![](assets/workflow5.png)

## Schritt 7: Berichte anzeigen {#section_2104BAACAE154DE29B6EEB967C46F226}

Sie können einen Bericht darüber anzeigen, welche Angebote bereitgestellt wurden und wie sie in einer Angebotsaktivität ausgeführt wurden. Dieser Bericht kann durch Auswahl der Registerkarte &quot;Berichte&quot;auf der Homepage von Adobe Campaign Standard angezeigt werden.
