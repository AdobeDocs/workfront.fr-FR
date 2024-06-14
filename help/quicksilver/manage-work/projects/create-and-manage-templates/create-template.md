---
product-area: templates
navigation-topic: templates-navigation-topic
title: Créer un modèle de projet
description: Vous pouvez créer et supprimer des modèles dans la zone Modèles . Lors de la création d’un modèle, vous pouvez saisir les informations pour toutes les tâches et pour les futurs paramètres du projet. Ces informations seront ensuite transférées vers tout projet que vous créez à partir du modèle.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 7%

---

# Créer un modèle de projet

<!-- Audited: 1/2024 -->

Vous pouvez créer et supprimer des modèles dans la zone Modèles . Lors de la création d’un modèle, vous pouvez saisir les informations pour toutes les tâches et pour les futurs paramètres du projet. Ces informations seront ensuite transférées vers tout projet que vous créez à partir du modèle.

>[!NOTE]
>
>Un modèle et ses tâches n’ont pas de dates réelles, mais plutôt une indication du jour (à partir duquel le projet peut démarrer) où une tâche peut commencer et le jour où la tâche peut devoir être terminée. Lors de l’utilisation de modèles pour créer les projets futurs, les projets recevront des dates réelles. Pour plus d’informations, voir [Création d’un projet](../create-projects/create-project.md).


Vous pouvez créer un modèle de la manière suivante :

* À partir de zéro, comme décrit dans cet article.
* À partir de projets existants, en enregistrant un projet en tant que modèle.

  Pour plus d’informations sur la création de modèles à partir de projets existants, voir [Enregistrement d’un projet en tant que modèle](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* En la copiant à partir d’un autre modèle.

  Pour plus d’informations sur la copie d’un modèle existant, voir [Copier un modèle de projet](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* En important des plans directeurs. Pour importer des plans directeurs, vous devez être un administrateur Workfront. Pour plus d’informations, voir [Configuration d’un plan directeur](../../../administration-and-setup/blueprints/configure-template-package.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard </p><p>Ou </p><p>Actuel : formule </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Vous devez être un administrateur système pour importer des modèles à partir de plans directeurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux modèles</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Par défaut, vous disposez des autorisations de gestion pour les modèles que vous créez.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un modèle

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Modèles**.

1. Cliquez sur **Nouveau modèle**.

   Le modèle est sans titre.

   ![Nouveau modèle](assets/create-template-nwe-2022-350x102.png)

1. Indiquez un nom pour le nouveau modèle dans l’en-tête du modèle, puis appuyez sur **Saisissez .**
1. Cliquez sur le bouton **Tâches de modèle** dans le panneau de gauche.
1. Cliquez sur **Commencer à ajouter des tâches de modèle**.

   Ou

   Cliquez sur **Nouvelle tâche de modèle** pour commencer à ajouter des tâches à votre modèle.

   L’ajout de tâches de modèle à un modèle est identique à l’ajout de tâches à un projet.

   Pour plus d’informations sur l’ajout de tâches à un projet, voir [Création de tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Vous ne pouvez pas ajouter de tâches récurrentes à un modèle.

1. (Facultatif) Cliquez sur le **Graphique Gantt** dans le coin supérieur droit de la liste des tâches pour afficher une représentation visuelle de la liste des tâches du modèle.

   >[!TIP]
   >
   >Vous ne pouvez pas modifier les tâches directement à partir de ce diagramme de Gantt.

1. Pour ajouter des informations à votre nouveau modèle, cliquez sur le bouton **Plus** menu ![](assets/more-icon.png), puis cliquez sur **Modifier**.

   Pour plus d’informations sur la modification d’un modèle, voir [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Cliquez sur **Enregistrer les modifications**.
1. (Facultatif) Pour ajouter des éléments supplémentaires au modèle, reportez-vous à la section [Ajouter des éléments supplémentaires à un modèle](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template) dans l’article [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Paramètres de modèle déterminés par l’association de groupe

L’association d’un modèle de projet à un groupe (ou l’absence d’un groupe) affecte la manière dont le projet, la tâche et les préférences d’émission déterminent certains paramètres du modèle. Pour plus d’informations, voir la section [Créer et modifier des modèles de projet de groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates) dans l’article [Créer et modifier des modèles de projet de groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
