---
description: Erstellen und verwalten Sie Angebote, die in Adobe Campaign verwendet werden sollen.
seo-description: Erstellen und verwalten Sie Angebote, die in Adobe Campaign verwendet werden sollen.
seo-title: Angebotsverwaltung
title: Angebotsverwaltung
uuid: 83e1d4cd-c5fa-4df0-9603-2914eb4648f8
index: y
translation-type: tm+mt
source-git-commit: 55ac24fe0fb177a5a81765af1f7d602acc0f5d0f

---


# Angebote

Erstellen und verwalten Sie Angebote, die in Adobe Campaign verwendet werden sollen.

Es gibt zwei Arten von Angeboten im [!UICONTROL Angebotsmanagement]:

| Typ | Beschreibung |
|---|---|
| Allgemeines Angebot | Ermöglicht Ihnen das Ausfüllen des vollständigen Angebotsdatenmodells (Berechtigungsregeln, Start- und Enddaten und Inhalt). |
| Fallback-Angebot | Das letzte Angebot, wenn ein Kunde für eines der anderen ausgewählten Angebote nicht berechtigt ist. Sie können keine Berechtigungsregeln oder Start- und Enddaten mit Ausweichangeboten verknüpfen. |

>[!NOTE]
>
>Bei einer Angebotsaktivität werden Sie immer aufgefordert, ein Ausweichangebot auszuwählen. Daher müssen Sie mindestens ein Ausweichangebot in Ihrem Angebotsbestand haben, bevor Sie eine Angebotsaktivität erstellen können.

## Create an offer {#task_6C4AE487377D424FA133ACCA6AF741D4}

Erstellen Sie ein Angebot, das Ihrem Angebotsbestand hinzugefügt wird.

1. Klicken Sie auf der Registerkarte [!UICONTROL Bestand] in [!UICONTROL Angebotsverwaltung]auf Neues Angebot **[!UICONTROL erstellen]**und wählen Sie dann Angebot**[!UICONTROL  erstellen]**.

   ![](assets/create-offerx.png)

1. Füllen Sie die folgenden Felder aus:

   <table id="table_60A4001CE9F34422ACB59FB62C9CBDCD">
<thead> 
  <tr> 
   <th colname="col1" class="entry"> Feld </th> 
   <th colname="col2" class="entry"> Beschreibung </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Angebotsname </p> </td> 
   <td colname="col2"> <p>Der Name, der mit dem Angebot verknüpft ist. Sie können nicht zwei Angebote mit doppelten Namen in Ihrem Bestand haben. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Startdatum </p> </td> 
   <td colname="col2"> <p>Das Datum, an dem das Angebot angezeigt werden kann. Wenn das Startdatum 15.01.17 gewählt ist, kann das Angebot ab 15.00 Uhr angezeigt werden. </p> <p>Die Angebotsverwaltung arbeitet nach dem UTC-Zeitstandard. Das heißt: </p> <p> 
     <ul id="ul_A9D49B4405F34E6DA8FB52A13437F799"> 
      <li id="li_9490D092B235479A981FC2D5DD0B17B4">Angebote gelten ab dem Tag, an dem das Angebot beginnen soll, um 00:00 Uhr UTC. </li> 
      <li id="li_C28BB1FEB9E1495593826403CF5F67A9">Angebote laufen am Tag nach dem Enddatum um 00:00 Uhr UTC ab. Wenn ein Angebot beispielsweise auf ein Enddatum von 5/14 eingestellt ist, läuft das Angebot am 15.00 Uhr UTC ab. Das Angebot wird dann archiviert. </li> 
      <li id="li_D3F7DCD1BF75410A8F4F5BC468B667AB">Wenn E-Mails in Adobe Campaign vorbereitet werden, werden nur Angebote angezeigt, die zu diesem Zeitpunkt gültig sind. </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Enddatum </p> </td> 
   <td colname="col2"> <p>Das Datum, an dem das Angebot endet. Wenn ein Enddatum vom 20.01.2017 ausgewählt ist, wird das Angebot nicht mehr nach 23.59 Uhr am 20.01.17 angezeigt. Wenn ein Angebot sein Enddatum überschreitet, wird es automatisch archiviert. </p><p>Die Angebotsverwaltung arbeitet nach dem UTC-Zeitstandard. Weitere Informationen finden Sie in der obigen Zeile. </p></td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Förderfähigkeitsregeln </p> </td> 
   <td colname="col2"> <p>Sie können Angebotsberechtigungsregeln auf der Grundlage der in der <span class="keyword"> Kampagnendatenbank</span> verfügbaren Daten erstellen. Die Berechtigungsregeln bestimmen, an wen und wann ein Angebot angezeigt werden kann. </p> <p>Sie können beispielsweise festlegen, dass nur dann ein "Angebot für Damen in Winterkleidung"angezeigt werden soll, wenn (Geschlecht = Weiblich) und (Region = Nordost). Die zum Erstellen dieser Regeln verwendeten Attribute stammen aus dem Kampagnen-Standard-Profil. </p> <p>Hinweis:  Wenn Sie zum ersten Mal auf Angebotsverwaltung zugreifen, stehen im Rule Builder keine Attribute zur Verfügung. Sie müssen Attribute über die Kampagnen-Benutzeroberfläche freigeben. Nach der Freigabe sind diese Attribute verfügbar. </p></td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Max. </p> </td> 
   <td colname="col2"> <p>Die maximale Zeit, die ein Angebot vorgeschlagen werden kann. </p> <p>Hinweis:  Die Häufigkeit, mit der ein Angebot vorgeschlagen wird, wird zum Zeitpunkt der E-Mail-Vorbereitung berechnet. Wenn Sie z. B. eine E-Mail mit einer Reihe von Angeboten erstellen, wird für diese Zahlen Ihre maximale Anzahl gezählt, unabhängig davon, ob die E-Mail gesendet wird oder nicht. </p></td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Max. Obergrenze pro Benutzer </p> </td> 
   <td colname="col2"> <p>Die maximale Zeit, die ein Angebot einem bestimmten Benutzer vorgeschlagen werden kann. </p> <p>Hinweis:  Die Anzahl der Angebote, die einem bestimmten Benutzer zur Zeit der E-Mail-Vorbereitung vorgeschlagen werden. Wenn Sie z. B. eine E-Mail mit einer Reihe von Angeboten vorbereiten, wird für diese Zahlen die maximale Anzahl pro Benutzer angegeben, unabhängig davon, ob die E-Mail gesendet wird oder nicht.</p> </td>
  </tr> 
  <tr> 
   <td colname="col1"> <p>Bezeichnungen </p> </td> 
   <td colname="col2"> <p>Fügen Sie einem Angebot Beschriftungen hinzu, um sie zu gruppieren. Sie können eingeben und die Eingabetaste drücken, um eine neue Beschriftung zu erstellen oder mit der Eingabe zu beginnen und ein vorhandenes Angebot aus der Dropdownliste auszuwählen. </p> </td> 
  </tr> 
 </tbody> 
</table>

1. Füllen Sie die Darstellungsdetails aus.

   | Feld | Beschreibung |
   |---|---|
   | Kanal | Der Kanal, in dem diese Inhaltsdarstellung bereitgestellt werden kann. Campaign Standard-E-Mails ist der einzige Kanal, der derzeit verfügbar ist. |
   | Platzierung | Wählen Sie die Stelle aus, an der diese Inhaltsdarstellung bereitgestellt werden kann. Platzierungen werden auf der Registerkarte Platzierungen vorausgefüllt. Sie müssen jede Inhaltsdarstellung mit einer Platzierung aus dem Dropdownmenü verknüpfen. Sie können nicht mehrere Inhaltsdarstellungen mit derselben Platzierung im gleichen Angebot erstellen. |
   | Inhaltstyp | Wählen Sie einen Inhaltstyp aus einem Bild, einer Bild-URL, einem Text oder HTML. |
   | Link umleiten | Dieses Feld wird angezeigt, wenn Sie einen Inhaltstyp des Bild- oder Bild-URL auswählen. Dies ist der Link, zu dem der Benutzer umgeleitet wird, wenn er in einer E-Mail auf dieses Angebot klickt. |

1. Klicken Sie auf **[!UICONTROL Speichern und Vorschau]**, um die Details Ihres Angebots vor dem Senden zu überprüfen.
1. Klicken Sie auf **[!UICONTROL Genehmigen]**, um das Angebot zu genehmigen. Sobald sich das Angebot im genehmigten Zustand befindet, kann es in einer Angebotsaktivität verwendet werden.

   Wenn Sie nicht über die erforderlichen Berechtigungen zum Genehmigen eines Angebots verfügen, klicken Sie stattdessen auf **[!UICONTROL Senden]**. Das Angebot wird dann in der Angebotsbibliothek mit einem ausstehenden Status angezeigt. Sobald ein Benutzer mit Genehmigungsrechten die Genehmigung erteilt hat, steht sie in einer Angebotsaktivität zur Verfügung.
