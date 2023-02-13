---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Alignement des objectifs en les connectant aux objectifs Adobe Workfront
description: Si vous contributeur individuel avez un objectif personnel, vous pouvez l’aligner sur les objectifs de votre équipe afin d’afficher efficacement la progression de votre propre objectif dans le contexte plus large de la stratégie de votre organisation.
author: Alina
feature: Workfront Goals
exl-id: 4276f1c9-2ee9-4f74-b011-ae1e19fefe35
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Alignement des objectifs en les connectant aux objectifs Adobe Workfront


Si vous contributeur individuel avez un objectif personnel, vous pouvez l’aligner sur les objectifs de votre équipe afin d’afficher efficacement la progression de votre propre objectif dans le contexte plus large de la stratégie de votre organisation.

Lorsque tous les membres de votre organisation ont leurs objectifs alignés sur les objectifs de votre organisation, ils peuvent clairement voir comment leurs contributions individuelles et les efforts de leur équipe aident à avancer vers des priorités plus importantes au niveau de l’entreprise. Pour plus d’informations sur les bonnes pratiques d’alignement des objectifs, voir [Alignement des objectifs - Aperçu dans les objectifs Adobe Workfront](../../workfront-goals/goal-alignment/goal-alignment-overview.md).

Il existe deux approches pour connecter les objectifs dans les objectifs Adobe Workfront :

* Vous pouvez créer un alignement entre les objectifs en liant les objectifs les uns aux autres.

* Vous pouvez aligner manuellement deux objectifs ou convertir les résultats et les activités d’un objectif existant en un autre. Le résultat ou l’activité converti devient l’objectif enfant de l’objectif d’origine.

>[!IMPORTANT]
>
>Un objectif peut avoir un total de 1000 indicateurs de progrès.

Cet article décrit comment aligner des objectifs en les connectant les uns aux autres. Pour plus d’informations sur l’alignement des objectifs en convertissant les résultats et les activités en objectifs, voir [Alignement des objectifs en convertissant les résultats et les activités en objectifs](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

## Exigences d’accès

<!--drfated for the P&P release: 

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

## Conditions préalables

Avant de pouvoir commencer, vous devez disposer des éléments suivants :

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.

## Alignement des objectifs en les connectant les uns aux autres

<!--
Aligning goals by connecting them differs depending on what environment you use. 

### Align goals by connecting them in the Production environment

1. Create two goals that you want to align. For information about creating goals, see [Create goals in Adobe Workfront Goals](../../workfront-goals/goal-management/create-goals.md).
1. (Optional) Activate the goals that you want to align. You can align goals that have a Draft, Active, or Inactive status. For information about activating goals, see [Activate goals in Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).
1. Go to the goal that you want to align (child goal) to another goal (parent goal) and click its name to open the **Goal Details** panel.

   For example, if you want Goal 2 to influence the progress of Goal 1, you must go to Goal 2. 

1. Click **Align to another goal** in the upper-right corner of the right panel.

   ![](assets/align-to-another-goal-link-highlighted-350x128.png)

1. Start typing the name of an existing goal or the name of an owner in the **Align to another goal** field, then select it when it appears in the list. Only goals that are from the same or future periods display in the list. 
1. Click **Save**.

   The goal you started with (Goal 2) is now the child goal of the goal you aligned it with (Goal 1).   
   The aligned goals display connected in the Goal Alignment section with Goal 2 as secondary to Goal 1.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Optional) To view the goals in the Goal Alignment section, do one of the following:

   * Click the Goal Alignment section in the left panel and find the goals by applying the correct filter. For information about filtering information in Workfront Goals, see [Filter information in Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).
   * Click the Goal List, Check-in, or Pulse sections in the left panel and find one of the goals, then click the **Alignment icon** ![](assets/align-icon.png) next to the goal name to go directly to the goal in the Goal Alignment section.

   For information about the Goal Alignment section, see [Navigate the Goal Alignment section in Adobe Workfront Goals](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md). 

1. (Optional) Add activities and results to either goal to indicate their progress. For information about adding activities and results, see the following articles:

   * [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md) 
   * [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Optional) Remove the alignment between two goals, when you consider that no longer is relevant to your organization's overall strategy For information about removing alignment between goals, see [Remove goal alignment in Adobe Workfront Goals](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

-->
1. Créez deux objectifs que vous souhaitez aligner. Pour plus d’informations sur la création d’objectifs, voir [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).
1. (Facultatif) Activez les objectifs que vous souhaitez aligner. Vous pouvez aligner les objectifs dont l’état est En création, Principal ou Inactif. Pour plus d’informations sur l’activation des objectifs, voir [Activation des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/activate-goals.md).
1. Accédez à l’objectif que vous souhaitez aligner (objectif enfant) sur un autre objectif (objectif parent) et cliquez sur son nom pour ouvrir la page d’objectif.

   >[!INFO]
   >
   >Par exemple, si vous souhaitez que l’objectif 2 influence la progression de l’objectif 1, vous devez accéder à l’objectif 2.

1. Cliquez sur **Détails de l’objectif** dans le panneau de gauche.

1. Dans le **Informations sur l’objectif parent** zone, cliquez sur **Ajouter** dans le **Objectif parent** champ s’il n’y a pas d’objectif parent,

   Ou

   Cliquez sur le nom de l’objectif parent pour en choisir un autre.

1. Commencez à saisir le nom d’un objectif existant dans la variable **Objectif parent** puis sélectionnez-la lorsqu’elle apparaît dans la liste. Seuls les objectifs issus de périodes identiques ou futures s’affichent dans la liste.

1. Cliquez sur **Enregistrer les modifications**.

   L’objectif avec lequel vous avez commencé (objectif 2) est désormais l’objectif enfant de l’objectif parent avec lequel vous l’avez aligné (objectif 1).\
   Les objectifs alignés s’affichent en deuxième position dans la section Alignement de l’objectif 2 par rapport à l’objectif 1.
L’objectif enfant s’affiche dans la section Indicateurs de progression de l’objectif parent lorsque sa progression met à jour la progression de l’objectif parent.

   ![](assets/goal-1-and-2-aligned-cards-350x427.png)

1. (Facultatif) Pour afficher les objectifs dans la section Alignement des objectifs , accédez à la zone Objectifs de Workfront, puis cliquez sur le bouton **Alignement des objectifs** dans le panneau de gauche. Pour plus d’informations sur la section Alignement de l’objectif, voir [Accédez à la section Alignement des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-alignment/navigate-goal-alignment-chart.md).

1. (Facultatif) Ajoutez des activités et des résultats à l’un ou l’autre des objectifs pour indiquer leur progression. Pour plus d’informations sur l’ajout d’activités et de résultats, consultez les articles suivants :

   * [Ajout d’activités aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md)
   * [Ajout de résultats aux objectifs dans les objectifs Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)

1. (Facultatif) Supprimez l’alignement entre deux objectifs lorsque vous considérez que n’est plus pertinent pour la stratégie globale de votre entreprise. Pour plus d’informations sur la suppression de l’alignement entre les objectifs, voir [Suppression de l’alignement d’objectif dans les objectifs Adobe Workfront](../../workfront-goals/goal-alignment/remove-goal-alignment.md).

