---
description: Erfahren Sie, wie Sie CX Enterprise-Trigger konfigurieren.
solution: Experience Cloud
title: Übersicht über Triggers
uuid: dab536e3-1969-4661-919e-5b15f423fecd
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 9dc26e2f-479b-49a5-93ce-b877559fea43
TQID: https://experienceleague.adobe.com/1R70ZEmKiP9VhhSRVCXHjGoJbOb7Mh8spKRm4FgNRPc
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2: id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2: id: b75843fa-0a67-4a44-a6b1-cc627b0481dcid: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: d3cdead0-685a-4489-9250-4bb709942f66id: e0eb8757-182f-49f3-94a4-1587d16f5094id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e56a5463246fe74bd7393de446687b6464760db1
workflow-type: tm+mt
source-wordcount: 817
ht-degree: 67%

---

# CX Enterprise-Trigger

Mit [!UICONTROL Trigger] in CX Enterprise können Sie wichtige Kundenverhaltensweisen identifizieren, definieren und überwachen. Anschließend können Sie eine programmübergreifende Kommunikation generieren, um erneut mit Besuchern zu interagieren. Sie können Trigger bei Echtzeit-Entscheidungen und Personalisierungen verwenden. Weitere Informationen zur Verwendung von [!UICONTROL Trigger] mit Adobe Campaign finden Sie unter [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard/using/integrating-with-adobe-cloud/working-with-campaign-and-triggers/using-triggers-in-campaign.html?lang=de).

Beispiel:

* Konfigurieren des schnellen Remarketing für Warenkorbabbrüche oder Warenkorbabbrüche mit entfernten Produkten
* Unvollständige Formulare und Anwendungen
* Aktionen oder Abfolgen von Aktionen auf der Site

![Trigger-Beispiel](../assets/trigger-abandonment-2.png)

>[!NOTE]
>
>Trigger sind nicht deterministisch. Wenn mehrere Benutzende einen Browser oder ein Gerät freigeben, z. B. ein freigegebenes oder ein öffentliches Gerät, ist es möglicherweise nicht möglich, einen Trigger der richtigen Besucher-ID zuzuordnen.

## Typen von Triggern

Im Allgemeinen kann ein Auslöser 15 bis 90 Minuten benötigen, um eine Marketing-Kampagne zu starten. Diese Verzögerung hängt von der Implementierung der Datenerfassung, der Auslastung der Pipeline, der benutzerdefinierten Konfiguration des definierten Triggers und dem Workflow in Adobe Campaign ab.

* **Abbruch:** Sie können einen Auslöser für den Fall erstellen, dass ein Besucher ein Produkt anzeigt, es jedoch nicht zum Warenkorb hinzufügt.
* **Aktion:** Sie können Sie Trigger erstellen, die beispielsweise nach der Newsletter-Anmeldung, E-Mail-Abonnements oder Kreditkartenanträgen (Bestätigungen) ausgelöst werden. Wenn Sie ein Händler sind, können Sie einen Trigger für einen Besucher erstellen, der sich für ein Treueprogramm anmeldet. Erstellen Sie in Medien und Unterhaltung Trigger für Besucher, die eine bestimmte Sendung ansehen. Sie können auch mit einer Umfrage reagieren.
* **Sitzungsbeginn und Sitzungsende:** Erstellen Sie einen Trigger für die Sitzungsbeginn- und Sitzungsende-Ereignisse.

## Erstellen eines CX Enterprise-Triggers

Erstellen Sie einen Trigger und konfigurieren Sie die Bedingungen für den Trigger. Sie können beispielsweise die Kriterien für die Regeln eines Triggers während eines Besuchs angeben, z. B. Metriken wie Warenkorbabbruch oder Dimensionen wie den Produktnamen. Wenn die Regeln erfüllt sind, wird der Trigger ausgeführt.

>[!NOTE]
>
>Derzeit existiert eine technische Begrenzung von 100 Triggern.

1. Klicken Sie in CX Enterprise auf ![Menü](../assets/menu-icon.png) und dann auf **[!UICONTROL Datenerfassung/Launch]**.
1. Klicken Sie auf der Karte {]}Trigger **[!UICONTROL auf &quot;Trigger verwalten]**.[!UICONTROL 
1. Klicken Sie **[!UICONTROL Neuer Trigger]** und geben Sie dann den Typ des Triggers an:

   ![Schritt Ergebnis](../assets/add-trigger.png)

1. Konfigurieren Sie den Auslöser, indem Sie die folgenden Felder vervollständigen und Metrik- und Dimensionselemente in die Regelbehälter ziehen:

   | Element | Beschreibung |
   | --- | --- |
   | [!UICONTROL Name] | Der Anzeigename für diesen Trigger. |
   | [!UICONTROL Beschreibung] | Die Beschreibung dieses Triggers, wie Sie ihn verwenden werden usw. |
   | [!UICONTROL Report Suite] | Die für diesen Trigger verwendete Analytics [Report Suite](https://experienceleague.adobe.com/docs/analytics/admin/manage-report-suites/report-suites-admin.html?lang=de). Diese Einstellung identifiziert die zu verwendenden Berichtsdaten. |
   | Besuch muss beinhalten<br>Besuch darf nicht beinhalten<br>Trigger nach ausbleibender Aktion<br>Metadaten einschließen | Sie können Kriterien oder Besucherverhalten, das auftreten soll, sowie Verhalten, das nicht auftreten soll, definieren. Regeln für einen einfachen Warenkorbabbruchs-Trigger können beispielsweise die folgenden sein:<ul><li>Besuch muss Folgendes beinhalten: [!UICONTROL Zusatz zum Warenkorb] (Metrik) und [!UICONTROL Vorhanden]. (Sie können die Regel mit einer bestimmten Produktansicht oder mit Dimensionen wie „Browsertypen“ weiter verfeinern.)</li><li>Besuch darf Folgendes nicht beinhalten: [!UICONTROL Checkout].</li><li>Auslöser nach ausbleibender Aktion bei: 10 Minuten.</li><li>[!UICONTROL Meta-Daten einschließen]: Ermöglicht das Hinzufügen einer bestimmten [!DNL Campaign] Dimension oder von Variablen, die für das Verhalten einer Besucherin oder eines Besuchers relevant sind. Dieses Feld kann für Adobe Campaign zum Verfassen der richtigen Remarketing-E-Mail nützlich sein.</li></ul><br>Sie können [!UICONTROL Beliebig], [!UICONTROL Und] oder [!UICONTROL Oder] Logik innerhalb oder zwischen Containern angeben, je nachdem, welche Kriterien Sie für die Regel für wichtig halten. |
   | [!UICONTROL Container] | In [!UICONTROL Containern] legen Sie Regeln, Bedingungen oder Filter zum Definieren eines Triggers fest und speichern diese. Wenn Sie Ereignisse gleichzeitig auftreten sollen, platzieren Sie sie im selben Container. Dies bedeutet, dass jeder Behälter unabhängig auf der Trefferebene arbeitet. Wenn Sie beispielsweise zwei Behälter mit dem Operator AND verbinden, treffen die Regeln zu, wenn zwei Treffer die Anforderungen erfüllen. |
   | Neue Sitzung starten nach | Erstellen Sie einen Trigger für die Ereignisse zum Sitzungsbeginn und Sitzungsende. |

   {style="table-layout:auto"}

1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. Verwenden Sie Trigger zum [Echtzeit-Remarketing](https://experienceleague.adobe.com/docs/campaign-standard/using/integrating-with-adobe-cloud/working-with-campaign-and-triggers/about-adobe-experience-cloud-triggers.html?lang=de) in [!DNL Adobe Campaign].

## Beispielauslöser

Beispiele für CX Enterprise-Trigger:

### Warenkorbabbruch - Trigger

Die folgende Seite zeigt beispielsweise Regeln, die Sie für einen Trigger [!UICONTROL Warenkorbabbruch] basierend auf Produkten, die während eines Besuchs angesehen wurden, verwenden können.

![Warenkorbabbruch-Trigger](../assets/abandonment-trigger.png)

### Referrer-Trigger

Der folgende Trigger wird ausgelöst, wenn ein Treffer mit dem Produkt „Herrenstiefel“ und Referrer „Facebook“ eingeht. Für die beiden Kriterien (*Produkte* und *Referrer*), die für denselben Treffer auszuwerten sind, sollten sie demselben Container hinzugefügt werden.

![Referrer-Trigger](../assets/fb-boots-promo.png)

## Überprüfen der Trigger-Aktivität

Um sicherzustellen, dass ein Trigger ausgelöst wurde, verwenden Sie die [!UICONTROL Trigger]-Schnittstelle, um die letzten Aktivitäten für den Trigger zu überprüfen. Auf der -Benutzeroberfläche wird eine begrenzte Anzahl von Trigger-Ereignissen der letzten Zeit angezeigt, sodass bei Implementierungen mit hohen Datenmengen möglicherweise nicht alle Trigger -Aktivitäten angezeigt werden. Die programmgesteuerte Überprüfung über eine API wird derzeit nicht unterstützt.
