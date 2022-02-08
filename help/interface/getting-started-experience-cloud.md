---
description: Hier erfahren Sie, wie Sie sich bei Adobe Experience Cloud anmelden, Kennwörter und Benachrichtigungen verwalten und eine standardmäßige Landingpage festlegen.
keywords: Zentrale Services, Anmeldung bei Experience Cloud
solution: Experience Cloud
title: 'Anmelden und Verwalten von der Experience Cloud-Profileinstellungen '
uuid: c1e13b99-0069-4fdb-8d72-ddcec3ed1121
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: 12addbb6-a29b-4d20-ac8f-77e0846150b5
source-git-commit: fef91c95f8ce5c8791b345ce64c99cd61a733966
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 97%

---

# Anmelden und Verwalten von der Experience Cloud-Profileinstellungen

Durch die Anmeldung bei Experience Cloud (anstelle der Anmeldung bei nur einem einzelnen Programm) wird Single Sign-on für alle Programme und Services aktiviert, die Sie besitzen. In diesem Hilfethema wird beschrieben, wie Sie sich bei der Experience Cloud anmelden, Kennwörter und Benachrichtigungen verwalten und eine Standard-Landingpage angeben.

>[!IMPORTANT]
>
>Administratoren finden Informationen über Aktualisierungen der Benutzer- und Produktverwaltung im Abschnitt [Administration](admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909).

## Bei der Experience Cloud anmelden (Administratoren) {#task_034FC955031347F3B02B686A09801A08}

Melden Sie sich an und stellen Sie sicher, dass Sie sich in der richtigen [Organisation](organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1) befinden.

1. Klicken Sie auf das Experience Cloud-Menü (![](assets/menu-icon.png)) und anschließend auf **[!UICONTROL Administration]**.

   Wird die Verknüpfung **[!UICONTROL Administration]** nicht angezeigt, sind Sie kein Experience Cloud-Administrator der angezeigten [Organisation](organizations.md#topic_C31CB834F109465A82ED57FF0563B3F1). Sollten Sie mit der Zuweisung von Administratorrechten Schwierigkeiten haben, wenden Sie sich an die Kundenunterstützung oder einen bereits bestehenden Experience Cloud-Administrator in Ihrem Unternehmen.
1. Wählen Sie **[!UICONTROL Administration]** aus.

1. Klicken Sie auf einen der folgenden Links, um fortzufahren:

| Element | Beschreibung |
|--- |--- |
| [Grundlagen der Admin Console](experience-cloud.md) | Hier lernen Sie die ersten Schritte kennen, die Sie mit Experience Cloud-Programmen ausführen müssen. |
| [Einrichten der Identität](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html) | Definieren Sie ein Identitätssystem, mit dem Ihre Endbenutzer authentifiziert werden und richten Sie es ein. |
| [Benutzerverwaltung](https://helpx.adobe.com/de/enterprise/using/users.html) | Erfahren Sie mehr über die Anmeldung an der Admin Console und die Verwaltung von Benutzerberechtigungen und Produktprofilen für die Experience Cloud. |
| [Admin Console starten](admin-getting-started.md) | Die Admin Console ist der zentrale Ort für die Verwaltung Ihrer Adobe-Benutzer und Produktberechtigungen in Ihrer gesamten Organisation.<br>Sie können sich auch über einen [direkten Link](https://adminconsole.adobe.com) bei der Admin Console anmelden. |
| [Creative Cloud-Benutzer verwalten](t-admin-add-cc-user.md) | Mit Experience Cloud Assets können Marketingexperten mithilfe der Creative Cloud Ordner mit Designern und anderen Kreativ-Assets gemeinsam verwenden, synchronisieren und mit ihnen zusammenarbeiten. Hier können Sie die Creative Cloud-Benutzer verwalten, die für die Zusammenarbeit mit Ihrem Unternehmen zugelassen sind. |
| [Report Suites zuordnen](core-services.md) | (Nur Analytics) Die zentralen Experience Cloud-Dienste sind mit einer Organisation anstelle einer einzelnen Report Suite verknüpft. Um sicherzustellen, dass diese Dienste ordnungsgemäß funktionieren, muss jede Analytics Report Suite einer Organisation zugeordnet werden. (Diese Aufgabe ist Teil eines längeren Arbeitsablaufs, mit dessen Hilfe [Analytics für Hauptdienste aktiviert wird](core-services.md#concept_07ED1D5C64234E77976E6D572E78FB9C)). |
| [Organisations-ID](organizations.md) | Die *Organisations-ID* in der URL gefunden wird, wenn sie sich in der Admin Console befindet. Sie können sie auch im [!UICONTROL User Data Debugger] Popup (`ctrl+i` oder `cmd+i`) von jeder Seite unter `https://experience.adobe.com`. Diese ID ist die mit Ihrem bereitgestellten Experience Cloud-Unternehmen verknüpfte ID. Diese ID besteht aus einer 24-stelligen alphanumerischen Zeichenfolge gefolgt von @AdobeOrg (erforderlich). |

{style=&quot;table-layout:auto&quot;}

## Bei der Experience Cloud anmelden (Benutzer) {#task_1BFE87E20DCB44078CAC82F3CD44B985}

Hilfe für Benutzer, die sich nicht als Administratoren bei der Experience Cloud anmelden.


1. Vergewissern Sie sich bei Ihrem Administrator, dass Ihre [Organisation](organizations.md) in der Experience Cloud bereitgestellt wurde.


1. Navigieren Sie zur [Adobe Experience Cloud](https://experience.adobe.com) ([!DNL experience.adobe.com]).
1. Klicken Sie auf **[!UICONTROL Mit Adobe ID anmelden]**.

   Ihr Experience Cloud-Administrator kann Ihnen bei der Bestimmung der Kontoart (Adobe ID oder Enterprise ID) behilflich sein.

1. Klicken Sie auf der Landingpage auf das Auswahlsymbol ![](assets/menu-icon.png), um das Pulldown-Menü aufzurufen.

   ![](assets/experience-cloud-core-services.png)

   Welche Programme und Services in diesem Menü angezeigt werden, hängt davon ab, welche Programmberechtigungen Ihnen von Ihrem [Administrator](admin-getting-started.md#topic_3FCB4099640647E3B2411ADBFCE81909) zugewiesen wurden.

## Persönliche Standard-Kontoeinstellungen konfigurieren {#task_73CBCAE6C91749D19C95421E5AC311BA}

Sie können persönliche Details bearbeiten und eine standardmäßige [Organisation](admin-getting-started.md#concept_705C626560A54CA2A4215F1C870C42B2) und Landingpage festlegen, die nach der Anmeldung in der Experience Cloud angezeigt werden soll.

1. Melden Sie sich bei Experience Cloud an und klicken Sie auf Ihr Profilsymbol.

   ![Wählen Sie Ihr Profil-Symbol aus](assets/edit-profile.png)
1. Wählen Sie **[!UICONTROL Profil bearbeiten]** aus.

   ![Standardorganisation und Landingpage in Experience Cloud](assets/default-organization.png)
1. Fahren Sie mit der Konfiguration und Bearbeitung Ihrer persönlichen Informationen fort und klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Benachrichtigungen aktivieren {#concept_0105453AD71847B8BFCAF4A40915F157}

Sie erhalten eine Benachrichtigung (per E-Mail oder im Produkt) über Systemaktualisierungen, Wartungshinweise, Beiträge, Erwähnungen und freigegebene Assets. Sie können auch die Produkte und Programme angeben, für die Sie Benachrichtigungen erhalten möchten, einschließlich des Upload-Status für Kundenattribute.

Um zu den Benachrichtigungen zu navigieren, klicken Sie auf das Symbol **[!UICONTROL Benachrichtigungen]** ![](assets/notifications-icon.png) und dann auf das Symbol **[!UICONTROL Einstellungen]**![](assets/icon_edit_board.png).

Sie können die Anzeige der Benachrichtigungen nach den für Sie wichtigen Benachrichtigungstypen sortieren und nach Benachrichtigungen suchen. Alternativ können Sie auch folgendermaßen vorgehen:

* Sortieren Sie nach den für Sie wichtigen Nachrichtentypen.
* Suchen Sie Benachrichtigungen.

![Experience Cloud-Benachrichtigungen](assets/notifications-admin.png)

<!-- <p> <b>Analytics</b> </p> 
<ul id="ul_91BF597858124FA5BF338C36F6C5533F"> 
 <li id="li_FAD3E93CDE6242F58F14D55C8A6E23D7">Contribution analysis completed </li> 
 <li id="li_03D33D3228884CECA371B58656B2F3E7">Guided analysis shared </li> 
 <li id="li_DCF710F89317487B8DAA86CC05C694CA">Scheduled report failure </li> 
</ul> 
<p> <b>Adobe Target</b> </p> 
<p>Test started or stopped </p> 
<p> <b>Media Optimizer</b> </p> 
<p>Performance alerts </p> 
<p> <b>Dynamic Tag Manager</b> </p> 
<ul id="ul_9ACDA418933E40918744D9C32A57DD4B"> 
 <li id="li_4DD0FFD3D9F84A428703611EF767D4D0">New web property created </li> 
 <li id="li_C6B923012E9D40BA91F4CBF7D2D72986">New user added </li> 
 <li id="li_EB0B9D1CFDE24E6987935CCCBFC7892A">Approvals - publishing and approval status for new rules, data elements, and tools </li> 
 <li id="li_17B0B176FF85435FB7EDD4317BC18201">Property has been published </li> 
</ul> -->

## Profile und Kennwörter verwalten {#task_7B89F4F38E5A4C4EB0FF842953856382}

Sie können Ihr Experience Cloud-Profil bearbeiten, eine Standardorganisation und -Landingpage festlegen und vieles mehr.

1. Melden Sie sich bei Experience Cloud an.

1. Klicken Sie in Experience Cloud auf Ihr Profilbild.

   ![Bearbeiten Ihres Experience Cloud-Profils](assets/edit-profile.png)
1. Wählen Sie **[!UICONTROL Profil bearbeiten]** aus.

   Füllen Sie auf der Seite „Profil und Kennwörter“ die Felder und Optionen unter „Persönliche Details“ aus.

## Kennwort zurücksetzen {#task_46541A2806164CB1A4AE8239604E4EB1}

1. Navigieren Sie zur Anmeldeseite Ihrer Lösung.
1. Wählen Sie **[!UICONTROL Kennwort vergessen]** aus.

   Durch das Zurücksetzen des Lösungskennworts sollten sich Probleme bei der Verknüpfung des Kennworts im Zuge der Experience Cloud-Kontenverknüpfung lösen lassen.

   Benutzer von Adobe Analytics können das Kennwort unter [https://sc2.omniture.com/password_recovery.html](https://sc2.omniture.com/password_recovery.html) zurücksetzen.

## Konfigurieren der Anmeldung bei einem Programm über einen direkten Link {#concept_8BE493A08786469B88B210E13F78FF2F}

Optional können Sie sich mit der über die Experience Cloud-Oberfläche bereitgestellten Authentifizierung bei einer bestimmten Seite in einer Lösung anmelden.

### URL-Vorlage

`https://experience.adobe.com/#/@<tenantId>/<solutionname>?destURL=<fullURL>`

Beispiel-URL:

`https://experience.adobe.com/#/@aem62tenant/analytics?destURL=https%3A%2F%2Fsc.omniture.com%2Freports%2F11562.html`

>[!NOTE]
>
>Sie müssen alle URLs vor Weitergabe an den Parameter `destURL` verschlüsseln. (Encoder-Sites wie [URL Decoder/Encoder](https://meyerweb.com/eric/tools/dencoder/) sind verfügbar.)

| Parameter | Beschreibung | Beispiel | Erforderlich/Optional |
|--- |--- |--- |--- |
| `tenantId` | Name des Mandanten, bei dem sich der Benutzer anmelden soll. | aem62tenant | Optional |
| `destURL` | Die vollständige URL zu dem Ort, an den der Benutzer geleitet werden soll. | http://sc.omniture.com/login/?r=%2Fx%2F1_7xxzf&amp;tenantId=obuengsc&amp;company=OBU+Eng+SC | Optional |
| `solutionname` | Name der MAC-Lösung, die Inhaber des des `destURL` Parameters ist. Er wird verwendet, um zu bestätigen, dass der Benutzer Zugriff auf das Programm hat, zu dem die URL gehört.  Die Programme müssen sicherstellen, dass der `applicationname` mit dem Parameter `destURL` übereinstimmt.  Beispiel: Wenn die URL `solutionname` als Social enthält und die bereitgestellte `destURL` eine Analytics-URL ist, wird der Benutzer auch dann zu der URL umgeleitet, wenn er keinen Zugriff auf Analytics hat. MAC überprüft NICHT, ob der Eigentümer der `destURL` mit dem Lösungsnamen synchronisiert ist. | analytics | Erforderlich, wenn `destURL` der Parameter verwendet wird. |

{style=&quot;table-layout:auto&quot;}
