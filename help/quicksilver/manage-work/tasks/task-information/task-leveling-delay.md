---
product-area: projects
navigation-topic: task-information
title: Mettre à jour le délai de nivellement de la tâche
description: Parfois, des conflits peuvent exister entre les planifications de tâches sur un projet. Vous pouvez niveler les ressources ou résoudre leurs conflits en replanifiant les ressources et les tâches, afin que toutes les tâches puissent être effectuées dans des délais réalistes. Pour plus d’informations sur le nivellement des tâches, voir la section Niveler les ressources dans le graphique de Gantt.
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 91%

---

# Mettre à jour le délai de nivellement de la tâche

Parfois, des conflits peuvent exister entre les planifications de tâches sur un projet. Vous pouvez niveler les ressources ou résoudre leurs conflits en replanifiant les ressources et les tâches, afin que toutes les tâches puissent être effectuées dans des délais réalistes. Pour plus d’informations sur le nivellement des tâches, voir la section [Niveler des ressources dans le graphique de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

En tant que personne responsable du projet ou personne cessionnaire de la tâche, vous pouvez également ajouter un délai de nivellement sur les tâches individuelles afin de tenir compte de tout conflit de ressource ou de planification. En d’autres termes, une tâche peut être planifiée avec un délai afin de s’assurer que lorsque Adobe Workfront nivelle les tâches, un planning plus réaliste surmonte les conflits de ressources.

L’ajout d’un retard de nivellement à une tâche ajuste la date d’achèvement prévisionnelle de la tâche. Pour plus d’informations sur la date d’achèvement prévisionnelle, voir la section [Vue d’ensemble de la date d’achèvement prévisionnelle pour les projets, tâches et problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

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
   <td> <p>Modifier l’accès aux tâches et aux projets</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur les tâches </p> <p>Autorisations Contribuer ou supérieures sur les projets</p> </td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to Tasks </p> <p>Contribute or higher permissions to Projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Ajouter un retard de nivellement à une tâche

1. Accédez à une tâche à laquelle vous souhaitez ajouter un retard de nivellement.
1. Cliquez sur l’icône **Plus** à droite du nom de la tâche, puis cliquez sur **Modifier**.

1. Cliquez sur **Paramètres**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Spécifiez le **Délai de nivellement**, en heures, puis choisissez une unité de temps.\
   Il s’agit de la durée du retard de la ressource au moment du lancement de la tâche en raison de conflits de ressources.

   Choisissez l’une des options suivantes pour les unités de temps :

   * Minutes
   * Heures. Il s’agit de la valeur par défaut.
   * Jours
   * Semaines
   * Mois
   * Minutes écoulées
   * Heures écoulées
   * Jours écoulés
   * Semaines écoulées
   * Mois écoulés

   >[!TIP]
   >
   >Le temps écoulé est une unité de temps pour la durée d’une tâche. Il s’agit de la durée entre la date de début et la date d’achèvement prévues d’une tâche qui comprend les jours fériés, les week-ends et les jours de congé. En d’autres termes, le temps écoulé est le nombre de jours calendaires écoulés.

1. Cliquer sur **Enregistrer**.


