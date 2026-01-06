---
product-area: templates
navigation-topic: templates-navigation-topic
title: Supprimer les informations sur les modèles d’un projet
description: Vous ne pouvez pas supprimer un modèle d’un projet. Vous ne pouvez supprimer manuellement que les informations qui ont été ajoutées au projet après qu’un modèle a été joint au projet. Pour plus d’informations sur la façon de joindre des modèles, voir Joindre un modèle à un projet.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 93%

---

# Supprimer les informations sur les modèles d’un projet

Vous ne pouvez pas supprimer un modèle d’un projet. Vous ne pouvez supprimer manuellement que les informations qui ont été ajoutées au projet après qu’un modèle a été joint au projet. Pour plus d’informations sur la façon de joindre des modèles, voir [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

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
   <p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux tâches</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès en gestion aux tâches </p> <p>Accès en contribution ou supérieur au projet</p>  </td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to tasks </p> <p>Contribute or higher access to the project </p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Options pour supprimer les informations sur les modèles d’un projet

Pour supprimer les informations sur les modèles qui ont été ajoutées au projet, vous pouvez procéder de l’une des manières suivantes :

* Supprimez manuellement des informations du projet après que le modèle a été joint.

  Pour plus d’informations, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

* Supprimez les tâches du projet qui ont été ajoutées avec le modèle.

  Pour plus d’nformations, voir la section [Supprimer les tâches créées à partir d’un modèle](#delete-tasks-created-from-a-template) de cet article.

* Supprimez le modèle de Workfront. La suppression du modèle dans Workfront ne supprime pas les tâches ajoutées à partir du modèle dans les projets.

  Pour plus d’informations, voir [Supprimer des modèles de projet](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Supprimer les tâches créées à partir d’un modèle {#delete-tasks-created-from-a-template}

1. Accédez à la section **Tâches** du projet.
1. Utilisez l’une des méthodes suivantes :

   * Créez un filtre pour la liste des tâches afin d’afficher uniquement les tâches créées à partir d’un modèle à l’aide de l’instruction suivante :

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     Pour plus d’informations sur la création d’un filtre, voir [Créer ou modifier des filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

     Lorsque vous appliquez le filtre, seules les tâches associées à un ID de tâche de modèle s’affichent dans la liste.

   * Créez une vue pour la liste des tâches afin d’afficher les champs **ID de tâche de modèle** ou **Nom de tâche de modèle** dans une colonne.

     Lorsque vous appliquez la vue, les tâches qui contiennent des informations dans la colonne ID de tâche de modèle ou Nom de tâche de modèle ont été créées à l’aide d’un modèle.

     Pour plus d’informations sur la création d’une vue, voir [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Sélectionnez toutes les tâches identifiées à l’étape 2 comme étant créées à partir d’un modèle, puis cliquez sur **l’icône Supprimer**&#x200B;**> Oui, supprimer**. Pour plus d’informations, voir [Supprimer des tâches](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
