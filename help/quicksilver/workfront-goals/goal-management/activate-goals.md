---
product-previous: workfront-goals
navigation-topic: goal-management
title: Activer des objectifs dans les objectifs Adobe Workfront
description: Lorsque vous créez un objectif, Objectifs Adobe Workfront l’enregistre avec le statut Brouillon. Les brouillons d’objectifs ne font pas partie de la gestion des objectifs.
author: Alina
feature: Workfront Goals
exl-id: fc556073-fe63-4f13-a313-505ca0ef1f9b
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 79%

---

# Activer les objectifs dans Objectifs Adobe Workfront

<!--Audited for P&P only: 4/2025-->

Lorsque vous créez un objectif, Objectifs Adobe Workfront l’enregistre avec le statut Brouillon. Les brouillons d’objectifs ne font pas partie de la gestion des objectifs.

Pour savoir si vous êtes sur le point d’atteindre un objectif lorsque vous mettez à jour sa progression, vous devez l’activer. Son statut devient alors Actif.

Pour plus d’informations sur la création d’un objectif, voir la section [Créer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Vous devez activer un objectif avant de pouvoir mettre à jour l’avancement de ses résultats et activités.


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
 <td role="rowheader">Configurations des niveaux d’accès</td>
 <td> <p>Modifier l’accès aux Objectifs</p> </td>
 </tr>
 <tr>
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

Pour plus d’informations, consultez la section [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
  <p> New product requirement: Workfront</p>
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
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

## Conditions préalables

Pour activer un objectif, celui-ci doit être associé à un indicateur de progression, tel qu’une activité, un résultat ou un projet, ou être aligné sur un autre objectif actif.

Pour pouvoir activer un objectif, procédez à au moins l’une des actions suivantes :

* Ajoutez un résultat à l’objectif.

  Pour plus d’informations, voir la section [Ajouter des résultats aux objectifs dans Objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Ajoutez une activité à l’objectif.

  Pour plus d’informations, voir la section [Ajouter des activités aux objectifs dans Objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Connectez un projet à l’objectif.

  Pour plus d’informations, voir la section [Ajouter des projets aux objectifs dans Objectifs Adobe Workfront](../results-and-activities/connect-projects-to-goals-overview.md).

* Alignez un autre objectif sur l’objectif que vous souhaitez activer.

  Pour plus d’informations, voir la section [Aligner des objectifs en les connectant dans Objectifs Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Activer des objectifs

Vous pouvez activer des objectifs que vous avez créés ou un objectif pour lequel vous avez des autorisations de gestion.

1. Accédez à un objectif que vous souhaitez activer. La page de l’objectif s’ouvre.

1. Cliquez sur le menu **Plus** ![icône Plus](../goal-management/assets/more-icon.png) à droite du nom de l’objectif, puis cliquez sur **Activer**.

   ![Menu Plus développé](assets/more-menu-on-goal-expanded-with-activate-unshimmed.png)

   Le statut de l’objectif devient Actif. Vous pouvez désormais suivre la progression de l’objectif. Celui-ci s’affiche dans la section Enregistrer et est pris en compte dans les sections Graphiques d’Objectifs Workfront.
