---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Ajouter des projets aux objectifs dans Objectifs Adobe Workfront
description: Vous pouvez lier les projets aux objectifs pour indiquer la progression de l’objectif, en fonction de la progression réelle du projet. Le projet devient un indicateur de progression pour l’objectif.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 86%

---

# Ajouter des projets aux objectifs dans Objectifs Adobe Workfront

<!--Audited for P&P only: 10/2025-->

Vous pouvez lier les projets aux objectifs pour indiquer la progression de l’objectif, en fonction de la progression réelle du projet. Le projet devient un indicateur de progression pour l’objectif.

En liant les projets aux objectifs, vous pouvez associer la planification stratégique (objectifs) de votre entreprise au travail réel effectué et réalisé par vos employés chaque jour (projets).

>[!IMPORTANT]
>
>Les objectifs au niveau du projet créés dans la zone Analyse de rentabilité d’un projet ne sont pas liés aux objectifs stratégiques créés dans les Objectifs Workfront. Pour plus d’informations sur les objectifs du projet d’analyse de rentabilité, voir [Créer des objectifs d’analyse de rentabilité](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Conditions d’accès

>[!NOTE]
>
>Votre entreprise peut choisir de continuer à utiliser les objectifs Adobe Workfront si elle a déjà acheté ce package par le passé. Pour plus de détails, contactez votre représentant de compte.
>
>Adobe Workfront Goals ne peut plus être acheté.

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Package Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licence Adobe Workfront</td>
 <td>
 <p>Contributeur ou version ultérieure</p>
<p>Requête ou supérieure</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuration du niveau d’accès</td>
 <td> <p>Modifier l’accès aux Objectifs</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <div>
  <p>Autorisations d’affichage ou de niveau supérieur sur l’objectif pour l’afficher</p>
  <p>Autorisations de gestion sur l’objectif pour le modifier</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Un modèle de mise en page comprenant la zone Objectifs du menu principal doit être affecté à tous les utilisateurs, y compris les administrateurs système. </p>  
</td>
  </tr>
</tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Observations relatives à la liaison des projets aux objectifs

* Vous pouvez ajouter à un objectif un projet qui répond aux critères suivants :

   * Vous devez disposer d’au moins une autorisation pour l’afficher.

     >[!NOTE]
     >
     >Si vous perdez les autorisations d’affichage du projet une fois que vous avez associé le projet à l’objectif, vous pouvez toujours afficher les informations du projet sur l’objectif, mais vous ne pouvez plus accéder au projet.

   * Le projet ne doit pas avoir le statut Inactif.

* Vous pouvez associer plusieurs projets à un objectif.
* Vous pouvez associer le même projet à plusieurs objectifs.
* Vous ne pouvez pas mettre à jour manuellement la progression d’un projet à partir de l’objectif auquel il est associé. Au lieu de cela, Workfront calcule le pourcentage terminé du projet et les Objectifs Workfront calculent la progression de l’objectif en utilisant ce pourcentage terminé. Cela met à jour l’objectif en temps réel après la mise à jour du pourcentage du projet.
* La durée du projet peut se trouver en dehors de la période d’un objectif. Si un projet dure plus longtemps que la date limite de l’objectif, vous pouvez toujours fermer votre objectif et le considérer comme terminé, mais le pourcentage terminé de l’objectif ne sera pas de 100 %. Le pourcentage terminé du projet n’est plus mis à jour sur l’objectif.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![Goal closed](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Lorsque vous supprimez un projet associé à un objectif, celui-ci est également supprimé de l’objectif.

  >[!CAUTION]
  >
  >Si l’objectif était actif avant que vous n’ayez supprimé le projet et qu’il n’existe aucun autre indicateur de progression sur l’objectif, celui-ci devient inactif.


## Ajouter des projets aux objectifs

1. Cliquez sur l&#39;icône **Menu principal** ![Icône du menu principal](assets/main-menu-icon.png) (brouillon pour Shell : ou cliquez sur les **Menu principal** ![lignes du menu principal](assets/three-line-main-menu-icon.png) dans le coin supérieur gauche, s&#39;il est disponible) , puis sur **Objectifs**.
1. Dans la liste des objectifs, cliquez sur le nom d’un objectif pour ouvrir la page de l’objectif.
1. Cliquez sur **Indicateurs de progression** dans le panneau de gauche.
1. Dans le menu déroulant **Nouvel indicateur de progression**, cliquez sur **Ajouter un projet existant**.

   La zone Ajouter des projets à un objectif s’affiche.
1. (Facultatif) Mettez à jour la **Vue**, le **Filtre** ou le **Regroupement** en cliquant sur les icônes correspondantes dans le coin supérieur droit de la liste pour modifier l’affichage de la liste des projets.
1. (Facultatif) Cliquez sur l’icône **Rechercher** ![Icône Rechercher](assets/search-icon.png) et commencez à saisir le nom d’un projet pour le trouver rapidement dans la liste.
1. Sélectionnez les projets que vous souhaitez ajouter à l’objectif, puis cliquez sur **Ajouter**.

   Les projets sélectionnés sont ajoutés à l’objectif et s’affichent dans la section Indicateurs de progression de la page de l’objectif, sous le regroupement **Projet**.

   Une fois l’objectif activé, sa progression est automatiquement actualisée lors de la mise à jour de la progression d’un projet. Pour plus d’informations sur l’activation d’un objectif, voir [Activer des objectifs dans Objectifs Adobe Workfront](../goal-management/activate-goals.md).

## Localiser les informations de projet sur les objectifs

<p>
Les informations de projet suivantes sont visibles au niveau de l’objectif dans la section Indicateurs de progression de la page d’un objectif :

</p>

<table>
  <tr>
   <td>Nom du projet
   </td>
   <td>Toutes les modifications apportées au nom du projet sont également répercutées dans le projet connecté.
   </td>
  </tr>
  <tr>
   <td>Propriétaire du projet
   </td>
   <td>Toutes les modifications apportées à la personne propriétaire du projet sont également répercutées dans le projet connecté.
   </td>
  </tr>
    <tr>
   <td>Progression en cours
   </td>
   <td> <p>Pourcentage terminé du projet. Vous ne pouvez pas mettre à jour manuellement le pourcentage terminé du projet à partir de l’objectif. Workfront le calcule automatiquement en fonction du pourcentage terminé des tâches. </p>
   </td>
  </tr>
  <tr>
   <td>Progression
   </td>
   <td>Pourcentage terminé du projet représenté par une barre. Toute modification du pourcentage terminé du projet met automatiquement à jour la progression de l’objectif à moins que l’objectif ne soit fermé.
   </td>
  </tr>

</table>

## Localiser les informations d’objectif sur les projets

Les informations d’objectif suivantes sont visibles dans une liste de projets ou un rapport :

| Informations sur l’objectif | Description |
|---|---|
| Objectifs | Liste de tous les objectifs auxquels un projet est associé. |
| Hiérarchie d’objectifs | Hiérarchie à laquelle un objectif appartient. Seuls les parents de l’objectif et l’objectif s’affichent dans ce champ. Les objectifs enfants ne s’affichent pas. |
| Nombre d’objectifs liés | Nombre d’objectifs liés à un projet. |
