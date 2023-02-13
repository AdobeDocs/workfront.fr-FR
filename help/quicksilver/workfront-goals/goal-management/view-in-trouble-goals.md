---
product-previous: workfront-goals
navigation-topic: goal-management
title: Révision des objectifs en difficulté dans les objectifs Adobe Workfront
description: Les objectifs présentant un état d’avancement des problèmes risquent de ne pas être atteints et sont représentés par une barre rouge de progression dans les objectifs d’Adobe Workfront. Vous devez souvent revoir vos objectifs et comprendre pourquoi les progrès sont à la traîne.
author: Alina
feature: Workfront Goals
exl-id: df2cdc12-9102-4759-9daa-1f8ae68f110b
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---

# Révision des objectifs en difficulté dans les objectifs Adobe Workfront

<!--
<p>(NOTE: the status of goals in "red" used to be called At Risk. Now, it is "in trouble") </p>
-->

Les objectifs présentant un progrès par rapport aux objectifs en difficulté risquent de ne pas être atteints et sont représentés par une barre de progression rouge dans les objectifs Adobe Workfront. Vous devez souvent revoir vos objectifs et comprendre pourquoi les progrès sont à la traîne. Pour plus d’informations sur la progression de l’objectif, voir [Présentation de la progression et de la condition des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/calculate-goal-progress.md).

## Exigences d’accès

<!--drafted for P&P release: replace the existing requirements with this:

You must have the following: 

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
     <p>Pour plus d’informations sur le partage des objectifs, voir <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partage d’un objectif dans les objectifs Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de pouvoir commencer, vous devez disposer des éléments suivants :

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.

## Recommendations pour empêcher les objectifs d’atteindre l’état En difficulté

Avant que les objectifs n’atteignent une progression de En danger, vous pouvez souvent les surveiller et ajuster leur progression lorsqu’ils atteignent une progression de En danger. Les objectifs qui sont menacés risquent de devenir en difficulté. Pour plus d’informations sur la progression de l’objectif, voir [Présentation de la progression et de la condition des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/calculate-goal-progress.md)

Avant que vos objectifs n’atteignent une progression de En problème, nous vous recommandons ce qui suit :

* Révisez les objectifs dont la condition est En danger et qui vous sont souvent assignés, ainsi que les objectifs organisationnels qui sont attribués à vos équipes, groupes ou organisation et qui peuvent être affectés par la progression de vos objectifs. Les objectifs à risque risquent de devenir des objectifs en difficulté. Les objectifs à risque sont marqués par une barre de progression jaune. Utilisez la liste des objectifs pour afficher les objectifs qui vous appartiennent, à vos équipes, à vos groupes ou à votre organisation.


## Révision des objectifs en difficulté dans la liste des objectifs

Vous pouvez consulter les objectifs dans n’importe quelle section des objectifs de Workfront. Pour plus d’informations sur les sections Objectifs de Workfront , voir [Présentation des sections Objectifs d’Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

Cet article décrit comment passer en revue les objectifs dans la liste des objectifs.

1. Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) > **Objectifs** dans le coin supérieur droit.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-management/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   La zone Objectifs de Workfront s’affiche alors et la section Liste des objectifs s’affiche par défaut.

1. (Recommandé) Ajustez les filtres suivants pour la zone Liste des objectifs afin de passer en revue les objectifs à risque :

   * Cliquez sur **Société**, puis **Mes équipes**, puis **Mes groupes**, puis **Personal** objectifs dans ce but afin d’afficher les objectifs qui appartiennent à votre organisation, vos équipes, vos groupes, puis vos propres objectifs.

      >[!TIP]
      >
      >Dans les objectifs Adobe Workfront, le filtre Société affiche les objectifs pour lesquels votre entreprise est sélectionnée en tant que propriétaire.
      >
      >
      >Vous ne pouvez pas rechercher des sociétés utilisant ce champ. Seule votre organisation propriétaire de votre instance Workfront est sélectionnée par défaut.

   * Pour chacune des entités organisationnelles que vous sélectionnez ci-dessus, cliquez sur **Nouveau filtre** > **Progression** > **En difficulté** >**Appliquez.**
   * (Facultatif) Sélectionnez la période pour laquelle vous souhaitez afficher les objectifs.

      L’indicateur de la barre de progression s’affiche en rouge pour chaque objectif de la liste d’objectifs.

      Pour plus d’informations sur le filtrage des objectifs à l’aide de tous les autres critères dans le panneau de droite, voir [Filtrage des informations dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

1. Passez la souris sur l’indicateur de la barre de progression pour voir quel est le pourcentage réel de progression et quelle est la valeur attendue pour le jour en cours.

   ![](assets/goal-progress-hover-over-detail-unshimmed.png)

1. (Facultatif) Utilisez les filtres pour rechercher les objectifs appartenant à un propriétaire spécifique.

   Les objectifs en difficulté pour les utilisateurs sélectionnés s’affichent dans la liste d’objectifs.

1. Cliquez sur un nom d’objectif pour ouvrir la page d’objectif, puis cliquez sur **Indicateurs de progression** dans le panneau de gauche. Identifier l’indicateur de progression qui provoque le retard de l’objectif et mettre à jour la progression de l’indicateur en ligne, dans la variable **Progression réelle** de la liste Indicateurs de progression.

   Pour plus d’informations sur la mise à jour des résultats et des activités, voir [Mise à jour de la progression de l’objectif dans les objectifs Adobe Workfront](../goal-review-and-workfront-goals-sections/check-in-goals.md)

   ![](assets/actual-progress-editable-column-in-indicator-list-unshimmed.png)

   >[!NOTE]
   >
   >Vous ne pouvez mettre à jour que les résultats et les activités dans la liste Indicateurs de progression . Vous devez mettre à jour les indicateurs de progression des objectifs pour les enfants en accédant aux objectifs et vous devez mettre à jour les tâches sur les projets connectés pour mettre à jour la progression des projets.


