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
source-git-commit: f65fbe7ceab19cee75aa0346c389907707c47c8b
workflow-type: tm+mt
source-wordcount: '401'
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
1. Pour chaque objet ayant une collision, sélectionnez la manière de résoudre la collision.

   Pour résoudre une collision, cliquez sur la flèche de liste déroulante en regard du type d’objet, puis sélectionnez l’action à effectuer.

   Pour plus d’informations, voir [Collisions](#collisions) dans cet article
1. Pour déployer le package dans le nouvel environnement, cliquez sur **Déployer** dans le coin supérieur droit de l’écran.

## Collisions

Des collisions se produisent lorsqu’un objet faisant partie du package d’installation existe déjà dans l’environnement cible. Lorsque cela se produit, vous pouvez choisir comment résoudre la collision. Les collisions sont résolues au niveau de l’objet.

Vous pouvez afficher les collisions en cliquant sur la liste déroulante en regard de chaque type d’objet. Les colonnes s&#39;affichent dans la colonne Collision .

Pour résoudre une collision, sélectionnez une action dans la colonne Action de déploiement ou utilisez l’action par défaut qui est déjà affichée.

* **Créer avec un nouveau nom**: créez un objet dans l’environnement cible. Si l’objet existe dans l’environnement cible, vous pouvez créer un objet portant un nouveau nom. S’il n’existe pas dans l’environnement cible, vous pouvez créer l’objet avec un nouveau nom ou avec le nom de l’objet dans le package.
* **Utiliser existant**: l’objet du package n’est pas installé et l’objet qui existait déjà dans l’environnement cible est inchangé.
* **Remplacer**: l’objet du package remplace l’objet existant dans l’environnement cible.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Les valeurs par défaut sont `Create new` si l’objet n’existe pas dans l’environnement cible, et `Use existing` si l’objet existe dans l’environnement cible. Vous pouvez rétablir le mappage par défaut en cliquant sur **Réinitialiser le mappage par défaut**.



<!--
## Collisions

A collision occurs when <!--???--.

In Workfront, a potential collision is marked with a blue dot. You can select 

You can select whether to show all package contents, or collisions only.

## Comparison tool

-->
