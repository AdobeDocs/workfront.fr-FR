---
product-area: projects
navigation-topic: task-information
title: Mettre à jour le délai de nivellement de la tâche
description: Parfois, des conflits peuvent exister entre les planifications de tâches sur un projet. Vous pouvez niveler les ressources ou résoudre leurs conflits en replanifiant les ressources et les tâches, afin que toutes les tâches puissent être effectuées dans des délais réalistes. Pour plus d’informations sur le nivellement des tâches, voir la section Niveler les ressources dans le graphique de Gantt.
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 100%

---

# Mettre à jour le délai de nivellement de la tâche

Parfois, des conflits peuvent exister entre les planifications de tâches sur un projet. Vous pouvez niveler les ressources ou résoudre leurs conflits en replanifiant les ressources et les tâches, afin que toutes les tâches puissent être effectuées dans des délais réalistes. Pour plus d’informations sur le nivellement des tâches, voir la section [Niveler des ressources dans le graphique de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

En tant que personne responsable du projet ou personne cessionnaire de la tâche, vous pouvez également ajouter un délai de nivellement sur les tâches individuelles afin de tenir compte de tout conflit de ressource ou de planification. En d’autres termes, une tâche peut être planifiée avec un retard afin de s’assurer que, lorsqu’Adobe Workfront nivelle les tâches, un planning plus réaliste permette de dépasser les conflits de ressources.

L’ajout d’un retard de nivellement à une tâche ajuste la date d’achèvement prévisionnelle de la tâche. Pour plus d’informations sur la date d’achèvement prévisionnelle, voir la section [Vue d’ensemble de la date d’achèvement prévisionnelle pour les projets, tâches et problèmes](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations sur les tâches </p> <p>Autorisations Contribuer ou supérieures sur les projets</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

## Ajouter un retard de nivellement à une tâche

1. Accédez à une tâche à laquelle vous souhaitez ajouter un retard de nivellement.
1. Cliquez sur l’icône **Plus** à droite du nom de la tâche, puis cliquez sur **Modifier**.

1. Cliquez sur **Paramètres**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Spécifiez le **Délai de nivellement**, en heures, puis choisissez une unité de temps.\
   Il s’agit de la durée du retard de la ressource au moment du lancement de la tâche en raison de conflits de ressources.

   Choisissez l’une des options suivantes pour les unités de temps :

   * Minutes
   * HeuresIl s’agit du paramètre par défaut.
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

1. Cliquez sur **Enregistrer**.

 
