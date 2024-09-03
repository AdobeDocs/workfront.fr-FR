---
product-area: projects
navigation-topic: manage-projects
title: Modifier le statut d’un projet
description: Si nécessaire, vous pouvez mettre à jour manuellement le statut d’un projet vers un autre statut. Vous pouvez mettre à jour manuellement le statut d’un projet avec le statut Terminé uniquement lorsque le mode d’achèvement du projet est défini sur Manuel.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: 7363e86f5c507e40955e16843c6776777c7ad823
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 100%

---

# Modifier le statut d’un projet

<!--Audited: 02/2024-->

Si nécessaire, vous pouvez mettre à jour manuellement le statut d’un projet vers un autre statut.

Vous pouvez mettre à jour manuellement le statut d’un projet avec le statut Terminé uniquement lorsque le mode d’achèvement du projet est défini sur Manuel.

Dans le cas contraire, Adobe Workfront marque automatiquement le projet comme terminé lorsque toutes les tâches et tous les problèmes du projet sont terminés et approuvés.

Pour plus d’informations sur le mode d’achèvement du projet, voir [Modifier des projets](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard </p> 
   Ou
   <p>Actuel : formule </p>
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

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considérations relatives à la mise à jour vers des statuts spécifiques

* **Lors de la mise à jour d’un projet à terminer :** assurez-vous que toutes les tâches et tous les problèmes sont terminés sur le projet. Vous ne pouvez pas sélectionner le statut Terminé d’un projet, ni aucun autre statut correspondant à Terminé lorsqu’il existe des tâches ou des problèmes qui n’ont pas été terminés sur le projet. Cela inclut l’approbation de toute tâche ou problème qui a un statut Terminé en attente d’approbation.
* **Lors de la mise à jour d’un projet de Terminé à En cours :** si toutes les tâches et tous les problèmes du projet sont terminés, assurez-vous que le mode d’achèvement du projet est défini sur Manuel. Si le mode d’achèvement du projet est automatique, le statut du projet reste Terminé.

## Modifier le statut du projet

1. Accédez au projet dont vous souhaitez mettre à jour le statut.
1. Dans l’en-tête du projet, cliquez sur le nom du statut dans le champ **Statut**, puis sélectionnez un nouveau statut.

   ![](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   Ou

   Cliquez sur le menu **Plus** ![](assets/qs-more-menu.png) en regard du nom du projet, puis cliquez sur **Modifier** et sélectionnez un nouveau statut dans le champ **Statut**, puis cliquez sur **Enregistrer**.

   Le statut du projet est mis à jour par rapport au statut que vous avez sélectionné.
