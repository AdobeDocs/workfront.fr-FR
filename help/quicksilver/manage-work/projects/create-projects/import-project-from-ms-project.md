---
product-area: projects
navigation-topic: create-projects
title: Importer un projet depuis Microsoft Project
description: Vous pouvez importer des projets de Microsoft Project dans Adobe Workfront et gérer tous vos projets dans une seule application. Chaque fois que vous importez un projet à partir d’un projet Microsoft, un nouveau projet est créé dans Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: 49bd393af77a67aa1e3a443c4189569178e99ada
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 16%

---

# Importer un projet depuis Microsoft Project

Vous pouvez importer des projets de Microsoft Project dans Adobe Workfront et gérer tous vos projets dans une seule application. Chaque fois que vous importez un projet à partir d’un projet Microsoft, un nouveau projet est créé dans Workfront.

>[!IMPORTANT]
>
>Tous les champs de projet Microsoft ne sont pas transférés vers Workfront.
>
>Pour plus d’informations sur la compatibilité des champs entre Workfront et Microsoft Project, voir [Mappage des champs du projet Microsoft aux projets Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouvelle licence : standard </p> 
   Ou
   <p>Licence actuelle : formule </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Modifier l’accès aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Lorsque vous créez un projet, vous recevez automatiquement les autorisations de gestion du projet. </p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--old permissions model: 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Création d’un projet à partir d’un projet MS

Vous pouvez créer un projet à partir de la zone Projets du menu principal ou de la zone Projets d’un portfolio ou d’un programme.

1. Accédez à Projet Microsoft et ouvrez un projet à partir duquel vous souhaitez importer des données dans Workfront.
1. Cliquez sur **Fichier**, puis sur **Enregistrer sous** pour enregistrer le projet sous la forme d’un fichier .xml.

1. Connectez-vous à Workfront.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur le **menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront ou cliquez sur le **menu principal** ![](assets/lines-main-menu.png) dans le coin supérieur gauche, le cas échéant, cliquez sur **Projets**, puis développez **Nouveau projet**.
   * Accédez à un portfolio, puis développez **Nouveau projet**.
   * Accédez à un programme, puis développez **Nouveau projet**.
   * Si vous êtes administrateur ou administratrice de groupes, vous pouvez également créer un projet dans la section Projets d’un groupe que vous gérez. Pour plus d’informations, voir [Créer et modifier des projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Choisissez l&#39;option **Importer un projet MS** .

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. Cliquez sur **Sélectionner un fichier**, puis recherchez le fichier .xml sur l’ordinateur que vous avez exporté à partir du projet Microsoft.
1. Importez le fichier sélectionné.

   Workfront lance le processus d’importation et crée un projet basé sur le fichier exporté à partir du projet Microsoft.

   Une fois le processus d’importation terminé, vous êtes dirigé vers la nouvelle page du projet qui affiche la confirmation que l’importation s’est correctement terminée.

   >[!NOTE]
   >
   >Workfront est limité à 15 minutes pour les téléchargements de fichiers. Si le téléchargement de fichier prend plus de temps, nous vous recommandons de diviser votre projet en projets plus petits et de les importer séparément. Une fois qu’ils ont été importés dans Workfront, déplacez les tâches d’un projet vers l’autre projet pour les combiner dans un seul projet. Pour plus d’informations sur le déplacement des tâches, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Facultatif) Continuez à modifier le projet dans Workfront. Pour plus d’informations sur la modification de projets, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

   L’état d’un nouveau projet créé à partir d’un modèle correspond à l’état défini par votre administrateur Workfront dans la zone Préférences du projet ou par un administrateur de groupe dans la zone Préférences du projet de groupe . Pour plus d’informations sur la configuration des préférences de projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
