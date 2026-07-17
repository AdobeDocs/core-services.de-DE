---
description: Erfahren Sie mehr über Organisationen (IMS-Organisations-ID), den Kontowechsel und die Verknüpfung von Lösungskonten.
solution: Experience Cloud
title: Organisationen und Konten
uuid: ae47ad18-ac33-4efa-8b68-2bfaf77397aa
feature: Organizations
topic: Administration
role: Admin
level: Experienced
exl-id: 6eb58530-2a7a-48c7-9a5b-48a6e980a034
TQID: https://experienceleague.adobe.com/DCb0MQWwB0MOGALSDbLD-d4ik4B0C249xncB9eZbZMU
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
  - id: bdea9bc8-5600-45db-b85e-d74bb59dfcff
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9c2010694b8bb32c3922dd65f846375e43b2caac
workflow-type: tm+mt
source-wordcount: 506
ht-degree: 17%

---

# Organisationen und Konten

Eine *Organisation* (Organisations-ID) ist die Entität, die es einem Administrator ermöglicht, Gruppen und Benutzer zu konfigurieren und Single Sign-on in CX Enterprise zu steuern.

Die Organisation agiert als Anmeldeunternehmen, das alle CX Enterprise-Produkte und -Anwendungen umfasst. Normalerweise besitzt eine Organisation den Namen Ihres Unternehmens. Ein Unternehmen kann jedoch über mehrere Organisationen verfügen.

**Menü Organisation**

![CX Enterprise-Organisationen](../assets/organizations-menu.png)

Um sicherzustellen, dass Sie sich bei Ihrer richtigen Organisation angemeldet haben, klicken Sie auf **[!UICONTROL Profil]**, um den standardmäßigen Organisationsnamen anzuzeigen. Wenn Sie Zugriff auf mehr als eine Organisation haben, können Sie in der Kopfzeilenleiste auch eine andere Organisation anzeigen und zu dieser wechseln.

>[!NOTE]
>
>Durch den Wechsel zwischen Organisationen können Sie auf die Admin Console für diese bestimmte Organisation zugreifen. Wenn die gewünschte Organisation nicht aufgeführt ist, müssen Sie möglicherweise den Zugriff von einem Administrator in dieser Organisation anfordern. (Wenn Sie mehrere Admin Consoles zusammenführen müssen, wenden Sie sich an den Kunden-Support von Adobe.)

## Federated IDs

Wenn Ihr Unternehmen Federated IDs verwendet, können Sie sich mit dem Single Sign-on Ihres Unternehmens anmelden, ohne Ihre E-Mail-Adresse und Ihr Passwort eingeben zu müssen. Fügen Sie `#/sso:@domain` zur CX Enterprise URL (`https://experience.adobe.com`) hinzu, um diese Aufgabe zu erfüllen.

Setzen Sie beispielsweise für eine Organisation mit Federated IDs und der Domain `example.com` Ihren URL-Link auf `https://experience.adobe.com/#/sso:@example.com`. Sie können auch direkt zu einem bestimmten Programm gehen, indem Sie diese URL, an die der Programmpfad angehängt ist, als Lesezeichen speichern. (Beispiel für Adobe Analytics: `https://experience.adobe.com/#/sso:@example.com/analytics`.)

## Federated Guest Accounts

Sie können [Federated Guest Access](https://helpx.adobe.com/business/enterprise/using/federated-guest-access.html) aktivieren, um Gastbenutzer sicher in Ihrer eigenen Domain zu authentifizieren. Wenn diese Option aktiviert ist, ändert sich das Organisationsmenü, damit diese Benutzer innerhalb der vorhandenen Organisation auf jeder CX Enterprise-Seite zwischen Konten wechseln können.

Um zu einem Federated Guest-Konto zu wechseln, suchen Sie **[!UICONTROL Andere Konten]** im Menü **[!UICONTROL Organisation]** auf einer beliebigen [CX Enterprise](https://experience.adobe.com)-Seite.

**Organisationsmenü für ein zusammengeführtes Gastkonto**

![Federated Account Switcher](../assets/federated-account-switcher.png)

## Organisations-ID anzeigen

Sie können die zugewiesene Organisations-ID zu Support-Zwecken finden. Mit der Auswahl „Organisation“ in der Kopfzeile können Sie überprüfen **[!UICONTROL ob Sie sich in der richtigen]** befinden, oder zwischen Organisationen wechseln.

Die Organisations-ID ist die ID, die Ihrem bereitgestellten CX Enterprise-Unternehmen zugeordnet ist. Diese ID besteht aus einer 24-stelligen alphanumerischen Zeichenfolge gefolgt von `@AdobeOrg` (zwingend erforderlich).

Sie können Ihre Organisations-ID zusammen mit anderen Kontoinformationen mithilfe des Tastaturbefehls **Strg+I** von jeder Seite aus auf `https://experience.adobe.com` einsehen.

**Anzeigen der Organisations-ID**

1. Drücken Sie [CX Enterprise](https://experience.adobe.com) auf **Tastatur** Strg+i).

   ![Zugewiesene Organisations-ID](../assets/assigned-organization.png)

1. Suchen Sie **[!UICONTROL Benutzerinformationen]** nach **[!UICONTROL Aktuelle Organisations-ID]**, und Sie können die Organisations-ID finden.

   Alternativ können sich Administratoren auch bei der Admin Console anmelden (navigieren Sie zu [https://adminconsole.adobe.com](https://adminconsole.adobe.com)) und Ihre Organisations-ID in der URL sehen.

   Beispielsweise in der folgenden URL:

   `https://adminconsole.adobe.com/C538193582390300A495CC9@AdobeOrg/overview`

   Hier lautet die ID:

   `C538193582390300A495CC9@AdobeOrg`

## Standardorganisation angeben

Sie können bei der Anmeldung eine Standardorganisation angeben.

1. Klicken Sie in der Kopfzeile auf **[!UICONTROL Profil]** und dann auf Voreinstellungen.

1. Wählen [!UICONTROL &#x200B; unter &#x200B;] eine Standardorganisation aus.


![Profil bearbeiten](../assets/edit-profile.png)
