---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Aligner les objectifs en convertissant les résultats et les activités en objectifs
description: Vous pouvez aligner manuellement deux objectifs ou convertir les résultats et les activités d’un objectif existant en un autre objectif. Le résultat converti ou l’activité convertie devient l’objectif enfant de l’objectif initial. Pour plus d’informations sur l’alignement manuel de deux objectifs, consultez la section « Aligner des objectifs en les reliant dans les Objectifs Adobe Workfront ».
author: Alina
feature: Workfront Goals
exl-id: 48371389-952c-4732-b519-9774cd4d1b93
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 94%

---

# Aligner les objectifs en convertissant les résultats et les activités en objectifs

Vous pouvez aligner manuellement deux objectifs ou convertir les résultats et les activités d’un objectif existant en un autre objectif. Le résultat converti ou l’activité convertie devient l’objectif enfant de l’objectif initial.
Pour plus d’informations sur l’alignement manuel de deux objectifs, consultez la section [Aligner des objectifs en les reliant dans les Objectifs Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

## Conditions d’accès


<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
 <td role="rowheader">Formule Adobe Workfront</td>
 <td>
 <p>Tous</p>

</td>
 </tr>
 <tr>
 <td role="rowheader">Licence Adobe Workfront*</td>
 <td>
 <p>Nouvelle licence : contributeur ou contributrice ou niveau supérieur</p>
 Ou
 <p>Licence actuelle : demande ou niveau supérieur</p> <p>Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Vue d’ensemble des licences Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produit*</td>
 <td>
 <p> Nouvelle exigence de produit, une des options suivantes : </p>
<ul>
<li>Un forfait Adobe Workfront Select ou Prime et une licence Objectifs Adobe Workfront supplémentaire.</li>
<li>Un forfait Workfront Ultimate qui inclut Objectifs Workfront par défaut. </li></ul>
 <p>Ou</p>
 <p>Exigence de produit actuelle : un forfait Workfront et une licence supplémentaire pour Objectifs Adobe Workfront. </p> <p>Pour plus d’informations, consultez la section <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Exigences pour l’utilisation des Objectifs Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Niveau d’accès</td>
 <td> <p>Modifier l’accès aux Objectifs</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Autorisations d’objet</td>
 <td>
  <div>
  <p>Autorisations d’affichage ou de niveau supérieur sur l’objectif pour l’afficher</p>
  <p>Autorisations de gestion sur l’objectif pour le modifier</p>
  <p>Pour plus d’informations sur le partage des objectifs, voir <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Partager un objectif dans Objectifs Workfront</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modèle de mise en page</p></td>
   <td> <p>Toutes les personnes, y compris les administrateurs et administratrices Workfront, doivent se voir attribuer un modèle de mise en page incluant la zone Objectifs dans le menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

   ![ Convertir en zone d’objectif ](assets/convert-to-goal-box-unshimmed.png)
1. Mettez à jour les informations suivantes :
   * **Nom de l’objectif** : par défaut, le nouvel objectif porte le même nom que le résultat ou l’activité d’origine.
   * **Période** : par défaut, la période du nouvel objectif est le trimestre en cours. Vous pouvez sélectionner le paramètre **Activer les dates personnalisées** pour définir une période personnalisée pour le nouvel objectif.
   * **Personne propriétaire de l’objectif** : par défaut, la nouvelle personne propriétaire de l’objectif est la personne propriétaire du résultat ou de l’activité d’origine.
   * **Description** : donnez du contexte au nouvel objectif.
1. Cliquer sur **Enregistrer**.

   Le résultat ou l’activité est maintenant converti(e) en un objectif enfant de l’objectif initial. Il s’inscrit comme objectif dans la liste des indicateurs de progression de l’objectif d’origine.



