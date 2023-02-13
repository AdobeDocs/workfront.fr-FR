---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Partage d’un objectif dans les objectifs Workfront
description: Lorsque vous partagez un objectif, vous accordez des autorisations de gestion à un objectif à une personne qui ne l’a pas créé.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 2%

---

# Partage d’un objectif dans les objectifs Adobe Workfront

Lorsque vous partagez un objectif, vous accordez des autorisations de gestion à un objectif à une personne qui ne l’a pas créé.

## Exigences d’accès

<!--drafted - replace the table below with this one when P&P releases: 

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
   <td> <p>Modifier l’accès aux objectifs ou plus</p> <p><b>NOTE</b><p>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir :</p> 
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
     <p>Pour plus d’informations sur le partage des objectifs, voir <a href="#" class="MCXref xref selected">Partage d’un objectif dans les objectifs Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de commencer, vous devez disposer des éléments suivants :

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.

## Observations relatives au partage des objectifs

* Les utilisateurs peuvent disposer des autorisations suivantes pour atteindre un objectif :

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Autorisations des objectifs</b></p></td> 
      <td>
      <p><b>Description</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Afficher</p></td> 
      <td>
      <p>Les utilisateurs sont autorisés à afficher l’objectif, mais ils ne peuvent pas modifier les informations de l’objectif, ils ne peuvent pas ajouter ni modifier les informations des résultats, ni les activités, mettre à jour l’état ou supprimer l’objectif.</p>      
      <p>Par défaut, tous les utilisateurs ayant accès aux objectifs peuvent afficher tous les objectifs du système. Les utilisateurs peuvent copier l’objectif s’ils disposent d’un accès Modifier aux objectifs à leur niveau d’accès.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Gérer</p></td> 
      <td> <p>Les utilisateurs peuvent modifier toutes les informations de l’objectif, y compris les résultats, ou les activités, y compris les supprimer.</p> 
      <p>Seuls les créateurs d’objectifs ou les utilisateurs auxquels sont spécifiquement attribués les autorisations Gérer pour un objectif peuvent gérer un objectif.</p> 
      Seuls les utilisateurs disposant des autorisations de gestion pour un objectif peuvent partager l’objectif avec d’autres afin de leur donner les autorisations de gestion pour l’objectif. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Vous pouvez partager les types d’objectifs suivants avec d’autres personnes :

   * Un objectif que vous avez créé
   * Objectif créé par une autre personne à laquelle vous avez été autorisé à gérer.

* Si vous disposez des autorisations de Gestion pour un objectif, vous pouvez modifier les autorisations sur l’objectif pour le créateur de l’objectif. Par défaut, ils disposent des autorisations Gérer lorsqu’ils créent l’objectif, mais vous pouvez modifier leurs autorisations en Afficher.

## Partage d’un objectif

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) > **Objectifs** dans le coin supérieur droit.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   La liste des objectifs s’affiche.

1. Cliquez sur le nom d’un objectif dans la liste. La page d’objectif s’ouvre.

1. Cliquez sur le bouton **Icône Plus** en regard du nom de l’objectif, puis cliquez sur **Partager**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   La zone Accès à l’objectif s’affiche.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Utilisez l’une des méthodes suivantes :

   * Sélectionnez la **Gestion à l’échelle du système** pour accorder les autorisations Manage à toutes les personnes du système ayant l’accès Modifier aux objectifs à leur niveau d’accès. Cette option est désélectionnée par défaut pour tous les nouveaux objectifs.
   * Commencez à saisir le nom d’un utilisateur auquel vous souhaitez accorder les autorisations de gestion dans la variable **Donnez à Gérer l’accès à** de la boîte. Sélectionnez le nom qui apparaîtra dans la liste.

      >[!TIP]
      >
      >Vous ne pouvez partager un objectif qu’avec d’autres utilisateurs. Vous ne pouvez pas partager des objectifs avec des groupes, des équipes ou votre entreprise.

1. Cliquez sur **Partager**.

   L’objectif est partagé avec les utilisateurs que vous avez spécifiés. Une étiquette &quot;à l’échelle du système&quot; ou le nom des utilisateurs qui disposent des autorisations de gestion pour l’objectif s’affiche dans le champ Accès à la gestion du panneau Détails de l’objectif .

## Options d’autorisation des objectifs

Le tableau suivant répertorie les autorisations que vous pouvez accorder lors du partage d’un objectif. Pour plus d’informations sur l’accès des utilisateurs en fonction de leur licence, voir [Accorder l’accès aux objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

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
   <td> <p>Affichage des résultats ou des activités</p> </td> 
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
   <td>Affichage des projets ajoutés en tant qu’activités** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Modifier l’objectif</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Modification de résultats ou d’activités</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ajouter des résultats ou des activités pour l’objectif</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Associer un projet en tant qu’activité à l’objectif**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Supprimer l’objectif</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Suppression de résultats ou d’activités</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Déconnexion des projets de l’objectif</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Vous devez disposer de l’accès Modifier aux objectifs dans votre niveau d’accès pour pouvoir convertir les résultats et les activités en objectifs.

**Vous devez avoir accès aux autorisations Afficher les projets et Afficher les projets ajoutés ou que vous souhaitez ajouter à l’objectif pour les afficher.

Pour plus d’informations sur le niveau d’accès au projet, voir [Accorder l’accès aux projets](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Pour plus d’informations sur les autorisations de projet, voir [Partage d’un projet dans Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
