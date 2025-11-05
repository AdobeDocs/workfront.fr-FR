---
product-area: projects
navigation-topic: manage-issues
title: Modifier les affectations d’utilisateurs et utilisatrices pour plusieurs problèmes dans une liste
description: Modifier les affectations d’utilisateurs et utilisatrices pour plusieurs problèmes dans une liste
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 47%

---

# Modifier les affectations d’utilisateurs et utilisatrices pour plusieurs problèmes dans une liste

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

<div class="preview">

Les informations surlignées sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Les mêmes fonctionnalités seront également disponibles dans l’environnement de production pour tous les clients et clientes à partir d’une semaine à compter de la version préliminaire.

Pour plus d’informations, voir [Modernisation des interfaces](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>

Vous pouvez modifier simultanément les affectations d’utilisateurs à plusieurs événements. Pour plus d’informations sur la modification des événements ou leur affectation un par un, consultez également les articles suivants :

* [Modifier les problèmes](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Attribuer des problèmes](../../../manage-work/issues/manage-issues/assign-issues.md)

Pour obtenir des informations générales sur l’affectation de problèmes, voir [Vue d’ensemble de la modification des affectations de problèmes](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Vous devez disposer au moins des autorisations de contribution à un problème pour pouvoir effectuer des affectations au problème.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Accédez en lecture seule ou à un niveau supérieur aux Projets et Tâches pour affecter un événement.</p> </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations liées aux problèmes</p> <p>Accordez des autorisations ou supérieures au projet ou à la tâche où se trouve le problème lors de l’affectation de plusieurs problèmes.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Modifier des affectations pour plusieurs problèmes

1. Accédez à la liste des événements qui contient les événements dont vous souhaitez modifier les affectations.
1. (Facultatif) Créez un filtre pour afficher uniquement les problèmes affectés à la personne cessionnaire que vous souhaitez modifier.

   Par exemple, vous pouvez créer un filtre pour afficher uniquement les événements disposant d’un rôle spécifique en tant que personne désignée.  Vous pouvez ensuite remplacer le rôle par un utilisateur ou une utilisatrice spécifique. Procédez comme suit :

   1. Cliquez sur la liste déroulante **Filtres**, puis sur **Nouveau filtre**.

   1. Dans le premier champ, commencez à saisir **Rôles pour l’affectation** et choisissez **Rôles pour l’affectation : Nom** dans la liste.
   1. Sélectionnez **Est l’un des** dans le menu déroulant des modificateurs, puis commencez à saisir le nom d’un rôle et sélectionnez-le lorsqu’il s’affiche dans la liste. Vous pouvez saisir plusieurs rôles.

      >[!TIP]
      >
      >N’utilisez pas l’option **Affecté à** car ce champ fait référence uniquement au propriétaire de l’événement et non à tous les cessionnaires.

      La liste des événements filtre automatiquement vos critères de filtrage.
   1. (Facultatif) Cliquez sur **Enregistrer en tant que nouveau** puis **Enregistrer**.

1. Sélectionnez les événements pour lesquels vous souhaitez modifier les affectations, puis cliquez sur l&#39;icône **Modifier** ![Modifier](assets/qs-edit-icon.png).

   La boîte **Modifier des problèmes** s’affiche. Le nombre d’éléments sélectionnés s’affiche dans le coin supérieur gauche de la page.

1. (Conditionnel) Dans l’environnement de Production, procédez comme suit :

   1. Accédez à la section **Affectations**, puis sélectionnez **Cessionnaire**.

      ![Zone Affectations](assets/classic-assignmens-area-on-edit-box-350x119.png)

   1. Utilisez l’une des méthodes suivantes :

      1. Pour ajouter un ou une cessionnaire :

         1. Commencez à saisir le nom d’une personne, d’un rôle ou d’une équipe, puis sélectionnez-le lorsqu’il s’affiche dans la liste. L’affectation est ajoutée et ne remplace pas les affectations actuelles sur les problèmes sélectionnés.

         >[!TIP]
         >
         >Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
         >
         >Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
         >
         >* Réaffectez la tâche aux ressources actives.
         >* Associez les utilisateurs et utilisatrices d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.

         Les informations communes à tous les problèmes sélectionnés s’affichent. Par exemple, si le même utilisateur est affecté à tous les événements, il s’affiche dans la colonne **Personne désignée**. Si des informations ne sont pas communes aux problèmes sélectionnés, aucune information ne s’affiche.

      1. Pour supprimer des personnes cessionnaires :

         1. Cliquez sur l’**icône X** en regard du nom de la personne cessionnaire que vous souhaitez supprimer si cette dernière s’affiche dans la liste Affectations.

            Ou

            Si la personne désignée que vous souhaitez supprimer ne s’affiche pas dans la section Affectations, car elle n’est affectée qu’à certains des événements que vous avez sélectionnés, cliquez sur **Supprimer un cessionnaire** et commencez à saisir le nom de la personne désignée que vous souhaitez supprimer, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

         1. Cliquez de nouveau sur **Supprimer le cessionnaire** pour ajouter un autre cessionnaire à supprimer.

      1. Pour supprimer toutes les personnes cessionnaires existantes :

         1. Cliquez sur **Supprimer toutes les personnes cessionnaires existantes**, puis sur **Oui, supprimer toutes les personnes cessionnaires**.

            Cela supprime non seulement les délégataires communs (délégataires affichés dans la boîte de dialogue de modification), mais aussi tous les délégataires pour tous les événements sélectionnés.

         1. (Facultatif) Modifiez l’une des options suivantes pour les personnes cessionnaires que vous avez sélectionnées afin de les associer aux problèmes :

            * **Propriétaire de l’événement :** sélectionnez le bouton radio pour indiquer la personne désignée comme propriétaire des événements. Si cette option n’est pas sélectionnée, Adobe Workfront désigne la première personne cessionnaire comme propriétaire du problème. Cette option n’est pas disponible pour les affectations d’équipe.
            * **Rôle de la personne cessionnaire** : sélectionnez un rôle dans la liste déroulante. Si cette option n’est pas sélectionnée, Workfront sélectionne automatiquement le rôle principal de l’utilisateur ou utilisatrice.

      1. Cliquez sur **Enregistrer les modifications**.

1. <span class="preview">Dans l’environnement de prévisualisation, procédez comme suit :</span>

   1. <span class="preview">Cliquez sur **Affectations** dans le panneau de gauche, puis cliquez sur l’icône **x** en regard de la personne désignée à supprimer. </span>

      >[!TIP]
      >
      ><span class="preview">Seuls les cessionnaires affectés à tous les événements sélectionnés s&#39;affichent dans la zone **Affectations**. </span>

      ![Zone Affectations dans les événements de modification en bloc](assets/assignments-area-on-bulk-edit-issues.png)

   1. <span class="preview">Commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe pour ajouter des délégataires à tous les événements sélectionnés. </span>

      >[!TIP]
      >
      >Vous pouvez affecter plusieurs utilisateurs et utilisatrices, fonctions ou équipes. Vous pouvez affecter uniquement les utilisateurs et utilisatrices, fonctions et équipes actifs.
      >
      >Si une personne, une fonction ou une équipe a été affectée avant d’être désactivée, elle reste affectée à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
      >
      >* Réaffectez la tâche aux ressources actives.
      >* Associez les utilisateurs et utilisatrices d’une équipe désactivée à une équipe active et réaffectez l’élément de travail à l’équipe active.

      <span class="preview">Les délégataires ajoutés sont ajoutés aux délégataires existants. Ils ne remplacent pas les problèmes existants pour chaque événement sélectionné. </span>
   1. <span class="preview">(Facultatif) Cliquez sur **M’affecter** pour vous affecter tous les problèmes.</span>
   1. <span class="preview">Cliquez sur **Enregistrer**. </span>




