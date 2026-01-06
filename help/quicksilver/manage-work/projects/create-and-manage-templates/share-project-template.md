---
product-area: templates
navigation-topic: templates-navigation-topic
title: Partager des modèles de projet
description: Vous pouvez partager un modèle avec des personnes ou définir comment les projets créés à partir d’un modèle seront partagés avec les personnes à l’aide des options de partage suivantes au niveau du modèle.
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 87%

---

# Partager des modèles de projet

Vous pouvez partager un modèle avec des personnes ou définir comment les projets créés à partir d’un modèle seront partagés avec les personnes à l’aide des options de partage suivantes au niveau du modèle.

Lors du partage d’un objet dans Adobe Workfront, vous autorisez d’autres personnes à afficher, contribuer ou modifier cet objet.

Pour plus d’informations sur les autorisations Workfront, voir [Vue d’ensemble des autorisations de partage sur les objets](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Pour plus d’informations sur les autorisations que vous pouvez donner aux personnes lors du partage d’un modèle, voir [Partager un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux modèles</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un modèle</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Partager un modèle {#share-a-template}

Vous pouvez partager vos modèles avec d’autres personnes à l’aide du partage de modèles. Cette action définit qui possède les autorisations pour le modèle.

>[!NOTE]
>
>Lorsque vous désigner une personne active comme propriétaire de modèle, cette personne reçoit automatiquement les autorisations de gestion sur le modèle. Pour plus d’informations sur la désignation d’une personne comme propriétaire de modèle, voir [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Pour partager un modèle :

{{step1-to-templates}}

1. Utilisez l’une des méthodes suivantes :\
   Cliquez sur le nom d’un modèle pour l’ouvrir, puis cliquez sur le menu **Plus** ![Icône Plus](assets/more-icon.png), puis sur **Partage de modèles**.

   Ou

   Sélectionnez un modèle dans la liste, cliquez sur l&#39;icône Partager ![Partager le modèle](assets/share-icon.png), puis sur **Modèle.**

   >[!TIP]
   >
   >Vous pouvez partager un objet uniquement avec des utilisateurs et utilisatrices, des équipes, des rôles ou des entreprises actifs.

1. Dans la boîte **Accès aux modèles**, sélectionnez les personnes, équipes, rôles, groupes ou entreprises avec lesquels vous souhaitez partager le modèle.

   Vous pouvez également cliquer sur l’icône **Options** pour rendre le modèle disponible à l’échelle du système :

1. Dans le menu déroulant de chaque entité avec laquelle vous partagez votre projet, sélectionnez l’une des options suivantes :

   * **Affichage** : les personnes disposant de ces autorisations peuvent afficher le modèle et créer un projet à l’aide de ce modèle ou le joindre à un projet existant.

     >[!TIP]
     >
     >Pour pouvoir créer des projets, votre administrateur ou administratrice Workfront doit vous donner l’accès à l’option Modifier.

   * **Gestion** : les personnes disposant de ces autorisations peuvent modifier ou supprimer le modèle.

     Pour plus d’informations sur les paramètres avancés ![icône d’engrenage](assets/gear-icon-in-access-levels.png) disponibles ici, consultez la section [Paramètres avancés du partage de modèles](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) dans l’article [Partage d’un modèle](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. Cliquer sur **Enregistrer**.

## Créer un projet à partir d’un modèle {#share-a-project-from-a-template}

Avec le partage de projets à partir d’un modèle, vous pouvez définir qui dispose des autorisations sur les projets créés à partir du modèle au niveau du modèle.

Pour partager les projets créés à partir d’un modèle avec des personnes :

1. Utilisez l’une des méthodes suivantes :\
   Cliquez sur le nom d’un modèle pour l’ouvrir, puis cliquez sur le menu **Plus** ![Icône Plus](assets/more-icon.png), puis sur **Partage de modèles**.

   ![Partager un projet à partir d’un modèle](assets/project-sharing-on-template-nwe-2022-350x172.png)

   Ou

   Sélectionnez un modèle dans la liste, cliquez sur **Partager**, puis cliquez sur **Projet.**

1. Dans la boîte **Accès au projet**, sélectionnez les personnes, équipes, rôles, groupes ou entreprises avec lesquels le modèle est partagé.

   >[!TIP]
   >
   >Vous pouvez partager un objet uniquement avec des utilisateurs et utilisatrices, des équipes, des rôles ou des entreprises actifs.

1. Dans le menu déroulant de chaque entité, sélectionnez l’une des options suivantes :

   * **Pas d’accès** : vous pouvez spécifier les utilisateurs et utilisatrices qui n’auront aucun accès au modèle.\
     Cette option est disponible uniquement lors du partage en masse de projets à partir de modèles.
   * **Afficher** : les utilisateurs disposant de ces autorisations peuvent afficher les projets créés à partir du modèle.
   * **Contribuer** : les utilisateurs disposant de ces autorisations peuvent contribuer aux projets créés à partir du modèle
   * **Gérer** : les utilisateurs disposant de ces autorisations peuvent gérer ou supprimer des projets créés à partir de ce modèle.

1. (Facultatif) Cliquez sur l’icône **Options** pour rendre les projets disponibles à l’échelle du système.
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

## Partager en masse des modèles et des projets à partir de modèles

Vous pouvez partager simultanément plusieurs modèles et des projets à partir de plusieurs modèles.

>[!NOTE]
>
>Lorsque vous sélectionnez plusieurs modèles, vous ne pouvez pas savoir qui dispose déjà d’autorisations sur les modèles individuels.

1. Accédez à une liste de modèles.
1. Sélectionnez plusieurs modèles, puis cliquez sur ![Partager](assets/share-icon.png).

   ![Partage de modèles ou de projets en masse](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >Vous pouvez partager un objet uniquement avec des utilisateurs et utilisatrices, des équipes, des rôles ou des entreprises actifs.

1. Cliquez sur **Modèle** pour partager les modèles sélectionnés.

   Ou

   Cliquez sur **Projet** pour partager les projets qui seront créés à partir des modèles sélectionnés.

1. Continuez à partager les modèles ou les projets, comme décrit dans les sections suivantes de cet article :

   * [Partager un modèle](#share-a-template)
   * [Créer un projet à partir d’un modèle](#share-a-project-from-a-template)
