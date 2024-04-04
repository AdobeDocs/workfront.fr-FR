---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Installer un package de promotion d’environnement
description: La fonctionnalité de promotion de l’environnement est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Découvrez comment installer un package de promotion d’environnement dans un environnement cible.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 5d84d50b8984bbff7bbc02ffc0ce86ec1f486742
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Installer un package de promotion d’environnement

>[!NOTE]
>
>Pour installer un package, vous devez être connecté à l’environnement dans lequel vous souhaitez installer le package. C’est l’environnement dans lequel vous copiez des objets. **to**.

1. Accédez à l’environnement dans lequel vous souhaitez installer le package.
1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionner **Système** dans le volet de navigation de gauche, puis sélectionnez **Promotion de l’environnement**.
1. Sélectionnez le package dans la liste affichée.
1. Pour installer le package, cliquez sur **Installer** dans le coin supérieur droit de l’écran.
1. Mappez chaque objet du package à l’objet correspondant dans l’environnement cible.

   Pour plus d’informations, voir [Mappage](#mapping) dans cet article


## Mappage

Chaque type d’objet est répertorié dans le volet de navigation de gauche et sur une carte. La carte affiche les objets de ce type et indique s’ils existent dans l’environnement cible. Vous pouvez déterminer comment ces objets seront déplacés vers l’environnement cible.

* Créer : créez un objet dans l&#39;environnement cible. Si l’objet existe dans l’environnement cible, vous pouvez créer un objet portant un nouveau nom. S’il n’existe pas dans l’environnement cible, vous pouvez créer l’objet avec un nouveau nom ou avec le nom de l’objet dans le package.
* Utiliser existant : l’objet du package n’est pas installé, et l’objet qui existait déjà dans l’environnement cible est inchangé.
* Remplacer existant : (actuellement indisponible) l’objet du package remplace l’objet existant dans l’environnement cible.
* Ne pas utiliser : l’objet du package n’est pas installé dans l’environnement cible. Si vous sélectionnez Ne pas utiliser, un message d’erreur s’affiche, détaillant l’impact de ce choix sur d’autres objets ou champs.

Les valeurs par défaut sont `Create new` si l’objet n’existe pas dans l’environnement cible, et `Use existing` si l’objet existe dans l’environnement cible. Vous pouvez rétablir le mappage par défaut en cliquant sur **Réinitialiser le mappage par défaut**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
