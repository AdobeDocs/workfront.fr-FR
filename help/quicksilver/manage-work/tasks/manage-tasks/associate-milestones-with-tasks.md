---
product-area: projects
navigation-topic: manage-tasks
title: Associer des jalons à des tâches
description: Vous pouvez associer des jalons à des tâches pour indiquer le moment où vous atteignez des étapes importantes au cours de la durée de vie du projet. Vous devez associer un chemin jalonné à un projet avant de pouvoir associer des jalons à des tâches sur le projet.
author: Alina
feature: Work Management
exl-id: 56410640-fde4-417f-8ea0-f089315476f7
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 90%

---

# Associer des jalons à des tâches

<!--Audited: 01/2024-->

Vous pouvez associer des jalons à des tâches pour indiquer le moment où vous atteignez des étapes importantes au cours de la durée de vie du projet.

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
   <p>Travail ou supérieur</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux tâches</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations pour la tâche</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, consultez la section [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>New license: Standard</p> 
   <p>Current license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Conditions préalables

Avant de pouvoir associer un jalon à une tâche, les éléments suivants doivent être présents :

* L’administrateur ou l’administratrice de Workfront doit créer un chemin jalonné, comme décrit dans la section [Créer un chemin jalonné](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).

* Vous devez associer un chemin jalonné à un projet.

  Pour plus d’informations, voir [Modifier les projets](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

* Pour associer un chemin jalonné à un projet, ce dernier doit être au statut Planification ou Actuel.

  >[!TIP]
  >
  >Pour obtenir une meilleure vue d’ensemble de la progression des jalons dans vos projets à l’aide de la vue jalonnée, vous devez créer des tâches parents et les associer à chaque phase majeure de votre projet. Associez ensuite ces tâches parents à chacun des jalons de votre chemin jalonné.

## Associer un jalon à une tâche

Une fois qu’un chemin jalonné est associé à un projet, les tâches peuvent se voir attribuer un jalon.

1. Accédez à une tâche, puis cliquez sur l’icône **Plus** ![Plus](assets/more-icon.png) à droite du nom de la tâche, puis sur **Modifier**.

   Les tâches et les jalons ont une relation :1. Vous ne pouvez pas joindre le même jalon à plusieurs tâches. Chaque tâche peut être associée à un jalon unique, ou chaque jalon peut être associé à une seule tâche.

1. Cliquez sur **Paramètres**, puis sélectionnez un jalon dans le champ **Jalon** pour la tâche.
1. Cliquer sur **Enregistrer**.
1. (Facultatif) Dans une liste de tâches, ajoutez la colonne **Icônes de statut** pour identifier les tâches comportant des jalons. L’indicateur de losange de jalon s’affiche dans la colonne Icônes de statut.

   Pour plus d’informations, voir [Créer ou modifier des vues dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

   ![Icônes de statut](assets/amwt3.png)

1. (Facultatif) Accédez à une liste des projets et sélectionnez la vue **Jalon** pour identifier la progression de vos tâches jalonnées.

   ![Liste des projets de la vue Jalon](assets/milestone-view-project-list.png)
