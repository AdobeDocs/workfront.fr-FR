---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Partager un objectif dans Objectifs Workfront
description: Lorsque vous partagez un objectif, vous accordez des autorisations de gestion d’un objectif à une personne qui ne l’a pas créé.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 91%

---

# Partager un objectif dans les Objectifs Adobe Workfront

Lorsque vous partagez un objectif, vous accordez des autorisations de gestion d’un objectif à une personne qui ne l’a pas créé.

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
  <td> <p>Package Adobe Workfront</p> </td> 
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
 <p>Current license: Request or higher</p> </td>
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

## Observations sur le partage des objectifs

* Les utilisateurs et les utilisatrices peuvent disposer des autorisations suivantes pour accéder à un objectif :

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Autorisations sur les objectifs</b></p></td> 
      <td>
      <p><b>Description</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Afficher</p></td> 
      <td>
      <p>Les utilisateurs et les utilisatrices ont le droit d’afficher l’objectif, mais n’ont pas l’autorisation de modifier ses informations, ni d’ajouter ou de modifier des informations sur ses résultats ou ses activités, ni mettre à jour son statut, ni le supprimer.</p>      
      <p>Par défaut, l’ensemble des utilisateurs et des utilisatrices ayant accès aux objectifs peut afficher tous les objectifs du système. Les utilisateurs et les utilisatrices peuvent copier l’objectif si l’autorisation de modifier les objectifs leur a été accordée.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Gérer</p></td> 
      <td> <p>Les utilisateurs et les utilisatrices peuvent modifier l’ensemble des informations concernant l’objectif, que ce soit les résultats ou les activités, et même les supprimer.</p> 
      <p>Seulement les personnes qui ont créé un objectif ou les utilisateurs et utilisatrices qui ont reçu des autorisations spécifiques de gestion peuvent gérer un objectif.</p> 
      Seulement les utilisateurs et les utilisatrices disposant d’autorisations de gestion pour un objectif peuvent partager l’objectif avec d’autres personnes afin de leur donner des autorisations de gestion pour l’objectif. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Vous pouvez partager les types d’objectifs suivants avec d’autres personnes :

   * Un objectif que vous avez créé.
   * Un objectif créé par quelqu’un d’autre et que vous avez le droit de gérer.

* Si vous avez l’autorisation de gérer un objectif, vous pouvez modifier les autorisations accordées à la personne qui l’a créé. Par défaut, cette personne a des droits de gestion lorsqu’elle crée l’objectif, mais vous pouvez la faire passer à des droits d’affichage.

## Partager un objectif

{{step1-to-goals}}

La liste des objectifs s’affiche.

1. Cliquez sur le nom d’un objectif dans la liste. La page de l’objectif s’ouvre.

1. Cliquez sur l’icône **Plus** à côté du nom de l’objectif, puis cliquez sur **Partager**.

   ![Menu Plus](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   La case Accès à l’objectif s’affiche.

   ![Accès aux objectifs](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Utilisez l’une des méthodes suivantes :

   * Sélectionnez le paramètre **Gérer à l’échelle du système** pour donner des autorisations de gestion à toutes les personnes du système qui disposent d’un accès Modifier aux objectifs par le biais de leur niveau d’accès. Cette option est désélectionnée par défaut pour tous les nouveaux objectifs.
   * Commencez à saisir le nom d’une personne à qui vous voulez donner les autorisations Gérer dans la zone **Autoriser l’accès en gestion à**. Sélectionnez le nom qui apparaîtra dans la liste.

     >[!TIP]
     >
     >Vous ne pouvez partager un objectif qu’avec d’autres personnes. Vous ne pouvez pas partager des objectifs avec des groupes, des équipes ou des entreprises.

1. Cliquez sur **Partager**.

   L’objectif est partagé avec les personnes que vous avez spécifiées. Un libellé « À l’échelle du système » ou les noms des personnes qui ont des autorisations de gestion pour l’objectif s’affichent dans le champ Accès à la gestion dans le panneau Détails de l’objectif.

## Options d’autorisation des objectifs

Le tableau suivant répertorie les autorisations que vous pouvez accorder lors du partage d’un objectif. Pour plus d’informations sur l’accès des personnes en fonction de leur licence, voir [Accorder l’accès aux Objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>Actions</strong> </p> </th> 
   <th> <p><strong>Gérer</strong> </p> </th> 
   <th> <p><strong>Afficher</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Afficher l’objectif</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Afficher des résultats ou des activités</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Copier l’objectif* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Convertir des résultats ou des activités en d’autres objectifs*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Afficher des projets ajoutés en tant qu’activités** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Modifier l’objectif</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modifier des résultats ou des activités</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ajouter des résultats ou des activités pour l’objectif</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Associer un projet en tant qu’activité à l’objectif**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Supprimer l’objectif</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Supprimer des résultats ou des activités</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Déconnecter les projets de l’objectif</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

* Vous devez disposer d’un accès Modifier aux objectifs dans votre niveau d’accès pour pouvoir convertir les résultats et les activités en objectifs.

** Vous devez avoir accès aux autorisations Afficher les projets et Afficher les autorisations sur les projets ajoutés ou que vous souhaitez ajouter à l’objectif pour les afficher.

Pour plus d’informations sur le niveau d’accès au projet, voir [Accorder l’accès aux projets](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Pour plus d’informations sur les autorisations de projet, voir [Partager un projet dans Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).


