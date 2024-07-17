---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Ajouter des projets aux objectifs dans Objectifs Adobe Workfront
description: Vous pouvez lier les projets aux objectifs pour indiquer la progression de l’objectif, en fonction de la progression réelle du projet. Le projet devient un indicateur de progression pour l’objectif.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '939'
ht-degree: 9%

---

# Ajouter des projets aux objectifs dans Objectifs Adobe Workfront

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Vous pouvez lier les projets aux objectifs pour indiquer la progression de l’objectif, en fonction de la progression réelle du projet. Le projet devient un indicateur de progression pour l’objectif.

En reliant les projets aux objectifs, vous pouvez lier la planification stratégique (objectifs) de votre entreprise au travail réel effectué par vos employés et terminer chaque jour (projets).

>[!IMPORTANT]
>
>Les objectifs au niveau du projet créés dans la zone Analyse de cas d’un projet ne sont pas liés aux objectifs stratégiques créés dans les objectifs Workfront. Pour plus d’informations sur les objectifs du projet Business Case, voir [Créer des objectifs de projet Business Case](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> 
   <p>Pour le nouveau plan et la nouvelle structure de licence :
  <ul><li>Un plan ultime </li>
  Ou
  <li>Une licence supplémentaire pour les objectifs Adobe Workfront pour les plans Prime ou Select Adobe Workfront. </li></ul> </p>
<p>Pour le plan actuel et la structure de licence : 
<ul><li> A Pro ou version ultérieure </li>
  <li>Une licence Adobe Workfront Goals en plus d’une licence Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licence Adobe Workfront*</td>
 <td>
 <p>Nouvelle licence : contributeur ou contributrice ou supérieure</p>
 Ou
 <p>Licence actuelle : demande ou supérieure</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produit*</td>
 <td>
 <p> Nouvelle exigence de produit, l’une des options suivantes : </p>
<ul>
<li>Un forfait Select ou Prime Adobe Workfront et une licence Adobe Workfront Goals supplémentaire.</li>
<li>Un plan Workfront Ultimate qui inclut par défaut les objectifs de Workfront. </li></ul>
 <p>Ou</p>
 <p>Exigences actuelles du produit : formule Workfront et licence supplémentaire pour les objectifs Adobe Workfront. </p> <p>Pour plus d’informations, consultez la section <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Exigences pour l’utilisation des Objectifs Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Niveau d’accès</td>
 <td> <p>Modifier l’accès aux objectifs</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <div>
  <p>Afficher ou des autorisations supérieures à l’objectif pour l’afficher</p>
  <p>Gérer les autorisations sur l’objectif pour le modifier</p>
  <p>Pour plus d’informations sur le partage des objectifs, consultez <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partager un objectif dans les Objectifs Workfront</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modèle de disposition</p></td>
   <td> <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
  >Si l’objectif était actif avant que vous n’ayez supprimé le projet et qu’il n’existe aucun autre indicateur de progression sur l’objectif, celui-ci devient inactif.


## Ajout de projets aux objectifs

1. Cliquez sur le **menu principal** ![](assets/main-menu-icon.png) (brouillon pour Shell : ou cliquez sur le **menu principal** ![](assets/three-line-main-menu-icon.png) dans le coin supérieur gauche, s&#39;il est disponible.) , puis sur **Objectifs**.
1. Dans la liste des objectifs, cliquez sur le nom d’un objectif pour ouvrir la page d’objectif.
1. Cliquez sur **Indicateurs de progression** dans le panneau de gauche.
1. Dans le menu déroulant **Nouvel indicateur de progression**, cliquez sur **Ajouter un projet existant**.

   La zone Ajouter des projets à l’objectif s’affiche.
1. (Facultatif) Mettez à jour la **vue**, le **filtre** ou le **regroupement** en cliquant sur les icônes respectives dans le coin supérieur droit de la liste pour modifier la façon dont la liste des projets s’affiche.
1. (Facultatif) Cliquez sur l’icône **Rechercher** ![](assets/search-icon.png) et commencez à saisir le nom d’un projet pour le trouver rapidement dans la liste.
1. Sélectionnez les projets à ajouter à l’objectif, puis cliquez sur **Ajouter**.

   Les projets sélectionnés sont ajoutés à l’objectif et s’affichent dans la section Indicateurs de progression de la page d’objectif, sous le regroupement **Projet** .

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
| Hiérarchie des objectifs | La hiérarchie à laquelle un objectif appartient. Seuls les parents de l’objectif et de l’objectif s’affichent dans ce champ. Les objectifs pour les enfants ne s’affichent pas. |
| Nombre d’objectifs liés | Nombre d’objectifs liés à un projet. |
