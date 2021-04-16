---
description: Hier erfahren Sie, wie Adobe Target Cookies verwendet, um Website-Betreibern die Möglichkeit zu geben, zu testen, welche Online-Inhalte und Angebote für Besucher am relevantesten sind.
keywords: Cookies, Datenschutz
solution: Experience Cloud,Analytics,Target,Social
title: 'Cookies in Adobe Target  '
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Administrator
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
translation-type: tm+mt
source-git-commit: dcb6fa5d8458995cba66bc2f89c954aa6bcd5923
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 55%

---

# Cookies in Adobe Target {#target-cookies}

Adobe Target verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, die Relevanz von Online-Inhalten und -Angeboten für Besucher zu testen.

Sie können diese Einstellungen bei Bedarf ändern, mit Ausnahme der Cookie-Dauer. Wenden Sie sich beim Ändern der Cookie-Einstellungen an Ihren Kundenbetreuer.

>[!NOTE]
>
>Benutzer von Adobe Target können auch benutzerdefinierte Drittanbieter-Cookies erstellen.

| Einstellung | Information |
| --- | --- |
| Cookie-Name | mbox. |
| Cookie-Domäne | Die zweite und oberste Ebene der Domänen, von denen Sie die mbox bedienen. Da die Belieferung von der Domäne Ihres Unternehmens stattfindet, handelt es sich um ein Erstanbieter-Cookie. Beispiel: `mycompany.com`. |
| Serverdomäne | `clientcode.tt.omtrdc.net`[!DNL Adobe Target], unter Verwendung des Kundencodes für Ihr Konto. |
| Cookie-Dauer | Das Cookie bleibt zwei Jahre nach der letzten Anmeldung des Besuchers in seinem Browser. Die Dauer des Cookies kann nicht geändert werden. |



>[!NOTE]
>
>Wenn einer Ihrer Domänennamen einen Ländercode enthält, wie beispielsweise `mycompany.co.uk`, konfigurieren Sie gemeinsam mit Ihrem Kundenservice die [!DNL at.js], damit dieser Domänenname unterstützt wird.

Das Cookie enthält eine Reihe von Werten, mit denen verwaltet werden kann, wie Ihre Besucher Adobe Target-Kampagnen erleben:

| Wert | Definition |
| --- | --- |
| session ID | Eine eindeutige ID für eine bestimmte Benutzersitzung. Standardmäßig läuft die Sitzung nach 30 Minuten Inaktivität ab. Wenn Sie sessionId selbst generieren (z. B. für serverseitige Implementierungen), stellen Sie Folgendes sicher:<ul><li>Die Sitzungs-ID kann jede druckbare Zeichenfolge sein, mit Ausnahme eines Leerzeichens, eines Fragezeichens ( ? ) oder einen Schrägstrich ( / ).</li><li>* Die Sitzungs-ID sollte zwischen 1 und 128 Zeichen lang sein.</li><li>Für eine bestimmte Sitzung muss der Wert für mehrere Anforderungen gleich bleiben</li><li>Sie sollten zu keinem Zeitpunkt parallele Sitzungen (eindeutige sessionIds) für einen bestimmten Besucher haben.</li></ul>Das Routing zu einem bestimmten Knoten im Edge-Cluster erfolgt mit der Sitzungs-ID.<ul><li>Die Sitzung ist auf der Serverseite 30 Minuten lang aktiv. Daher sollten Sie für ein bestimmtes `tntId/thirdPartyId` innerhalb von 30 Minuten nach der letzten Anforderung mit dem `tntId/thirdPartyId` keine andere Sitzungs-ID verwenden. Andernfalls könnten Änderungen am Profil inkonsistent und unvorhersehbar sein.</li><li>Die Verwendung derselben Sitzungs-ID mit mehreren `tntIds/thirdPartyIds` kann zu unvorhersehbaren Änderungen an den Profilen führen, die durch das `tntId/thirdPartyIDs` identifiziert werden.</li></ul> |
| pc ID | Eine semi-permanente ID für den Browser eines Besuchers. Sie ist gültig, bis Cookies manuell gelöscht werden. |
| check | Ein einfacher Testwert zur Bestimmung, ob ein Besucher Cookies unterstützt. Wird jedes Mal festgelegt, wenn ein Besucher eine Seite anfordert. |
| disable | Wird eingestellt, wenn die Ladezeit des Besuchers den in der Datei &quot;at.js&quot;konfigurierten Timeout überschreitet. Standardmäßig ist dieser Wert eine Stunde gültig. |

