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
recommendations: noDisplay, noCatalog
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: b26f20b13a18c6e727fcf9e267ba9c53e5b566dc
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 2%

---

# Installer un package de promotion d’environnement

Après avoir créé un package, vous pouvez l’installer dans un autre environnement.

Vous devez installer un package dans l’environnement dans lequel vous souhaitez copier des objets. **to**. Par exemple, si vous configurez un projet dans votre environnement Sandbox d’actualisation personnalisée et que vous le faites passer à votre environnement de production, vous devez installer le package dans votre environnement de production.

>[!IMPORTANT]
>
>Si votre environnement de test d’actualisation personnalisée est actualisé pendant que vous configurez l’objet pour la promotion de l’environnement, cette configuration sera perdue lors de l’actualisation. Nous vous recommandons de ne pas actualiser votre sandbox d’actualisation personnalisée à moins que tous les objets et packages de promotion d’environnement en cours n’aient été promus avec succès.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan</strong>
   </td>
   <td> Prime ou Ultimate (Nouveaux plans uniquement)
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licences</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configurations du niveau d’accès
   </td>
   <td>Vous devez être un [!DNL Workfront] administrateur.
   </td>
  </tr>
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Un package de promotion d’environnement doit être créé avant de pouvoir être installé.

Pour obtenir des instructions, voir [Créer ou modifier un package de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## État du package pour l’installation

Un package doit être à l’état ACTIF pour être installé dans votre environnement de production.

Nous vous recommandons de déplacer le package vers l’état TEST et de l’installer dans un autre environnement de test pour tester le package.  Si ce test est réussi, sans erreur, déplacez le package vers ACTIVE pour l’installer dans votre environnement de production.

Pour modifier l’état d’un module :

1. Sélectionnez le module comme décrit dans la section  [Modifier ou assembler un package existant](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) dans l’article Créer et modifier des packages de promotion d’environnement.
1. Cliquez sur **Modifier le module**.
1. Cliquez sur **État**.
1. Sélectionnez un état dans le menu déroulant.

Pour plus d’informations sur les états, voir [Statuts des promotions d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) dans l’article Présentation du déplacement d’objets entre les environnements Workfront.

## Installer un package

>[!NOTE]
>
>* Pour installer un package, vous devez être connecté à l’environnement dans lequel vous souhaitez installer le package. C’est l’environnement dans lequel vous copiez des objets. **to**.

1. Accédez à l’environnement dans lequel vous souhaitez installer le package.
1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionner **Système** dans le volet de navigation de gauche, puis sélectionnez **Promotion de l’environnement**.
1. Sélectionnez le package dans la liste affichée.
1. Pour chaque objet ayant une collision, sélectionnez la manière de résoudre la collision.

   Pour résoudre une collision, cliquez sur la flèche déroulante en regard du type d’objet, puis sélectionnez l’action à effectuer.

   Pour plus d’informations, voir [Collisions](#collisions) dans cet article
1. Pour déployer le package dans le nouvel environnement, cliquez sur **Déployer** dans le coin supérieur droit de l’écran.

## Collisions

Une collision est un objet qui se trouve dans l’environnement cible d’une installation qui correspond à l’un des objets installés à partir de l’environnement source. Les collisions sont détectées en comparant les noms et les identifiants des objets sources aux objets de l’environnement cible. Les collisions sont également détectées en comparant les objets source aux enregistrements d’objets précédemment installés.

Lorsqu’une collision se produit, vous pouvez sélectionner la manière de résoudre la collision. Les collisions sont résolues au niveau de l’objet.

Vous pouvez afficher les collisions en cliquant sur la liste déroulante en regard de chaque type d’objet. Les colonnes s&#39;affichent dans la colonne Collision .

>[!NOTE]
>
>Les collisions détectées peuvent ne pas être les objets que vous souhaitez remplacer ou utiliser dans votre installation. Nous vous recommandons de valider les collisions détectées pour vous assurer que les cibles d’installation sont correctes.

Pour résoudre une collision, sélectionnez une action dans la colonne Action de déploiement ou utilisez l’action par défaut qui est déjà affichée.

* **Créer avec un nouveau nom**: créez un objet dans l’environnement cible. Si l’objet existe dans l’environnement cible, vous pouvez créer un objet portant un nouveau nom. S’il n’existe pas dans l’environnement cible, vous pouvez créer l’objet avec un nouveau nom ou avec le nom de l’objet dans le package.
* **Utiliser existant**: l’objet du package n’est pas installé et l’objet qui existait déjà dans l’environnement cible est inchangé.
* **Remplacer**: l’objet du package remplace l’objet existant dans l’environnement cible.

  Vous pouvez également choisir des objets à remplacer même si une collision n’est pas détectée.

  Pour plus d’informations sur l’impact du remplacement sur les objets parents et enfants, voir [Remplacement des objets parents et enfants](#overwriting-parent-and-child-objects) dans cet article.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Les valeurs par défaut sont `Create new` si l’objet n’existe pas dans l’environnement cible, et `Use existing` si l’objet existe dans l’environnement cible. Vous pouvez rétablir le mappage par défaut en cliquant sur **Réinitialiser le mappage par défaut**.

## Remplacement des objets parents et enfants

Certains objets de votre package de promotion peuvent comporter des objets enfants. Par exemple, un projet (parent) comporte des tâches (enfants). Lors du remplacement d’un objet parent, les objets enfants sont traités comme suit :

* Les objets enfants présents dans le package et la cible sont mis à jour dans la cible pour correspondre au package.
* Les objets enfants qui existent dans le package mais pas dans la cible seront créés.
* Les objets enfants qui existent dans la cible, mais pas dans le package, restent inchangés.

Cette fonctionnalité affecte les objets parents et enfants suivants :

| Objet parent | Objets enfant |
|---|---|
| Projet | Tâche<br>QueueDef (définition de file d’attente)<br>RoutingRule |
| Modèle | TemplateTask<br>QueueDef (définition de file d’attente)<br>RoutingRule |
| Paramètre (champ de formulaire personnalisé) | ParameterOption (option de champ de formulaire personnalisé) |
| CalendarInfo | Section du calendrier |
| QueueDef (définition de file d’attente) | QueueTopicGroup<br>QueueTopic |

