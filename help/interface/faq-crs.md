---
description: Häufig gestellte Fragen zu [!DNL Customer Attributes] in Adobe Experience Cloud für Adobe Analytics und Adobe Target.
solution: Experience Cloud
title: Häufig gestellte Fragen zu [!DNL Customer Attributes]
uuid: e93eb531-23c7-4d75-92e8-75699f58546a
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 6031e544-822b-4843-b3d8-98a36a3c40e8
source-git-commit: f229ec33ff721527e6a4c920ea63eabb4102935a
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 63%

---

# Häufig gestellte Fragen zu [!DNL Customer Attributes]

Häufig gestellte Fragen und Best Practices für [!DNL Customer Attributes] in Adobe Analytics und Adobe Target.

## Best Practices und Einschränkungen {#section_7F5189B3DAA84EE6865B91D2026EE05A}

Anleitungen und Einschränkungen bei der Verwendung von [!DNL Customer Attributes].

| Problem | Beschreibung |
|--- |--- |
| Abonnementeinschränkungen für das [!UICONTROL Kundenattribut] | Bei einem Upgrade auf Analytics Premium dauert es 24 Stunden, bis weitere Attribute verfügbar sind. Während dieser Verzögerung wird Ihnen möglicherweise eine Fehlermeldung über einen [!UICONTROL Attributabonnement-Maximalwert] angezeigt. |
| Mehrere Anmeldungen auf demselben Gerät | Bei Verwendung von [!DNL Customer Attributes] Um Kundenprofile in eine Datenquelle hochzuladen, empfiehlt Adobe, dass Benutzende Geräte gemeinsam nutzen (d. h. dieselbe Experience Cloud-ID). Die Experience Cloud ID (ECID) bleibt auf dem Gerät erhalten. Die gemeinsame Nutzung von Geräten kann dazu führen, dass die ECID mehrere Benutzer mit derselben ECID verknüpft, was zu unerwarteten Ergebnissen in [!DNL Target] führt. **Hinweis:** Bei Mobile ist die ECID dauerhaft, nachdem die Mobile App installiert wurde. Sie müssen die Mobile App neu installieren, um eine neue ECID zu generieren. Bei der Web-Version wird nach dem Löschen des Browser-Cookies eine neue ECID generiert. |
| Begrenzung des täglichen Hochladevorgangs | Adobe empfiehlt eine Aktualisierung [!DNL Customer Attributes] Nur einmal pro Tag. Sie müssen mindestens 24 Stunden warten, um eine weitere Kundenprofil-Datendatei für denselben Profilsatz hochzuladen. |
| Benutzerspezifische Analytics-ID (`s.visitorID`) | In Analytics können Besucher identifiziert werden, indem eine Kunden-ID mit `s.visitorID` festgelegt wird. Integrationen, in denen [!DNL Analytics] Daten, die mit dem ID-Service exportiert oder importiert werden, funktionieren nicht, wenn ein Besucher mithilfe von identifiziert wird. `s.visitorID.`<br>Dazu gehören unter anderem freigegebene Zielgruppen, [!DNL Analytics] für Adobe Target (A4T) und [!DNL Customer Attributes].<br>Bei diesen Integrationen wird die Festlegung einer benutzerdefinierten Analytics ID nicht unterstützt. |
| Zeichenlängenbeschränkungen in [!DNL Analytics] | Beim Erstellen eines [!DNL Analytics]-Abonnements werden die Feldlängen für die hochgeladenen Dateien auf 255 gekürzt. |

{style="table-layout:auto"}

## Häufig gestellte Fragen zu [!DNL Customer Attributes] {#section_E47866EEA83348E09FE43CEC5E44C461}

| Frage | Antwort |
|--- |--- |
| Kann ich Benachrichtigungen über den Upload-Status für erhalten? [!DNL Customer Attributes]? | Ja. |
| Was sollte ich tun, um loszulegen? [!DNL Customer Attributes]? | <ol><li>Sie benötigen eine Bereitstellung. Wenn Sie Analytics-Kunde sind, stellt Adobe Sie für Folgendes bereit [!DNL Customer Attributes]. Wenn Sie nur Adobe Target verwenden und nicht über Analytics verfügen, fordern Sie die Bereitstellung der zentralen Dienste an, indem Sie sich an die Kundenunterstützung wenden.</li> <li>Reden Sie mit Ihrem CRM-Team. Finden Sie heraus, welche Kundendaten in Analytics und im gesamten Experience Cloud verfügbar sind.</li><li>Implementieren von zentralen Services. Anweisungen zur Modernisierung Ihrer Implementierung finden Sie unter [Aktivieren Ihrer Programme für zentrale Services](core-services.md). (Wichtige Informationen finden Sie im Abschnitt zum Synchronisieren von Kunden-IDs.)</li></ol> **Hinweis:** Eine FAQ-Rubrik für Administratoren zur Implementierung von Core Services finden Sie [hier](faq.md). |
| Wie viele [!DNL Customer Attributes] Darf ich verwenden? | Sie können Hunderte von `.csv`-Spalten in den Kundenattributservice hochladen. Beim Konfigurieren von Abonnements und beim Auswählen von Attributen gelten – je nachdem, welche Programme Sie besitzen – die folgenden Einschränkungen (pro Report Suite):  <ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: 3 insgesamt</li><li>Premium: 200</li><li>Adobe Target Standard: 5</li><li>Adobe Target Premium: 200</li></ul> |
| Ist eine Migration zum Experience Cloud ID-Dienst erforderlich? | Die Migration hängt von den verwendeten Programmen ab. <ul><li>Adobe Analytics: dringend empfohlen </li><li>Adobe Target: erforderlich. </li></ul><br>Die Verwendung des Experience Cloud ID-Dienstes ermöglicht die neuesten Experience Cloud-Funktionen, einschließlich Echtzeit-Zielgruppen, der Adobe Target-Modernisierung, der Analytics-Integration und des Video Heartbeat-Trackings. <br> Weitere Informationen finden Sie unter [Aktivieren Ihrer Programme für zentrale Services](core-services.md). <br>**Hinweis:** Der [Experience Cloud ID-Service](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=de) ist die modernisierte Implementierung des _Analytics-Besucher-ID-Services_. |
| In welcher Beziehung steht die Kundenattributfunktion zu Adobe Audience Manager? | Audience Manager kann zwar Daten empfangen, um die Zielgruppe zu identifizieren, jedoch keine Analysefunktionen durchführen, um Attribute mit historischen Verhaltensdaten zu verknüpfen. Audience Manager bietet außerdem nicht die in Adobe Analytics verfügbaren Berichte-, Analyse- und Segmentierungsfunktionen. [!UICONTROL Personen] Ermöglicht die Verknüpfung umfangreicher Daten aus verschiedenen Anwendungen und deren Verknüpfung mit einer einzigen ID zur Verwendung auf allen Experience Cloud. <br>In Adobe Target [!DNL Customer Attributes] erscheinen als einzelne Attribute, die mit anderen Regeln kombiniert werden können, um Zielgruppen zu erstellen. Zielgruppen, die für den [!UICONTROL Personen]-Service freigegeben wurden, sind vollständige Zielgruppen, die nicht geändert werden können. |
| **(Nur Analytics)** Worin unterscheidet sich diese Funktion von der in Analytics Premium bereitgestellten Funktionalität? | In der Vergangenheit haben sich Kunden, die Kundenattributdaten mit Analytics-Daten kombinieren wollten, bei dieser Funktion stark auf das Data Workbench-Tool verlassen. [!DNL Customer Attributes] stellt diese Funktion einer breiteren Zielgruppe zur Verfügung, indem [!DNL Customer Attributes] als Dimensionen und Metriken in Reports &amp; Analytics, Ad Hoc Analysis und Report Builder. Analytics Standard-Kunden haben Zugriff auf [!DNL Customer Attributes], jedoch mit eingeschränkten Funktionen. Die vollständige Funktionalität steht Analytics Premium-Kunden zur Verfügung. |
| **(Nur Adobe Target)** Kann ich Daten für in Adobe Target unbekannte Kunden vorab laden oder hochladen? | Ja. Wenn der Besucher seine erste Anfrage an Adobe Target stellt, ruft das System die vorhandenen Informationen, die Adobe über ihn hat, von ab [!DNL Customer Attributes] und verwenden diese Daten für das Targeting. **Hinweis:** Das Abrufen dieser Daten kann ab der ersten Interaktion des Besuchers mit Adobe Target bis zu 20 Minuten dauern. |
| **(Nur Adobe Target)** Kann ich eine Super-Zielgruppe erstellen, indem ich Kundenattributdaten mit freigegebenen Zielgruppendaten kombiniere? | Nein. Bei freigegebenen Zielgruppendaten handelt es sich um eine abgeschlossene Zielgruppe. |
| **(Nur Adobe Target)** Wie funktioniert das [!DNL Customer Attributes] Funktionsvergleich mit der Massenprofil-API von Adobe Target? | Mit der Bulk-Profil-API können Adobe Target-Profile direkt über die API aktualisiert werden – entweder für ein einzelnes Profil oder in Profilgruppen. Die Funktion ist ähnlich wie [!DNL Customer Attributes], mit den folgenden Hauptunterschieden:<ul><li>Die Profil-API ist ein REST-API-Aufruf und [!DNL Customer Attributes] verwendet FTP.</li><li>Die Profil-API von Adobe Target sendet nur Daten an Adobe Target und nicht an die gesamte Experience Cloud.</li><li>[!DNL Customer Attributes] bietet eine einfache Schnittstelle zum Erstellen und Verwalten dieser externen Daten.</li></ul> |
| **(Nur Adobe Target)** Lädt Daten von [!DNL Customer Attributes] Möchten Sie die Profillebensdauer eines Adobe Target-Besuchers durch Adobe Target verlängern? | Ja. Weitere Informationen finden Sie unter [Lebensdauer von Besucherprofilen](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/visitor-profile.html?lang=de) in der Hilfe zu Adobe Target. |
| **(Nur Adobe Target)** Kann ich auf die in hochgeladenen Daten abzielen? [!DNL Customer Attributes] unmittelbar nachdem der Besucher durch die Kunden-ID identifiziert wurde? | Ja. Beim Server-Aufruf an Adobe Target, der die mbox-Drittanbieter-ID beinhaltet, stehen alle Kundenattributdaten zur Verfügung. |
| **(Nur Adobe Target)** Was bedeutet die Spalte **[!UICONTROL Synchronisierungsstatus]** für Dateien, die in die Kundenattributquelle hochgeladen wurden? | Die Anzahl der von Adobe Target veröffentlichten und synchronisierten Datensätze kann durch Klicken auf das Synchronisierungsstatus-Symbol für eine bestimmte Attributdatei angezeigt werden. `Sync %` ist eine Echtzeitmetrik, die den Prozentsatz der Profile angibt, die in Adobe Target synchronisiert wurden.<br> **Hinweis:** Die Synchronisierung von Attributen mit Adobe Target kann bis zu 24 Stunden dauern. |
| Was bedeuten die Dateiupload-Metriken in [!DNL Customer Attributes] Quelle? | Sie können den Status der in hochgeladenen Attribute überprüfen [!DNL Customer Attributes] mithilfe der folgenden Metriken: <ul><li>Datensätze: Anzahl Datensätze in der Attributdatei.</li><li>**Neue Datensätze:** Anzahl neuer Datensätze, die in der Attributdatei vorhanden sind.</li> <li>**Aktualisierte Einträge:** Anzahl der Datensätze in , die in vorhanden sind [!DNL Customer Attributes] mit aktualisierten Werten in der Datei.</li><li>**Alle Daten (Datensätze):** Gesamtzahl der erfolgreich in hochgeladenen Datensätze [!DNL Customer Attributes].</li></ul> |

{style="table-layout:auto"}