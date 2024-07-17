---
product-area: projects
navigation-topic: plan-a-project
title: Mettre à jour les personnes propriétaires et sponsors des projets
description: Lorsque vous créez un projet dans Adobe Workfront, vous êtes automatiquement défini comme propriétaire du projet. Vous pouvez mettre à jour ce champ avec un autre utilisateur. Vous pouvez également mettre à jour le champ Sponsor de projet d’un projet.
author: Alina
feature: Work Management
exl-id: 10421cab-237a-49a5-bb5b-5be510dc4c46
source-git-commit: 49bd393af77a67aa1e3a443c4189569178e99ada
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 13%

---


# Mettre à jour les personnes propriétaires et sponsors des projets

<!--Audited: 07/2024-->

Lorsque vous créez un projet dans Adobe Workfront, vous êtes automatiquement défini comme propriétaire du projet. Vous pouvez mettre à jour ce champ avec un autre utilisateur. Vous pouvez également mettre à jour le champ Sponsor de projet d’un projet.

Pour plus d’informations sur les propriétaires et les sponsors de projets, voir [Présentation des propriétaires et des sponsors de projets](../../../manage-work/projects/planning-a-project/project-owners-and-sponsors.md).

>[!TIP]
>
>Vous pouvez identifier un propriétaire et un sponsor pour un modèle. Lorsque vous créez un projet à partir de ce modèle, le propriétaire du modèle devient le propriétaire du projet et le parrain du modèle devient le parrain du projet.
>
>Si le modèle ne comporte pas de propriétaire, l’utilisateur qui crée le projet à partir du modèle devient le propriétaire du projet.
>
>Pour plus d’informations sur la modification de modèles, voir [Modifier des modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Conditions d’accès

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td><p>Nouvelle : standard</p> 
   <p>Actuelle : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Modification des autorisations d’un projet</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mise à jour du propriétaire d’un projet

Lorsque vous ajoutez un utilisateur en tant que propriétaire de projet, Workfront lui accorde automatiquement des autorisations pour afficher le projet.

1. Accédez au projet que vous souhaitez mettre à jour.
1. Cliquez sur **Détails du projet** dans le panneau de gauche.
1. Cliquez sur l’icône **Modifier** ![](assets/qs-edit-icon.png) dans le coin supérieur droit de la zone Détails du projet, puis cliquez sur **Aperçu**.

1. Indiquez le nom d’un utilisateur pour le champ **Propriétaire du projet**.

   Seuls les utilisateurs actifs peuvent être spécifiés en tant que propriétaires de projet.

1. Cliquez sur **Enregistrer les modifications**.

   Le propriétaire du projet se met à jour dans l’en-tête du projet et dans la zone Détails du projet.

   ![](assets/project-stakeholders-owner-highlighted-nwe-350x149.png)

## Mise à jour du parrain d’un projet

Lorsque vous ajoutez un utilisateur en tant que responsable de projet d’un projet, Workfront lui accorde automatiquement des autorisations d’affichage du projet.

>[!TIP]
>
>Si l’utilisateur que vous ajoutez en tant que responsable de projet est un administrateur système, il n’est pas ajouté à la liste de partage du projet.

1. Accédez au projet que vous souhaitez mettre à jour.
1. Cliquez sur **Détails du projet** dans le panneau de gauche.
1. Cliquez sur l’icône **Modifier** ![](assets/qs-edit-icon.png) dans le coin supérieur droit de la zone Détails du projet, puis cliquez sur **Aperçu**.

1. Indiquez le nom d’un utilisateur pour le champ **Project Sponsor**.

   Seuls les utilisateurs actifs peuvent être spécifiés en tant que parrains de projet.

1. Cliquez sur **Enregistrer les modifications**.

   Le parrain du projet est mis à jour dans la zone Détails du projet.

   ![](assets/project-stakeholders-sponsor-highlighted-nwe-350x147.png)
