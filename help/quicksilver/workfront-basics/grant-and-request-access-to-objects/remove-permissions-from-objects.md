---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: Supprimer les autorisations des objets
description: Vous pouvez supprimer les autorisations d’autres utilisateurs et utilisatrices sur les objets pour lequel vous disposez d’autorisations de partage. La suppression des autorisations des objets est identique pour tous les objets qui peuvent être partagés.
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 100%

---

# Supprimer les autorisations des objets

<!--Audited: 01/2024-->

Vous pouvez supprimer les autorisations d’autres utilisateurs et utilisatrices sur les objets pour lequel vous disposez d’autorisations de partage. La suppression des autorisations des objets est identique pour tous les objets qui peuvent être partagés.

Les mêmes remarques que pour le partage d’objets s’appliquent à la suppression des autorisations sur les objets. Pour plus d’informations, voir la section [Considérations sur le partage d’objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) dans l’article [Vue d’ensemble du partage des autorisations sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Conditions d’accès

Pour partager des objets, vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Workfront*</td> 
   <td> <p>Nouvelle licence : contribution ou niveau supérieur</p>
   Ou  
   <p>Licence actuelle : demande ou niveau supérieur</p>
   <p><b>NOTE</b></p>

<p>Certains objets nécessitent un accès plus élevé que le niveau de demande. </p>

<p>Par exemple, pour la nouvelle licence, un contributeur ou une contributrice peut partager des problèmes, mais seuls les utilisateurs et utilisatrices de la licence Standard peuvent partager un projet.</p>

<p>Pour la licence actuelle, une personne titulaire d’une licence de demande peut partager des problèmes, mais seules les personnes titulaires d’une licence de travail ou de plan peuvent partager un projet.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès Affichage ou supérieur aux objets que vous souhaitez partager.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations d’affichage ou supérieures pour les objets que vous souhaitez partager.</p> <p>Autorisations de gestion pour supprimer les autorisations héritées sur les objets</p>  </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Supprimer des entités de la liste de partage d’un objet {#remove-entities-from-the-sharing-list-of-an-object}

Vous pouvez supprimer des entités (utilisateurs et utilisatrices, fonctions, équipes, groupes, entreprises) de la liste de partage d’un objet. Cela supprime leurs autorisations sur l’objet.

1. Accédez à l’objet pour lequel vous souhaitez supprimer les autorisations.

   Pour plus d’informations sur les objets qui peuvent être partagés, voir [Vue d’ensemble des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Le cas échéant) Pour les programmes, les portfolios et les documents, procédez comme suit :

   1. Cliquez sur l’icône **Plus** ![](assets/more-icon.png) en regard du nom de l’objet, puis sur **Partage** ou sur **Partager**.

      ![](assets/share-a-document-350x160.png)

   1. Cliquez sur la croix (**x**) en regard du nom d’une personne, d’une équipe, d’un groupe, d’une entreprise ou d’une fonction pour supprimer l’élément de la zone d’accès à l’objet.

      ![](assets/remove-permissions-on-portfolio.png)

   1. Dans le menu déroulant **L’accès Workfront de &lt; Nom d’utilisateur ou d’utilisatrice > sera supprimé sur l’objet**, choisissez si vous souhaitez que leur accès soit supprimé uniquement pour l’objet que vous avez sélectionné ou pour tous les objets enfant qui lui sont associés.

1. (Le cas échéant) Pour les projets, les tâches et les problèmes, procédez comme suit :

   1. Cliquez sur **Partager** à droite du nom de l’objet.

      ![](assets/new-share-button.png)
   1. Recherchez la personne, le rôle, l’équipe, le groupe ou l’entreprise que vous souhaitez supprimer de l’objet.
   1. Cliquez sur **Supprimer**.
Dans le menu déroulant **Supprimer &lt; Nom d’utilisateur ou d’utilisatrice > de**, choisissez si vous souhaitez que son accès soit supprimé uniquement pour l’objet que vous avez sélectionné ou pour tous les objets enfant qui lui sont associés.

      ![](assets/remove-permissions-on-project-nwe-350x479.png)

   Les scénarios suivants sont possibles :

   * Si vous ne supprimez l’entité que de l’objet, cette entité perd ses autorisations sur l’objet, ainsi que les autorisations dont elle a hérité pour les objets enfants. Si elle a déjà obtenu des autorisations pour les éléments enfants individuellement, elle conserve les mêmes autorisations pour tous les objets enfants associés lorsque vous sélectionnez cette option.
   * Si vous supprimer l’entité de l’objet et de tous les objets enfants, cette entité perd ses autorisations sur l’objet ainsi que sur tous les objets enfants, même si elle avait auparavant obtenu des autorisations individuelles sur chaque objet enfant.

1. Cliquer sur **Enregistrer**.

## Supprimer les autorisations de plusieurs objets en masse

Vous pouvez supprimer des entités (personnes, fonctions, équipes, groupes, entreprises) de plusieurs objets à la fois lorsque vous les sélectionnez en masse dans une liste.

>[!NOTE]
>
>Il n’est pas possible de voir les accès dont disposent les entités pour tous les objets sélectionnés lorsque vous les sélectionnez en masse. Vous devez savoir quelle entité vous voulez supprimer du partage des objets sélectionnés avant de supprimer leurs autorisations.

1. Accédez à la liste des objets que vous souhaitez partager.

   Pour plus d’informations sur les objets qui peuvent être partagés, voir [Vue d’ensemble des autorisations de partage sur les objets](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Sélectionnez plusieurs objets dans la liste, puis cliquez sur l’icône **Partager** ![](assets/share-icon.png) en haut de la liste.
1. Saisissez le nom de la personne, du rôle, de l’équipe, du groupe ou de l’entreprise à qui vous souhaitez supprimer l’accès dans le champ **Modifier l’accès de `<Object Name>` à**.
1. Dans le menu déroulant de l’accès, sélectionnez **Pas d’accès**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. Si l’accès Workfront de `<User Name>` sera supprimé de ce menu déroulant, sélectionnez si vous souhaitez que son accès soit supprimé uniquement pour les objets que vous avez sélectionnés ou pour tous les autres objets enfants associés.\
   Les scénarios suivants sont possibles :

   * Si vous ne supprimez l’entité que de l’objet, cette entité perd ses autorisations sur l’objet, ainsi que les autorisations dont elle a hérité pour les objets enfants. Si elle a déjà obtenu des autorisations pour les éléments enfants individuellement, elle conserve les mêmes autorisations pour tous les objets enfants associés lorsque vous sélectionnez cette option. 
   * Si vous supprimer l’entité de l’objet et de tous les objets enfants, cette entité perd ses autorisations sur l’objet ainsi que sur tous les objets enfants, même si elle avait auparavant obtenu des autorisations individuelles sur chaque objet enfant.

   **Exemple :** choisissez de supprimer les autorisations juste pour les tâches sélectionnées dans une liste ou pour les problèmes et les documents attachés à ces tâches.

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Facultatif) Pour modifier les autorisations en bloc pour plusieurs objets, sélectionnez un autre niveau de partage pour l’entité sélectionnée.

   Par exemple, s’ils ont des autorisations de gestion, sélectionnez Contribuer ou Afficher à la place.

1. Cliquer sur **Enregistrer**.

## Supprimer des autorisations héritées

Les autorisations héritées peuvent être supprimées des objets. Cela permet ainsi aux personnes propriétaires d’identifier spécifiquement les personnes qui auront accès aux objets enfants, indépendamment de l’accès d’une personne à un objet parent.

>[!IMPORTANT]
>
>Seules les personnes disposant de l’autorisation de gestion peuvent supprimer les autorisations héritées.

Pour supprimer des autorisations héritées :

1. Accédez à un objet pour lequel vous avez des autorisations de gestion. Par exemple, rendez-vous sur une tâche.
1. Accédez à la zone d’accès de l’objet comme décrit dans la section [Supprimer des entités de la liste de partage d’un objet](#remove-entities-from-the-sharing-list-of-an-object) de cet article.
1. Sélectionnez le **x** à côté de **Autorisation héritée** dans la zone de partage pour supprimer les personnes qui y figurent.

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   Cela permet de s’assurer qu’aucune personne disposant des autorisations sur l’objet parent (par exemple, le projet) n’a de droits sur cette tâche par défaut. Vous devez répertorier les entités individuelles dans la liste de partage de la tâche pour accorder des autorisations sur la tâche.

   >[!TIP]
   >
   >Vous ne pouvez pas supprimer des entités individuelles de la liste des autorisations héritées. Vous ne pouvez désactiver les autorisations héritées que pour toutes les entités répertoriées.

1. Cliquez sur **Enregistrer**.

## Rendre un objet privé

Si vous avez partagé un objet à l’échelle du système ou si vous l’avez partagé avec des utilisateurs et utilisatrices externes en le rendant public, vous pouvez le rendre à nouveau privé en supprimant les autorisations à l’échelle du système ou les autorisations publiques. 

Pour plus d’informations sur la mise à disposition d’un objet à l’échelle du système ou publiquement, voir [Partager un objet](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Pour rendre un objet privé :

1. Accédez à l’objet que vous souhaitez rendre privé.\
   Par exemple, rendez-vous sur un rapport.
1. Cliquez sur **Actions de rapport**, puis sur **Partage**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. Cliquez sur **Supprimer l’accès public** pour supprimer l’accès des utilisateurs et utilisatrices externes à l’affichage du rapport.
1. Cliquez sur **Supprimer l’accès à l’échelle du système** pour ne plus le partager avec l’ensemble des utilisateurs et utilisatrices de Workfront.
1. Cliquer sur **Enregistrer**.
