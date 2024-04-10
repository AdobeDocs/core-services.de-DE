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
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 15%

---

# Cookies in Adobe Target

[!DNL Adobe Target] verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, zu testen, welche Online-Inhalte und -Angebote für Besucher relevanter sind.

>[!NOTE]
>
>Die Informationen in diesem Artikel gelten für [[!DNL Target] at.js-JavaScript-Bibliothek](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=de){target=_blank} Nur.
>
>Für Informationen über Cookies, die in einem [!DNL Target] Implementierung mithilfe der [[!DNL Adobe Experience Platform Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html?lang=de){target=_blank}, see "Does the [!DNL Adobe Experience Platform Web SDK] use cookies? If so, what cookies does it use?" in [Frequently Asked questions in the DNL Platform Web SDK overview guide](https://experienceleague.adobe.com/docs/experience-platform/edge/web-sdk-faq.html){target=_blank}.
>
>Sie können die in diesem Artikel besprochenen Einstellungen bei Bedarf ändern, mit Ausnahme der Cookie-Dauer. [Wenden Sie sich an Ihren Kontobeauftragten](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html?lang=de){target=_blank} beim Ändern der Cookie-Einstellungen.
>
>[!DNL Target] Benutzer können auch benutzerdefinierte Drittanbieter-Cookies erstellen.

## Erstanbieter-Cookies

Die folgenden Erstanbieter-Cookies werden in der Domain des Kunden gespeichert:

| Cookie | Details |
| --- | --- |
| mbox | Speichert anonyme Kennungen des Besuchers.<P>**Cookie-Domain**: Die Domain, von der aus Sie die Mbox bereitstellen. Da dieses Cookie von der Domain Ihres Unternehmens bereitgestellt wird, handelt es sich bei dem Cookie um ein Erstanbieter-Cookie. Beispiel: `mycompany.com`. Wenn einer Ihrer Domänennamen einen Ländercode enthält, z. B. `mycompany.co.uk`Wenden Sie sich an Ihren Client-Dienst, um at.js so zu konfigurieren, dass dieser Code unterstützt wird. Informationen zum Anpassen der Cookie-Domain, falls erforderlich, finden Sie unter &quot;`cookieDomain`&quot; unter [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=de){target=_blank} in der *[!DNL Adobe Target]Entwicklerhandbuch*.<P>**Serverdomäne**: `clientcode.tt.omtrdc.net`, unter Verwendung des Client-Codes für Ihre [!DNL Target] Konto.<P>**Cookie-Dauer**: Das Cookie verbleibt zwei Jahre nach der letzten Anmeldung im Browser des Besuchers. Die Dauer des Cookies kann nicht geändert werden.<P>Das Cookie speichert einige Werte, um zu verwalten, wie Ihre Besucher erleben [!DNL Target] Aktivitäten:<P>**Sitzungs-ID**: Eine eindeutige Kennung für eine bestimmte Benutzersitzung. Standardmäßig läuft die Sitzung nach 30 Minuten Inaktivität ab. Wenn Sie Folgendes erzeugen `sessionId` selbst (z. B. für [Server-seitige Implementierungen](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html?lang=de){target=_blank}), stellen Sie Folgendes sicher:<ul><li>Die Sitzungs-ID kann eine beliebige druckbare Zeichenfolge sein, mit Ausnahme von Leerzeichen, Fragezeichen ( ? ) und Schrägstrichen ( / ).</li><li>Die Sitzungs-ID sollte zwischen 1 und 128 Zeichen lang sein.</li><li>Für eine bestimmte Sitzung muss der Wert des Cookies bei mehreren Anfragen gleich bleiben.</li><li>Sie sollten nie parallele Sitzungen haben (unterschiedlich) `sessionIds`) für eine bestimmte Besucherin oder einen bestimmten Besucher zu einem beliebigen Zeitpunkt.</li></ul>Das Routing zu einem bestimmten Knoten im Edge-Cluster erfolgt mithilfe der Sitzungs-ID.<ul><li>Die Sitzung ist auf der Server-Seite 30 Minuten lang aktiv. Daher sollten Sie für eine bestimmte Sitzung keine andere Sitzungs-ID verwenden `tntId/thirdPartyId` innerhalb von 30 Minuten nach der letzten Anfrage an die `tntId/thirdPartyId`. Andernfalls könnten Änderungen am Profil inkonsistent und unvorhersehbar sein.</li><li>Nach dreißig Minuten Inaktivität eines Besuchers muss eine neue Sitzungs-ID verwendet werden.</li><li>Verwenden derselben Sitzungs-ID mit mehreren `tntIds/thirdPartyIds` kann zu unvorhersehbaren Änderungen an den Profilen führen, die von der `tntId/thirdPartyIDs`.</li></ul>HINWEIS: Siehe [Begrenzung der Anzahl gleichzeitiger Anfragen](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=de#content-delivery){target=_blank} für eine bestimmte Sitzungs-ID.<P>**PC-ID**: Eine semipermanente ID für den Browser eines Besuchers. Sie ist gültig, bis Cookies manuell gelöscht werden.<P>**nachprüfen**: Ein einfacher Testwert, mit dem bestimmt wird, ob ein Besucher Cookies unterstützt. Wird jedes Mal festgelegt, wenn ein Besucher eine Seite anfordert.<P>**deaktivieren**: Festlegen, ob die Ladezeit eines Besuchers den in der Datei at.js konfigurierten Timeout überschreitet. Standardmäßig beträgt diese maximale Wartezeit eine Stunde. |
| at_check | Temporäres Cookie, um zu überprüfen, ob die Lese-/Schreibfunktion des Cookies im Browser aktiviert ist. |
| mboxEdgeCluster | Dieses Cookie ist nur vorhanden, wenn/wenn [Einstellung von overrideMboxEdgeServer](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html?lang=de){target=_blank} ist festgelegt auf `true`. |

Es ist nicht möglich, HTTPOnly nur für diese Erstanbieter-Cookies zu verwenden. Die at.js-JavaScript-Bibliothek muss diese Cookies lesen/schreiben. Diese Cookies werden von at.js erstellt und nicht vom Server festgelegt.

Die `secure` Die -Einstellung kann für alle diese Cookies aktiviert werden, indem `secureOnly: true` Konfiguration in der at.js-Implementierung.

## Drittanbieter-Cookies

Die folgenden Drittanbieter-Cookies werden gespeichert unter `tt.omtrdc.net`:

| Cookie | Details |
| --- | --- |
| customerclientcode!mboxPC | Dieses Cookie ist vorhanden, wenn domänenübergreifend aktiviert ist. |
| customerclientcode!mboxSession | Dieses Cookie ist vorhanden, wenn domänenübergreifend aktiviert ist. |

Diese Drittanbieter-Cookies sind standardmäßig HTTPOnly und werden von der [!DNL Target] Edge-Server.

Die `secure` Die -Einstellung kann für alle Cookies mithilfe der `secureOnly: true` Konfiguration in der at.js-Implementierung.