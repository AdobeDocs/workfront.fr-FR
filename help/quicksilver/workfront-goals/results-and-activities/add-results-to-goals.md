---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Ajouter des résultats aux objectifs dans les Objectifs Adobe Workfront
description: Les résultats mesurent la progression d’un objectif. L’activation de l’objectif et l’enregistrement des progrès réalisés ne sont possibles que si des résultats, des activités ou des objectifs alignés sont associés à l’objectif.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 85%

---

# Ajouter des résultats aux objectifs dans les Objectifs Adobe Workfront

<!--Audited for P&P only: 10/2025-->

Les résultats mesurent la progression d’un objectif. L’activation de l’objectif et l’enregistrement des progrès réalisés ne sont possibles que si des résultats, des activités ou des objectifs alignés sont associés à l’objectif.

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
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p>  </td>
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

* Un modèle de mise en page qui inclut la zone Objectifs dans le menu principal.
* Objectif existant.

  Pour plus d’informations sur la création d’objectifs, consultez la section [Créer des objectifs dans Objectifs Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>Un objectif ne peut pas dépasser 1 000 activités, résultats, projets et objectifs alignés.

## Ajouter un résultat à un objectif

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![Add result inside goal](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![Results value](assets/results-value-initial-target-boxes-350x49.png)

   Select from the following options:

   |Option|Value type|
   |---|---|
   | # |Number value |
   | % |Percentage value |
   |$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪  |Currency values |

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value.

   >[!TIP]
   >
   >The result Type is always Metric and cannot be edited.

1. In the Initial field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the Target field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1. Click **Save**.

   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result.

-->

1. Cliquez sur le menu principal ![icône du menu principal](assets/main-menu-icon.png), puis sur **Objectifs**.

1. Pour ouvrir la page d’un objectif, cliquez sur son nom dans la **Liste des objectifs**.
1. Cliquez sur **Indicateurs de progression** dans le panneau de gauche.
1. Développez le menu déroulant **Nouvel indicateur de progression**, puis cliquez sur **Créer un résultat**.

   La boîte de dialogue « Nouveau résultat » s’affiche.

   ![Nouvelle zone de résultat](assets/new-result-box-unshimmed.png)

1. Saisissez un nom pour le résultat dans le champ **Nom du résultat**. Champ obligatoire.
1. (Facultatif) Supprimez votre nom du champ **Personne propriétaire du résultat** si vous souhaitez affecter le résultat à un autre utilisateur ou une autre utilisatrice. Par défaut, vous êtes la personne propriétaire d’une activité que vous créez.

   >[!NOTE]
   >
   >Vous ne pouvez pas affecter une équipe, un groupe ou l’entreprise en tant que propriétaire de résultat.

1. Dans la zone **Comment voulez-vous mesurer votre résultat ?**, renseignez les informations suivantes :
   * **Type de valeur** : indique comment mesurer la progression par rapport au résultat. Vous pouvez mesurer la progression de manière numérique, en pourcentage ou en utilisant une valeur en devise.

     Sélectionnez un type de valeur parmi les options répertoriées dans le tableau suivant :

     | Type de valeur | Description |
     |---------------------------------------------------------|------------------|
     | Nombre | Valeur numérique |
     | % | Valeur en pourcentage |
     | CN¥, DKK, KR, Mex$, R, R$, zł, £, ¥, €, ₹, ฿, MYR, ₪, $ | Valeurs en devise |

   * **Valeur initiale** : valeur initiale du résultat avant toute progression enregistrée.
   * **Valeur cible** : valeur que le résultat vise à atteindre lorsqu’il est considéré comme terminé.
1. Cliquez sur **Créer un résultat**.

   Le résultat s’affiche dans la section des indicateurs de progression de la page d’objectifs, sous le regroupement « Résultats ».

   Une fois l’objectif activé, sa progression est automatiquement actualisée lorsque vous mettez à jour la progression d’un résultat. Pour plus d’informations sur l’activation d’un objectif, consultez la section [Activer des objectifs dans Objectifs Adobe Workfront](../goal-management/activate-goals.md).
