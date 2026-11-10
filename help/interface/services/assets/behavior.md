---
description: Erfahren Sie mehr über Regeln, wie sich freigegebene Ordner verhalten, wenn sie in CX Enterprise verschoben, gelöscht und wiederhergestellt werden.
keywords: Asset-Freigabe; Creative Cloud; zentrale Dienste
solution: CX Enterprise
title: Verhalten freigegebener Ordner
uuid: 86348401-f4b1-4efe-acd1-7e73a7030edf
feature: Assets
topic: Administration
role: Admin
level: Experienced
exl-id: 5ddcb2f0-b491-466d-b357-aeacbfcf0b8e
TQID: 'https://experienceleague.adobe.com/sRgVt31HAxmjTMmMB0Kfs5fYEXKDjDu73hhAgfixu4o'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
    internal-label: Administration
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
    internal-label: Support
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
    internal-label: Getting started
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 26b7f77165cfe16db6bc816f83ba6bfdf9c925d4
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 90%
---
# Verhalten freigegebener Ordner

Richtlinien zum Verhalten freigegebener Ordner beim Verschieben, Löschen und Wiederherstellen.

>[!NOTE]
>
>Freigegebene CX Enterprise-Ordner und -Assets werden 1:1 auf dem Creative Cloud-Desktop gespiegelt. Wenn ein CX Enterprise-Benutzer einen Ordner ändert (löscht, fügt hinzu oder entfernt die Freigabe), wird die Aktion auf dem Creative Cloud-Desktop und im Web gespiegelt. Wenn die Freigabe eines Ordners aufgehoben wird, werden daher der Ordner und die Assets vom lokalen Computer gelöscht. Nachdem die Freigabe aufgehoben wurde, werden der Ordner und sein Inhalt in den Papierkorb auf Ihrem lokalen Computer verschoben, von wo Sie sie manuell auf Ihrem Computer wiederherstellen können.

## Nicht freigegebener Ordner in einen freigegebenen Ordner

Sie verschieben einen nicht freigegebenen Ordner in einen freigegebenen Ordner:

![Nicht freigegebener Ordner in freigegebenen Ordner](../../assets/01_assets_move.png)

**Ergebnis**: Beide Ordner werden freigegeben.

## Freigegebener Ordner in einen nicht freigegebenen Ordner

Sie verschieben einen freigegebenen Ordner in einen nicht freigegebenen Ordner.

![Freigegebener Ordner in nicht freigegebenen Ordner](../../assets/02_assets_move.png)

**Ergebnis**: Der nicht freigegebene Ordner bleibt nicht freigegeben. Der freigegebene Ordner bleibt freigegeben.

## Inhalt eines nicht freigegebenen Ordners in freigegebenen Ordner

Sie verschieben Content aus einem nicht freigegebenen Ordner in einen freigegebenen Ordner.

![Inhalte eines nicht freigegebenen Ordners in freigegebenen Ordner](../../assets/03_assets_move.png)

**Ergebnis:** Der Inhalt wird jetzt freigegeben, und alle Mitwirkenden können ihn sehen. Der Platz für die Datenspeicherung erhöht sich um die Inhaltsgröße.

## Archivierter und gelöschter freigegebener Inhalt

Sie archivieren oder löschen Inhalte, die sich in einem freigegebenen Ordner befinden.

![Archivierte und gelöschte freigegebene Inhalte](../../assets/04_assets_move.png)

**Ergebnis:** Der Inhalt wird für den Eigentümer des Ordners archiviert. Mitwirkende, die nicht Eigentümer des Content sind, können nicht mehr darauf zugreifen.

## Eigener freigegebener Inhalt in nicht freigegebenen Ordner

Sie verschieben Inhalte aus einem freigegebenen Ordner, dessen Eigentümer Sie sind, in einen nicht freigegebenen Ordner.

![Eigene freigegebene Inhalte in nicht freigegebenen Ordner](../../assets/05_assets_move.png)

**Ergebnis:** Die Inhalte werden jetzt nicht mehr freigegeben. Die am freigegebenen Ordner Mitwirkenden haben auf den Inhalt keinen Zugriff mehr.

## Inhalt eines anderen Benutzers in nicht freigegebenen Ordner

Sie verschieben Inhalte aus freigegebenen Ordnern, die Eigentum einer anderen Person sind, in einen nicht freigegebenen Ordner.

![Inhalte eines anderen Benutzers in nicht freigegebenen Ordner](../../assets/06_assets_move.png)

**Ergebnis:** Der Inhalt wird im nicht freigegebenen Ordner angezeigt und aus dem freigegebenen Ordner entfernt. Die am freigegebenen Ordner Mitwirkenden haben auf den Inhalt keinen Zugriff mehr. Der Inhalt wird für den Eigentümer des freigegebenen Ordners archiviert.

Eigentümer und Editoren können Inhalte verschieben, die ihnen nicht gehören, aber Betrachter können dies nicht. Wenn Eigentümer bzw. Eigentümerinnen und Editoren Inhalte verschieben, stehen diese keinem Benutzenden in einem freigegebenen Ordner zur Verfügung.

## Archivierter oder gelöschter eigener Ordner

Sie archivieren (über das Web) oder löschen (über den Desktop) einen freigegebenen Ordner, dessen Eigentümer bzw. Eigentümerin Sie sind.

![Archivierte oder gelöschte eigene Inhalte](../../assets/07_assets_move.png)

**Ergebnis:** Der Ordner wird nicht freigegeben; anschließend wird er archiviert. Die Mitwirkenden haben keinen Zugriff mehr auf den Ordner.

## Freigegebener Ordner in einen anderen freigegebenen Ordner

Sie verschieben einen freigegebenen Ordner, dessen Eigentümer Sie sind, in einen anderen freigegebenen Ordner, egal ob Sie dessen Eigentümer sind oder nicht.

![Freigegebener Ordner in anderen freigegebenen Ordner](../../assets/09_assets_move.png)

**Ergebnis:** Wenn der Ordner in Ordner 2 verschoben wird, wird er für die neuen Mitwirkenden freigegeben.

## Freigegebener Inhalt in einen anderen freigegebenen Ordner

Sie verschieben Inhalte aus einem freigegebenen Ordner in einen anderen freigegebenen Ordner.

![Freigegebene Inhalte in anderen freigegebenen Ordner](../../assets/11_assets_move.png)

**Ergebnis:** Der Inhalt wird in Ordner 2 angezeigt und jetzt für neue Mitwirkende freigegeben. Der Content wird aus dem Ordner 1 entfernt, und der Eigentümer bzw. die Eigentümerin sieht ihn als archiviert, während die anderen Mitwirkenden keinen Zugriff mehr darauf haben.

## Aus Archiv wiederhergestellter Inhalt

Sie stellen Content aus einem Archiv wieder her, das zu einem freigegebenen Ordner gehörte. Sie waren zum Zeitpunkt der Archivierung Eigentümer des Inhalts.

![Aus Archiv wiederhergestellte Inhalte](../../assets/12_assets_move.png)

**Ergebnis:** Der Inhalt wird im freigegebenen Ordner wiederhergestellt und alle Mitwirkenden können erneut darauf zugreifen. Wenn der freigegebene Ordner nicht mehr vorhanden ist, wird der Inhalt in eine nicht freigegebene Kopie des/der ursprünglichen übergeordneten Ordner(s) eingefügt.
