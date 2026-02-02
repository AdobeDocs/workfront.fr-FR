---
product-area: projects
navigation-topic: create-tasks
title: Créer des sous-tâches
description: Dans Adobe Workfront, les tâches peuvent avoir des relations parent-enfant. Les tâches enfant sont appelées sous-tâches. Vous pouvez créer des sous-tâches dans la liste des tâches en convertissant une tâche principale en sous-tâche. L’opération inverse est également possible.
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 68%

---

# Créer des sous-tâches

<!-- Audited: 01/2025 -->

Dans Adobe Workfront, les tâches peuvent avoir des relations parent-enfant. Les tâches enfant sont appelées sous-tâches. Vous pouvez créer des sous-tâches dans la liste des tâches en faisant d&#39;une tâche principale une sous-tâche d&#39;une autre tâche. L’opération inverse est également possible.

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
   <td> <p>Modifier l’accès aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribuer pour le projet avec la capacité d’ajouter des tâches ou autorisations supérieures</p> 
   <p>Lorsque vous créez une tâche, vous recevez automatiquement des autorisations de gestion de la tâche.</p> 
    </td> 
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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project and the parent task with ability to Add Tasks or higher</p> <p>You automatically receive Manage permissions to the task after you create it.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Créer des sous-tâches

Vous pouvez créer des sous-tâches à partir de la liste des tâches ou de la section Sous-tâches de tâche.

>[!TIP]
>
>La création de sous-tâches pour un projet est similaire à la création de sous-tâches de modèle pour des tâches de modèle sur un modèle.


### Créer des sous-tâches à partir de la liste des tâches {#create-subtasks-from-the-task-list}

1. Accédez au projet dans lequel vous souhaitez créer des sous-tâches.
1. Cliquez sur la section **Tâches** dans le panneau de gauche.
1. (Conditionnel) Si la tâche que vous souhaitez rendre la tâche enfant n’est pas déjà située directement sous la tâche que vous souhaitez rendre la tâche parent, faites-la glisser et déposez-la à l’emplacement approprié dans la liste des tâches.
1. Sélectionnez la tâche à convertir en sous-tâche et effectuez l’une des opérations suivantes :

   * Cliquez sur l’icône **Mettre en retrait** ![Icône Mettre en retrait](assets/indent-icon-nwe-33x29.png) pour faire de la tâche sélectionnée une sous-tâche de la tâche directement au-dessus.
   * Effectuez le raccourci Option+> (Mac) ou Alt+> (Windows) à l’aide d’un clavier QWERTY. Pour les autres langues, effectuez Option+, (Mac) ou Alt+, (Windows) pour l’indentation.

     >[!TIP]
     >
     >Les raccourcis clavier ne fonctionnent pas lorsque vous modifiez des tâches en ligne. Dans ce cas, utilisez l’icône Mettre en retrait ![icône Mettre en retrait](assets/indent-icon-nwe-33x29.png) pour créer des sous-tâches.

   * Placez la tâche au-dessus de la tâche qui deviendra la tâche parent.

     >[!NOTE]
     >
     >Vous ne pouvez mettre en retrait les tâches que lorsque la liste des tâches est triée par Numéro de tâche et lorsqu’aucun regroupement n’est appliqué à la liste des tâches.

### Créer des sous-tâches à partir de la section Sous-tâches de la tâche {#create-subtasks-from-the-task-subtasks-section}

>[!NOTE]
>
>Votre administrateur Workfront ou de groupe peut supprimer la section Sous-tâches dans votre environnement à l’aide d’un modèle de mise en page.

1. Accédez au projet dans lequel vous souhaitez créer des sous-tâches.
1. Cliquez sur la section **Tâches** dans le panneau de gauche.
1. Cliquez sur le nom de la tâche dans laquelle vous souhaitez créer une sous-tâche.
1. Cliquez sur la section **Sous-tâches** dans le panneau de gauche, le cas échéant.
1. Cliquez sur **Nouvelle tâche.**

   Pour plus d’informations sur la création de tâches, voir [Créer des tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Cliquez sur **Créer une tâche.**

   La nouvelle tâche est créée en tant que sous-tâche de la tâche que vous avez sélectionnée à l&#39;étape 3. <!--ensure this is accurate-->

## Convertir une sous-tâche en tâche principale

1. Accédez au projet dans lequel vous souhaitez faire d’une sous-tâche une tâche principale.
1. Cliquez sur la section **Tâches** dans le panneau de gauche.
1. Sélectionnez la sous-tâche à convertir en tâche.
1. Cliquez sur l’icône **Ajouter un retrait négatif** ![Icône Ajouter un retrait négatif](assets/outdent-icon-nwe-31x29.png) pour faire de la sous-tâche une tâche principale.

   Ou

   Sur un clavier QWERTY anglais standard, appuyez sur Option+&lt; (Mac) ou Alt+&lt; (Windows). D’autres langues peuvent utiliser les commandes Option+. (Mac) ou Alt+. (Windows) pour les retraits négatifs.

   >[!NOTE]
   >
   >Vous ne pouvez supprimer des alinéas pour des tâches que lorsque la liste des tâches est triée par numéro de tâche et lorsqu’aucun regroupement n’est appliqué à la liste.
