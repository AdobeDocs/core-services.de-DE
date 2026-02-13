---
description: Hier erfahren Sie, wie Lösungen und Services in Adobe Experience Cloud Cookies verwenden.
title: Verwendung von Cookies in Experience Cloud
uuid: 4255a13a-917b-4b5f-a7d4-4b2e7521d189
exl-id: 60f1a89e-d989-461b-a6a3-c1df022cd30b
TQID: https://experienceleague.adobe.com/GH5WHcI9440NKYpUzizHlhOMlBSf-Y0WQ5GDBaSvqNI
product_v2: id: e1971122-7081-4556-9222-8a31bd71800c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: d095671a-1355-40aa-8b5f-06c33c68080bid: d3cdead0-685a-4489-9250-4bb709942f66id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 0d253888322194189fea6d492ae19cf248357960
workflow-type: tm+mt
source-wordcount: 600
ht-degree: 11%

---

# Verwenden von Cookies in Experience Cloud

Adobe Experience Cloud verwendet Cookies. Ein Cookie ist ein kleines Datenelement, das eine Website an Ihren Browser sendet, der es zur späteren Verwendung speichert. Cookies helfen der Website, sich Dinge zu merken, wenn Sie erneut besuchen oder zwischen Seiten wechseln. Cookies helfen dabei, Besuche zu verfolgen und ein Gerät vom anderen zu unterscheiden.

Gesetze verlangen oft, dass man eine Erlaubnis einholt, bevor man Cookies auf dem Gerät einer Person speichert oder verwendet. Adobe empfiehlt, sich mit Ihrer Rechtsabteilung in Verbindung zu setzen, um die geltenden Regeln zu verstehen.

## Informationen zu Erstanbieter-Cookies

Adobe Experience Cloud verwendet Cookies, um Informationen zu verfolgen, die zwischen Seitenansichten oder Browser-Sitzungen nicht dauerhaft sind. Wenn möglich, verwendet Adobe Erstanbieter-Cookies (die an Ihre eigene Website gebunden sind). Um Aktivitäten über mehrere Sites oder Domains hinweg zu verfolgen, deren Inhaber Sie sind, werden Drittanbieter-Cookies benötigt.

Einige Browser und Anti-Spyware-Tools blockieren Cookies von Drittanbietern. Adobe bietet Möglichkeiten, sicherzustellen, dass Cookies auch dann funktionieren, wenn Cookies blockiert sind. Wie dies funktioniert, hängt davon ab, ob Sie Experience Platform Identity Service (ECID) oder ältere Analytics-Cookies (wie das `s_vi`-Cookie) verwenden:

* [Experience Cloud Identity Service](https://experienceleague.adobe.com/en/docs/id-service/using/intro/overview): Der ECID-Service setzt immer Erstanbieter-Cookies, unabhängig davon, ob Ihre Erfassungs-Domain mit Ihrer Website-Domain übereinstimmt. Es verwendet JavaScript, um das Cookie in der Domain Ihrer Site zu platzieren.

* [Legacy-IDs von Analytics](analytics.md) (z. B. das `s_vi`-Cookie): Ob Cookies Erstanbieter- oder Drittanbieter-Cookies sind, hängt von Ihrer Einrichtung ab:

   * Wenn Ihr Datenerfassungsserver mit der Domain Ihrer Website übereinstimmt, sind Cookies Erstanbieter.
   * Wenn sie nicht übereinstimmt, sind Cookies Drittanbieter. Wenn Drittanbieter-Cookies blockiert werden, setzt Adobe ein Ausweich-Cookie (`s_fid`) anstelle des üblichen.

Um sicherzustellen, dass Ihr Erfassungsserver mit der Domain Ihrer Website übereinstimmt, können Sie ein **CNAME-Setup** verwenden. Dazu müssen Sie Ihre DNS-Einstellungen aktualisieren, um eine benutzerdefinierte Domain (in Ihrem Besitz) auf die Server von Adobe zu verweisen. Dadurch wird das Tracking-Cookie als Erstanbieter angezeigt. Ein CNAME kann zwar über mehrere Domains hinweg funktionieren, aber jede Domain, die nicht mit dem CNAME übereinstimmt, setzt dennoch Drittanbieter-Cookies.

>[!NOTE]
>
>Die Intelligent Tracking Prevention (ITP) von Apple beschränkt die Dauer der Erstanbieter-Cookies von Adobe, auch wenn Ihre Erfassungs-Domain mit Ihrer Website-Domain übereinstimmt. ITP wirkt sich auf Safari auf macOS und alle Browser auf iOS und iPadOS aus. Seit November 2020 laufen mit CNAME gesetzte Cookies genauso schnell ab wie mit JavaScript gesetzte Cookies. Diese Frist kann sich in Zukunft ändern.

Hier ist eine vereinfachte Version des Textes:

## Cookies und Datenschutz

Adobe nimmt Datenschutz und Datensicherheit ernst. Es arbeitet mit Datenschutzorganisationen, Regulierungsbehörden und Programmen wie AdChoices zusammen, um den Menschen die Kontrolle über die Verwendung ihrer Daten zu geben.

Die meisten Cookies von Adobe Experience Cloud speichern keine personenbezogenen Daten. Sie sind sicher und werden nur von Ihrem Unternehmen für Reporting, Inhalte und Werbung verwendet. Adobe gibt diese Daten nicht an andere Kunden oder Dritte weiter, außer in anonymen, branchenweiten Berichten (z. B. Digital Marketing Insight Reports).

Adobe führt keine Browser-Daten über verschiedene Unternehmen hinweg zusammen. Zum Schutz der Privatsphäre können einige Adobe-Tools jeder Website einen eigenen Satz von Cookies zuweisen. Einige erlauben auch die Verwendung Ihrer eigenen Domain für Cookies, wodurch sie First-Party-Cookies und sicherer werden.

Cookies können nur Informationen speichern, die zuvor darin gespeichert wurden. Sie können auf Ihrem Gerät weder Code ausführen noch andere Daten lesen. Darüber hinaus erlauben Webbrowser nur, dass Cookies von der Website gelesen werden, die sie setzt. Beispielsweise kann nur Adobe.com Cookies lesen, die es setzt.

Die folgende Abbildung zeigt die Verwendung von Cookies für eine Standard-Bildanforderung:

![Verwendung von Cookies für eine Standardbildanforderung](assets/CookiesProcessGraphic-01.png)

Die folgende Abbildung zeigt die Verwendung von Cookies für eine direkte Bildanforderung (in Szenarien, in denen keine JS-Datei geladen wird):

![Cookie-Nutzung für eine direkte Bildanforderung](assets/CookiesProcessGraphic2.png)

