---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Suppression des autorisations des objets
description: Vous pouvez supprimer les autorisations d’autres utilisateurs sur les objets que vous avez accès à Partager. La suppression des autorisations des objets est identique pour tous les objets qui peuvent être partagés.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 1%

---

# Suppression des autorisations des objets

Vous pouvez supprimer les autorisations d’autres utilisateurs sur les objets que vous avez accès à Partager. La suppression des autorisations des objets est identique pour tous les objets qui peuvent être partagés. 

Les mêmes considérations que pour le partage d’objets s’appliquent pour supprimer des autorisations d’objets. Pour plus d’informations, voir la section [Observations relatives au partage d’objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) dans l’article [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## Exigences d’accès

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or  
   <p>Legacy license: Request or higher</p>
   <p><b>NOTE</b></p>

   <p>Some objects require a higher access than Request. </p>
   
   <p>For example, for the current license, a Contributor can share issues, but only Standard-license users can share a project.</p>
   
   <p>For the legacy license, a Requestor can share issues, but only Workers or Planners can share a project.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you want to share</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p> <p>Manage permissions to remove inherited permissions on objects</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Pour partager des objets, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Workfront*</td> 
   <td> <p>Requête ou supérieure</p>
   <p><b>NOTE</b></p>

Certains objets nécessitent un accès supérieur à Demander. Par exemple, un demandeur peut partager des problèmes, mais seuls les travailleurs ou les planificateurs peuvent partager un projet.

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Afficher l’accès ou une version ultérieure aux objets que vous souhaitez partager</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher les autorisations ou plus pour les objets que vous souhaitez partager</p> <p>Gestion des autorisations pour supprimer les autorisations héritées sur les objets</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Supprimer des entités de la liste de partage d’un objet {#remove-entities-from-the-sharing-list-of-an-object}

Vous pouvez supprimer des entités (utilisateurs, rôles de tâche, équipes, groupes, entreprises) de la liste de partage d’un objet. Cela supprime leurs autorisations sur l’objet .

1. Accédez à l’objet que vous souhaitez partager.

   Pour plus d’informations sur les objets qui peuvent être partagés, voir [Présentation des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Cliquez sur le bouton **Plus** icon ![](assets/more-icon.png)en regard du nom de l’objet, puis cliquez sur **Partage** ou **Partagez.**

   ![](assets/share-a-document-350x160.png)

1. Cliquez sur le bouton **x** en regard du nom d’un utilisateur, d’une équipe, d’un groupe, d’une société, d’un rôle de tâche pour le supprimer dans la zone d’accès aux objets.

   ![](assets/remove-permissions-on-project-nwe-350x479.png)

1. Dans le `<User Name>`L’accès Workfront de sera supprimé de ce menu déroulant. Indiquez si vous souhaitez que leur accès soit supprimé uniquement de l’objet que vous avez sélectionné ou de tous les objets enfants qui lui sont associés.\
   Les scénarios suivants existent :

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

1. Sélectionnez plusieurs objets dans la liste, puis cliquez sur le bouton **Partager** icon ![](assets/share-icon.png)en haut de la liste.
1. Saisissez le nom de l’utilisateur, du rôle, de l’équipe, du groupe ou de la société pour lequel vous souhaitez supprimer l’accès dans la variable **Modifier `<Object Name>` accès à** champ .
1. Dans le menu déroulant d’accès, sélectionnez **Accès interdit**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. Dans le `<User Name>`L’accès Workfront de sera supprimé de ce menu déroulant. Indiquez si vous souhaitez que leur accès soit supprimé uniquement des objets que vous avez sélectionnés ou de tous les autres objets enfants qui lui sont associés.\
   Les scénarios suivants existent :

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
1. Accédez à la zone d’accès aux objets comme décrit dans la section [Supprimer des entités de la liste de partage d’un objet](#remove-entities-from-the-sharing-list-of-an-object) dans cet article.
1. Sélectionnez la **x** en regard de **Autorisation héritée** dans la boîte de partage pour supprimer tous ceux qui y sont répertoriés.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   Cela garantit qu’aucune personne à qui des autorisations sont accordées à l’objet parent (par exemple, le projet) ne dispose par défaut d’autorisations sur cette tâche. Vous devez répertorier les entités individuelles dans la liste de partage de la tâche pour accorder des autorisations sur la tâche.

   >[!TIP]
   >
   >Vous ne pouvez pas supprimer des entités individuelles de la liste Autorisations héritées. Vous pouvez uniquement désactiver les autorisations héritées pour toutes les entités répertoriées.

1. Cliquer sur **Enregistrer**. 

## Rendre un objet privé

Si vous avez partagé un objet à l’échelle du système ou si vous l’avez partagé avec des utilisateurs externes en le rendant public, vous pouvez le rendre privé à nouveau en supprimant les autorisations à l’échelle du système ou publiques. 

Pour plus d’informations sur la mise à disposition d’un objet à l’échelle du système ou publiquement, voir [Partage d’un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Pour rendre un objet privé :

1. Accédez à l’objet que vous souhaitez rendre privé.\
   Par exemple, accédez à un rapport.
1. Cliquez sur **Actions de rapport**, puis **Partage**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. Cliquez sur **Suppression de l’accès public** pour supprimer l’accès des utilisateurs externes à l’affichage du rapport.
1. Cliquez sur **Suppression de l’accès à l’échelle du système** pour arrêter de le partager avec tous les utilisateurs de Workfront. 
1. Cliquer sur **Enregistrer**.
