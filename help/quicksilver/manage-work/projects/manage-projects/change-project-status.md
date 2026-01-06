---
product-area: projects
navigation-topic: manage-projects
title: Modifier le statut d’un projet
description: Si nécessaire, vous pouvez mettre à jour manuellement le statut d’un projet vers un autre statut. Vous pouvez mettre à jour manuellement le statut d’un projet avec le statut Terminé uniquement lorsque le mode d’achèvement du projet est défini sur Manuel.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 85%

---

# Modifier le statut d’un projet

<!--Audited: 02/2024-->

Si nécessaire, vous pouvez mettre à jour manuellement le statut d’un projet vers un autre statut.

Vous pouvez mettre à jour manuellement le statut d’un projet avec le statut Terminé uniquement lorsque le mode d’achèvement du projet est défini sur Manuel.

Dans le cas contraire, Adobe Workfront marque automatiquement le projet comme terminé lorsque toutes les tâches et tous les problèmes du projet sont terminés et approuvés.

Pour plus d’informations sur le mode d’achèvement du projet, voir [Modifier des projets](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

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
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur le projet</p> </td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Considérations relatives à la mise à jour vers des statuts spécifiques

* **Lors de la mise à jour d’un projet à terminer :** assurez-vous que toutes les tâches et tous les problèmes sont terminés sur le projet. Vous ne pouvez pas sélectionner le statut Terminé d’un projet, ni aucun autre statut correspondant à Terminé lorsqu’il existe des tâches ou des problèmes qui n’ont pas été terminés sur le projet. Cela inclut l’approbation de toute tâche ou problème qui a un statut Terminé en attente d’approbation.
* **Lors de la mise à jour d’un projet de Terminé à En cours :** si toutes les tâches et tous les problèmes du projet sont terminés, assurez-vous que le mode d’achèvement du projet est défini sur Manuel. Si le mode d&#39;achèvement du projet est Automatique, le statut du projet reste Terminé.

## Modifier le statut du projet

1. Accédez au projet dont vous souhaitez mettre à jour le statut.
1. Dans l’en-tête du projet, cliquez sur le nom du statut dans le champ **Statut**, puis sélectionnez un nouveau statut.

   ![Modifier le statut du projet](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   Ou

   Cliquez sur le menu **Plus** ![Plus](assets/qs-more-menu.png) en regard du nom du projet et cliquez sur **Modifier** et sélectionnez un nouveau statut dans le champ **Statut**, puis cliquez sur **Enregistrer**.

   Le statut du projet est mis à jour par rapport au statut que vous avez sélectionné.
