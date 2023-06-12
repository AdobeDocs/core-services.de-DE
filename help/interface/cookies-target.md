---
description: Hier erfahren Sie, wie Adobe Target Cookies verwendet, um Website-Betreibern die Möglichkeit zu geben, zu testen, welche Online-Inhalte und Angebote für Besucher am relevantesten sind.
solution: Experience Cloud,Analytics,Target
title: Cookies in Adobe Target
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: a1d24f95b1ac567686d58af8adf0132e5beb8f2a
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 24%

---

# Cookies in Adobe Target

[!DNL Adobe Target] verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, die Relevanz von Online-Inhalten und -Angeboten für Besucher zu testen.

>[!NOTE]
>
>Die Informationen in diesem Artikel beziehen sich auf die [[!DNL Target] JavaScript-Bibliothek &quot;at.js&quot;](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=de){target=_blank} nur.
>
>Informationen zu Cookies, die in einer [!DNL Target] Implementierung mithilfe der [[!DNL Adobe Experience Platform Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html?lang=de){target=_blank}, see "Does the [!DNL Adobe Experience Platform Web SDK] use cookies? If so, what cookies does it use?" in [Frequently Asked questions in the DNL Platform Web SDK overview guide](https://experienceleague.adobe.com/docs/experience-platform/edge/web-sdk-faq.html){target=_blank}.
>
>Sie können bei Bedarf die in diesem Artikel besprochenen Einstellungen ändern, mit Ausnahme der Cookie-Dauer. [Wenden Sie sich beim Ändern der Cookie-Einstellungen an Ihren Kundenbetreuer.](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html?lang=de){target=_blank}
>
>[!DNL Target]Benutzer von können auch benutzerdefinierte Drittanbieter-Cookies erstellen.

## Erstanbieter-Cookies

Die folgenden Erstanbieter-Cookies werden in der Domäne des Kunden gespeichert:

| Cookie | Details |
| --- | --- |
| mbox | Speichert anonyme Kennungen zum Besucher.<P>**Cookie-Domäne**: Die Domäne, von der Sie die Mbox beliefern. Da dieses Cookie von der Domäne Ihres Unternehmens bereitgestellt wird, handelt es sich bei dem Cookie um ein Erstanbieter-Cookie. Beispiel: `mycompany.com`. Wenn einer Ihrer Domänennamen einen Ländercode enthält, z. B. `mycompany.co.uk`, konfigurieren Sie gemeinsam mit Ihren Kundendiensten at.js, um diesen Code zu unterstützen. Informationen zum Anpassen der Cookie-Domäne finden Sie bei Bedarf unter`cookieDomain`&quot; [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=de){target=_blank} im *[!DNL Adobe Target]Entwicklerhandbuch*.<P>**Serverdomäne**: `clientcode.tt.omtrdc.net`, wobei der Clientcode für Ihre [!DNL Target] -Konto.<P>**Cookie-Dauer**: Das Cookie verbleibt zwei Jahre nach der letzten Anmeldung im Browser des Besuchers. Die Dauer des Cookies kann nicht geändert werden.<P>Das Cookie enthält einige Werte, mit denen verwaltet werden kann, wie Ihre Besucher erleben [!DNL Target] Aktivitäten:<P>**session ID**: Eine eindeutige Kennung für eine bestimmte Benutzersitzung. Standardmäßig läuft die Sitzung nach 30 Minuten Inaktivität ab. Wenn Sie `sessionId` selbst (z. B. für [Serverseitige Implementierungen](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html){target=_blank}), stellen Sie Folgendes sicher:<ul><li>Die Sitzungs-ID kann eine beliebige druckbare Zeichenfolge sein, mit Ausnahme eines Leerzeichens, eines Fragezeichens ( ? ) und Schrägstrichen ( / ).</li><li>Die Sitzungs-ID sollte zwischen 1 und 128 Zeichen lang sein.</li><li>Für eine bestimmte Sitzung muss der Wert des Cookies über mehrere Anforderungen hinweg gleich bleiben.</li><li>Sie sollten niemals parallele Sitzungen (unterschiedliche `sessionIds`) für einen bestimmten Besucher zu einem beliebigen Zeitpunkt.</li></ul>Das Routing zu einem bestimmten Knoten im Edge-Cluster erfolgt mithilfe der Sitzungs-ID.<ul><li>Die Sitzung ist auf der Server-Seite 30 Minuten lang aktiv. Daher sollten Sie für eine bestimmte `tntId/thirdPartyId` innerhalb von 30 Minuten nach der letzten Anfrage mit der `tntId/thirdPartyId`. Andernfalls könnten Änderungen am Profil inkonsistent und unvorhersehbar sein.</li><li>Eine neue Sitzungs-ID muss nach einer Inaktivität von dreißig Minuten von einem Besucher verwendet werden.</li><li>Verwenden derselben Sitzungs-ID mit mehreren `tntIds/thirdPartyIds` kann zu unvorhersehbaren Änderungen an den Profilen führen, die von der `tntId/thirdPartyIDs`.</li></ul>HINWEIS: Siehe [Begrenzung der Anzahl gleichzeitiger Anfragen](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=de#content-delivery){target=_blank} für eine bestimmte Sitzungs-ID.<P>**pc ID**: Eine semi-permanente ID für den Browser eines Besuchers. Sie ist gültig, bis Cookies manuell gelöscht werden.<P>**check**: Ein einfacher Testwert, der bestimmt, ob ein Besucher Cookies unterstützt. Wird jedes Mal festgelegt, wenn ein Besucher eine Seite anfordert.<P>**disable**: Wird eingestellt, wenn die Ladezeit eines Besuchers den in der Datei at.js konfigurierten Timeout überschreitet. Standardmäßig ist diese Zeitüberschreitung eine Stunde gültig. |
| at_check | Temporäres Cookie, um zu überprüfen, ob die Lese-/Schreibfunktion des Cookies im Browser aktiviert ist. |
| mboxEdgeCluster | Diese Cookies sind nur vorhanden, wenn/wenn [overrideMboxEdgeServer-Einstellung](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=de){target=_blank} auf `true`. |

Es ist nicht möglich, HTTPOnly für diese Erstanbieter-Cookies zu verwenden. Die JavaScript-Bibliothek at.js muss in diese Cookies lesen/schreiben. Diese Cookies werden von at.js erstellt und nicht vom Server gesetzt.

Die `secure` -Einstellung kann für alle diese Cookies mit dem `secureOnly: true` Konfiguration in der at.js-Implementierung.

## Drittanbieter-Cookies

Die folgenden Drittanbieter-Cookies werden in gespeichert `tt.omtrdc.net`:

| Cookie | Details |
| --- | --- |
| customerclientcode!mboxPC | Dieses Cookie ist vorhanden, wenn domänenübergreifend aktiviert ist. |
| customerclientcode!mboxSession | Dieses Cookie ist vorhanden, wenn domänenübergreifend aktiviert ist. |

Diese Drittanbieter-Cookies sind standardmäßig HTTPOnly und werden von der [!DNL Target] Edge-Server.

Die `secure` -Einstellung kann für alle Cookies mit der `secureOnly: true` Konfiguration in der at.js-Implementierung.