---
product-previous: workfront-goals
navigation-topic: goal-management
title: Copie d’objectifs dans les objectifs Adobe Workfront
description: Vous pouvez copier des objectifs dans les objectifs Adobe Workfront pour créer un objectif. Certaines des informations d’objectif d’origine sont transférées vers le nouvel objectif.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Copie d’objectifs dans les objectifs Adobe Workfront

Vous pouvez copier des objectifs dans les objectifs Adobe Workfront pour créer un objectif. Certaines des informations d’objectif d’origine sont transférées vers le nouvel objectif.

## Exigences d’accès

<!--drafted for P&P release: 

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
   <td> <p>Modifier l’accès aux objectifs ou plus</p> <p><b>NOTE</b>

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

## Observations relatives à la copie des objectifs

Vous devez avoir accès à Modifier les objectifs dans votre niveau d’accès avant de pouvoir copier les objectifs. Pour plus d’informations sur l’octroi de l’accès aux Objectifs, voir [Accorder l’accès aux objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Voici quelques-unes des raisons pour lesquelles vous souhaitez copier un objectif existant :

* À la fin d’une période (trimestre ou année), lorsque vous souhaitez recréer le même objectif pour la période suivante.
* À la fin d’une période, lorsque l’objectif ne peut pas être atteint et que vous souhaitez y travailler pendant une autre période.
* Lorsque plusieurs membres de l’équipe ont des objectifs similaires et que vous devrez peut-être en créer un pour chacun d’eux.

>[!TIP]
>
>Vous pouvez copier un objectif dans n’importe quel état. Pour plus d’informations sur les états d’objectif, voir [Présentation de l’état des objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

Tenez compte des points suivants lors de la copie des objectifs :

* Toutes les informations sur l’objectif sont également copiées vers le nouvel objectif.
* Vous pouvez choisir de copier les résultats d’un objectif existant. Le nom des résultats est transféré vers le nouvel objectif, mais la progression actuelle des résultats sur l’objectif existant ne copie pas vers le nouvel objectif. Par défaut, les résultats copiés sont attribués au même propriétaire.

   >[!NOTE]
   >
   >Si le propriétaire d’origine a été supprimé ou désactivé de Workfront, le nouveau résultat est attribué à l’utilisateur connecté.

* Vous ne pouvez pas copier les activités d’un objectif lorsque vous copiez ce dernier.

## Copie d’objectifs

<!--
Copying goals differs depending on what environment you use. 

To copy goals in the Production environment:

1. Go to a goal and click it to open the Goal Details panel.

   For information about accessing an individual goal, see the "Access individual goals" section in [Access and open goals in Adobe Workfront Goals](../../workfront-goals/goal-management/access-goals-in-wf-goals.md).

   This opens the Goal Details panel.

1. Click the **More icon** ![](assets/more-icon.png), then click **Copy**. 

1. Update any of the following information for the copied goal:

   | Field |Description  |
   |---|---|
   | New Goal |The name of the new goal. The default is the name of the original goal.  |
   | Period |The time period during which you want to achieve the goal. Select a time period from the drop-down menu or click **Define custom dates** to indicate a custom time period. By default, the Period is always the current quarter. |
   | Owner |The owner of the goal. It can be a user, team, group, or a company. The default is the owner of the original goal.  |
   | Description |Additional information about the goal.  |

1. (Conditional) Select **Copy results** if the original goal had results added to it and you want to copy them to the new goal. This duplicates the original results to the new goal. The results of the copied goal have the same owner, names and measured values as the results of the original goal.

   >[!TIP]
   >
   >* The progress of the original result does not transfer to the copied goal. 
   >* If the original owner was deleted or deactivated from Workfront, the new result is assigned to the logged in user.

1. Click **Save**.

   The copied goal is saved with a status of Draft and displays in the Goal Details panel.

   >[!IMPORTANT]
   >
   >If you have not copied the results from the original goal, you must first associate the new goal with a progress indicator before you can activate it and start working towards achieving it. 
   >
   >Do at least one of the following to be able to activate a goal: 
   >   
   >* Add a Result
   >   
   >  For information about adding results, see [Add results to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-results-to-goals.md).
   >   
   >* Add an Activity
   >   
   >  For information about adding activities, see [Add activities to goals in Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md). 
   >   
   >* Align another goal to it
   >   
   >  For information about aligning goals, see [Align goals by connecting them in Adobe Workfront Goals](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).
   >
   > For information about activating a goal, see [Activate goals in Adobe Workfront Goals](../goal-management/activate-goals.md). 

1. Click the **X** icon in the upper-right of the Goal Details panel to close it.

   The copied goal displays in the following sections:

   * Goal List 
   * Check-in (after it is activated)
   * Goal Alignment section (after it is activated) 
   * Pulse
(!--drafted - this was important when we could not update the goal timeframe in the past but we can do that now - not needed
1. (Optional and conditional) If you have copied a goal that was not achieved in a previous time period to continue working on it in the following time period, do the following:

   1. Go to the original goal in the Goal List, Check-in page, or Pulse section and comment on the goal, to indicate that this goal was copied to another, more current goal. For information about commenting on a goal, see [Manage goal comments in Adobe Workfront Goals](../../workfront-goals/goal-management/manage-goal-comments.md).
   1. Close the original goal, to preserve the progress in its original time period. For information about closing goals, see [Close and reopen goals in Adobe Workfront Goals](../../workfront-goals/goal-management/close-and-reopen-goals.md). 
   1. Update the the **Initial** value of the new Result to match the **End At** value of the previous result, so that your new goal progress will start calculating from the point you achieved in the previous period.
   
-->


1. Accédez à un objectif et cliquez sur le bouton **Plus** menu ![](assets/more-icon.png), puis cliquez sur **Copier l’objectif**.

   ![](assets/copy-goal-box-unshimmed.png)

1. Mettez à jour les informations suivantes pour l’objectif copié :
   * **Nom de l’objectif**: Nom du nouvel objectif. Le nom par défaut de l’objectif copié est &quot;Copie de &lt;original goal=&quot;&quot;>&quot;.
   * **Période**: La période pendant laquelle vous souhaitez atteindre l’objectif. Sélectionnez une période dans le menu déroulant.

      Ou

      Sélectionner **Activation des dates personnalisées** pour spécifier des dates personnalisées pour le **Début** et **Dates de fin**. Le paramètre Activer les dates personnalisées est désactivé par défaut.

      >[!TIP]
      >
      >   La désélection de l’option Activer les dates personnalisées rétablit la période de l’objectif d’origine.

      * **Propriétaire de l’objectif**: Propriétaire de l’objectif. Il peut s’agir d’un utilisateur, d’une équipe, d’un groupe ou d’une société. La valeur par défaut est le propriétaire de l’objectif d’origine.
      * **Description**: Informations supplémentaires sur l’objectif.
      * **Copie de résultats**: Sélectionnez cette option si vous souhaitez transférer les résultats de l’objectif actuel vers l’objectif copié. Cela duplique les résultats d’origine et les joint à l’objectif copié. Les résultats de l’objectif copié ont les mêmes propriétaire, noms et valeurs mesurées que les résultats de l’objectif d’origine.

         >[!NOTE]
         >
         >* La progression du résultat d’origine ne passe pas à l’objectif copié.
         >* Si le propriétaire d’origine a été supprimé ou désactivé de Workfront, le nouveau résultat est attribué à l’utilisateur connecté.


1. Cliquez sur **Copier l’objectif**.

   Un objectif similaire à l’objectif d’origine est créé et il est dans l’état Brouillon.

   >[!NOTE]
   >
   >Si vous n’avez pas copié les résultats de l’objectif d’origine, vous devez d’abord associer le nouvel objectif à un indicateur de progression avant de pouvoir l’activer et commencer à travailler à son accomplissement.
   >Pour plus d’informations sur l’association des objectifs aux indicateurs de progression, voir les articles suivants :
   >* [Ajout de résultats aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/add-results-to-goals.md)
   >* [Ajout d’activités aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   >* [Alignement des objectifs en les connectant aux objectifs Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md)

   >
   >Pour plus d’informations sur l’activation des objectifs, voir [Activation des objectifs](../goal-management/activate-goals.md).

