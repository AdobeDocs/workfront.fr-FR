---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Aligner les objectifs en convertissant les résultats et les activités en objectifs
description: Vous pouvez aligner manuellement deux objectifs ou convertir les résultats et les activités d’un objectif existant en un autre objectif. Le résultat converti ou l’activité convertie devient l’objectif enfant de l’objectif initial. Pour plus d’informations sur l’alignement manuel de deux objectifs, consultez la section « Aligner des objectifs en les reliant dans les Objectifs Adobe Workfront ».
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 81%

---

# Aligner les objectifs en convertissant les résultats et les activités en objectifs

<!--Audited P&P only: 4/2025-->

Vous pouvez aligner manuellement deux objectifs ou convertir les résultats et les activités d’un objectif existant en un autre objectif. Le résultat converti ou l’activité convertie devient l’objectif enfant de l’objectif initial.
Pour plus d’informations sur l’alignement manuel de deux objectifs, consultez la section [Aligner des objectifs en les reliant dans les Objectifs Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Conditions d’accès

>[!NOTE]
>
>Votre entreprise peut choisir de continuer à utiliser les objectifs Adobe Workfront si elle a déjà acheté ce package par le passé. Pour plus de détails, contactez votre représentant de compte.
>
>Adobe Workfront Goals ne peut plus être acheté.

+++Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>

<td> <p>Package Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>Licence Adobe Workfront</p> </td> 
   <td> <p>Contributeur ou version ultérieure</p> 
     <p>Demandeur ou supérieur</p> </td> 
  </tr>

<td><p>Configurations des niveaux d’accès</p> </td> 
   <td> <p>Modifier l’accès aux Objectifs</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Gestion des autorisations relatives à un objectif</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Un modèle de mise en page comprenant la zone Objectifs du menu principal doit être affecté à tous les utilisateurs, y compris les administrateurs système. </p>  
</td>
  </tr>
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès à la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   Or
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

Vous devez disposer des éléments suivants avant de pouvoir démarrer :

* Un objectif existant avec des résultats et des activités existants.

  Pour plus d’informations sur la création d’objectifs, voir [Créer des objectifs dans les Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Un objectif peut avoir jusqu’à 1 000 indicateurs de progression.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Éléments à prendre en compte pour convertir les résultats et les activités en objectifs

Parfois, un résultat ou une activité peut avoir une portée plus large que prévu et il serait plus logique d’en faire des objectifs. Vous pouvez convertir les résultats et les activités d’un objectif existant en un nouvel objectif. Il s’agit d’une approche ascendante de l’alignement des objectifs.

Tenez compte des éléments suivants lorsque vous convertissez des résultats et des activités en objectifs :

* Le résultat converti ou l’activité convertie devient l’objectif enfant de l’objectif d’origine, et les deux objectifs s’alignent.
* L’objectif nouvellement créé devient l’unique indicateur de progrès pour l’objectif initial, s’il n’y a pas de résultats ou d’activités supplémentaires pour l’objectif d’origine. Vous devez ajouter des résultats et des activités à l’objectif enfant pour pouvoir suivre la progression de cet objectif.
* La conversion d’un résultat ou d’une activité en un objectif est irréversible. Une fois converti, le nouvel objectif enfant ne peut plus jamais devenir un résultat ou une activité pour l’objectif parent.

## Convertir un résultat ou une activité en objectif

<!--
<span class="preview">Converting results and activities differs depending on what environment you use. </span>

### Convert a result or activity to a goal in the Production environment

1. Go to a goal that has a result or an activity that you want to convert to a goal.
1. Click the name of the goal to open the **Goal Details** panel.
1. Expand the **Results** or **Activities** right-pointing arrows to see a list of results or activities for the goal. 

1. Click the **gear icon** ![Gear icon](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![Convert to goal](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Accédez à un objectif dont vous souhaiter convertir le résultat ou l’activité en objectif.
1. Sur la page de l’objectif, cliquez sur **Indicateurs de progression** dans le panneau de gauche.
1. Sélectionnez un résultat ou une activité dans la liste des indicateurs de progression, puis cliquez sur l’icône **Convertir en objectif** ![Convertir en objectif](assets/convert-to-goal-icon-unshimmed.png) en haut de la liste des indicateurs de progression. La boîte de dialogue Convertir en objectif s’affiche.

   ![&#x200B; Convertir en zone d’objectif &#x200B;](assets/convert-to-goal-box-unshimmed.png)
1. Mettez à jour les informations suivantes :
   * **Nom de l’objectif** : par défaut, le nouvel objectif porte le même nom que le résultat ou l’activité d’origine.
   * **Période** : par défaut, la période du nouvel objectif est le trimestre en cours. Vous pouvez sélectionner le paramètre **Activer les dates personnalisées** pour définir une période personnalisée pour le nouvel objectif.
   * **Personne propriétaire de l’objectif** : par défaut, la nouvelle personne propriétaire de l’objectif est la personne propriétaire du résultat ou de l’activité d’origine.
   * **Description** : donnez du contexte au nouvel objectif.
1. Cliquer sur **Enregistrer**.

   Le résultat ou l’activité est maintenant converti(e) en un objectif enfant de l’objectif initial. Il s’inscrit comme objectif dans la liste des indicateurs de progression de l’objectif d’origine.



