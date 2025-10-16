---
product-area: projects
navigation-topic: update-work-in-a-project
title: Appliquer des statuts au travail associé à un groupe
description: Si un projet est lié à un groupe, vous pouvez appliquer les statuts au niveau du système, ainsi qu’un statut personnalisé lié à ce groupe, au projet, à la tâche ou aux problèmes de ce projet.
author: Alina
feature: Work Management
exl-id: 7564ab6a-8ddf-4e76-8e45-d59f9cf8d38b
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 90%

---

# Appliquer des statuts à un travail associé à un groupe

<!--
Alina, I moved this out of an admin article about statuses (Create and customize statuses)
-->

Si un projet est lié à un groupe, vous pouvez appliquer les statuts au niveau du système, ainsi qu’un statut personnalisé lié à ce groupe, au projet ou aux tâches et problèmes de ce projet. Pour plus d’informations sur les statuts d’un groupe dans Adobe Workfront, consultez la section [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

>[!TIP]
>
>Vous ne pouvez associer que des projets à des groupes. Les problèmes et les tâches héritent le groupe du projet auquel ils appartiennent.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations de gestion pour le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
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
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Mettre à jour le groupe du projet et le statut

Quand vous mettez à jour le groupe d’un projet, les choix pour les statuts des tâches, des problèmes ou du projet s’adaptent pour correspondre au groupe.

1. Accédez à un projet ou créez-en un, comme décrit dans la section [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).
1. Cliquez sur l’icône **Plus** ![Icône Plus](assets/more-icon.png), puis sur **Modifier**.

1. Dans la zone **Modifier le projet** qui s’affiche, près du bas de la section **Vue d’ensemble**, sélectionnez le groupe dans le menu déroulant **Groupe**.

1. Dans le menu déroulant **Statut**, sélectionnez le statut personnalisé.

   >[!NOTE]
   >
   >Si vous sélectionnez un autre groupe dans le menu déroulant **Groupe**, les statuts personnalisés dans le menu **Statut** changent automatiquement pour établir une corrélation avec le nouveau groupe.
   >
   >
   >![Liste déroulante Statut développée avec des statuts personnalisés pour le projet](assets/status-drop-down-expanded-with-custom-statuses-for-project-nwe.png)
   >

1. Sélectionnez le statut du projet. Les statuts personnalisés que vous avez créés et appliqués à ce groupe s’affichent dans la liste.
