---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Ajout de projets aux objectifs dans les objectifs Adobe Workfront
description: Vous pouvez lier les projets aux objectifs pour indiquer la progression de l’objectif, en fonction de la progression réelle du projet. Le projet devient un indicateur de progression pour l’objectif.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# Ajout de projets aux objectifs dans les objectifs Adobe Workfront

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Vous pouvez lier les projets aux objectifs pour indiquer la progression de l’objectif, en fonction de la progression réelle du projet. Le projet devient un indicateur de progression pour l’objectif.

En reliant les projets aux objectifs, vous pouvez lier la planification stratégique (objectifs) de votre entreprise au travail réel effectué par vos employés et terminer chaque jour (projets).

>[!IMPORTANT]
>
>Les objectifs au niveau du projet créés dans la zone Analyse de cas d’un projet ne sont pas liés aux objectifs stratégiques créés dans les objectifs Workfront. Pour plus d’informations sur les objectifs du projet Business Case, voir [Créer des objectifs de Business Case](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Exigences d’accès

<!--drafted for P&P release: replace the table below with this: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>

-->
Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td> <p>Pour accéder aux fonctionnalités décrites dans cet article, vous devez acheter une licence supplémentaire pour les objectifs d’Adobe Workfront. </p> <p>Pour plus d’informations, voir <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Conditions requises pour utiliser les objectifs Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux objectifs</p> <p><b>NOTE</b>

<p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir :</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Accorder l’accès aux objectifs Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> 
    <div> 
     <p>Gérer les autorisations pour l’objectif</p> 
     <p>Pour plus d’informations sur le partage des objectifs, voir <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partage d’un objectif dans les objectifs Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

Pour plus d’informations sur l’accès aux objectifs de Workfront, voir [Conditions requises pour utiliser les objectifs Workfront](../goal-management/access-needed-for-wf-goals.md).

## Observations relatives à la connexion des projets aux objectifs

* Vous pouvez ajouter à un objectif un projet qui répond aux critères suivants :

   * Vous devez disposer au moins des autorisations nécessaires pour l’afficher.

      >[!NOTE]
      >
      >Si vous perdez les autorisations d’affichage du projet une fois que vous avez joint le projet à l’objectif, vous pouvez toujours afficher les informations du projet sur l’objectif, mais vous ne pouvez plus accéder au projet.

   * Le projet ne doit pas avoir le statut de Mort.

* Vous pouvez associer plusieurs projets à un objectif.
* Vous pouvez associer le même projet à plusieurs objectifs.
* Vous ne pouvez pas mettre à jour manuellement la progression d’un projet à partir de l’objectif auquel il est rattaché. Au lieu de cela, Workfront calcule le pourcentage d’achèvement du projet et Workfront Goals calcule la progression de l’objectif en utilisant ce pourcentage d’achèvement. Cela met à jour l’objectif en temps réel après la mise à jour du pourcentage du projet.
* La durée du projet peut se trouver en dehors de la période d’un objectif. Si un projet dure plus longtemps que la date limite de l’objectif, vous pouvez toujours fermer votre objectif et le considérer comme terminé, mais le pourcentage d’achèvement de l’objectif ne sera pas de 100 %. Le pourcentage d’achèvement du projet n’est plus mis à jour par rapport à l’objectif.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Lorsque vous supprimez un projet associé à un objectif, celui-ci est également supprimé de l’objectif.

   >[!CAUTION]
   >
   >Si l’objectif était principal avant que vous n’ayez supprimé le projet et qu’il n’existe aucun autre indicateur de progression sur l’objectif, celui-ci devient inactif.


## Ajout de projets aux objectifs

1. Cliquez sur le bouton **Menu Principal** ![](assets/main-menu-icon.png) (Version préliminaire pour Shell : ou cliquez sur le bouton **Menu Principal** ![](assets/three-line-main-menu-icon.png) dans le coin supérieur gauche, s’il est disponible.) , puis **Objectifs**.
1. Dans la liste des objectifs, cliquez sur le nom d’un objectif pour ouvrir la page d’objectif.
1. Cliquez sur **Indicateurs de progression** dans le panneau de gauche.
1. Dans la **Nouvel indicateur de progression** menu déroulant, cliquez sur **Ajouter un projet existant**.

   La zone Ajouter des projets à l’objectif s’affiche.
1. (Facultatif) Mettez à jour la variable **Affichage**, **Filtrer** ou **Regroupement** en cliquant sur les icônes correspondantes dans le coin supérieur droit de la liste pour modifier l’affichage de la liste des projets.
1. (Facultatif) Cliquez sur le **Rechercher** icon ![](assets/search-icon.png) et commencez à saisir le nom d’un projet pour le trouver rapidement dans la liste.
1. Sélectionnez les projets à ajouter à l’objectif, puis cliquez sur **Ajouter**.

   Les projets sélectionnés sont ajoutés à l’objectif et s’affichent dans la section Indicateurs de progression de la page d’objectif, sous la balise **Projet** regroupement.

   Une fois l’objectif activé, la progression de l’objectif est automatiquement mise à jour lorsque la progression d’un projet est mise à jour. Pour plus d’informations sur l’activation d’un objectif, voir [Activation des objectifs dans les objectifs Adobe Workfront](../goal-management/activate-goals.md).

## Recherche des informations du projet sur les objectifs

<p>
Les informations de projet suivantes sont visibles au niveau de l’objectif dans la section Indicateurs de progression de la page d’un objectif :

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
   <td>Toutes les modifications apportées au propriétaire du projet sont également répercutées dans le projet connecté.
   </td>
  </tr>
    <tr>
   <td>Progression en cours
   </td>
   <td> <p>Le pourcentage de réalisation du projet. Vous ne pouvez pas mettre à jour manuellement le pourcentage de projet terminé à partir de l’objectif. Workfront le calcule automatiquement en fonction du pourcentage d’achèvement des tâches. </p>
   </td>
  </tr>
  <tr>
   <td>Progression
   </td>
   <td>Pourcentage de réalisation du projet représenté par une barre. Toute modification du pourcentage de réalisation du projet met automatiquement à jour la progression de l’objectif à moins que l’objectif ne soit fermé.
   </td>
  </tr>

</table>

## Recherche des informations d’objectif sur les projets

Les informations d’objectif suivantes sont visibles dans une liste de projets ou un rapport :

| Informations sur les objectifs | Description |
|---|---|
| Objectifs | Liste de tous les objectifs auxquels un projet est associé. |
| Hiérarchie des objectifs | La hiérarchie à laquelle un objectif appartient. Seuls les parents de l’objectif et de l’objectif s’affichent dans ce champ. Les objectifs enfants ne s’affichent pas. |
| Nombre d’objectifs liés | Nombre d’objectifs liés à un projet. |
