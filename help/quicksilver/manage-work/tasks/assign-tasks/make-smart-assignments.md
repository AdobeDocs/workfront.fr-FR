---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Créer des affectations intelligentes
description: Vous pouvez utiliser des affectations intelligentes pour identifier la meilleure personne pour effectuer le travail. Les affectations intelligentes sont des suggestions destinées aux utilisateurs et utilisatrices, aux rôles ou aux équipes qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources en fonction d’un algorithme qui détermine la ressource la plus appropriée pour le traitement. Pour plus d’informations sur les affectations intelligentes, voir Vue d’ensemble des affectations intelligentes.
author: Lisa
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 91%

---

# Créer des affectations intelligentes

<!--Audited: 07/2024-->

Tirez parti des affectations intelligentes pour identifier la personne idéale à la réalisation du travail.

Les affectations intelligentes sont des suggestions destinées aux utilisateurs et utilisatrices, aux rôles ou aux équipes qu’Adobe Workfront vous présente lorsque vous affectez des éléments de travail à des ressources. Workfront base ses suggestions sur un algorithme qui détermine la ressource la plus appropriée pour le traitement.

<!--<span class="preview">There are two separate algorithms in Workfront that calculate smart assignments that work differently for tasks and for issues.</span> -->

Pour plus d’informations sur les critères utilisés pour déterminer les affectations intelligentes, voir [Vue d’ensemble des affectations intelligentes](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Travail ou supérieur</p>
   </td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux tâches et aux problèmes</p> <p>Accès en affichage ou supérieur aux projets</p> </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td>
   <td>Autorisations de contribution ou autorisations supérieures avec la possibilité d’affecter des tâches et des problèmes</td>
  </tr>
 </tbody>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer des affectations intelligentes

Les affectations intelligentes sont disponibles dans la plupart des emplacements où vous pouvez effectuer des affectations dans Workfront.

1. Dans les zones suivantes, cliquez sur le champ **Affectations** ou **Affecter ceci à** :

   * Tâche, liste de problèmes ou rapport.
   * En-tête de tâche ou de problème.
   * Panneau Résumé de la tâche ou du problème.
   * Tâche ou problème dans l’équilibreur de charge de travail.
     <!--* <span class="preview">A New Task</span> or New Issue box, as you add <span class="preview">a new task</span> or issue to a project-->

1. Placez le curseur dans le champ d’affectation et attendez deux secondes.

   <!--For issues, the smart assignments display in the following sections: 
      * **Users and teams**
      * **Job roles**
        ![Smart assignments issue header](assets/smart-assignments-issue-header.png)-->

   Les affectations intelligentes s’affichent dans les sections suivantes <!--, depending on which phase of the algorithm's calculation identified the assignments-->

   <!--* <span class="preview">**Suggested assignments**: Displays assignments identified in the first phase of the task smart assignment algorithm.</span> -->
   * **Utilisateurs et équipes** ou **Fonctions** <!--or **Rate card job roles**: Assignments identified in the second phase of the task smart assignment's algorithm calculation.-->

   ![Exemple d&#39;affectations intelligentes dans la liste des tâches](assets/smart-assignments-task-list.png)

   Pour en savoir plus, consultez la section [Vue d’ensemble des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Sélectionnez la ressource dans la liste des recommandations en cliquant sur son nom.

1. (Facultatif) Cliquez sur **Me l’affecter** pour vous attribuer l’élément de travail.

   >[!TIP]
   >
   >S’il n’existe aucune suggestion, la liste de suggestions ne s’ouvre pas.

1. (Facultatif) Si vous ne souhaitez pas utiliser l’une des personnes recommandées dans la liste des affectations intelligentes, commencez à saisir le nom de la ressource souhaitée et sélectionnez le nom lorsqu’il apparaît dans la liste.
1. Cliquez sur **Entrée** pour donner l’affectation.

   La personne sélectionnée est alors affectée à la tâche ou au problème.
