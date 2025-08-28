---
description: Häufig gestellte Fragen zu  [!DNL Customer Attributes]  in Adobe Experience Cloud, für Adobe Analytics und Adobe Target.
solution: Experience Cloud
title: Häufig gestellte Fragen zu  [!DNL Customer Attributes]
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 6031e544-822b-4843-b3d8-98a36a3c40e8
source-git-commit: b296b7fe76ad686d45a5927c55f798dc0203c684
workflow-type: tm+mt
source-wordcount: '1035'
ht-degree: 80%

---

# Häufig gestellte Fragen zu [!DNL Customer Attributes]

Häufig gestellte Fragen und Best Practices zu [!DNL Customer Attributes] in Adobe Analytics und Adobe Target.

## Best Practices und Einschränkungen {#best_practices}

Hinweise und Einschränkungen bei der Verwendung von [!DNL Customer Attributes].

| Problem | Beschreibung |
|--- |--- |
| [!UICONTROL Kundenattribut] Abonnementbeschränkungen | Bei einem Upgrade auf Analytics Premium dauert es 24 Stunden, bis weitere Attribute verfügbar sind. Während dieser Verzögerung wird möglicherweise ein [!UICONTROL Attribut „Abonnement &#x200B;]&quot; ausgegeben. |
| Mehrere Anmeldungen auf demselben Gerät | Wenn Sie [!DNL Customer Attributes] zum Hochladen von Kundenprofilen in eine Datenquelle verwenden, empfiehlt Adobe, dass Benutzerinnen und Benutzer dasselbe Gerät (d. h. dieselbe Experience Cloud ID) verwenden. Die Experience Cloud ID (ECID) bleibt auf dem Gerät erhalten. Die gemeinsame Nutzung von Geräten kann dazu führen, dass die ECID mehrere Benutzer mit derselben ECID verknüpft, was zu unerwarteten Ergebnissen in [!DNL Target] führt. **Hinweis:** Bei Mobile ist die ECID dauerhaft, nachdem die Mobile App installiert wurde. Sie müssen die Mobile App neu installieren, um eine neue ECID zu generieren. Bei der Web-Version wird nach dem Löschen des Browser-Cookies eine neue ECID generiert. |
| Begrenzung des täglichen Hochladevorgangs | Adobe empfiehlt, [!DNL Customer Attributes] nur einmal pro Tag zu aktualisieren. Sie müssen mindestens 24 Stunden warten, um eine weitere Kundenprofil-Datendatei für denselben Profilsatz hochzuladen. |
| Benutzerspezifische Analytics-ID (`s.visitorID`) | Das Festlegen einer Kunden-ID mithilfe von `s.visitorID` ist eine Methode, Benutzende in Adobe Analytics zu identifizieren. Integrationen, in denen [!DNL Analytics] Analytics-Daten mit dem ID-Service exportiert oder importiert werden, funktionieren jedoch nicht, wenn eine Besucherin bzw. ein Besucher per `s.visitorID.`<br> identifiziert wird. Dazu gehören unter anderem gemeinsam verwendete Zielgruppen [!DNL Analytics] für Adobe Target (A4T) und [!DNL Customer Attributes].<br>Bei diesen Integrationen wird die Festlegung einer benutzerdefinierten Analytics ID nicht unterstützt. |
| Zeichenlängenbeschränkungen in [!DNL Analytics] | Beim Erstellen eines [!DNL Analytics]-Abonnements werden die Feldlängen für die hochgeladenen Dateien auf 255 gekürzt. |

{style="table-layout:auto"}

## Häufig gestellte Fragen zu [!DNL Customer Attributes] {#section_E47866EEA83348E09FE43CEC5E44C461}

| Question | Antwort |
|--- |--- |
| Kann ich Benachrichtigungen zum Upload-Status für [!DNL Customer Attributes] erhalten? | Ja. |
| Wie sollte ich bei den ersten Schritten mit [!DNL Customer Attributes] vorgehen? | <ol><li>Sie benötigen eine Bereitstellung. Wenn Sie Adobe Analytics-Kunde sind, stellt Adobe Sie für [!DNL Customer Attributes] bereit. Wenn Sie nur Adobe Target verwenden und nicht über Analytics verfügen, fordern Sie Bereitstellung für zentrale Services an, indem Sie sich an die Kundenunterstützung wenden.</li> <li>Reden Sie mit Ihrem CRM-Team. Finden Sie heraus, welche Art Kundendaten zur Verfügung stehen, die Sie in Analytics und in der gesamten Experience Cloud verwenden möchten.</li><li>Implementieren von zentralen Services.</li></ol> |
| Wie viele Kundenattribute darf ich verwenden? | Sie können mehrere hundert `.csv`-Spalten für den Kundenattributdienst hochladen. Beim Konfigurieren von Abonnements und beim Auswählen von Attributen gelten – je nachdem, welche Programme Sie besitzen – die folgenden Einschränkungen (pro Report Suite):  <ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: 3 insgesamt</li><li>Premium: 200</li><li>Adobe Target Standard: 5</li><li>Adobe Target Premium: 200</li></ul> |
| Ist eine Migration zum Experience Cloud ID-Dienst erforderlich? | Die Migration hängt von den verwendeten Programmen ab. <ul><li>Adobe Analytics: dringend empfohlen </li><li>Adobe Target: erforderlich. </li></ul><br>Die Verwendung des Experience Cloud ID-Service ermöglicht die neuesten Experience Cloud-Funktionen, einschließlich Echtzeit-Zielgruppen, der Adobe Target-Modernisierung, der Analytics-Integration und der Video-Heartbeat-Verfolgung. |
| In welcher Beziehung steht die Kundenattributfunktion zu Adobe Audience Manager? | Audience Manager kann zwar Daten empfangen, um die Zielgruppe zu identifizieren, jedoch keine Analysefunktionen durchführen, um Attribute mit historischen Verhaltensdaten zu verknüpfen. Audience Manager bietet außerdem nicht die in Adobe Analytics verfügbaren Berichte-, Analyse- und Segmentierungsfunktionen. [!DNL Customer Attributes] können umfangreiche Daten aus verschiedenen Programmen verknüpft und einer einzelnen ID zugeordnet werden, um sie in Experience Cloud zu verwenden. <br>In Adobe Target erscheinen Kundenattribute als individuelle Attribute, die mit anderen Regeln kombiniert werden können, um Zielgruppen zu erstellen. Zielgruppen, die für den [!UICONTROL Personen]-Service freigegeben wurden, sind vollständige Zielgruppen, die nicht geändert werden können. |
| **(Nur Adobe Analytics)** Wie unterscheidet sich diese Funktion von der in Analytics Premium? | In der Vergangenheit haben sich Kunden, die Kundenattributdaten mit Analytics-Daten kombinieren wollten, bei dieser Funktion stark auf das Data Workbench-Tool verlassen. [!DNL Customer Attributes] stellt diese Funktion einer breiteren Zielgruppe zur Verfügung, indem Kundenattribute als Dimensionen und Metriken in Report Builder bereitgestellt werden. Kundinnen und Kunden von Analytics Standard haben Zugriff auf [!DNL Customer Attributes], jedoch mit eingeschränkten Funktionen. Die vollständige Funktionalität steht Analytics Premium-Kunden zur Verfügung. |
| **(Nur Adobe Target)** Kann ich Daten für in Adobe Target unbekannte Kunden vorab laden oder hochladen? | Ja. Wenn die Besucherin oder der Besucher die erste Anforderung an Adobe Target stellt, ruft das System die vorhandenen Informationen, die Adobe über diese Person hat, aus den [!DNL Customer Attributes] ab und verwendet diese Daten für das Targeting. **Hinweis:** Das Abrufen dieser Daten kann ab der ersten Interaktion des Besuchers mit Adobe Target bis zu 20 Minuten dauern. |
| **(Nur Adobe Target)** Kann ich eine Super-Zielgruppe erstellen, indem ich Kundenattributdaten mit freigegebenen Zielgruppendaten kombiniere? | Nein. Bei freigegebenen Zielgruppendaten handelt es sich um eine abgeschlossene Zielgruppe. |
| **(Nur Adobe Target)** Wie lässt sich [!DNL Customer Attributes] mit der Adobe Target-Bulk-Profil-API vergleichen? | Mit der Bulk-Profil-API können Adobe Target-Profile direkt über die API aktualisiert werden – entweder für ein einzelnes Profil oder in Profilgruppen. Die Funktion ähnelt den [!DNL Customer Attributes], wobei folgende wesentliche Unterschiede gelten:<ul><li>Die Profil-API ist ein REST-API-Aufruf, während [!DNL Customer Attributes] FTP verwenden.</li><li>Die Profil-API von Adobe Target sendet nur Daten an Adobe Target und nicht an die gesamte Experience Cloud.</li><li>[!DNL Customer Attributes] bieten eine einfache Schnittstelle zum Erstellen und Verwalten dieser externen Daten.</li></ul> |
| **(Nur Adobe Target)** Verlängert das Hochladen von Daten aus [!DNL Customer Attributes] in Adobe Target die Lebensdauer des Adobe Target-Besucherprofils? | Ja. Weitere Informationen finden Sie unter [Lebensdauer von Besucherprofilen](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/visitor-profile.html?lang=de) in der Hilfe zu Adobe Target. |
| **(Nur Adobe Target)** Kann ich ein Targeting für die in [!DNL Customer Attributes] hochgeladenen Daten sofort vornehmen, nachdem die Besucherin oder der Besucher durch die Kunden-ID identifiziert wurde? | Ja. Beim Server-Aufruf an Adobe Target, der die mbox-Drittanbieter-ID enthält, stehen alle Kundenattributdaten zur Verfügung. |
| **(Nur Adobe Target)** Was bedeutet die Spalte **[!UICONTROL Synchronisierungsstatus]** für Dateien, die in die Kundenattributquelle hochgeladen wurden? | Die Anzahl der von Adobe Target veröffentlichten und synchronisierten Einträge kann durch Klicken auf das Synchronisierungsstatus-Symbol für eine bestimmte Attributdatei angezeigt werden. `Sync %` ist eine Echtzeitmetrik, die den Prozentsatz der Profile angibt, die in Adobe Target synchronisiert wurden.<br> **Hinweis:** Die Synchronisierung von Attributen mit Adobe Target kann bis zu 24 Stunden dauern. |
| Was stellen die Metriken zum Hochladen von Dateien in der Quelle von [!DNL Customer Attributes] dar? | Mithilfe der folgenden Metriken können Sie den Status von Attributen überprüfen, die in [!DNL Customer Attributes] hochgeladen wurden: <ul><li>Einträge: Anzahl Einträge in der Attributdatei.</li><li>**Neue Einträge:** Anzahl neuer Einträge, die in der Attributdatei vorhanden sind.</li> <li>**Aktualisierte Einträge:** Anzahl der Einträge, die in den [!DNL Customer Attributes] mit aktualisierten Werten in der Datei vorhanden sind.</li><li>**Alle Daten (Einträge):** Gesamtzahl der erfolgreich in [!DNL Customer Attributes] hochgeladenen Einträge.</li></ul> |

{style="table-layout:auto"}
