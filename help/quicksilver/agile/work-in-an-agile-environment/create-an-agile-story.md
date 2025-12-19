---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: Créer une histoire agile
description: Vous pouvez créer une histoire Agile sur une itération de différentes manières. Après avoir créé une histoire Agile, vous pouvez ajouter des sous-tâches à l’histoire.
author: Jenny
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '695'
ht-degree: 78%

---

# Créer une histoire Agile

Vous pouvez créer une histoire agile sur une itération de différentes manières. Après avoir créé une histoire agile, vous pouvez y ajouter des sous-tâches.

Lorsque vous ajoutez une histoire ou une sous-tâche dans une itération, le type de durée est défini sur [!UICONTROL Simple] et la contrainte de tâche est définie sur Dates fixes, avec les dates verrouillées dans l’itération. Vous ne pouvez pas modifier le type de durée ou la contrainte de tâche dans une itération. En outre, la durée de la tâche doit être supérieure à 0 minute.

Pour plus d’informations sur la gestion de l’histoire après son ajout à l’itération, voir [Itérations](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td role="rowheader">Autorisations d’objet</td> 
   <td>Gérer l’accès au projet sur lequel porte l’histoire </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Création d’une histoire agile dans une itération

1. Accédez à l’itération Agile dans laquelle vous souhaitez créer l’histoire :

   {{step1-to-team}}

   1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

   1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Itérations]** pour sélectionner une itération spécifique, ou sélectionnez **[!UICONTROL Itération actuelle]**.
   1. Cliquez sur le nom de l’itération spécifique où vous souhaitez créer une histoire.

   ![Ajouter une nouvelle histoire à l’itération](assets/iteration-stories-list.png)

1. Cliquez sur **[!UICONTROL Nouvelle histoire].**
1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>Tapez un nom pour l’histoire.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Saisissez une description pour l’histoire.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>Sélectionnez cette option si l’histoire est prête à être ajoutée à une itération. Lorsque cette option est sélectionnée, elle indique aux utilisateurs et utilisatrices quelles histoires de la liste d’attente sont prêtes à être ajoutées à une itération.<br>Une histoire peut être ajoutée à une itération, qu’elle soit marquée comme <strong>[!UICONTROL Ready] ou non.</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate] (points)</strong></td>
      <td>Indiquez l’estimation de l’histoire. Si votre équipe Agile est configurée pour estimer les histoires en points, alors par défaut 1 point équivaut à 8 heures. Les estimations sont ajoutées sous la forme d’[!UICONTROL Planned Hours] sur l’histoire.<br>Par exemple, si vous estimez qu’une histoire comporte 3 points, le comportement par défaut consiste à ajouter 24 [!UICONTROL Planned Hours] à l’histoire.<br>Si une histoire contient des sous-tâches, n’oubliez pas que les estimations combinées pour toutes les sous-tâches déterminent l’estimation de l’histoire parent. Pour plus d’informations, voir <a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">Ajouter des histoires à une itération existante</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Commencez à saisir le nom du projet auquel cette histoire sera associée.<br>Par défaut, l’histoire s’affiche avec la même couleur que les autres histoires de ce projet.<br>Le statut du projet doit être défini sur [!UICONTROL Current]. Si le statut du projet n’est pas [!UICONTROL Current], il n’est pas affiché dans le menu déroulant.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>Après avoir choisi un projet parent, vous avez la possibilité de choisir une tâche parent. Lorsque vous sélectionnez une tâche parent, l’histoire est créée en tant que sous-tâche de la tâche parent sur le projet que vous avez sélectionné.<br>Commencez à saisir le nom de la tâche parent pour l’histoire, puis cliquez dessus lorsqu’il apparaît dans la liste déroulante.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Sélectionnez les formulaires personnalisés à ajouter à l’histoire.</td>
     </tr>
    </tbody>
   </table>

1. Cliquez sur **[!UICONTROL Enregistrer l’histoire]**.

## Créer une histoire Agile dans la liste d’attente

Vous pouvez créer une histoire Agile à partir de la liste d’attente Agile, comme décrit dans la section [Créer de nouvelles histoires sur la liste d’attente](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories) dans l’article [[!UICONTROL Gérer] la liste d’attente Agile](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

## Ajouter une tâche ou un événement sous la forme d’une histoire agile

Vous pouvez ajouter une tâche existante ou un problème existant en tant qu’histoire à une itération. Pour plus d’informations, voir [Ajouter des histoires à une itération existante](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) ou [Ajouter des histoires et des problèmes à partir du panorama [!UICONTROL Scrum]](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md).

## Créer des sous-tâches pour une histoire agile

Vous pouvez créer une sous-tâche dans une histoire agile à l’aide de l’une des méthodes suivantes :

* En utilisant l’onglet **[!UICONTROL Sous-tâches]**, comme décrit dans la section [Créer des sous-tâches](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks) dans [Créer des sous-tâches](../../manage-work/tasks/create-tasks/create-subtasks.md).

* Directement à partir du panorama d’histoire, comme décrit dans [Créer une itération](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
