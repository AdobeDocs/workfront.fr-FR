---
product-area: templates
navigation-topic: templates-navigation-topic
title: Supprimer les informations sur les modèles d’un projet
description: Vous ne pouvez pas supprimer un modèle d’un projet. Vous ne pouvez supprimer manuellement que les informations qui ont été ajoutées au projet après qu’un modèle a été joint au projet. Pour plus d’informations sur la façon de joindre des modèles, voir Joindre un modèle à un projet.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 100%

---

# Supprimer les informations sur les modèles d’un projet

Vous ne pouvez pas supprimer un modèle d’un projet. Vous ne pouvez supprimer manuellement que les informations qui ont été ajoutées au projet après qu’un modèle a été joint au projet. Pour plus d’informations sur la façon de joindre des modèles, voir [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux tâches</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès en gestion aux tâches </p> <p>Accès en contribution ou supérieur au projet </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Options pour supprimer les informations sur les modèles d’un projet

Pour supprimer les informations sur les modèles qui ont été ajoutées au projet, vous pouvez procéder de l’une des manières suivantes :

* Supprimez manuellement des informations du projet après que le modèle a été joint.

  Pour plus d’informations, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

* Supprimez les tâches du projet qui ont été ajoutées avec le modèle.

  Pour plus d’nformations, voir la section [Supprimer les tâches créées à partir d’un modèle](#delete-tasks-created-from-a-template) de cet article.

* Supprimez le modèle dans Workfront. La suppression du modèle dans Workfront ne supprime pas les tâches ajoutées à partir du modèle dans les projets.

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

1. Sélectionnez toutes les tâches identifiées à l’étape 2 comme étant créées à partir d’un modèle, puis cliquez sur **l’icône Supprimer****> Oui, supprimer**. Pour plus d’informations, voir [Supprimer des tâches](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
