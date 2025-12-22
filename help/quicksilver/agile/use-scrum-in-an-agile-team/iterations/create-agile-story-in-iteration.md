---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Création d’une histoire agile dans une itération
description: Cet article décrit comment créer une nouvelle histoire agile lorsque vous êtes déjà dans l’itération.
author: Jenny
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 80%

---

# Création d’une histoire agile dans une itération

Cet article décrit comment créer une nouvelle histoire agile lorsque vous êtes déjà dans l’itération. Pour plus d’informations sur la création d’une histoire agile à partir d’une tâche, d’un problème ou d’une autre zone de [!DNL Adobe Workfront], voir [Ajouter des histoires à une itération existante](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
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

   1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Itérations]**.
   1. Cliquez sur le nom de l’itération spécifique où vous souhaitez créer une histoire.
   1. Dans le panneau de gauche, sélectionnez **[!UICONTROL Histoires]**.

1.  Cliquez sur **[!UICONTROL Nouvelle histoire]**.
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
      <td>Indiquez l’estimation de l’histoire. Si votre équipe Agile est configurée pour estimer les histoires en points, alors par défaut 1 point équivaut à 8 heures. Les estimations sont ajoutées sous la forme d’[!UICONTROL Planned Hours] sur l’histoire.<br>Par exemple, si vous estimez qu’une histoire comporte 3 points, le comportement par défaut est d’ajouter 24 heures prévues à l’histoire.<br>Si une histoire contient des sous-tâches, n’oubliez pas que les estimations combinées pour toutes les sous-tâches déterminent l’estimation de l’histoire parent. Pour plus d’informations, consultez <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Ajouter une sous-tâche à une histoire existante sur le panorama [!UICONTROL Scrum]</a>.</td>
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
