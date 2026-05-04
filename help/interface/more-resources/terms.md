---
description: Erfahren Sie mehr über Begriffe in Adobe CX Enterprise und darüber, wie sie sich in Creative Cloud unterscheiden.
solution: Experience Cloud
title: Terminologie
feature-set: Experience Cloud Services
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: 3799f806-2794-43ab-9e70-06ee693871e7
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: bdea9bc8-5600-45db-b85e-d74bb59dfcff
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 581cd64936e5740d6288564abd25b5dd358f0dc6
workflow-type: tm+mt
source-wordcount: 1273
ht-degree: 68%

---

# Terminologie

<!--
TQID: https://experienceleague.adobe.com/6wm7HcuAbaV1iV3AgN55dY5WR---BnMM7lJgN0HZDsk
-->

Eine Terminologiereferenz für CX Enterprise-Anwender und ggf. die Verwendung dieser Begriffe in Creative Cloud.

| Begriff | Creative Cloud | CX Enterprise |
| --- | ----- | ---- |
| **Asset** | In der Creative Cloud ist ein Asset normalerweise eine Bilddatei.<br>Bei Assets kann es sich um Ebenen in einer Photoshop-Datei, Folien in einer PowerPoint-Datei, Seiten in einem PDF-Dokument oder Dateien in einer ZIP-Datei handeln. | In CX Enterprise ist ein Asset ein digitales Dokument, Bild, Video oder Audio, das über mehrere Ausgabedarstellungen und Unter-Assets verfügen kann. Zu den Beispielen gehören:<ul><li>Datei</li><li>Dokument</li><li>Bild</li><li>Video</li><li>Audio-Clip</li><li>Präsentation</li><li>Bildvorlage</li><li>Videovorlage</li></ul> |
| **Attribut** | | Was Personen gemeinsam haben, wenn sie sich für ein [Segment](https://experienceleague.adobe.com/docs/analytics/components/segmentation/seg-home.html) qualifizieren. (Ähnlich wie ein [Merkmal](https://experienceleague.adobe.com/docs/audience-manager/user-guide/aam-glossary.html) in Audience Manager.) |
| **Zielgruppen** | In der Creative Cloud kann eine Zielgruppe die Person sein, die ein Video aufruft. | In CX Enterprise sind Zielgruppen Sammlungen von Personen, die Sie in Kampagnenaktivitäten ansprechen können.<br>Die Zugehörigkeit zu einer Zielgruppe kann auf Basis eines Regelsatzes im Besucherkontext ermittelt werden oder in einer Liste festgelegt sein. Beispielsweise einer Liste mit E-Mail-Abonnenten oder Mitgliedern einer Facebook-Gruppe.<br>In [CX Enterprise Audiences](../services/audiences/overview.md) ist das Erstellen und Verwalten von Audiences mit dem Erstellen und Verwalten von Segmenten vergleichbar, hinzu kommt jedoch die Möglichkeit, dass die Audiences für CX Enterprise freigegeben werden können.<br>**Adobe Target**<br> In Adobe Target wurden Audiences zuvor als Segmente bezeichnet.<br>**Adobe Analytics:**<br> In Analytics können Zielgruppen als Besucher einer Website betrachtet werden. Sie können Zielgruppensegmente erstellen und die Zielgruppe in CX Enterprise veröffentlichen. |
| **Kampagnen** | In der Creative Cloud versteht man unter einer Kampagne eine Marketing-Kampagne, bei der Bild-Assets aus der Creative Cloud verwendet werden. | In CX Enterprise bestimmen Kampagnen, welche Inhalte der Zielgruppe angezeigt werden. Sie bestimmen auch, wo (Position) der Inhalt angezeigt wird und wann. Eine Kampagne hat ein bestimmtes Ziel, das von Metriken verfolgt wird.<br>Die Durchführung einer Kampagne setzt voraus, dass der Besucherkontext mit dem Regelsatz der Kampagne übereinstimmt und der Inhalt gemäß den technischen Einschränkungen des Kanals der Position bereitgestellt wird.<br>In Adobe Target sind die Begriffe Kampagne und Aktivität synonym. |
| **Kanal** | In der Creative Cloud können Kanäle Graustufenbilder sein, die verschiedene Arten von Informationen speichern. Es sind in diesem Fall Informationskanäle und Farbkanäle. | In CX Enterprise ist ein Kanal ein Attribut eines Standorts oder eine Aktivität in einer Kampagne.<br>In Analytics werden Marketing-Kanäle zumeist verwendet, um Einblicke dazu zu bieten, wie Besucher auf Ihre Website gelangen, beispielsweise über E-Mail-Kampagnen.<br>Zu den Beispielen gehören:<ul><li>E-Mail</li><li>Display-Anzeigen</li><li>Soziale Netzwerke</li><li>Paid Search</li><li>Normale Suche</li><li>Referrerdomänen</li></ul> |
| **Inhalt** | In Creative Cloud bezieht sich Inhalt auf den Text und die Bilder einer Seite. Der Begriff wird in ähnlicher Weise bei Creative und CX Enterprises verwendet. | In CX Enterprise bezieht sich Inhalt auf Marketing-Inhalte, die im Rahmen einer Kampagne verwendet werden können, um ein bestimmtes Ziel zu unterstützen.<br>Der Inhalt wird in bestimmten Positionen verwendet und kann aus Assets bestehen. Inhalt kann strukturiert (wie Produktinformationen) oder unstrukturiert (wie eine Webseite oder ein Bildschirm einer mobilen Anwendung) sein.<br>Zu den Beispielen gehören:<ul><li>Webseiten</li><li>Banner</li><li>Statusaktualisierungen</li><li>Kommentare</li><li>Textwerbung</li><li>Produktinformationen</li><li>Produktprüfungen</li><li>Formulardaten</li><li>Dokumente in einem Suchindex</li><li>Social-Beiträge</li><li>Artikel</li><li>Veröffentlichungen</li></ul> |
| **Dashboard** | Keine festgeschriebene Verwendung. | Eine Sammlung von Datenvisualisierungen, die mehrere Schlüsselmetriken in einer einzelne Ansicht überlagern. |
| **Durchsetzung der Datennutzung** | Keine festgeschriebene Verwendung. | Die Richtlinien, das System-Design, die Praktiken und Verfahren (Programme, Apps, Services, SDKs, APIs usw.), die in einem System festgelegt und definiert wurden, um mithilfe von Metadaten zur Datenverwendung die Einhaltung der Datenschutzrichtlinien von Adobe, der vertraglichen Erwägungen und der allgemeinen Datenschutzgrundsätze zu ermöglichen. |
| **Gerät** | Keine festgeschriebene Verwendung. | Ein Hardware-Gerät wie ein Tablet, Smartphone oder Desktop, auf dem Anwendungen ausgeführt werden. |
| **Device Co-op** | Keine festgeschriebene Verwendung. | Eine Gruppe von Marken, die sich bereit erklärt haben, Daten über die Geräte auszutauschen, die von den Verbrauchern verwendet werden, um eine bessere Identifikation des einzelnen Geräts und ein bedeutenderes, konsistenteres Erlebnis zu gewährleisten. |
| **[!UICONTROL CX Enterprise ID Service] (ECID)** | Keine festgeschriebene Verwendung. | Die eindeutige, beständige ID, die einem Site-Besucher zugewiesen ist. Dies ist eine bestimmte Entität, die vom Experience Platform Identity Service verwendet werden kann. [Mehr...](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=de) |
| **[!UICONTROL Experience Platform Identity Service]** | Keine festgeschriebene Verwendung. | Der Service, der Identitäten verknüpft. Es handelt sich dabei um den Service zum Verknüpfen von Geräten für das personenbasierte Erlebnis-Management. |
| **Verknüpfung** | Keine festgeschriebene Verwendung. „Verknüpfung“ bezieht sich auf die Navigation via Hyperlinks sowie auf die Verknüpfung von Elementen wie Schriften, Eigenschaften, Ebenen usw. | In CX Enterprise bezieht sich die Verknüpfung normalerweise auf die Verknüpfung verschiedener Programmkonten mit der Benutzeroberfläche.<br>Siehe [Organisationen und Kontoverknüpfung](../administration/organizations.md).<br>Verknüpfung bezieht sich auch auf die an andere Benutzer gesendeten Standard-URLs für Analytics-Berichte. |
| **Standorte** | In der Creative Cloud bezieht sich der Ort auf Dateispeicherorte oder auf eine Stelle auf einem geöffneten Bild oder einem geöffneten Dokument. | In CX Enterprise sind Speicherorte die Orte, an denen Inhalte von Zielgruppen angezeigt werden (und mit denen interagiert werden kann). Die Verbindung von Position und Inhalt kann mehr oder weniger statisch sein oder dynamisch gemäß den Regeln einer Kampagne verwaltet werden. Ein Standort gehört immer zu einem bestimmten Kanal, der bestimmt, wie Inhalte bereitgestellt und Metriken erfasst werden können.<br>Zu den Beispielen gehören:<ul><li>Seiten</li><li>Eigenschaften (Social)</li><li>Inventar anzeigen</li><li>Landingpages</li><li>Apps</li><li>Slots (Video)</li></ul> |
| **Metriken** | Wird nicht in Creative Cloud verwendet. | Gesamtzahlen zu Schlüsselkonzepten und -zielen. In Analytics sind Metriken quantitative Informationen über Besucheraktivitäten, wie Ansichten, Select-Throughs, Neuladungen, durchschnittliche Besuchszeit, Einheiten, Bestellungen, Umsatz usw. |
| **Organisation** | Wird nicht in Creative Cloud verwendet. | Eine Organisation ist eine CX Enterprise-Entität, mit der ein Administrator Benutzer und Produkte konfigurieren und Single Sign-on in CX Enterprise steuern kann. Meistens handelt es sich bei der Organisation um das abrechnende Unternehmen. |
| **Portfolio** | Eine Zusammenstellung aus mehreren Dateien oder Assets. | Ein Container mit Kampagnen. |
| **Produktprofil** | Siehe [Verwalten von Produkten und Profilen](https://helpx.adobe.com/de/enterprise/using/manage-products.html). | Damit ein Benutzer berechtigt sein kann, ein Produkt oder einen Service zu verwenden, muss er Teil eines Produktprofils sein. Der Produktadministrator weist einem Produktprofil Lizenzen zu, indem er es mit einem von Ihnen erworbenen Plan verknüpft.<br>Ein Benutzer kann mehreren Produktprofilen angehören, von denen jede dem Benutzer andere Lizenzen verleiht. Die finale Eignung eines Benutzers ist die Vereinigung aller Lizenzen, die er von den einzelnen Produktprofilen erhält. |
| **Planung** | Kann sich auf eine Folge von Szenen in Adobe Story oder auf geplante Aufgaben in ColdFusion beziehen. | In CX Enterprise ist ein Zeitplan das Startdatum (Jahr, Monat, Tag) und Enddatum für die Aktivierung von Kampagnen, Kanälen und Aktivitäten. Zeitpläne für Aktivitäten haben eine bis auf die Minute gestaffelte Granularität. Beim Ändern eines Zeitplans wird eine Karte erstellt.<br>Zu den Beispielen gehören:<ul><li>Kampagnenzeitpläne</li><li>Kanalzeitpläne</li><li>Aktivitätszeitpläne</li></ul> |
| **Segment** | K. A. | Die Ausgabe eines Regelsatzes zur Qualifizierung einer Zielgruppe. In Analytics können [Segmente](https://experienceleague.adobe.com/docs/analytics/components/segmentation/seg-home.html) optional verwendet werden, um eine Zielgruppe zu definieren, die an CX Enterprise übergeben werden kann. <br>In Audience Manager ist ein Segment eine Sammlung von [Merkmalen](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/traits/traits-overview.html) und allen Kriterien, die Besucher für die Zugehörigkeit zu diesem oder Aufnahme in dieses Segment qualifizieren. Es ist auch eine Sammlung von Personen, die diese allgemeinen Attribute teilen. |
| **Freigabe** | In Creative Cloud können Dateien extern über Plattformen freigegeben werden (soziale Medien, Communitys, E-Mails usw.). | In CX Enterprise können Assets nur als Karte innerhalb der Pinnwände in der Benutzeroberfläche freigegeben werden. Die Freigabe steht allen Personen zur Verfügung, die bei der Site angemeldet sind. |
| **Lösung** | Keine festgeschriebene Verwendung. | In CX Enterprise sind Anwendungen Produkte wie Adobe Analytics, Adobe Target usw. |
| **Eigenschaft** | k. A. | Ein Schlüssel-Wert-Paar, z. B. color=blue. In Audience Manager werden [Merkmale](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/traits/traits-overview.html) zum Erstellen von Segmenten verwendet. |

{style="table-layout:auto"}

