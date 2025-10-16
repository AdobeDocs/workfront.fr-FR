---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Vue d’ensemble de la date de début effective du projet
description: Les projets, les tâches et les problèmes ont une date de début effective dans Adobe Workfront. Pour les tâches et les problèmes, il s’agit de la date à laquelle ils ont été marqués comme En cours. Pour les projets, il s’agit de la date à laquelle la première tâche du projet est marquée comme En cours ou est terminée.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 95%

---

# Vue d’ensemble de la date de début effective du projet

Les projets, les tâches et les problèmes ont une date de début effective dans Adobe Workfront. Pour les tâches et les problèmes, il s’agit de la date à laquelle ils ont été marqués comme En cours. Pour les projets, il s’agit de la date à laquelle la première tâche du projet est marquée comme En cours ou est terminée.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td><p>Léger ou supérieur</p> 
   <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou supérieur aux projets</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou de niveau supérieur sur un projet</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Remarques concernant les dates de début effectives dans Workfront

* La date de début effective se trouve dans la section Détails des projets, tâches et problèmes. 
* La date de début effective d’un projet, d’une tâche ou d’un problème n’est pas renseignée lors de la création de ces éléments.
* La date de début effective est renseignée lorsque le travail commence réellement sur le projet, la tâche ou le problème.
* La date de début effective ne s’affiche pas dans l’onglet Détails du projet si le travail sur le projet n’a pas encore commencé.

  La date de début effective est vide dans les onglets Détails de la tâche et du problème si le travail n’a pas encore commencé dessus.

* Vous pouvez modifier manuellement la date de début effective d’une tâche ou d’un problème, mais vous ne pouvez pas modifier la date de début effective d’un projet.

## Remarques concernant les dates de début effectives des projets

* Workfront définit automatiquement la date effective d’un projet lorsque l’un des événements suivants se produit :

   * Une personne cessionnaire de tâche modifie le statut d’une tâche, passant de *Nouveau* à tout autre statut qui n’équivaut pas à *Nouveau*.

   * Une personne cessionnaire de tâche modifie le pourcentage de tâche terminé.

     >[!IMPORTANT]
     >
     >La date de début effective du projet n’est pas renseignée lorsque le projet est marqué comme Actuel.Le travail effectif doit commencer sur les tâches du projet avant que la date de début effective du projet ne soit renseignée.

     Dans ce cas, la date de début effective du projet est définie sur la date et l’heure auxquelles ces actions se sont produites pour la première tâche du projet. Cela indique que le projet a réellement commencé à cette date et cette heure.

## Localiser la date de début effective d’un projet

Vous pouvez localiser la date de début effective d’un projet dans les zones suivantes :

* dans la section Détails d’un projet ;
* dans un rapport ou une vue de projet, lorsque vous ajoutez la date de début effective de l’objet Projet dans le rapport.

  Pour plus d’informations sur la création de rapports, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Pour localiser la date de début effective dans la section Détails du projet, procédez comme suit :

1. Cliquez sur l’icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **Projets**.
1. Cliquez sur le projet pour lequel vous souhaitez afficher la date de début effective.
1. Cliquez sur **Détails du projet** dans le panneau de gauche, puis accédez à la section **Vue d’ensemble**.

   La date de début effective s’affiche avec les autres dates du projet.

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)


