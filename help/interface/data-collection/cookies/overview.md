---
description: Hier erfahren Sie, wie Lösungen und Services in Adobe Experience Cloud Cookies verwenden.
title: Verwendung von Cookies in Experience Cloud
uuid: 4255a13a-917b-4b5f-a7d4-4b2e7521d189
exl-id: 60f1a89e-d989-461b-a6a3-c1df022cd30b
source-git-commit: b4d7cc357393798f2265e09885dd4ea2f80ab31e
workflow-type: tm+mt
source-wordcount: '890'
ht-degree: 58%

---

# In Experience Cloud verwendete Cookies

Viele Dienste in der Adobe Experience Cloud verwenden Cookies. Ein Cookie ist ein kleines Datenelement, das von einer Website einem Webbrowser präsentiert wird. Der Browser speichert diese Dateneinheit, sodass eine Website bei Bedarf auf ihre Daten verweisen kann. Diese Aktion wird bei jeder nachfolgenden Anforderung für Seiten und Bilder ausgeführt.

Cookies werden bereitgestellt, um während und manchmal auch zwischen Website-Besuchen Informationen beizubehalten. Cookies ermöglichen eine eindeutige Unterscheidung zwischen Geräten und anderen Browsern, in denen die Site angezeigt wird.

Aufgrund von Gesetzen, Regulierungen und Selbstregulierungsvorschriften sind Sie dazu verpflichtet, die Zustimmung von Besuchern einzuholen, bevor Sie Informationen auf einem Computer oder einem anderen mit dem Internet verbundenen Gerät speichern oder abrufen können. Adobe empfiehlt Ihnen, mit dem Rechtsbeistand Ihres Unternehmens zu besprechen, welche Gesetze, Vorschriften und Grundsätze Ihre Verwendung von Cookies steuern.

## Informationen zu Erstanbieter-Cookies

Adobe Experience Cloud-Dienste verwenden Cookies, um Informationen zu Variablen und Komponenten bereitzustellen, die nicht zwischen Bildanforderungen und Browsersitzungen bestehen bleiben. Adobe verwendet nach Möglichkeit Erstanbieter-Cookies, um Aktivitäten auf Ihrer Site aufzuzeichnen. Um Aktivitäten auf verschiedenen Websites aufzuzeichnen, z. B. auf anderen Domains, deren Inhaber Sie sind, sind Drittanbieter-Cookies erforderlich.

Viele Browser und Anti-Spyware-Anwendungen sind dafür konzipiert, Drittanbieter-Cookies abzulehnen und zu löschen. Adobe stellt sicher, dass Cookies immer gesetzt werden können, auch wenn Drittanbieter-Cookies blockiert werden. Das spezifische Verhalten variiert je nachdem, ob Sie den Experience Platform Identity Service (ECID-Dienst) oder die Legacy-IDs von Analytics (z. B. das `s_vi` -Cookie) verwenden:

* Der [Experience Platform Identity-Dienst (ECID-Dienst)](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=de) setzt Erstanbieter-Cookies automatisch, unabhängig davon, ob Ihre Erfassungsdomäne mit Ihrer Site-Domäne übereinstimmt. Wenn sie nicht übereinstimmen, verwendet der Identitätsdienst JavaScript, um Cookies in der Domäne Ihrer Site zu setzen.
* Wenn Sie [Legacy-IDs von Analytics](analytics.md) verwenden (z. B. das Cookie `s_vi` ), hängt es davon ab, wie Sie Ihren Datenerfassungsserver konfiguriert haben. Wenn der Datenerfassungsserver mit der Domain Ihrer Website übereinstimmt, werden Cookies als First-Party gesetzt. Wenn der Erfassungsserver nicht mit Ihrer aktuellen Domäne übereinstimmt, werden Cookies als Drittanbieter gesetzt. Wenn Drittanbieter-Cookies blockiert werden, setzt Analytics in diesem Fall eine Erstanbieter-Ausweich-ID (`s_fid`) anstelle des standardmäßigen `s_vi` -Cookies.

Wenn Sie sicherstellen möchten, dass Ihr Erfassungsserver mit der Domäne Ihrer Site übereinstimmt, können Sie eine CNAME-Implementierung verwenden, die die Weiterleitung von einer benutzerdefinierten Domäne ermöglicht, die in Ihrer CNAME-Implementierung an Adobe-Erfassungsserver angegeben ist. Diese Aufgabe umfasst Änderungen an den DNS-Einstellungen Ihres Unternehmens, um einen CNAME-Alias zu konfigurieren, der auf eine von Adobe gehostete Domäne verweist. Beachten Sie, dass verschiedene Adobe-Produkte zwar die Verwendung eines CNAME unterstützen, der CNAME jedoch in allen Fällen zum Erstellen eines vertrauenswürdigen First-Party-Endpunkts für einen bestimmten Kunden verwendet wird und sich im Besitz dieses Kunden befindet. Wenn Sie mehrere Domänen steuern, können sie einen einzelnen CNAME-Endpunkt verwenden, um Benutzer domänenübergreifend zu verfolgen. Wenn die Site-Domäne jedoch nicht mit den CNAME-Domänen-Cookies übereinstimmt, werden sie als Drittanbieter festgelegt.

>[!NOTE]
>
>Unabhängig davon, ob Ihre Erfassungsdomäne mit Ihrer Site-Domäne übereinstimmt, setzt das ITP-Programm (Intelligent Tracking Prevention) von Apple die Erstanbieter-Cookies, die von Adobe gesetzt werden, in Browsern mit kurzer Lebensdauer, die von ITP verwaltet werden. Dazu gehören Safari in macOS und alle Browser in iOS und iPadOS. Ab November 2020 laufen über CNAME gesetzte Cookies genauso ab wie über JavaScript gesetzte Cookies. Diese Ablaufzeit kann sich ändern.

## Cookies und Datenschutz

Die Wahrung der Privatsphäre und die Datensicherheit der Kunden hat bei Adobe oberste Priorität. Adobe beteiligt sich bei mehreren Datenschutzorganisationen und arbeitet mit Datenschutzbehörden und nach Selbstregulierungsgrundsätzen. Diese Zusammenarbeit umfasst das Programm „Digital Advertising Alliance AdChoices“, mit dem Kunden Informationen über die Verwendung ihrer Informationen erhalten und Auswahlmöglichkeiten bezüglich der Verwendung haben.

Die meisten von Experience Cloud-Produkten gesetzten Cookies enthalten keine personenbezogenen Informationen. Diese Cookies und zugehörige Daten sind sicher und werden nur für die Berichte in Ihrem Unternehmen sowie zur Bereitstellung relevanter Inhalte und Werbeanzeigen genutzt. Die Daten werden nicht an Drittanbieter oder andere Kunden von Adobe weitergegeben, es sei denn in aggregierter Form für Branchenberichte. Beispielsweise werden im [!DNL Digital Marketing Insight Report] aggregierte und anonyme Daten mehrerer Einzelhändler analysiert.

Adobe führt unternehmensübergreifend keine Informationen auf Browserebene zusammen. Zum Schutz der Privatsphäre und der Sicherheit von Kundendaten ermöglichen einige Dienste innerhalb des Experience Cloud-Angebots den Unternehmen die Verwendung eines separaten Satzes mit Cookies für jede verfolgte Site. Einige Angebote bieten Kunden auch die Möglichkeit, ihren eigenen Domänennamen als Eigentümer des Cookies zu verwenden. Dadurch entsteht eine zusätzliche Datenschutz- und Sicherheitsstufe, da die Experience Cloud-Cookies *Erstanbieter-Cookies* sind, die dauerhaft zur Website des Unternehmens gehören.

Cookies können nur die Informationen speichern und bereitstellen, die zuvor in ihnen abgelegt wurden. Sie sind nicht in der Lage, Code auszuführen oder andere auf dem Computer gespeicherte Informationen abzurufen. Darüber hinaus schränken Webbrowser den Zugriff auf Cookie-Daten ein. Browser erzwingen eine Cookie-Sicherheitsrichtlinie, die alle Cookie-Daten nur der Website zur Verfügung stellt, die die Informationen ursprünglich eingestellt hat.

Beispielsweise können Daten, die in Cookies enthalten sind, die von der Adobe.com-Website eingestellt werden, auf keiner anderen Website als Adobe.com angezeigt werden.

Die folgende Abbildung zeigt die Verwendung von Cookies für eine Standard-Bildanforderung:

![Verwendung von Cookies für eine Standardbildanforderung](assets/CookiesProcessGraphic-01.png)

Die folgende Abbildung zeigt die Verwendung von Cookies für eine direkte Bildanforderung (in Szenarien, in denen keine JS-Datei geladen wird):

![Cookie-Nutzung für eine direkte Bildanforderung](assets/CookiesProcessGraphic2.png)
