---
product-previous: workfront-goals
navigation-topic: goal-management
title: Copier des objectifs dans Objectifs Adobe Workfront
description: Vous pouvez copier des objectifs dans les objectifs Adobe Workfront pour créer un objectif. Certaines des informations d’objectif d’origine sont transférées vers le nouvel objectif.
author: Alina
feature: Workfront Goals
exl-id: 690a6030-ee29-4e50-869f-cd014050b364
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 13%

---

# Copier des objectifs dans Objectifs Adobe Workfront

Vous pouvez copier des objectifs dans les objectifs Adobe Workfront pour créer un objectif. Certaines des informations d’objectif d’origine sont transférées vers le nouvel objectif.

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

## Observations relatives à la copie des objectifs

Vous devez avoir accès à Modifier les objectifs dans votre niveau d’accès avant de pouvoir copier les objectifs. Pour plus d’informations sur l’octroi de l’accès aux objectifs, voir [Accorder l’accès aux objectifs Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Voici quelques-unes des raisons pour lesquelles vous souhaitez copier un objectif existant :

* À la fin d’une période (trimestre ou année), lorsque vous souhaitez recréer le même objectif pour la période suivante.
* À la fin d’une période, lorsque l’objectif ne peut pas être atteint et que vous souhaitez y travailler pendant une autre période.
* Lorsque plusieurs membres de l’équipe ont des objectifs similaires et que vous devrez peut-être en créer un pour chacun d’eux.

>[!TIP]
>
>Vous pouvez copier un objectif dans n’importe quel état. Pour plus d’informations sur les états d’objectif, consultez la [présentation de l’état de l’objectif dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/goal-status-overview.md).

Tenez compte des points suivants lors de la copie d’objectifs :

* Toutes les informations relatives à l’objectif sont également copiées vers le nouvel objectif.
* Vous pouvez choisir de copier les résultats d’un objectif existant. Le nom des résultats est transféré vers le nouvel objectif, mais la progression actuelle des résultats sur l’objectif existant ne copie pas vers le nouvel objectif. Par défaut, les résultats copiés sont attribués au même propriétaire.

  >[!NOTE]
  >
  >Si le propriétaire d’origine a été supprimé ou désactivé de Workfront, le nouveau résultat est attribué à l’utilisateur connecté.

* Vous ne pouvez pas copier les activités d’un objectif lorsque vous copiez ce dernier.

## Copier des objectifs

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


1. Accédez à un objectif et cliquez sur le menu **Plus** ![](assets/more-icon.png), puis cliquez sur **Copier l’objectif**.

   ![](assets/copy-goal-box-unshimmed.png)

1. Mettez à jour les informations suivantes pour l’objectif copié :
   * **Nom de l’objectif** : nom du nouvel objectif. Le nom par défaut de l’objectif copié est &quot;Copie de &lt;goal d’origine>&quot;.
   * **Période** : période pendant laquelle vous souhaitez atteindre l’objectif. Sélectionnez une période dans le menu déroulant.

     Ou

     Sélectionnez **Activer les dates personnalisées** pour spécifier des dates personnalisées pour les **dates de début** et **dates de fin** de l’objectif. Le paramètre Activer les dates personnalisées est désactivé par défaut.

     >[!TIP]
     >
     >   La désélection de l’option Activer les dates personnalisées rétablit la période de l’objectif d’origine.

      * **Propriétaire de l’objectif** : propriétaire de l’objectif. Il peut s’agir d’un utilisateur, d’une équipe, d’un groupe ou d’une société. Le ou la propriétaire de l’objectif initial est désigné par défaut.
      * **Description** : informations supplémentaires sur l’objectif.
      * **Copier les résultats** : sélectionnez cette option si vous souhaitez transférer les résultats de l’objectif actuel vers l’objectif copié. Cela duplique les résultats d’origine et les joint à l’objectif copié. Les résultats de l’objectif copié ont les mêmes propriétaire, noms et valeurs mesurées que les résultats de l’objectif initial.

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
   >* [Ajouter des résultats aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/add-results-to-goals.md)
   >* [Ajouter des activités aux objectifs dans les objectifs Adobe Workfront](../results-and-activities/add-activities-to-goals.md)
   >* [Aligner les objectifs en les connectant dans les objectifs Adobe Workfront](../goal-alignment/align-goals-by-connecting-them.md)
   >
   >Pour plus d’informations sur l’activation des objectifs, voir [Activation des objectifs](../goal-management/activate-goals.md).

