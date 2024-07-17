---
product-area: templates
navigation-topic: templates-navigation-topic
title: Supprimer les informations sur les modèles d’un projet
description: Vous ne pouvez pas supprimer un modèle d’un projet. Vous ne pouvez supprimer manuellement les informations ajoutées au projet qu’une fois qu’un modèle a été joint au projet. Pour plus d’informations sur l’association de modèles, voir Joindre un modèle à un projet.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 25%

---

# Supprimer les informations sur les modèles d’un projet

Vous ne pouvez pas supprimer un modèle d’un projet. Vous ne pouvez supprimer manuellement les informations ajoutées au projet qu’une fois qu’un modèle a été joint au projet. Pour plus d’informations sur l’association de modèles, voir [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux tâches</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer l’accès aux tâches </p> <p>Accès Contribute ou supérieur au projet </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Options de suppression des informations de modèle d’un projet

Pour supprimer les informations de modèle ajoutées au projet, vous pouvez effectuer l’une des opérations suivantes :

* Supprimez manuellement les informations du projet une fois le modèle joint.

  Pour plus d’informations, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

* Supprimez les tâches du projet qui ont été ajoutées avec le modèle.

  Pour plus d’informations, reportez-vous à la section [Supprimer les tâches créées à partir d’un modèle](#delete-tasks-created-from-a-template) de cet article.

* Supprimez le modèle de Workfront. La suppression du modèle de Workfront ne supprime pas les tâches ajoutées du modèle des projets.

  Pour plus d’informations, voir [Suppression de modèles de projet](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Supprimer des tâches créées à partir d’un modèle {#delete-tasks-created-from-a-template}

1. Accédez à la section **Tâches** du projet.
1. Utilisez l’une des méthodes suivantes :

   * Créez un filtre pour que la liste des tâches affiche uniquement les tâches qui ont été créées à partir d&#39;un modèle en utilisant l&#39;instruction suivante :

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     Pour plus d’informations sur la création d’un filtre, voir [Création ou modification de filtres dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

     Lorsque vous appliquez le filtre, seules les tâches associées à un identifiant de tâche de modèle s’affichent dans la liste.

   * Créez une vue pour la liste des tâches afin d’afficher les champs **Template Task ID** ou **Template Task Name** dans une colonne.

     Lorsque vous appliquez la vue, les tâches qui contiennent des informations dans la colonne ID de tâche du modèle ou Nom de la tâche du modèle ont été créées à l’aide d’un modèle.

     Pour plus d’informations sur la création d’une vue, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Sélectionnez toutes les tâches identifiées à l&#39;étape 2 comme étant créées à partir d&#39;un modèle, puis cliquez sur **l&#39;icône Supprimer****> Oui, Supprimer**. Pour plus d’informations, voir [Suppression de tâches](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
