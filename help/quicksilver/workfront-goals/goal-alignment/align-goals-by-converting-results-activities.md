---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Alignement des objectifs en convertissant les résultats et les activités en objectifs
description: Vous pouvez aligner manuellement deux objectifs ou convertir les résultats et activités d’un objectif existant en un autre. Le résultat ou l’activité converti devient l’objectif enfant de l’objectif d’origine. Pour plus d’informations sur l’alignement manuel de deux objectifs, voir Aligner les objectifs en les reliant dans les objectifs Adobe Workfront.
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 25%

---

# Alignement des objectifs en convertissant les résultats et les activités en objectifs

Vous pouvez aligner manuellement deux objectifs ou convertir les résultats et activités d’un objectif existant en un autre. Le résultat ou l’activité converti devient l’objectif enfant de l’objectif d’origine.
Pour plus d’informations sur l’alignement manuel de deux objectifs, voir [Alignement des objectifs en les connectant aux objectifs Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Conditions d’accès


<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Forfait Adobe Workfront</td>
 <td>
 <p>N’importe quelle</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Licence Adobe Workfront*</td>
 <td>
 <p>Licence actuelle : contributeur ou version ultérieure</p>
 Ou
 <p>Licence héritée : demande ou supérieure</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences Adobe Workfront</a>.</p> </td>
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
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Tous les utilisateurs, y compris les administrateurs de Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Vous devez disposer des éléments suivants avant de commencer :

* Objectif existant avec des résultats et des activités existants.

  Pour plus d’informations sur la création d’objectifs, voir [Création d’objectifs dans les objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>
>Un objectif peut comporter jusqu’à 1 000 indicateurs de progression.

<!--drafted for goal redesign: At PRODUCTION: update the sentence above to remove Production/ Preview references-->

## Considérations relatives à la conversion de résultats et d’activités en objectifs

Parfois, un résultat ou une activité peut avoir une portée plus large que prévu et il serait plus logique qu’ils deviennent des objectifs. Vous pouvez convertir les résultats et les activités d’un objectif existant en un nouvel objectif. Il s’agit d’une approche ascendante de l’alignement des objectifs.

Tenez compte des points suivants lors de la conversion de résultats et d’activités en objectifs :

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

1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result or activity name that you want to convert, then click **Convert into a Goal**.

   ![](assets/convert-to-goal-link-highlighted-350x191.png)

1. (Optional) Remove the name of the original activity or result owner from the **Goal Owner** field and replace it with another user, team, group, or your organization's name. By default, Workfront selects the owner of the result or the activity as the goal owner. 
1. Click **Convert**. The activity or result displays as an aligned goal in the Goal Details panel of the original goal and the original activity or result is removed from the original goal and transferred to the second goal. By default, the new goal has the same name as the original converted result or activity. 
1. (Optional) Click the name of the new goal to open the **Goal Details** panel and edit the name of the goal. For information about editing any information for an existing goal, see [Edit goals in Adobe Workfront Goals](../../workfront-goals/goal-management/edit-goals.md).
-->

1. Accédez à un objectif comportant un résultat ou une activité que vous souhaitez convertir en objectif.
1. Sur la page de l’objectif, cliquez sur **Indicateurs de progression** dans le panneau de gauche.
1. Sélectionnez un résultat ou une activité dans la liste des indicateurs de progression, puis cliquez sur le bouton **Convertir en objectif** icon ![](assets/convert-to-goal-icon-unshimmed.png) en haut de la liste des indicateurs de progression. La zone Convertir en objectif s’ouvre.

   ![](assets/convert-to-goal-box-unshimmed.png)
1. Mettez à jour les informations suivantes :
   * **Nom de l’objectif**: par défaut, le nouvel objectif porte le même nom que le résultat ou l’activité d’origine.
   * **Période**: par défaut, la période du nouvel objectif est le trimestre en cours. Vous pouvez sélectionner la variable **Activation des dates personnalisées** pour définir une période personnalisée pour le nouvel objectif.
   * **Propriétaire de l’objectif**: par défaut, le nouveau propriétaire de l’objectif est le propriétaire du résultat ou de l’activité d’origine.
   * **Description**: ajoutez des informations supplémentaires sur le nouvel objectif.
1. Cliquez sur **Enregistrer**

   Le résultat ou l’activité est désormais converti en objectif enfant de l’objectif d’origine. Il est répertorié comme un objectif dans la liste des indicateurs de progression de l’objectif d’origine.



