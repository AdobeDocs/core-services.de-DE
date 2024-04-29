---
description: Hier erfahren Sie, wie Adobe Target Cookies verwendet, um Website-Betreibern die Möglichkeit zu geben, zu testen, welche Online-Inhalte und Angebote für Besucher am relevantesten sind.
solution: Target
title: Cookies in Adobe Target
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: 9ee4d9b0e670dec35cda530892c49e36bf7cc107
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 18%

---

# Cookies in Adobe Target

Adobe Target verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, die Relevanz von Online-Inhalten und -Angeboten für Besucher zu testen.

>[!NOTE]
>
>Die Informationen in diesem Artikel gelten nur für die [Adobe Target JavaScript-Bibliothek](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=de){target=_blank} (`at.js`). Siehe [Adobe Experience Platform Web SDK-Cookies](web-sdk.md) für Informationen zu Target-Implementierungen mit dem Web SDK.
>
>Sie können bei Bedarf die in diesem Artikel besprochenen Einstellungen ändern, mit Ausnahme der Cookie-Dauer. [Kundenbetreuer konsultieren](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html?lang=de){target=_blank} beim Ändern der Cookie-Einstellungen.

## Erstanbieter-Cookies

Die folgenden Erstanbieter-Cookies werden in der Domäne des Kunden gespeichert:

| Cookie | Details |
| --- | --- |
| `mbox` | Speichert anonyme Kennungen zum Besucher.<P>**Cookie-Domäne**: Die Domäne, von der Sie die Mbox beliefern. Da dieses Cookie von der Domäne Ihres Unternehmens bereitgestellt wird, handelt es sich bei dem Cookie um ein Erstanbieter-Cookie. Wenn einer Ihrer Domänennamen einen Ländercode enthält, z. B. `example.co.uk`, arbeiten Sie mit Client Services zusammen, um `at.js` um diesen Code zu unterstützen. Informationen zum Anpassen der Cookie-Domäne finden Sie bei Bedarf unter `cookieDomain` under [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=de){target=_blank} im Adobe Target-Entwicklerhandbuch.<P>**Serverdomäne**: `clientcode.tt.omtrdc.net`, unter Verwendung des Clientcodes für Ihr Adobe Target-Konto.<P>**Cookie-Dauer**: Das Cookie verbleibt zwei Jahre nach der letzten Anmeldung im Browser des Besuchers. Die Dauer des Cookies kann nicht geändert werden.<P>Das Cookie enthält einige Werte, mit denen verwaltet werden kann, wie Ihre Besucher erleben [!DNL Target] Aktivitäten:<P>**session ID**: Eine eindeutige Kennung für eine bestimmte Benutzersitzung. Standardmäßig läuft die Sitzung nach 30 Minuten Inaktivität ab. Wenn Sie `sessionId` selbst (z. B. für [Serverseitige Implementierungen](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html?lang=de){target=_blank}), stellen Sie Folgendes sicher:<ul><li>Die Sitzungs-ID kann eine beliebige druckbare Zeichenfolge sein, mit Ausnahme eines Leerzeichens, eines Fragezeichens ( ? ) und Schrägstrichen ( / ).</li><li>Die Sitzungs-ID sollte zwischen 1 und 128 Zeichen lang sein.</li><li>Für eine bestimmte Sitzung muss der Wert des Cookies über mehrere Anforderungen hinweg gleich bleiben.</li><li>Sie sollten niemals parallele Sitzungen (unterschiedliche `sessionIds`) für einen bestimmten Besucher zu einem beliebigen Zeitpunkt.</li></ul>Das Routing zu einem bestimmten Knoten im Edge-Cluster erfolgt mithilfe der Sitzungs-ID.<ul><li>Die Sitzung ist auf der Server-Seite 30 Minuten lang aktiv. Daher sollten Sie für eine bestimmte `tntId/thirdPartyId` innerhalb von 30 Minuten nach der letzten Anfrage mit der `tntId/thirdPartyId`. Andernfalls könnten Änderungen am Profil inkonsistent und unvorhersehbar sein.</li><li>Eine neue Sitzungs-ID muss nach einer Inaktivität von dreißig Minuten von einem Besucher verwendet werden.</li><li>Verwenden derselben Sitzungs-ID mit mehreren `tntIds/thirdPartyIds` kann zu unvorhersehbaren Änderungen an den Profilen führen, die von der `tntId/thirdPartyIDs`.</li></ul>HINWEIS: Siehe [Begrenzung der Anzahl gleichzeitiger Anfragen](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html#content-delivery){target=_blank} für eine bestimmte Sitzungs-ID.<P>**pc ID**: Eine semi-permanente ID für den Browser eines Besuchers. Sie ist gültig, bis Cookies manuell gelöscht werden.<P>**check**: Ein einfacher Testwert, mit dem bestimmt wird, ob ein Besucher Cookies unterstützt. Wird jedes Mal festgelegt, wenn ein Besucher eine Seite anfordert.<P>**disable**: Wird eingestellt, wenn die Ladezeit eines Besuchers den in der Datei at.js konfigurierten Timeout überschreitet. Standardmäßig ist diese Zeitüberschreitung eine Stunde gültig. |
| `at_check` | Temporäres Cookie, um zu überprüfen, ob die Lese-/Schreibfunktion des Cookies im Browser aktiviert ist. |
| `mboxEdgeCluster` | Diese Cookies sind nur vorhanden, wenn/wenn [overrideMboxEdgeServer-Einstellung](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=de){target=_blank} auf `true`. |

Es ist nicht möglich `HTTPOnly` auf diesen Erstanbieter-Cookies. Die `at.js` Die JavaScript-Bibliothek muss in diese Cookies lesen/schreiben. Diese Cookies werden von `at.js` und werden nicht vom Server festgelegt.

Die `secure` -Einstellung kann für alle diese Cookies mit dem `secureOnly: true` Konfiguration in `at.js`.

## Drittanbieter-Cookies

Adobe Target-Benutzer können benutzerdefinierte Drittanbieter-Cookies erstellen. Die folgenden Drittanbieter-Cookies werden in gespeichert `tt.omtrdc.net`:

| Cookie | Details |
| --- | --- |
| `customerclientcode!mboxPC` | Vorhanden, wenn domänenübergreifend aktiviert ist. |
| `customerclientcode!mboxSession` | Vorhanden, wenn domänenübergreifend aktiviert ist. |

Diese Drittanbieter-Cookies sind standardmäßig HTTPOnly und werden von Adobe Target-Datenerfassungsservern gesetzt.

Die `secure` -Einstellung kann für alle Cookies mit der `secureOnly: true` Konfiguration in `at.js`.
