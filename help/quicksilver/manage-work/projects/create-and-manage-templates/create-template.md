---
product-area: templates
navigation-topic: templates-navigation-topic
title: Créer un modèle de projet
description: Vous pouvez créer et supprimer des modèles à partir de la zone Modèles. Lors de la création d’un modèle, vous pouvez saisir les informations de toutes les tâches et des paramètres du futur projet. Ces informations seront ensuite transférées vers tout projet que vous créez à partir du modèle.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 98%

---

# Créer un modèle de projet

<!-- Audited: 1/2024 -->

Vous pouvez créer et supprimer des modèles à partir de la zone Modèles. Lors de la création d’un modèle, vous pouvez saisir les informations de toutes les tâches et des paramètres du futur projet. Ces informations seront ensuite transférées vers tout projet que vous créez à partir du modèle.

>[!NOTE]
>
>Un modèle et ses tâches n’ont pas de dates réelles, mais plutôt une indication du jour (à partir duquel le projet peut démarrer) où une tâche peut commencer et le jour où la tâche devra être terminée. Lors de l’utilisation de modèles pour créer les projets futurs, les projets recevront des dates réelles. Pour plus d’informations, voir [Créer un projet](../create-projects/create-project.md).


Vous pouvez créer un modèle de la manière suivante :

* À partir de zéro, comme décrit dans cet article.
* À partir de projets existants, en enregistrant un projet en tant que modèle.

  Pour plus d’informations sur la création de modèles à partir de projets existants, voir [Enregistrer un projet en tant que modèle](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* En le copiant à partir d’un autre modèle.

  Pour plus d’informations sur la copie d’un modèle existant, voir [Copier un modèle de projet](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* En important des plans directeurs. Vous devez être un administrateur ou une administratrice Workfront pour importer des plans directeurs. Pour plus d’informations, voir [Configurer un plan directeur](../../../administration-and-setup/blueprints/configure-template-package.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

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
   <td> <p>Nouvelle : standard </p><p>Ou </p><p>Actuelle : formule </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Vous devez être un administrateur ou une administratrice système pour importer des modèles à partir de plans directeurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux modèles</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Par défaut, vous disposez d’autorisations de gestion sur les modèles que vous créez.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un modèle

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (si disponible), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis sur **Modèles**.

1. Cliquez sur **Nouveau modèle**.

   Le modèle n’a pas de titre.

   ![Nouveau modèle](assets/create-template-nwe-2022-350x102.png)

1. Spécifiez un nom pour le nouveau modèle dans l’en-tête du modèle, puis appuyez sur **Entrée**.
1. Cliquez sur la section **Tâches de modèles** dans le panneau de gauche.
1. Cliquez sur **Commencer à ajouter des tâches de modèles**

   Ou

   Cliquez sur **Nouvelle tâche de modèle** pour commencer à ajouter des tâches à votre modèle.

   L’ajout de tâches de modèles à un modèle est identique à l’ajout de tâches à un projet.

   Pour plus d’informations sur l’ajout de tâches à un projet, voir [Créer des tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Vous ne pouvez pas ajouter de tâches récurrentes à un modèle.

1. (Facultatif) Cliquez sur l’icône **Graphique de Gantt** dans le coin supérieur droit de la liste des tâches pour afficher une représentation visuelle de la liste des tâches du modèle.

   >[!TIP]
   >
   >Vous ne pouvez pas modifier les tâches directement à partir de ce graphique de Gantt.

1. Pour ajouter des informations à votre nouveau modèle, cliquez sur le menu **Plus** ![](assets/more-icon.png), puis sur **Modifier**.

   Pour plus d’informations sur la modification d’un modèle, voir [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Cliquez sur **Enregistrer les modifications**.
1. (Facultatif) Pour ajouter des éléments supplémentaires au modèle, reportez-vous à la section [Ajouter des éléments supplémentaires à un modèle](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template) dans l’article [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Paramètres de modèle déterminés par l’association de groupe

L’association d’un modèle de projet à un groupe (ou l’absence d’un groupe) affecte la manière dont les préférences de projet, de tâche et de problème déterminent certains paramètres du modèle. Pour plus d’informations, voir la section [Créer et modifier des modèles de projet d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates) dans l’article [Créer et modifier des modèles de projet d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
