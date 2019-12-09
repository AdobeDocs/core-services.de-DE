---
description: Überlegungen und Best Practices hinsichtlich persönlich identifizierbarer Informationen (PII), die in die Adobe Experience Cloud hochgeladen und darüber ausgetauscht werdenю.
keywords: customer attributes;core services
seo-description: Überlegungen und Best Practices hinsichtlich persönlich identifizierbarer Informationen (PII), die in die Adobe Experience Cloud hochgeladen und darüber ausgetauscht werdenю.
seo-title: Überlegungen zum Datenschutz – Kundenattribute
solution: Experience Cloud
title: Überlegungen zum Datenschutz – Kundenattribute
uuid: 5666dc4e-55fa-4196-9985-cf530cfb9247
translation-type: tm+mt
source-git-commit: ae97db27349940a8df7ee2ba6678683f57585678

---


# Überlegungen zum Datenschutz – Kundenattribute

Überlegungen und Best Practices hinsichtlich persönlich identifizierbarer Informationen (PII), die in die Adobe Experience Cloud hochgeladen und darüber ausgetauscht werdenю.


<!-- <p>https://wiki.corp.adobe.com/display/omtrplatform/Visitor+Enrichment+and+privacy#VisitorEnrichmentandprivacy-INFORMATIONASSOCIATIONOPTIONS </p> -->


* Vor- und Nachname
* Privatadresse oder eine andere physische Adresse
* E-Mail-Adresse
* Telefonnummer
* Sozialversicherungsnummer
* Andere Daten, die es ermöglichen, mit der betreffenden Person real oder online in Kontakt zu treten. (Ortsabhängig. Informieren Sie sich über die Datenschutz- und PII-Vorschriften und -Richtlinien an den Orten, an denen Sie Niederlassungen oder Geschäfte betreiben.)


Adobe bietet Tools, die Anbietern die Erfassung von Verhaltensdaten der Verbraucher erlauben, die ihre Sites besuchen oder ihre Anwendungen benutzen. Adobe bietet darüber hinaus auch Tools, die den Anbietern die Zusammenführung dieser Informationen mit offline oder extern vorliegenden Kundendatensätzen ermöglichen, die der Anbieter in anderen Informationsmanagementsystemen pflegt.

Der Beweggrund für diese Zusammenführung ist häufig eine Optimierung der verfügbaren Daten, um Marketing- und Werbeentscheidungen möglichst punktgenau und verbraucherorientiert treffen zu können. Adobe Analytics und Target ermöglichen Anbietern das Hochladen von persönlich identifizierbaren Informationen (PII-Daten) wie E-Mail-Adressen nur in einem Hash-Format, sodass eine Kontaktaufnahme mit der Person, die sich hinter diesen Daten verbirgt, unmöglich ist. Auch im Hash-Format können Informationen zu Analyse- und Marketingzwecken genutzt werden. Wir möchten Sie daran erinnern, dass Adobe es seinen Nutzern ausdrücklich untersagt, in Adobe sensible persönliche Informationen wie Daten zum Gesundheitszustand, Finanzdaten oder Daten zu Kindern einzuspeisen.

Adobe weiß darum, dass diese Arten von Marketing- und Werbeentscheidungen in Konflikt mit den Datenschutzbestimmungen für Verbraucher stehen können. Aus diesem Grund hat Adobe in seine Produkte Steuerelemente für den Datenschutz integriert, die Anbietern und Werbetreibenden helfen sollen, die diesbezüglichen Erwartungen ihrer Kunden zu erfüllen. Adobe empfiehlt Anbietern, genau zu prüfen, welche Daten unter welchen Umständen zu Marketingzwecken geeignet sind und verwendet werden dürfen.

**Best Practices**

Adobe empfiehlt, die PII-Daten, die in Adobe Analytics oder Target eingespeist werden sollen, vor dem Hochladen in einem Hash-Format zu verschlüsseln. Auch im Hash-Format können Informationen zu Analyse- und Marketingzwecken genutzt werden. Wir möchten Sie daran erinnern, dass Adobe es seinen Nutzern ausdrücklich untersagt, in Adobe Analytics und Target sensible persönliche Informationen wie Daten zum Gesundheitszustand, Finanzdaten oder Daten zu Kindern einzuspeisen.

Adobe empfiehlt Anbietern, genau zu prüfen, welche Daten unter welchen Umständen zu Marketingzwecken geeignet sind und verwendet werden dürfen.

Auch wenn sich die Datenschutzbestimmungen für Verbraucher ändern, empfiehlt Adobe seinen Anbietern, sich an drei allgemeingültige Grundsätze zu halten:

1. Tun Sie, was Sie sagen (in Ihren Datenschutzrichtlinien).
1. Sagen Sie, was Sie tun (in Ihren Datenschutzrichtlinien).
1. Stellen Sie den Verbraucher nicht vor Überraschungen.

Dessen eingedenk empfiehlt Adobe Anbietern, wenn sie Browsing-Aktivitäten mit PII-Daten verbinden, Hinweise oder andere Personalisierungen anzubringen, an denen der Verbraucher erkennt, dass er authentifiziert wird. Ein sanfter Hinweis könnte zum Beispiel eine persönliche Begrüßung in der Kopfzeile der Website sein. Adobe empfiehlt Anbietern außerdem, in ihren Datenschutzrichtlinien anzugeben, welche Arten von Browsing-Informationen auf ihrer Website mit PII-Daten verknüpft werden und unter welchen Umständen dies geschieht. Schließlich legt Adobe Anbietern nahe, die Opt-out-Möglichkeiten, die sie ihren Verbrauchern bieten, zu überprüfen, um sicherzugehen, dass sie nicht authentifizierte Profilinformationen auch nach einem Opt-out korrekt verwenden (wenn sie dann überhaupt noch verwendet werden dürfen).

<!-- <p> <b>Vinay Geol</b> should help craft privacy regarding how all MAC uses privacy/cookies. Privacy implications around each part of the workflow. Moving from CRM to MAC. Can it include PII? What is PII? What isn't PII? </p> 
<p>CRM data is Known Data or Info. Going to combine with activity that occurs when visitor was not authenticated. PII wiki: </p> 
<p>https://wiki.corp.adobe.com/display/omtrplatform/Visitor+Enrichment+and+privacy#VisitorEnrichmentandprivacy-INFORMATIONASSOCIATIONOPTIONS </p> 
<p>Refactoring of implementation docs as it relates to privacy and cookies. </p> 
<p>Add content to t-publish-audience-segment, as follows: </p> 
<p> Audiences are not filtered based on the authentication state of a visitor. If a visitor can browse your site in un-authenticated and authenticated states, actions that occur when a visitor is un-authenticated can still cause a visitor to be included in an audience. Please review <link> to understand the full privacy implications of audience sharing. </p> 
<p>That "link" goes to a topic dedicated to PII, with this text: </p> 
<p> - Adobe Analytics allows its advertisers to upload personally identifiable information (PII) such as email addresses. When uploading PII to Adobe Analytics, Adobe recommends that the customer should hash PII prior to uploading it to Adobe. Hashed information can still be used for analysis and for marketing purposes. As a reminder, Adobe prohibits advertisers from sending sensitive personal information to Adobe Analytics, such as medical records, financial account information, and information about minors. </p> 
<p> - Adobe recommends its advertisers carefully consider which information is appropriate to use for marketing purposes and in which circumstances the advertiser has permission to use such information. </p> 
<p> - As consumer privacy law remains in flux, Adobe recommends that advertisers respect three common tenets: 1) Do what you say (in your privacy policy); 2) Say what you do (in your privacy policy); and 3) Don't surprise your consumers. </p> 
<p> - With these expectations in mind, Adobe recommends that when an advertiser associates browsing activities to PII, the advertiser provide notices/personalization indicating that the consumer is authenticated. An example of this is including a 'Hello, Jane' greeting within the header of the website. Adobe also recommends that advertisers describe in its privacy policy what type of browsing information it associates with PII and under what circumstances browsing information is associated with PII. Lastly, Adobe strongly recommends advertisers review the opt out choices they provide their consumers to understand whether and how they can use unauthenticated profile information post opt out. </p> 
<p>Possibly revamp the cookies to include privacy, with best practices: https://docs.adobe.com/content/help/en/core-services/interface/ec-cookies/cookies-privacy.html </p> -->
