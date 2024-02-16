---
product-area: projects
navigation-topic: manage-projects
title: Modification de l’état d’un projet
description: Si nécessaire, vous pouvez mettre à jour manuellement l’état d’un projet vers un autre état. Vous pouvez mettre à jour manuellement l’état d’un projet avec l’état Terminé uniquement lorsque le mode d’exécution du projet est défini sur Manuel.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
source-git-commit: 7363e86f5c507e40955e16843c6776777c7ad823
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Modification de l’état d’un projet

<!--Audited: 02/2024-->

Si nécessaire, vous pouvez mettre à jour manuellement l’état d’un projet vers un autre état.

Vous pouvez mettre à jour manuellement l’état d’un projet avec l’état Terminé uniquement lorsque le mode d’exécution du projet est défini sur Manuel.

Dans le cas contraire, Adobe Workfront marque automatiquement le projet comme terminé lorsque toutes les tâches et tous les problèmes du projet sont terminés et approuvés.

Pour plus d’informations sur le mode d’achèvement du projet, voir [Modification de projets](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard </p> 
   Ou
   <p>Actuel : formule </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Modifier l’accès aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations sur le projet</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considérations relatives à la mise à jour vers des états spécifiques

* **Lors de la mise à jour d’un projet à terminer :** Assurez-vous que toutes les tâches et tous les problèmes sont terminés sur le projet. Vous ne pouvez pas sélectionner l’état Terminé d’un projet, ni aucun autre état correspondant à Terminé lorsqu’il y a des tâches ou des problèmes qui n’ont pas été terminés sur le projet. Cela inclut l’approbation de toute tâche ou problème qui est à l’état Terminé en attente d’approbation.
* **Lors de la mise à jour d’un projet de la fin à actuel :** Si toutes les tâches et tous les problèmes du projet sont terminés, assurez-vous que le mode d’achèvement du projet est défini sur Manuel. Si le mode d’achèvement du projet est automatique, l’état du projet reste Terminé.

## Modification de l’état du projet

1. Accédez au projet dont vous souhaitez mettre à jour l’état.
1. Dans l’en-tête du projet, cliquez sur le nom de l’état dans la **État** , puis sélectionnez un nouvel état.

   ![](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   Ou

   Cliquez sur le bouton **Plus** menu ![](assets/qs-more-menu.png) en regard du nom du projet, puis cliquez sur **Modifier** et sélectionnez un nouvel état dans le **État** , puis cliquez sur **Enregistrer**.

   L’état du projet est mis à jour par rapport à l’état que vous avez sélectionné.
