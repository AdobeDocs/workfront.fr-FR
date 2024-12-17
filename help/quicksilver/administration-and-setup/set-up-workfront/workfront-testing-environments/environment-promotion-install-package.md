---
user-type: administrator
content-type: how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Installer un package de promotion environnementale
description: La fonctionnalité de promotion d’environnement est destinée à fournir la possibilité de déplacer des objets liés à la configuration d’un environnement à un autre. Découvrez comment installer un package de promotion d’environnement dans un environnement cible.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: fe213fe7-5bb8-479c-926b-761cbdd7ba4e
source-git-commit: 8fe93796b2bc89352ac2c924d6a5e3bf25551ff0
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 9%

---

# Installer un package de promotion environnementale

Après avoir créé un package, vous pouvez l’installer dans un autre environnement.

Vous devez installer un package dans l’environnement dans lequel vous souhaitez copier des objets **vers**. Par exemple, si vous configurez un projet dans votre environnement de sandbox d’actualisation personnalisée et que vous le promouvez dans votre environnement de production, vous devez installer le package dans votre environnement de production.

>[!IMPORTANT]
>
>* Si votre sandbox d’actualisation personnalisée est actualisé pendant que vous configurez l’objet pour la promotion de l’environnement, cette configuration est perdue lors de l’actualisation. Nous vous recommandons de ne pas actualiser votre sandbox d’actualisation personnalisée tant que tous les objets et packages de promotion d’environnement en attente n’ont pas été promus avec succès.
>* Les objets créés dans l’environnement cible dans le cadre de l’installation du package n’ont **pas** le même identifiant que l’objet de l’environnement d’origine. Cela est dû au fait que les identifiants sont attribués par le système lors de la création des objets.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td>Plan <strong>[!DNL Adobe Workfront]</strong>
   </td>
   <td> Prime ou Ultimate (nouveaux plans uniquement)
   </td>
  </tr>
  <tr>
   <td>Licences <strong>[!DNL Adobe Workfront]</strong>
   </td>
   <td> [!UICONTROL Standard]
   </td>
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td>Vous devez être administrateur ou administratrice [!DNL Workfront].
   </td>
  </tr>
</table>

Pour plus d’informations sur ce tableau, voir la section [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Un package de promotion d’environnement doit être créé avant de pouvoir être installé.

Pour obtenir des instructions, voir [Créer ou modifier un package de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md).

## Statut du package pour l’installation

Un package doit avoir le statut ACTIF pour être installé dans votre environnement de production.

Nous vous recommandons de déplacer le package au statut TEST et de l’installer dans un autre sandbox pour le tester.  Si ce test réussit, sans erreur, déplacez le package vers ACTIF pour l’installer dans votre environnement de production.

Pour modifier le statut d’un package :

1. Sélectionnez le package comme décrit dans la section [Modifier ou assembler un package existant](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md#create-or-edit-an-environment-promotion-package) de l’article Créer et modifier des packages de promotion d’environnement.
1. Cliquez sur **Modifier le package**.
1. Cliquez sur **Statut**.
1. Sélectionnez le statut souhaité dans le menu déroulant.

Pour plus d’informations sur les statuts, voir [Statuts de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) dans l’article Présentation du déplacement d’objets entre les environnements Workfront.

## Installer un package

>[!NOTE]
>
>* Pour installer un package, vous devez être connecté à l’environnement dans lequel vous souhaitez installer le package. Il s’agit de l’environnement dans lequel vous copiez des objets **vers**.

1. Accédez à l’environnement dans lequel vous souhaitez installer le package.
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **[!UICONTROL Configuration]** ![Icône Configuration](/help/_includes/assets/gear-icon-setup.png).
1. Sélectionnez **Système** dans le volet de navigation de gauche, puis sélectionnez **Promotion de l’environnement**.
1. Sélectionnez le package dans la liste qui s&#39;affiche.
1. Pour chaque objet qui présente une collision, sélectionnez comment résoudre la collision.

   Pour résoudre une collision, cliquez sur la flèche déroulante en regard du type d’objet, puis sélectionnez l’action à effectuer.

   Pour plus d’informations, voir [Collisions](#collisions) dans cet article
1. Pour déployer le package dans le nouvel environnement, cliquez sur **Déployer** dans le coin supérieur droit de l’écran.

## Collisions

Une collision est un objet trouvé dans l’environnement cible d’une installation qui correspond à l’un des objets installés à partir de l’environnement source. Les collisions sont détectées en comparant les noms et identifiants des objets sources avec ceux des objets de l’environnement cible. Les collisions sont également détectées en comparant les objets source aux enregistrements d&#39;objets installés précédemment.

Lorsqu’une collision se produit, vous pouvez choisir comment la résoudre. Les collisions sont résolues au niveau de l’objet.

Vous pouvez afficher les collisions en cliquant sur la liste déroulante en regard de chaque type d’objet. Les collisions s’affichent dans la colonne Collision .

>[!NOTE]
>
>Les collisions détectées peuvent ne pas être les objets que vous souhaitez remplacer ou utiliser dans votre installation. Nous vous recommandons de valider les collisions détectées pour vous assurer que les cibles d’installation sont correctes.

Pour résoudre une collision, sélectionnez une action dans la colonne Action de déploiement ou utilisez l’action par défaut déjà affichée.

* **Créer avec un nouveau nom** : créez un objet dans l’environnement cible. Si l’objet existe dans l’environnement cible, vous pouvez créer un objet portant un nouveau nom. S’il n’existe pas dans l’environnement cible, vous pouvez créer l’objet avec un nouveau nom ou avec le nom que l’objet porte dans le package.
* **Utiliser existant** : l’objet du package n’est pas installé et l’objet qui existait déjà dans l’environnement cible reste inchangé.
* **Remplacer** : l’objet du package remplace l’objet existant dans l’environnement cible.

  Vous pouvez également choisir des objets à remplacer même si aucune collision n’est détectée.

  Pour plus d’informations sur l’impact du remplacement sur les objets parents et enfants, consultez la section [Remplacement des objets parents et enfants](#overwriting-parent-and-child-objects) de cet article.
<!--
* Do not use: The object in the package is not installed in the target environment. If you select Do not use, an error message will appear detailing how this choice will affect other objects or fields.
-->

Les valeurs par défaut sont `Create new` si l’objet n’existe pas dans l’environnement cible et `Use existing` si l’objet existe dans cet environnement. Vous pouvez revenir au mappage par défaut en cliquant sur **Réinitialiser au mappage par défaut**.

## Remplacement des objets parents et enfants

Certains objets de votre package de promotion peuvent avoir des objets enfants. Par exemple, un projet (parent) a des tâches (enfants). Lors du remplacement d’un objet parent, les objets enfants sont traités comme suit :

* Les objets enfants qui existent à la fois dans le package et la cible sont mis à jour dans la cible pour correspondre au package.
* Les objets enfants qui existent dans le package mais pas la cible seront créés.
* Les objets enfants qui existent dans la cible mais pas dans le package resteront inchangés.

Cette fonctionnalité affecte les objets parents et enfants suivants :

| Objet parent | Objets enfants |
|---|---|
| Projet | Task<br>QueueDef (Définition de file d’attente)<br>RoutingRule |
| Modèle | TemplateTask<br>QueueDef (définition de file d&#39;attente)<br>RoutingRule |
| Paramètre (champ de formulaire personnalisé) | ParameterOption (option de champ de formulaire personnalisé) |
| CalendarInfo | CalendarSection |
| QueueDef (définition de file d’attente) | QueueTopicGroup<br>QueueTopic |

