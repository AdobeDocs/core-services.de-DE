---
description: Hier erfahren Sie, wie Adobe Target Cookies verwendet, um Website-Betreibern die Möglichkeit zu geben, zu testen, welche Online-Inhalte und Angebote für Besucher am relevantesten sind.
solution: Experience Cloud,Analytics,Target
title: Cookies in Adobe Target
feature: Cookies
topic: Administration
role: Administrator
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: ea50808d2514ff3c94ffa1bee2d9aa3ddf51f120
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 95%

---

# Cookies in Adobe Target{#target-cookies}

Adobe Target verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, die Relevanz von Online-Inhalten und -Angeboten für Besucher zu testen.

Sie können diese Einstellungen bei Bedarf ändern, mit Ausnahme der Dauer der Cookies. Wenden Sie sich beim Ändern der Cookie-Einstellungen an Ihren Kundenbetreuer.

>[!NOTE]
>
>Benutzer von Adobe Target können auch benutzerdefinierte Drittanbieter-Cookies erstellen.

| Einstellung | Information |
| --- | --- |
| Cookie-Name | mbox. |
| Cookie-Domäne | Die zweite und oberste Ebene der Domänen, von denen Sie die mbox bedienen. Da die Belieferung von der Domain Ihres Unternehmens stattfindet, handelt es sich um ein Erstanbieter-Cookie. Beispiel: `mycompany.com`. |
| Serverdomäne | `clientcode.tt.omtrdc.net`, unter Verwendung des Kundencodes für Ihr [!DNL Adobe Target] Konto. |
| Cookie-Dauer | Das Cookie bleibt zwei Jahre nach der letzten Anmeldung des Besuchers in seinem Browser. Die Dauer des Cookies kann nicht geändert werden. |



>[!NOTE]
>
>Wenn einer Ihrer Domänennamen einen Ländercode enthält, wie beispielsweise `mycompany.co.uk`, konfigurieren Sie gemeinsam mit Ihrem Kundenservice die [!DNL at.js], damit dieser Domänenname unterstützt wird.

Das Cookie enthält eine Reihe von Werten, mit denen verwaltet werden kann, wie Ihre Besucher Adobe Target-Kampagnen erleben:

| Wert | Definition |
| --- | --- |
| session ID | Eine eindeutige Kennung für eine Benutzersitzung. Standardmäßig läuft die Sitzung nach 30 Minuten Inaktivität ab. Wenn Sie die Sitzungs-ID selbst generieren (z. B. für Server-seitige Implementierungen), stellen Sie Folgendes sicher:<ul><li>Die Sitzungs-ID kann jede druckbare Zeichenfolge sein, mit Ausnahme von Leerzeichen, Fragezeichen ( ?  ) und Schrägstrichen ( / ).</li><li>* Die Sitzungs-ID muss zwischen 1 und 128 Zeichen lang sein.</li><li>Für eine bestimmte Sitzung muss der Wert für mehrere Anfragen gleich bleiben</li><li>Sie sollten zu keinem Zeitpunkt parallele Sitzungen (verschiedene Sitzungs-IDs) für einen bestimmten Besucher haben.</li></ul>Das Routing zu einem bestimmten Knoten im Edge-Cluster erfolgt mithilfe der Sitzungs-ID.<ul><li>Die Sitzung ist auf der Server-Seite 30 Minuten lang aktiv. Daher sollten Sie für eine bestimmte `tntId/thirdPartyId` innerhalb von 30 Minuten nach der letzten Anfrage mit der `tntId/thirdPartyId`. Andernfalls könnten Änderungen am Profil inkonsistent und unvorhersehbar sein.</li><li>Die Verwendung derselben Sitzungs-ID mit mehreren `tntIds/thirdPartyIds` kann zu unvorhersehbaren Änderungen an den Profilen führen, die durch die `tntId/thirdPartyIDs` identifiziert werden.</li></ul>**Hinweis**: Siehe [Begrenzung der Anzahl zeitgleicher Anfragen](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=de#content-delivery) für eine bestimmte Sitzungs-ID. |
| pc ID | Eine semi-permanente ID für den Browser eines Besuchers. Sie ist gültig, bis Cookies manuell gelöscht werden. |
| check | Ein einfacher Testwert zur Bestimmung, ob ein Besucher Cookies unterstützt. Wird jedes Mal festgelegt, wenn ein Besucher eine Seite anfordert. |
| disable | Wird festgelegt, wenn die Ladezeit des Besuchers den in der Datei at.js konfigurierten Timeout überschreitet. Standardmäßig ist dieser Wert eine Stunde gültig. |

