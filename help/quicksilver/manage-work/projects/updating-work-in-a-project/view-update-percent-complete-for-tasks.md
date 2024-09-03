---
product-area: projects
navigation-topic: update-work-in-a-project
title: Afficher et mettre à jour le pourcentage terminé des tâches
description: Vous pouvez mettre à jour le pourcentage terminé d’une tâche pour indiquer la progression de la tâche vers son achèvement.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 4c17466705873b06e7ea7bb08bb78a7e68078f8b
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 100%

---

# Afficher et mettre à jour le pourcentage terminé des tâches

<!--Audited:01/2024-->

Vous pouvez mettre à jour le pourcentage terminé d’une tâche pour indiquer la progression de la tâche vers son achèvement.

## Conditions d’accès

Vous devez disposer des accès suivants pour mettre à jour manuellement les tâches :

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
   <td> <p>Nouvelle licence : Standard</p> 
   Ou
   <p>Licence actuelle : Travail ou version supérieure</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux tâches</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations pour la tâche</p>  </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Zones dans lesquelles vous pouvez mettre à jour le pourcentage terminé d’une tâche

Vous pouvez mettre à jour le pourcentage terminé d’une tâche dans l’un des domaines suivants :

* **Dans une liste de tâches** : vous pouvez mettre à jour le pourcentage terminé d’une tâche lorsque la colonne Pourcentage terminé est affichée.\
  Pour plus d’informations sur la modification en ligne, voir [Modifier en ligne des éléments dans une liste dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **Dans la vue de Jalon** : vous pouvez mettre à jour le pourcentage terminé d’une tâche lors de l’utilisation de la vue de Jalon sur une liste de projets ou un rapport de projet. Pour plus d’informations, voir [Utiliser la vue de Jalon](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **Dans l’en-tête de la tâche** : vous pouvez mettre à jour le pourcentage terminé d’une tâche dans l’en-tête de la tâche. Pour plus d’informations, voir [Modifier les tâches](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **Dans le panneau Résumé d’une tâche** : vous pouvez mettre à jour le pourcentage terminé d’une tâche en haut du panneau Résumé lorsque vous affichez la tâche dans les zones suivantes :

   * Liste ou rapport de tâches
   * Feuille de temps
   * Équilibreur de charge de travail

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  Pour plus d’informations, consultez la [Vue d’ensemble du résumé](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md).

* **Accueil** : vous pouvez mettre à jour le pourcentage terminé d’une tâche ou d’un problème à partir du panneau Résumé dans la zone Accueil ou à partir du widget Mon travail.

Pour plus d’informations, voir [Commencer avec la nouvelle zone Accueil](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

## Considérations relatives à la mise à jour du pourcentage terminé d’une tâche

* Lorsque vous marquez une tâche comme 100 % terminée, le statut de la tâche est mis à jour sur Terminé.
* Les scénarios suivants existent pour les tâches parent :
   * Vous ne pouvez pas mettre à jour le pourcentage terminé d’une tâche parent à 100 % lorsque le mode d’achèvement du résumé du projet est défini sur Automatique et que les sous-tâches ne sont pas terminées.
   * Vous pouvez mettre à jour le pourcentage terminé d’une tâche parent à 100 % lorsque le mode d’achèvement du résumé du projet est défini sur Manuel et que les sous-tâches sont terminées ou incomplètes.

  Pour plus d’informations, voir [Modifier les projets](../manage-projects/edit-projects.md).

## Mettre à jour le pourcentage terminé d&#39;une tâche

1. Accédez à l’une des zones suivantes de Workfront :

   * Liste de tâches
   * La liste des projets et l’application de la vue de Jalon
   * Une tâche, en accédant à la page de la tâche
1. Recherchez le champ **Pourcentage terminé** pour la tâche dont vous souhaitez mettre à jour le pourcentage terminé.

   >[!TIP]
   >
   >  Le champ Pourcentage terminé s’affiche toujours en haut du panneau Résumé.


1. Cliquez dans le champ **Pourcentage terminé** et saisissez un nombre compris entre 0 et 100.

   Ou

   Cliquez et faites glisser la barre **Pourcentage terminé** au nombre nécessaire pour indiquer la quantité de la tâche que vous avez effectuée, le cas échéant.

   >[!NOTE]
   >
   >Lorsque vous indiquez que 100 % de la tâche est terminée, le statut de la tâche est également mis à jour sur Terminé.


1. Appuyez sur Entrée du clavier pour enregistrer le pourcentage terminé.

Le pourcentage terminé du projet est également automatiquement mis à jour.

