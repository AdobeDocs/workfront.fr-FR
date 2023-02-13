---
product-area: templates
navigation-topic: templates-navigation-topic
title: Partage de modèles de projet
description: Vous pouvez partager un modèle avec des utilisateurs ou définir comment les projets créés à partir d’un modèle seront partagés avec les utilisateurs à l’aide des options de partage suivantes au niveau du modèle.
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 2%

---

# Partage de modèles de projet

Vous pouvez partager un modèle avec des utilisateurs ou définir comment les projets créés à partir d’un modèle seront partagés avec les utilisateurs à l’aide des options de partage suivantes au niveau du modèle.

Lors du partage d’un objet dans Adobe Workfront, vous autorisez d’autres utilisateurs à afficher, contribuer ou modifier cet objet.

Pour plus d’informations sur les autorisations Workfront, voir [Présentation des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Pour plus d’informations sur les autorisations que vous pouvez donner aux utilisateurs lors du partage d’un modèle, voir [Partage d’un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

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
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux modèles</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un modèle</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Partage d’un modèle {#share-a-template}

Vous pouvez partager vos modèles avec d’autres utilisateurs à l’aide du partage de modèles. Cette action définit qui possède les autorisations pour le modèle.

>[!NOTE]
>
>Lorsque vous désigner un utilisateur principal comme propriétaire de modèle, cet utilisateur reçoit automatiquement les autorisations de gestion sur le modèle. Pour plus d’informations sur la désignation d’une personne comme propriétaire de modèle, voir [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Pour partager un modèle :

1. Dans la **Menu Principal** icon ![](assets/main-menu-icon.png), cliquez sur **Modèles**.

1. Utilisez l’une des méthodes suivantes :\
   Cliquez sur le nom d’un modèle pour l’ouvrir, puis cliquez sur le bouton **Plus** menu ![](assets/qs-more-icon-on-an-object.png), puis **Partage de modèles**.

   Ou

   Sélectionnez un modèle dans la liste, puis cliquez sur l’icône Partager ![](assets/share-icon.png), puis cliquez sur **Modèle.**

   >[!TIP]
   >
   >Vous pouvez partager un objet uniquement avec des utilisateurs, équipes, rôles ou entreprises principaux.

1. Dans le **Accès aux modèles** , sélectionnez les personnes, équipes, rôles, groupes ou entreprises avec lesquels vous souhaitez partager le modèle.

   Vous pouvez également cliquer sur le bouton **Options** pour rendre le modèle disponible à l’échelle du système :

1. Dans le menu déroulant de chaque entité avec laquelle vous partagez votre projet, sélectionnez l’une des options suivantes :

   * **Affichage**: Les utilisateurs disposant de ces autorisations peuvent afficher le modèle et créer un projet à l’aide de celui-ci ou le joindre à un projet existant.

      >[!TIP]
      >
      >Pour pouvoir créer des projets, votre administrateur Workfront doit vous donner l’accès à l’option Modifier .

   * **Gérer**: Les utilisateurs disposant de ces autorisations peuvent modifier ou supprimer le modèle.

      Pour plus d’informations sur les paramètres avancés ![](assets/gear-icon-in-access-levels.png) disponibles ici, voir la section [Paramètres avancés pour le partage de modèles](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) dans l’article [Partage d’un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. Cliquer sur **Enregistrer**.

## Partage d’un projet à partir d’un modèle {#share-a-project-from-a-template}

Avec le modèle Partage de projets, vous pouvez définir qui dispose des autorisations sur les projets créés à partir du modèle au niveau du modèle.

Pour partager avec des utilisateurs les projets créés à partir d’un modèle :

1. Utilisez l’une des méthodes suivantes :\
   Cliquez sur le nom d’un modèle pour l’ouvrir, puis cliquez sur le bouton **Plus** menu ![](assets/qs-more-icon-on-an-object.png), puis **Partage de modèles**.

   ![Partage d’un projet à partir d’un modèle](assets/project-sharing-on-template-nwe-2022-350x172.png)

   Ou

   Sélectionnez un modèle dans la liste, puis cliquez sur **Partager**, puis cliquez sur **Projet.**

1. Dans le **Accès au projet** , sélectionnez les personnes, équipes, rôles, groupes ou entreprises avec lesquels le modèle est partagé.

   >[!TIP]
   >
   >Vous pouvez partager un objet uniquement avec des utilisateurs, équipes, rôles ou entreprises principaux.

1. Dans le menu déroulant de chaque entité, sélectionnez l’une des options suivantes :

   * **Accès interdit**: Vous pouvez spécifier les utilisateurs qui n’auront pas accès au modèle.\
      Cette option est disponible uniquement lors du partage en masse de projets à partir de modèles. 
   * **Affichage**: Les utilisateurs disposant de ces autorisations peuvent afficher les projets créés à partir du modèle.
   * **Contribution**: Les utilisateurs disposant de ces autorisations peuvent contribuer aux projets créés à partir du modèle. 
   * **Gérer**: Les utilisateurs disposant de ces autorisations peuvent gérer ou supprimer des projets créés à partir de ce modèle.

1. (Facultatif) Cliquez sur le **Options** pour rendre les projets disponibles à l’échelle du système.
1. Cliquer sur **Enregistrer**.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Overview of project sharing from other sources</h3>
<p>You may already have been assigned access to projects from other areas of Workfront. <br>You may have been assigned access to projects from the following areas: </p>
<ul>
<li>When a project is created<br>For more information about sharing projects when the project is created, see the "Access" section in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li>When your Workfront administrator sets user access levels<br>For more information about setting access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>
<li>When using the project access template</li>
</ul>
<p>When using the Template Project Sharing feature, if a user's access to a project is View, but you set the access permissions for Template Project Sharing to Manage, the user will have Manage permission for every project created using this specific template. The user will only have View permission for the other projects they are on.</p>
</div>
-->

## Partage en masse de modèles et de projets à partir de modèles

Vous pouvez partager simultanément plusieurs modèles et projets à partir de plusieurs modèles.

>[!NOTE]
>
>Lorsque vous sélectionnez plusieurs modèles, vous ne pouvez pas savoir qui dispose déjà d’autorisations sur les modèles individuels.

1. Accédez à une liste de modèles.
1. Sélectionnez plusieurs modèles, puis cliquez sur ![Partager](assets/share-icon.png).

   ![Partage de modèles ou de projets en masse](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >Vous pouvez partager un objet uniquement avec des utilisateurs, équipes, rôles ou entreprises principaux.

1. Cliquez sur **Modèle** pour partager les modèles sélectionnés.

   Ou

   Cliquez sur **Projet** pour partager les projets qui seront créés à partir des modèles sélectionnés.

1. Continuez à partager les modèles ou les projets, comme décrit dans les sections suivantes de cet article :

   * [Partage d’un modèle](#share-a-template)
   * [Partage d’un projet à partir d’un modèle](#share-a-project-from-a-template)
