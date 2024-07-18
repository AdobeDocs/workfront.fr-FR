---
product-area: projects
navigation-topic: manage-issues
title: Modifier les affectations d’utilisateurs et utilisatrices pour plusieurs problèmes dans une liste
description: Modifier les affectations d’utilisateurs et utilisatrices pour plusieurs problèmes dans une liste
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 070b0525f0cb2880d3c7daf88777ba48968ce759
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 18%

---

# Modifier les affectations d’utilisateurs et utilisatrices pour plusieurs problèmes dans une liste

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

Vous pouvez simultanément modifier les affectations d’utilisateurs pour plusieurs problèmes. Pour plus d’informations sur la modification des problèmes ou leur attribution une par une, reportez-vous également aux articles suivants :

* [Modification des problèmes](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Attribuer les problèmes](../../../manage-work/issues/manage-issues/assign-issues.md)

Pour obtenir des informations générales sur l’affectation des problèmes, consultez [Présentation de la modification des affectations de problèmes](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Vous devez disposer au moins des autorisations Contribute pour un problème afin de pouvoir effectuer des affectations sur le problème.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Nouvelle : standard </p>
   <p>Actuelle : demande ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Affichage ou accès supérieur à Projets et tâches pour affecter un problème</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations liées au problème</p> <p>Autorisations Contribute ou supérieures au projet ou à la tâche où se trouve le problème, lors de l’attribution de plusieurs problèmes.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Modification des affectations pour plusieurs problèmes

1. Accédez à la liste des problèmes contenant les problèmes dont vous souhaitez modifier les affectations.
1. (Facultatif) Créez un filtre pour afficher uniquement les problèmes affectés à la personne désignée que vous souhaitez modifier.

   Par exemple, vous pouvez créer un filtre pour afficher uniquement les problèmes avec un rôle spécifique comme personne désignée. Vous pouvez ensuite remplacer le rôle par un utilisateur spécifique. Procédez comme suit :

   1. Cliquez sur la liste déroulante **Filtre** , puis sur **Nouveau filtre**.

      La boîte de dialogue Nouveau filtre s’affiche.

   1. Cliquez sur **Ajouter une règle de filtre.**
   1. Pour filtrer un rôle spécifique, développez **Rôles d’affectation,**, puis cliquez sur **ID.**

      Ou

      Pour filtrer un utilisateur spécifique, développez **Assignment Users,**, puis cliquez sur **ID.**

      >[!TIP]
      >
      >N’utilisez pas **Affecté à**, car ce champ ne fait référence qu’au propriétaire du problème et non à tous les cessionnaires.

   1. Dans la liste déroulante, sélectionnez **Equal** comme qualificateur de filtre.
   1. Commencez à saisir le nom de l’utilisateur ou du rôle pour lequel vous souhaitez filtrer les données, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.
   1. Cliquez sur **Enregistrer le filtre.**

1. Sélectionnez les problèmes pour lesquels vous souhaitez modifier les affectations, puis cliquez sur l&#39;icône **Modifier** ![](assets/qs-edit-icon.png).

   L’écran **Modifier les problèmes** s’affiche. Les éléments modifiés s’affichent dans le coin supérieur gauche de la page.

1. Accédez à la section **Assignments** , puis sélectionnez **Assignee**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Utilisez l’une des méthodes suivantes :

   1. Pour ajouter une nouvelle personne désignée :

      1. Commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe, puis sélectionnez-le lorsqu’il s’affiche dans la liste. L’affectation est ajoutée et ne remplace pas les affectations actuelles sur les problèmes sélectionnés.

         >[!TIP]
         >
         >Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
         >
         >Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
         >
         >* Réaffectez l’élément de travail aux ressources actives.
         >* Associez les personnes d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.

         Les informations communes à tous les problèmes sélectionnés s’affichent. Par exemple, si le même utilisateur est affecté à tous les problèmes, il s’affiche dans la colonne **Assignation**. Si des informations ne sont pas communes aux problèmes sélectionnés, aucune information ne s’affiche.

   1. Pour supprimer des personnes désignées :

      1. Cliquez sur l’icône **X** en regard du nom de la personne désignée à supprimer si la personne désignée s’affiche dans la liste Affectations.

         Ou

         (Conditionnel) Si la personne désignée à supprimer ne s’affiche pas dans la section Affectations car elle n’est affectée qu’à certains des problèmes que vous avez sélectionnés, cliquez sur **Supprimer la personne désignée** et commencez à saisir le nom de la personne désignée à supprimer, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

      1. Cliquez à nouveau sur **Supprimer le cessionnaire** pour ajouter une autre cessionnaire à supprimer.

   1. Pour supprimer tous les cessionnaires existants :

      1. Cliquez sur **Supprimer tous les cessionnaires existants**, puis sur **Oui, Supprimer tous les cessionnaires**.

         Cela supprime non seulement les personnes désignées courantes (personnes désignées qui s’affichent dans la boîte de dialogue de modification), mais également toutes les personnes désignées sur tous les problèmes sélectionnés.

1. (Facultatif) Modifiez l’une des options suivantes pour les personnes désignées que vous avez sélectionnées afin de les associer aux problèmes :

   * **Propriétaire du problème :** Sélectionnez le bouton radio pour indiquer quelle personne désignée est désignée comme propriétaire des problèmes. Si cette option n’est pas sélectionnée, Adobe Workfront désigne la première personne désignée comme propriétaire du problème. Cette option n’est pas disponible pour les affectations d’équipe.
   * **Rôle du cessionnaire** : sélectionnez un rôle dans la liste déroulante. Si cette option n’est pas sélectionnée, Workfront sélectionne automatiquement le rôle de Principal de l’utilisateur.

1. Cliquez sur **Enregistrer les modifications**.
