---
description: Überlegungen und Best Practices hinsichtlich persönlich identifizierbarer Informationen (PII), die in die Adobe Experience Cloud hochgeladen und darüber ausgetauscht werdenю.
keywords: customer attributes;core services
seo-description: Überlegungen und Best Practices hinsichtlich persönlich identifizierbarer Informationen (PII), die in die Adobe Experience Cloud hochgeladen und darüber ausgetauscht werdenю.
seo-title: Überlegungen zum Datenschutz – Kundenattribute
solution: Experience Cloud
title: Überlegungen zum Datenschutz – Kundenattribute
uuid: 5666dc4e-55fa-4196-9985-cf530cfb9247
translation-type: tm+mt
source-git-commit: f7ec8bf6087a18be41c9efbf05f60e6cfd24e566

---


# Überlegungen zum Datenschutz – Kundenattribute

Überlegungen und Best Practices hinsichtlich persönlich identifizierbarer Informationen (PII), die in die Adobe Experience Cloud hochgeladen und darüber ausgetauscht werdenю.


<!-- <p>https://wiki.corp.adobe.com/display/omtrplatform/Visitor+Enrichment+and+privacy#VisitorEnrichmentandprivacy-INFORMATIONASSOCIATIONOPTIONS </p> -->


* Vor- und Nachname
* Privatadresse oder andere physische Adresse
* E-Mail  Adresse
* Telefonnummer
* Sozialversicherungsnummer
* Andere Kennung, die die physische oder Online-Kontaktaufnahme mit einer Einzelperson ermöglicht. (Variiert nach Ort. Bitte überprüfen und beachten Sie die lokalen Gesetze und Vorschriften bezüglich Datenschutz und PII für alle Orte, an denen Sie geschäftlich tätig sind.)


Adobe stellt Tools bereit, mit denen Werbetreibende Verhaltensdaten über Kunden erfassen können, die ihre Sites besuchen oder ihre Anwendungen verwenden. Adobe bietet darüber hinaus Tools, mit denen Werbetreibende diese Informationen mit Offline- oder externen Kundendatensätzen erweitern können, die der Advertiser in anderen Informationsmanagementsystemen hat.

Ein häufiger Grund dafür ist, dass Werbetreibende die verfügbaren Informationen verbessern, wenn sie verbrauchergerechte Marketing- und Werbeentscheidungen treffen. Mit Adobe Analytics und der Adobe-Zielgruppe können Werbetreibende persönliche identifizierbare Informationen (PII) wie E-Mail-Adressen erst hochladen, nachdem sie Hashing durchgeführt haben, um die Kontaktaufnahme mit der betreffenden Person zu verhindern. Hash-Informationen können weiterhin für Analysen und Marketingzwecke verwendet werden. Zur Erinnerung: Adobe verbietet Anbietern, vertrauliche persönliche Daten wie z. B. medizinische Aufzeichnungen, finanzielle Kontoinformationen und Informationen über Minderjährige an Adobe zu senden.

Adobe ist sich bewusst, dass diese Arten von Marketing- und Werbeentscheidungen Auswirkungen auf die Privatsphäre der Verbraucher haben können. Aus diesem Grund hat Adobe Datenschutzkontrollen eingeführt, um Werbetreibenden zu helfen, die Erwartungen ihrer Kunden zu erfüllen. Adobe empfiehlt Anbietern, sorgfältig zu prüfen, welche Informationen für Marketingzwecke geeignet sind und unter welchen Umständen der Anbieter zur Verwendung solcher Informationen berechtigt ist.

**Best Practices**

Beim Hochladen von PII in Adobe Analytics oder Adobe Zielgruppe empfiehlt Adobe, dass der Kunde PII-Dateien vor dem Hochladen in Adobe hackt. Hash-Informationen können weiterhin für Analysen und Marketingzwecke verwendet werden. Zur Erinnerung: Adobe verbietet Anbietern, vertrauliche persönliche Daten an Adobe Analytics und Adobe Zielgruppe zu senden, wie z. B. medizinische Aufzeichnungen, Finanzdaten und Informationen über Minderjährige.

Adobe empfiehlt Anbietern, sorgfältig zu prüfen, welche Informationen für Marketingzwecke geeignet sind und unter welchen Umständen der Anbieter zur Verwendung solcher Informationen berechtigt ist.

Da sich das Datenschutzrecht der Verbraucher im Fluss befindet, empfiehlt Adobe, dass Anzeigenkunden drei allgemeine Grundsätze beachten:

1. Tu, was du sagst (in deinen Datenschutzrichtlinien).
1. Sagen Sie, was Sie tun (in Ihren Datenschutzrichtlinien).
1. Erstaunen Sie Ihre Verbraucher nicht.

Unter Berücksichtigung dieser Erwartungen empfiehlt Adobe, dass der Advertiser, wenn er Browsing-Aktivitäten mit PII verknüpft, Hinweise oder Personalisierungen angibt, die darauf hinweisen, dass der Kunde authentifiziert ist. Ein Beispiel hierfür ist die Aufnahme eines Begrüßungsworts in der Kopfzeile der Website. Adobe empfiehlt Anbietern außerdem, in ihren Datenschutzrichtlinien zu beschreiben, welche Arten von Browserinformationen mit PII verknüpft sind und unter welchen Umständen Browserinformationen mit PII verbunden sind. Schließlich empfiehlt Adobe Anbietern dringend, die Opt-out-Optionen zu überprüfen, die sie ihren Verbrauchern bieten, um zu verstehen, ob und wie sie nicht authentifizierte Profil-Informationen nach Opt-out verwenden können.

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
