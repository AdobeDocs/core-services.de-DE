---
description: Erfahren Sie [!DNL Adobe Target]  wie -Cookies verwendet, um Betreibern von Websites die Möglichkeit zu geben, zu testen, welche Online-Inhalte und -Angebote für Besucher relevanter sind.
solution: Experience Cloud,Analytics,Target
title: Cookies in Adobe Target
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
source-git-commit: 3ca021a0a2e6b0b6e265d35084d89d7720c28908
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 8%

---

# Cookies in Adobe Target

[!DNL Adobe Target] verwendet Cookies, um Betreibern von Websites die Möglichkeit zu geben, die Relevanz von Online-Inhalten und -Angeboten für Besucher zu testen.

>[!NOTE]
>
>Die Informationen in diesem Artikel gelten nur für die [[!DNL Target] at.js-JavaScript](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank}Bibliothek.
>
>Weitere Informationen über Cookies, die in einer [!DNL Target] Implementierung mit dem [[!DNL Adobe Experience Platform Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html?lang=de){target=_blank} verwendet werden, finden Sie unter „Verwendet der [!DNL Adobe Experience Platform Web SDK] Cookies? Wenn ja, welche Cookies werden verwendet?“ in [[!DNL Häufig gestellte Fragen im Handbuch Platform Web SDK - Übersicht]](https://experienceleague.adobe.com/docs/experience-platform/edge/web-sdk-faq.html){target=_blank}.
>
>Sie können die in diesem Artikel besprochenen Einstellungen bei Bedarf ändern, mit Ausnahme der Cookie-Dauer. [Wenden Sie sich beim Ändern ](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html){target=_blank} Cookie-Einstellungen an Ihren Kundenbetreuer.
>
>[!DNL Target] Benutzer können auch benutzerdefinierte Drittanbieter-Cookies erstellen.

## Erstanbieter-Cookies

Die folgenden Erstanbieter-Cookies werden in der Domain des Kunden gespeichert:

| Cookie | Details |
| --- | --- |
| mbox | Speichert anonyme Kennungen des Besuchers.<P>**Cookie-Domain**: Die Domain, von der aus Sie die Mbox bereitstellen. Da dieses Cookie von der Domain Ihres Unternehmens bereitgestellt wird, handelt es sich bei dem Cookie um ein Erstanbieter-Cookie. Beispiel: `mycompany.com`. Wenn einer Ihrer Domänennamen einen Ländercode enthält, wie z. B. `mycompany.co.uk`, konfigurieren Sie at.js gemeinsam mit Ihrem Kundendienst, damit dieser Domänenname unterstützt wird. Informationen zum Anpassen der Cookie-Domain, falls erforderlich, finden Sie unter &quot;`cookieDomain`&quot; unter [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} im *[!DNL Adobe Target]Entwicklerhandbuch*.<P>**Serverdomain**: `clientcode.tt.omtrdc.net`, wobei der Clientcode für Ihr [!DNL Target] verwendet wird.<P>**Cookie-Dauer**: Das Cookie verbleibt zwei Jahre nach der letzten Anmeldung im Browser des Besuchers. Die Dauer des Cookies kann nicht geändert werden.<P>Das Cookie enthält einige Werte, um zu verwalten, wie Ihre Besucher [!DNL Target] Aktivitäten erleben:<P>**Sitzungs-ID**: Eine eindeutige Kennung für eine bestimmte Benutzersitzung. Standardmäßig läuft die Sitzung nach 30 Minuten Inaktivität ab. Wenn Sie `sessionId` selbst generieren (z. B. für [Server-seitige Implementierungen](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html){target=_blank}), stellen Sie Folgendes sicher:<ul><li>Die Sitzungs-ID kann eine beliebige druckbare Zeichenfolge sein, mit Ausnahme von Leerzeichen, Fragezeichen ( ? ), geschweifte Klammern ( { } ) oder Schrägstrichen ( / ).</li><li>Die Sitzungs-ID sollte zwischen 1 und 128 Zeichen lang sein.</li><li>Für eine bestimmte Sitzung muss der -Wert des Cookies bei mehreren Anfragen gleich bleiben.</li><li>Sie sollten zu keinem Zeitpunkt parallele Sitzungen (verschiedene `sessionIds`) für einen bestimmten Besucher haben.</li></ul>Das Routing zu einem bestimmten Knoten im Edge-Cluster erfolgt mithilfe der Sitzungs-ID.<ul><li>Die Sitzung ist auf der Server-Seite 30 Minuten lang aktiv. Daher sollten Sie für eine bestimmte `tntId/thirdPartyId` innerhalb von 30 Minuten nach der letzten Anfrage mit der `tntId/thirdPartyId` keine andere Sitzungs-ID verwenden. Andernfalls könnten Änderungen am Profil inkonsistent und unvorhersehbar sein.</li><li>Nach dreißig Minuten Inaktivität eines Besuchers muss eine neue Sitzungs-ID verwendet werden.</li><li>Die Verwendung derselben Sitzungs-ID mit mehreren `tntIds/thirdPartyIds` kann zu unvorhersehbaren Änderungen an den Profilen führen, die vom `tntId/thirdPartyIDs` identifiziert werden.</li></ul>HINWEIS: Siehe [Begrenzung der Anzahl gleichzeitiger Anfragen](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=de#content-delivery){target=_blank} für eine bestimmte Sitzungs-ID.<P>**pc ID**: Eine semipermanente ID für den Browser eines Besuchers. Sie ist gültig, bis Cookies manuell gelöscht werden.<P>**check**: Ein einfacher Testwert, mit dem bestimmt wird, ob ein Besucher Cookies unterstützt. Wird jedes Mal festgelegt, wenn ein Besucher eine Seite anfordert.<P>**deaktivieren**: Wird festgelegt, wenn die Ladezeit eines Besuchers den in der Datei at.js konfigurierten Timeout überschreitet. Standardmäßig ist diese maximale Wartezeit eine Stunde gültig. |
| at_check | Temporäres Cookie, um zu überprüfen, ob die Lese-/Schreibfunktion des Cookies im Browser aktiviert ist. |
| mboxEdgeCluster | Dieses Cookie ist nur vorhanden, wenn/wenn [ Einstellung „overrideMboxEdgeServer](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} auf &quot;`true`&quot; gesetzt ist. |

Es ist nicht möglich, HTTPO nur für diese Erstanbieter-Cookies zu verwenden. Die at.js-JavaScript-Bibliothek muss diese Cookies lesen/schreiben. Diese Cookies werden von at.js erstellt und nicht vom Server festgelegt.

Die `secure` Einstellung kann für alle diese Cookies mithilfe der `secureOnly: true` in der at.js-Implementierung aktiviert werden.

## Drittanbieter-Cookies

Die folgenden Drittanbieter-Cookies werden auf `tt.omtrdc.net` gespeichert:

| Cookie | Details |
| --- | --- |
| customerClientCode!mboxPC | Dieses Cookie ist vorhanden, wenn domänenübergreifend aktiviert. |
| customerClientCode!mboxSession | Dieses Cookie ist vorhanden, wenn domänenübergreifend aktiviert. |

Diese Drittanbieter-Cookies sind standardmäßig HTTPOnly und werden von den [!DNL Target] Edge-Servern festgelegt.

Die `secure` Einstellung kann für alle Cookies mithilfe der `secureOnly: true` in der at.js-Implementierung aktiviert werden.