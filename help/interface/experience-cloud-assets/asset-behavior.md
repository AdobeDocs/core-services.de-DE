---
description: Richtlinien zum Verhalten freigegebener Ordner beim Verschieben, Löschen und Wiederherstellen.
keywords: Asset-Freigabe; Creative Cloud; Hauptdienste
seo-description: Richtlinien zum Verhalten freigegebener Ordner beim Verschieben, Löschen und Wiederherstellen.
seo-title: Verhalten freigegebener Ordner
solution: Experience Cloud
title: Verhalten freigegebener Ordner
uuid: 86348401-f4b1-4efe-acd1-7e73a7030edf
translation-type: tm+mt
source-git-commit: af5339fe58ce884345804574c209907d6504a483

---


# Verhalten freigegebener Ordner

Richtlinien zum Verhalten freigegebener Ordner beim Verschieben, Löschen und Wiederherstellen.

>[!NOTE]
>
>Freigegebene Experience Cloud-Ordner und -Assets werden 1:1 auf dem Creative Cloud-Desktop gespiegelt. Wenn ein Experience Cloud-Benutzer einen Ordner bearbeitet (löscht, hinzufügt, Freigabe entfernt), wird diese Aktion auf dem Creative Cloud-Desktop und im Web gespiegelt. Wird die Freigabe eines Ordners aufgehoben, so verschwindet dieser Ordner mit seinen Assets also von Ihrem lokalen System. Dabei werden der ehemals freigegebene Ordner und sein Inhalt in Ihren Systempapierkorb verschoben, von wo aus Sie ihn auf Ihrem System wiederherstellen können.

## Nicht freigegebener Ordner in freigegebenen Ordner {#section_A9BAC1A244A246A984AC62660E61E0C0}

Sie verschieben einen nicht freigegebenen Ordner in einen freigegebenen Ordner.

![](assets/01_assets_move.png)

**Ergebnis:** Beide Ordner sind nun freigegeben.

## Freigegebener Ordner in nicht freigegebenen Ordner {#section_8BA83001DCEC4CF084B980C4A660F59A}

Sie verschieben einen freigegebenen Ordner in einen nicht freigegebenen Ordner.

![](assets/02_assets_move.png)

**Ergebnis**: Der nicht freigegebene Ordner bleibt nicht freigegeben. Der freigegebene Ordner bleibt freigegeben.

## Inhalt eines nicht freigegebenen Ordners in freigegebenen Ordner {#section_2941ED0DC52E4573AC1AB4C22313DD8E}

Sie verschieben Inhalt aus einem nicht freigegebenen Ordner in einen freigegebenen Ordner.

![](assets/03_assets_move.png)

**Ergebnis:** Der Inhalt ist nun freigegeben, und alle Mitwirkenden können ihn sehen. Der Speicherbedarf erhöht sich entsprechend der Größe des Inhalts.

## Archivierter und gelöschter freigegebener Inhalt {#section_5210D5F4943A44D0BA675D8EB4EAE20F}

Sie archivieren und löschen Inhalt aus einem freigegebenen Ordner.

![](assets/04_assets_move.png)

**Ergebnis:** Der Inhalt wird für den Eigentümer des Ordners archiviert. Mitwirkende, denen der Inhalt nicht gehört, können nicht mehr darauf zugreifen.

## Eigener freigegebener Inhalt in nicht freigegebenen Ordner {#section_3810A364B67E4B8C9CA244BC52BF91BB}

Sie verschieben Inhalt aus einem freigegebenen Ordner, der Ihnen gehört, in einen nicht freigegebenen Ordner.

![](assets/05_assets_move.png)

**Ergebnis:** Der Inhalt ist nun nicht mehr freigegeben. Die am freigegebenen Ordner Mitwirkenden haben auf den Inhalt keinen Zugriff mehr.

## Inhalt eines anderen Benutzers in nicht freigegebenen Ordner {#section_310766EBF0DC4C0BB4AB3E8A4DAEBE07}

Sie verschieben Inhalt aus einem freigegebenen Ordner, der einem anderen Mitwirkenden gehört, in einen nicht freigegebenen Ordner.

![](assets/06_assets_move.png)

**Ergebnis:** Der Inhalt wird aus dem freigegebenen Ordner entfernt und im nicht freigegebenen Ordner angezeigt. Die am freigegebenen Ordner Mitwirkenden haben auf den Inhalt keinen Zugriff mehr. Der Inhalt wird für den Eigentümer des freigegebenen Ordners archiviert.

Eigentümer und Editoren können Inhalt, der ihnen nicht gehört, verschieben, Benutzer mit reiner Anzeigeberechtigung hingegen nicht. Inhalt, der durch Eigentümer oder Editoren verschoben wurde, steht keinem Benutzer mehr in einem freigegebenen Ordner zur Verfügung.

## Archivierter oder gelöschter eigener Inhalt {#section_B314B13512A5409C87C49DFDB7602E14}

Einen freigegebenen Ordner, der Ihnen gehört, können Sie im Web archivieren bzw. auf Ihrem Desktop löschen.

![](assets/07_assets_move.png)

**Ergebnis:** Die Freigabe des Ordners wird aufgehoben, bevor der Ordner archiviert wird. Danach haben die Mitwirkenden keinen Zugriff mehr auf den Ordner.

## Freigegebener Ordner in anderen freigegebenen Ordner {#section_0A3F203D048D4D1586E9850DC92C51E9}

Sie verschieben einen freigegebenen Ordner, der Ihnen gehört, in einen anderen freigegebenen Ordner, der Ihnen oder einem anderen Benutzer gehört.

![](assets/09_assets_move.png)

**Ergebnis:** Da der Ordner in Ordner 2 verschoben wird, wird er für die neuen Mitwirkenden freigegeben.

## Freigegebener Inhalt in anderen freigegebenen Ordner {#section_69F6C312792A4CD2831BD14A340F850E}

Sie verschieben Inhalt aus einem freigegebenen Ordner in einen anderen freigegebenen Ordner.

![](assets/11_assets_move.png)

**Ergebnis:** Der Inhalt wird im zweiten Ordner angezeigt und nun mit anderen Mitwirkenden geteilt. Aus dem ersten Ordner wird der Inhalt entfernt. Der Eigentümer sieht ihn als archiviert, während die früheren Mitwirkenden keinen Zugriff mehr darauf haben.

## Aus Archiv wiederhergestellter Inhalt {#section_DEA990B3581741F89FBB81D18C2AB449}

Sie stellen Inhalt aus einem Archiv wieder her, der sich zuvor in einem freigegebenen Ordner befand. Bei der Archivierung waren Sie Eigentümer des Inhalts.

![](assets/12_assets_move.png)

**Ergebnis:** Der Inhalt wird im ehemaligen freigegebenen Ordner wiederhergestellt, und alle Mitwirkenden können wieder darauf zugreifen. Falls der freigegebene Ordner nicht mehr existiert, wird der Inhalt in eine nicht freigegebene Kopie des bzw. der ursprünglichen übergeordneten Ordner(s) eingefügt.
