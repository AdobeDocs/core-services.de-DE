---
description: Häufig gestellte Fragen zu Kundenattributen in Adobe Experience Cloud, für Adobe Analytics und Adobe Target.
solution: Experience Cloud
title: Antworten auf häufig gestellte Fragen zu Kundenattributen
uuid: e93eb531-23c7-4d75-92e8-75699f58546a
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 6031e544-822b-4843-b3d8-98a36a3c40e8
source-git-commit: eb2ad8a8255915be47b6002a78cc810b522170d2
workflow-type: ht
source-wordcount: '1176'
ht-degree: 100%

---

# Häufig gestellte Fragen zu [!UICONTROL Kundenattributen].

Häufig gestellte Fragen und Best Practices zu [!UICONTROL Kundenattributen] in Adobe Analytics und Adobe Target.

## Best Practices und Einschränkungen {#section_7F5189B3DAA84EE6865B91D2026EE05A}

Hinweise und Einschränkungen bei der Verwendung von [!UICONTROL Kundenattributen].

| Problem | Beschreibung |
|--- |--- |
| Abonnementeinschränkungen für das [!UICONTROL Kundenattribut] | Bei einem Upgrade auf Analytics Premium dauert es 24 Stunden, bis weitere Attribute verfügbar sind. Während dieser Verzögerung wird Ihnen möglicherweise eine Fehlermeldung über einen [!UICONTROL Attributabonnement-Maximalwert] angezeigt. |
| Mehrere Anmeldungen auf demselben Gerät | Wenn Sie [!UICONTROL Kundenattribute] zum Hochladen von Kundenprofilen in eine Datenquelle verwenden, empfiehlt Adobe, dass Benutzer dasselbe Gerät (d. h. dieselbe Experience Cloud ID) verwenden. Die Experience Cloud ID (ECID) bleibt auf dem Gerät erhalten. Die gemeinsame Nutzung von Geräten kann dazu führen, dass die ECID mehrere Benutzer mit derselben ECID verknüpft, was zu unerwarteten Ergebnissen in [!DNL Target] führt. **Hinweis:** Bei Mobile ist die ECID dauerhaft, nachdem die Mobile App installiert wurde. Sie müssen die Mobile App neu installieren, um eine neue ECID zu generieren. Bei der Web-Version wird nach dem Löschen des Browser-Cookies eine neue ECID generiert. |
| Begrenzung des täglichen Hochladevorgangs | Adobe empfiehlt, Kundenattribute nur einmal pro Tag zu aktualisieren. Sie müssen mindestens 24 Stunden warten, um eine weitere Kundenprofil-Datendatei für denselben Profilsatz hochzuladen. |
| Benutzerspezifische Analytics-ID (`s.visitorID`) | In Analytics können Besucher identifiziert werden, indem eine Kunden-ID mit `s.visitorID` festgelegt wird. Integrationen, in denen [!DNL Analytics] Analytics-Daten mit dem ID-Service exportiert oder importiert werden, funktionieren jedoch nicht, wenn ein Besucher per `s.visitorID.`<br>identifiziert wird. Dazu gehören unter anderem freigegebene Zielgruppen [!DNL Analytics] für Adobe Target (A4T) und [!UICONTROL Kundenattribute].<br>Bei diesen Integrationen wird die Festlegung einer benutzerdefinierten Analytics ID nicht unterstützt. |
| Zeichenlängenbeschränkungen in [!DNL Analytics] | Beim Erstellen eines [!DNL Analytics]-Abonnements werden die Feldlängen für die hochgeladenen Dateien auf 255 gekürzt. |

{style=&quot;table-layout:auto&quot;}

## Häufig gestellte Fragen zu Kundenattributen {#section_E47866EEA83348E09FE43CEC5E44C461}

| Frage | Antwort |
|--- |--- |
| Kann ich Benachrichtigungen zum Upload-Status für Kundenattribute erhalten? | Ja. |
| Wie sollte ich bei den ersten Schritten mit Kundenattributen vorgehen? | <ol><li>Sie benötigen eine Bereitstellung. Wenn Sie Analytics-Kunde sind, stellt Adobe Kundenattribute für Sie bereit. Wenn Sie nur Adobe Target verwenden und nicht über Analytics verfügen, fordern Sie die Bereitstellung der zentralen Dienste an, indem Sie sich an die Kundenunterstützung wenden.</li> <li>Reden Sie mit Ihrem CRM-Team. Finden Sie heraus, welche Art Kundendaten zur Verfügung stehen, die Sie in Analytics und in der gesamten Experience Cloud verwenden möchten.</li><li>Implementieren von zentralen Services. Anweisungen zur Modernisierung Ihrer Implementierung finden Sie unter [Aktivieren Ihrer Programme für zentrale Services](core-services.md). (Wichtige Informationen finden Sie im Abschnitt zum Synchronisieren von Kunden-IDs.)</li></ol> **Hinweis:** Eine FAQ-Rubrik für Administratoren zur Implementierung von Hauptdiensten finden Sie [hier](faq.md). |
| Wie viele Kundenattribute darf ich verwenden? | Sie können Hunderte von `.csv`-Spalten in den Kundenattributservice hochladen. Beim Konfigurieren von Abonnements und beim Auswählen von Attributen gelten – je nachdem, welche Programme Sie besitzen – die folgenden Einschränkungen (pro Report Suite):  <ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: 3 insgesamt</li><li>Premium: 200</li><li>Adobe Target Standard: 5</li><li>Adobe Target Premium: 200</li></ul> |
| Ist eine Migration zum Experience Cloud ID-Dienst erforderlich? | Die Migration hängt von den verwendeten Programmen ab. <ul><li>Adobe Analytics: dringend empfohlen </li><li>Adobe Target: erforderlich. </li></ul><br>Die Verwendung des Experience Cloud ID-Dienstes ermöglicht die neuesten Experience Cloud-Funktionen, einschließlich Echtzeit-Zielgruppen, der Adobe Target-Modernisierung, der Analytics-Integration und des Video Heartbeat-Trackings. <br> Weitere Informationen finden Sie unter [Aktivieren Ihrer Programme für zentrale Services](core-services.md). <br>**Hinweis:** Der [Experience Cloud ID-Service](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=de) ist die modernisierte Implementierung des _Analytics-Besucher-ID-Services_. |
| In welcher Beziehung steht die Kundenattributfunktion zu Adobe Audience Manager? | Audience Manager kann zwar Daten empfangen, um die Zielgruppe zu identifizieren, jedoch keine Analysefunktionen durchführen, um Attribute mit historischen Verhaltensdaten zu verknüpfen. Audience Manager bietet außerdem nicht die in Adobe Analytics verfügbaren Berichte-, Analyse- und Segmentierungsfunktionen. Mit [!UICONTROL Personen] können umfangreiche Daten aus verschiedenen Programmen verknüpft und einer einzelnen ID zugeordnet werden, um sie in Experience Cloud zu verwenden. <br>In Adobe Target erscheinen Kundenattribute als individuelle Attribute, die mit anderen Regeln kombiniert werden können, um Zielgruppen zu erstellen. Zielgruppen, die für den [!UICONTROL Personen]-Service freigegeben wurden, sind vollständige Zielgruppen, die nicht geändert werden können. |
| **(Nur Analytics)** Worin unterscheidet sich diese Funktion von der in Analytics Premium bereitgestellten Funktionalität? | In der Vergangenheit haben sich Kunden, die Kundenattributdaten mit Analytics-Daten kombinieren wollten, bei dieser Funktion stark auf das Data Workbench-Tool verlassen. [!UICONTROL Kundenattribute] stellen diese Funktion einer breiteren Zielgruppe zur Verfügung, indem sie Kundenattribute als Dimensionen und Metriken in Reports &amp; Analytics, Ad Hoc Analysis und Report Builder bereitstellen. Kunden von Analytics Standard haben Zugriff auf Kundenattribute, jedoch mit eingeschränkten Funktionen. Die vollständige Funktionalität steht Analytics Premium-Kunden zur Verfügung. |
| **(Nur Adobe Target)** Kann ich Daten für in Adobe Target unbekannte Kunden vorab laden oder hochladen? | Ja. Wenn der Besucher die erste Anforderung an Adobe Target stellt, ruft das System die vorhandenen Informationen, die Adobe über ihn hat, aus den Kundenattributen ab und verwendet diese Daten für das Targeting. **Hinweis:** Das Abrufen dieser Daten kann ab der ersten Interaktion des Besuchers mit Adobe Target bis zu 20 Minuten dauern. |
| **(Nur Adobe Target)** Kann ich eine Super-Zielgruppe erstellen, indem ich Kundenattributdaten mit freigegebenen Zielgruppendaten kombiniere? | Nein. Bei freigegebenen Zielgruppendaten handelt es sich um eine abgeschlossene Zielgruppe. |
| **(Nur Adobe Target)** Wie lässt sich die Funktionalität der [!UICONTROL Kundenattribute] mit der Bulk-Profil-API von Adobe Target vergleichen? | Mit der Bulk-Profil-API können Adobe Target-Profile direkt über die API aktualisiert werden – entweder für ein einzelnes Profil oder in Profilgruppen. Die Funktion ähnelt den Kundenattributen, wobei folgende wesentliche Unterschiede gelten:<ul><li>Die Profil-API ist ein REST-API-Aufruf und Kundenattribute verwenden FTP.</li><li>Die Profil-API von Adobe Target sendet nur Daten an Adobe Target und nicht an die gesamte Experience Cloud.</li><li>Kundenattribute bieten eine einfache Schnittstelle zum Erstellen und Verwalten dieser externen Daten.</li></ul> |
| **(Nur Adobe Target)** Verlängert das Hochladen von Daten aus Kundenattributen in Adobe Target die Lebensdauer des Adobe Target-Besucherprofils? | Ja. Weitere Informationen finden Sie unter [Lebensdauer von Besucherprofilen](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/visitor-profile.html?lang=de) in der Hilfe zu Adobe Target. |
| **(Nur Adobe Target)** Kann ich ein Targeting für die in Kundenattribute hochgeladenen Daten vornehmen, nachdem der Besucher durch die Kunden-ID identifiziert wurde? | Ja. Beim Server-Aufruf an Adobe Target, der die mbox-Drittanbieter-ID beinhaltet, stehen alle Kundenattributdaten zur Verfügung. |
| **(Nur Adobe Target)** Was bedeutet die Spalte **[!UICONTROL Synchronisierungsstatus]** für Dateien, die in die Kundenattributquelle hochgeladen wurden? | Die Anzahl der von Adobe Target veröffentlichten und synchronisierten Datensätze kann durch Klicken auf das Synchronisierungsstatus-Symbol für eine bestimmte Attributdatei angezeigt werden. `Sync %` ist eine Echtzeitmetrik, die den Prozentsatz der Profile angibt, die in Adobe Target synchronisiert wurden.<br> **Hinweis:** Die Synchronisierung von Attributen mit Adobe Target kann bis zu 24 Stunden dauern. |
| Was stellen die Metriken zum Hochladen von Dateien in der Kundenattributquelle dar? | Mithilfe der folgenden Metriken können Sie den Status von Attributen überprüfen, die in Kundenattribute hochgeladen wurden: <ul><li>Datensätze: Anzahl Datensätze in der Attributdatei.</li><li>**Neue Datensätze:** Anzahl neuer Datensätze, die in der Attributdatei vorhanden sind.</li> <li>**Aktualisierte Datensätze:** Anzahl der Datensätze, die in den Kundenattributen mit aktualisierten Werten in der Datei vorhanden sind.</li><li>**Alle Daten (Datensätze):** Gesamtzahl der erfolgreich in Kundenattributen hochgeladenen Datensätze.</li></ul> |

{style=&quot;table-layout:auto&quot;}