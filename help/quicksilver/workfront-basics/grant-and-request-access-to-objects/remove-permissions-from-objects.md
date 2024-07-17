---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Supprimer les autorisations des objets
description: Vous pouvez supprimer les autorisations d’autres utilisateurs sur les objets que vous avez accès à Partager. La suppression des autorisations des objets est identique pour tous les objets qui peuvent être partagés.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 5%

---

# Supprimer les autorisations des objets

<!--Audited: 01/2024-->

Vous pouvez supprimer les autorisations d’autres utilisateurs sur les objets que vous avez accès à Partager. La suppression des autorisations des objets est identique pour tous les objets qui peuvent être partagés.

Les mêmes considérations que pour le partage d’objets s’appliquent pour supprimer des autorisations d’objets. Pour plus d’informations, reportez-vous à la section [Observations relatives au partage d’objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) dans l’article [  Aperçu des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## Conditions d’accès

Pour partager des objets, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Workfront*</td> 
   <td> <p>Nouvelle licence : contributeur ou version ultérieure</p>
   Ou  
   <p>Licence actuelle : demande ou supérieure</p>
   <p><b>NOTE</b></p>

<p>Certains objets nécessitent un accès supérieur à Demander. </p>

<p>Par exemple, pour la nouvelle licence, un contributeur peut partager des problèmes, mais seuls les utilisateurs sous licence standard peuvent partager un projet.</p>

<p>Pour la licence actuelle, un demandeur peut partager des problèmes, mais seuls les travailleurs ou les planificateurs peuvent partager un projet.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Afficher l’accès ou une version ultérieure aux objets que vous souhaitez partager</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations ou plus pour les objets que vous souhaitez partager</p> <p>Gestion des autorisations pour supprimer les autorisations héritées sur les objets</p>  </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations, consultez les [Conditions d’accès de la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Supprimer des entités de la liste de partage d’un objet {#remove-entities-from-the-sharing-list-of-an-object}

Vous pouvez supprimer des entités (utilisateurs, rôles de tâche, équipes, groupes, entreprises) de la liste de partage d’un objet. Cela supprime leurs autorisations sur l’objet .

1. Accédez à l’objet duquel vous souhaitez supprimer des autorisations.

   Pour plus d’informations sur les objets qui peuvent être partagés, voir [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Conditionnel) Pour les programmes, les portefeuilles et les documents, procédez comme suit :

   1. Cliquez sur l&#39;icône **Plus** ![](assets/more-icon.png) en regard du nom de l&#39;objet, puis sur **Partage** ou **Partager.**

      ![](assets/share-a-document-350x160.png)

   1. Cliquez sur le **x** en regard du nom d’un utilisateur, d’une équipe, d’un groupe, d’une société, d’un rôle de tâche pour le supprimer dans la zone d’accès aux objets.

      ![](assets/remove-permissions-on-portfolio.png)

   1. Dans le menu déroulant **&lt; Nom d’utilisateur > l’accès Workfront sera supprimé de ce menu déroulant**, choisissez si vous souhaitez que leur accès soit supprimé uniquement de l’objet que vous avez sélectionné ou de tous les objets enfants qui y sont associés.

1. (Conditionnel) Pour les projets, les tâches et les problèmes, procédez comme suit :

   1. Cliquez sur **Partager** à droite du nom de l’objet.

      ![](assets/new-share-button.png)
   1. Recherchez l’utilisateur, le rôle, l’équipe, le groupe ou la société que vous souhaitez supprimer de l’objet.
   1. Cliquez sur **Supprimer**.
Dans le menu déroulant **Supprimer &lt; nom d’utilisateur > de**, choisissez si vous souhaitez que leur accès soit supprimé uniquement de l’objet que vous avez sélectionné ou de tous les objets enfants qui lui sont associés.

      ![](assets/remove-permissions-on-project-nwe-350x479.png)

   Les scénarios suivants sont possibles :

   * Si vous supprimez uniquement l’entité de l’objet, cette entité perd ses autorisations sur l’objet et ses autorisations héritées sur les objets enfants. S’ils disposaient auparavant d’autorisations individuelles pour les éléments enfants, ils conservent les mêmes autorisations sur tous les objets enfants qui leur sont associés lorsque vous sélectionnez cette option.
   * Si vous supprimez l’entité de l’objet et de tous les objets enfants, cette entité perd ses autorisations sur l’objet ainsi que sur tous les objets enfants, même lorsqu’elle a précédemment reçu une autorisation individuelle sur chaque objet enfant.

1. Cliquer sur **Enregistrer**.

## Supprimer des autorisations de plusieurs objets en bloc

Vous pouvez supprimer des entités (utilisateurs, rôles de tâche, équipes, groupes, entreprises) de plusieurs objets à la fois lorsque vous les sélectionnez en masse dans une liste.

>[!NOTE]
>
>Vous ne pouvez pas afficher les entités d’accès disponibles pour tous les objets sélectionnés lorsque vous les sélectionnez en bloc. Vous devez savoir quelle entité vous souhaitez supprimer du partage des objets sélectionnés avant de supprimer leurs autorisations.

1. Accédez à la liste des objets que vous souhaitez partager.

   Pour plus d’informations sur les objets qui peuvent être partagés, voir [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Sélectionnez plusieurs objets dans la liste, puis cliquez sur l’icône **Partager** ![](assets/share-icon.png) en haut de la liste.
1. Saisissez le nom de l’utilisateur, du rôle, de l’équipe, du groupe ou de la société pour lequel vous souhaitez supprimer l’accès dans le champ **Modifier l’accès à `<Object Name>` vers** .
1. Dans le menu déroulant d&#39;accès, sélectionnez **No Access**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. Dans le menu déroulant, l’accès Workfront de `<User Name>` sera supprimé de ce menu déroulant. Choisissez si vous souhaitez que leur accès soit supprimé uniquement des objets que vous avez sélectionnés ou de tous les autres objets enfants qui y sont associés.\
   Les scénarios suivants sont possibles :

   * Si vous supprimez uniquement l’entité de l’objet, cette entité perd ses autorisations sur l’objet et ses autorisations héritées sur les objets enfants. S’ils disposaient auparavant d’autorisations individuelles pour les éléments enfants, ils conservent les mêmes autorisations sur tous les objets enfants qui leur sont associés lorsque vous sélectionnez cette option. 
   * Si vous supprimez l’entité de l’objet et de tous les objets enfants, cette entité perd ses autorisations sur l’objet ainsi que sur tous les objets enfants, même lorsqu’elle a précédemment reçu une autorisation individuelle sur chaque objet enfant.

   **Exemple :** Choisissez de supprimer les autorisations pour les tâches sélectionnées dans une liste ou pour les problèmes et documents associés aux tâches.

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Facultatif) Pour modifier les autorisations en bloc pour plusieurs objets, sélectionnez un autre niveau de partage pour l’entité sélectionnée.

   Par exemple, s’ils disposent des autorisations Gérer, sélectionnez Contribute ou Afficher à la place.

1. Cliquer sur **Enregistrer**.

## Suppression des autorisations héritées

Les autorisations héritées peuvent être supprimées des objets permettant aux propriétaires d’identifier spécifiquement qui aura accès aux objets enfants, quel que soit l’accès d’un utilisateur à un objet parent.

>[!IMPORTANT]
>
>Seuls les utilisateurs disposant de l’autorisation Gérer peuvent supprimer les autorisations héritées.

Pour supprimer les autorisations héritées :

1. Accédez à un objet auquel vous disposez des autorisations de gestion. Par exemple, accédez à une tâche.
1. Accédez à la zone d’accès aux objets comme décrit dans la section [Supprimer les entités de la liste de partage d’un objet](#remove-entities-from-the-sharing-list-of-an-object) de cet article.
1. Sélectionnez le **x** en regard de **Autorisation héritée** dans la zone de partage pour supprimer toutes les personnes répertoriées là-bas.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   Cela garantit qu’aucune personne à qui des autorisations sont accordées à l’objet parent (par exemple, le projet) ne dispose par défaut d’autorisations sur cette tâche. Vous devez répertorier  entités individuelles dans la liste de partage de la tâche pour accorder des autorisations sur la tâche.

   >[!TIP]
   >
   >Vous ne pouvez pas supprimer des entités individuelles de la liste Autorisations héritées. Vous pouvez uniquement désactiver les autorisations héritées pour toutes les entités répertoriées.

1. Cliquez sur **Enregistrer**. 

## Rendre un objet privé

Si vous avez partagé un objet à l’échelle du système ou si vous l’avez partagé avec des utilisateurs externes en le rendant public, vous pouvez le rendre privé à nouveau en supprimant les autorisations à l’échelle du système ou publiques. 

Pour plus d’informations sur la mise à disposition d’un objet à l’échelle du système ou publiquement, voir [Partage d’un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Pour rendre un objet privé :

1. Accédez à l’objet que vous souhaitez rendre privé.\
   Par exemple, accédez à un rapport.
1. Cliquez sur **Actions de rapport**, puis sur **Partage**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. Cliquez sur **Supprimer l’accès public** pour supprimer l’accès des utilisateurs externes à l’affichage du rapport.
1. Cliquez sur **Supprimer l’accès à l’échelle du système** pour arrêter de le partager avec tous les utilisateurs de Workfront. 
1. Cliquer sur **Enregistrer**.
