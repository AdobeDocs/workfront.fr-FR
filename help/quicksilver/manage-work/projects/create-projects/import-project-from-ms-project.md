---
product-area: projects
navigation-topic: create-projects
title: Importer un projet à partir de Microsoft Project
description: Vous pouvez importer des projets de Microsoft Project dans Adobe Workfront et gérer tous vos projets dans une seule application. Chaque fois que vous importez un projet depuis Microsoft Project, un nouveau projet est créé dans Workfront.
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: b38c98ec79617a78c76510bcb109da2ff83247af
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 67%

---

# Importer un projet à partir de Microsoft Project

<!-- Audited: 4/2025 -->

Vous pouvez importer des projets de Microsoft Project dans Adobe Workfront et gérer tous vos projets dans une seule application. Chaque fois que vous importez un projet depuis Microsoft Project, un nouveau projet est créé dans Workfront.

>[!IMPORTANT]
>
>Tous les champs de Microsoft Project ne sont pas transférés dans Workfront.
>
>Pour plus d’informations sur la compatibilité des champs entre Workfront et Microsoft Project, voir [Mapper des champs Microsoft Project à des projets Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau : Standard </p> 
   Ou
   <p>Actuelle : formule </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Accès en modification aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Lorsque vous créez un projet, vous recevez automatiquement les droits de gestion du projet. </p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

## Créer un projet à partir d’un projet MS

Vous pouvez créer un projet à partir de la zone **Projets** du **Menu principal** ou à partir de la zone **Projets** d’un portefeuille ou d’un programme.

1. Connectez-vous au projet Microsoft et ouvrez un projet à partir duquel vous souhaitez effectuer un import dans Workfront.
1. Cliquez sur **Fichier**, puis sur **Enregistrer sous** pour enregistrer le projet en tant que fichier .xml.

1. Connectez-vous à Workfront.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur l’icône **Menu principal** ![Icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, ou cliquez sur les **Menu principal** ![Lignes du menu principal](assets/lines-main-menu.png) dans le coin supérieur gauche, si disponible, cliquez sur **Projets**, puis développez **Nouveau projet**.
   * Accédez à un portfolio, puis développez **Nouveau projet**.
   * Accédez à un programme, puis développez **Nouveau projet**.
   * Si vous êtes un administrateur de groupes, vous pouvez créer un projet dans la section **Projets** d’un groupe que vous gérez. Pour plus d’informations, voir [Créer et modifier les projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. Cliquez sur **Importer MS Project**. La boîte de dialogue **Importer un fichier MS** s&#39;affiche.

   ![Liste déroulante du nouveau projet](assets/import-ms-project-option.png)

1. Cliquez sur **Sélectionner un fichier**, puis recherchez le fichier .xml sur votre ordinateur que vous avez exporté à partir du projet Microsoft.
1. Importer le fichier sélectionné. Workfront commence le processus d’import et crée un nouveau projet basé sur le fichier exporté de Microsoft Project.

   Une fois le processus d’import terminé, vous faites l’objet d’une redirection vers la page du nouveau projet qui affiche une confirmation que l’import s’est déroulé avec succès.

   >[!NOTE]
   >
   >Workfront a une limite de temps de 15 minutes pour les chargements de fichiers. Si le chargement du fichier prend plus de temps, nous vous recommandons de diviser votre projet en plusieurs projets plus petits et de les importer séparément. Une fois qu’elles ont été importées dans Workfront, déplacez les tâches d’un projet à l’autre pour les combiner en un seul projet. Pour plus d’informations sur le déplacement des tâches, voir [Déplacer des tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. (Facultatif) Continuez à modifier le projet dans Workfront. Pour plus d’informations sur la modification des projets, voir [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).


   >[!NOTE]
   >
   >Le statut d’un nouveau projet créé à partir d’un modèle correspond au statut défini par l’administrateur de Workfront dans la zone **Préférences du projet** ou par un administrateur de groupes dans la zone **Préférences du projet du groupe**. Pour plus d’informations sur la configuration des préférences de projet, voir [Configurer les préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
