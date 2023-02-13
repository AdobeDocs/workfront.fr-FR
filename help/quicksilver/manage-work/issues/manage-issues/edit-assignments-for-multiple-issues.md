---
product-area: projects
navigation-topic: manage-issues
title: Modification des affectations d’utilisateurs pour plusieurs problèmes dans une liste
description: Modification des affectations d’utilisateurs pour plusieurs problèmes dans une liste
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# Modification des affectations d’utilisateurs pour plusieurs problèmes dans une liste

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

Vous pouvez simultanément modifier les affectations d’utilisateurs pour plusieurs problèmes. Pour plus d’informations sur la modification des problèmes ou leur attribution une par une, reportez-vous également aux articles suivants :

* [Modification des problèmes](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Attribuer des problèmes](../../../manage-work/issues/manage-issues/assign-issues.md)

Pour obtenir des informations générales sur l’affectation de problèmes, voir [Modification de l’aperçu des affectations de problème](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Vous devez disposer au moins des autorisations de contribution à un problème pour pouvoir effectuer des affectations au problème.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux problèmes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations liées au problème</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

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

   Par exemple, vous pouvez créer un filtre pour afficher uniquement les problèmes avec un rôle spécifique comme personne désignée. Vous pouvez ensuite remplacer le rôle par un utilisateur spécifique. Procédez comme suit :

   1. Cliquez sur le bouton **Filtrer** liste déroulante, puis cliquez sur **Nouveau filtre**.

      La boîte de dialogue Nouveau filtre s’affiche.

   1. Cliquez sur **Ajoutez une règle de filtrage.**
   1. Pour filtrer un rôle spécifique, développez **Rôles d’affectation,** puis cliquez sur **ID.**

      Ou

      Pour filtrer un utilisateur spécifique, développez **Affecter des utilisateurs,** puis cliquez sur **ID.**

      >[!TIP]
      >
      >Ne pas utiliser **Affecté à** car ce champ fait uniquement référence au propriétaire du problème et non à tous les cessionnaires.

   1. Dans la liste déroulante, sélectionnez **Égal** comme qualificateur de filtre.
   1. Commencez à saisir le nom de l’utilisateur ou du rôle pour lequel vous souhaitez filtrer les données, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.
   1. Cliquez sur **Enregistrer le filtre.**

1. Sélectionnez les problèmes pour lesquels vous souhaitez modifier les affectations, puis cliquez sur le bouton **Modifier** icon ![](assets/qs-edit-icon.png).

   Le **Modification des problèmes** s’affiche. Les éléments modifiés s’affichent dans le coin supérieur gauche de la page.

1. Accédez au **Affectations** , puis sélectionnez **Cessionnaire**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Utilisez l’une des méthodes suivantes :

   1. Pour ajouter une nouvelle personne désignée :

      1. Commencez à saisir le nom d’un utilisateur, d’un rôle ou d’une équipe, puis sélectionnez-le lorsqu’il s’affiche dans la liste. L’affectation est ajoutée et ne remplace pas les affectations actuelles sur les problèmes sélectionnés.

         >[!TIP]
         Vous pouvez affecter plusieurs utilisateurs, rôles de tâche ou équipes. Vous ne pouvez affecter que des utilisateurs, des rôles de tâche et des équipes principaux.
         Si un utilisateur, un rôle de tâche ou une équipe a été affecté avant d’être désactivé, il reste attribué à l’élément de travail. Dans ce cas, nous vous recommandons ce qui suit :
         * Réaffectez l’élément de travail aux principales ressources.
         * Associez les utilisateurs d’une équipe désactivée à une équipe principale et réaffectez l’élément de travail à l’équipe principale.


         Les informations communes à tous les problèmes sélectionnés s’affichent. Par exemple, si le même utilisateur est affecté à tous les problèmes, il s’affiche dans la variable **Cessionnaire** colonne . Si des informations ne sont pas communes aux problèmes sélectionnés, aucune information ne s’affiche.
   1. Pour supprimer des personnes désignées :

      1. Cliquez sur le bouton **Icône X** en regard du nom de la personne désignée que vous souhaitez supprimer si la personne désignée s’affiche dans la liste Affectations .

         Ou

         (Conditionnel) Si la personne désignée à supprimer ne s’affiche pas dans la section Affectations , car elle n’est affectée qu’à certains des problèmes que vous avez sélectionnés, cliquez sur **Supprimer le cessionnaire** et commencez à saisir le nom de la personne désignée à supprimer, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.

      1. Cliquez sur **Supprimer le cessionnaire** pour ajouter une autre personne désignée à supprimer.
   1. Pour supprimer tous les cessionnaires existants :

      1. Cliquez sur **Supprimer tous les cessionnaires existants**, puis cliquez sur **Oui, supprimer tous les cessionnaires**.

         Cela supprime non seulement les personnes désignées courantes (personnes désignées qui s’affichent dans la boîte de dialogue de modification), mais également toutes les personnes désignées sur tous les problèmes sélectionnés.



1. (Facultatif) Modifiez l’une des options suivantes pour les personnes désignées que vous avez sélectionnées afin de les associer aux problèmes :

   * **Propriétaire du problème :** Sélectionnez le bouton radio pour indiquer la personne désignée comme propriétaire des problèmes. Si cette option n’est pas sélectionnée, Adobe Workfront désigne la première personne désignée comme propriétaire du problème. Cette option n’est pas disponible pour les affectations d’équipe.
   * **Le rôle du cessionnaire**: Sélectionnez un rôle dans la liste déroulante. Si cette option n’est pas sélectionnée, Workfront sélectionne automatiquement le rôle Principal de l’utilisateur.

1. Cliquez sur **Enregistrer les modifications**.
