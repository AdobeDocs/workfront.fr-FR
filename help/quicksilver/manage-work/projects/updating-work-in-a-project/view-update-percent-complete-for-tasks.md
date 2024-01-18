---
product-area: projects
navigation-topic: update-work-in-a-project
title: Afficher et mettre à jour le pourcentage d’achèvement pour les tâches
description: Vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche pour indiquer l’avancement de la tâche vers son achèvement.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Afficher et mettre à jour le pourcentage d’achèvement pour les tâches

<!--Audited:01/2024-->

Vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche pour indiquer l’avancement de la tâche vers son achèvement.

## Conditions d’accès

Vous devez disposer des accès suivants pour mettre à jour manuellement les tâches :

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
   <td> <p>Nouvelle licence : Standard</p> 
   Ou
   <p>Licence actuelle : travail ou version ultérieure</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Modifier l’accès aux tâches</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour la tâche</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Zones dans lesquelles vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche

Vous pouvez mettre à jour le pourcentage de réalisation d’une tâche dans l’un des domaines suivants :

* **Dans une liste de tâches**: vous pouvez mettre à jour le pourcentage de fin d’une tâche lorsque la colonne Pourcentage de fin est affichée.\
  Pour plus d’informations sur la modification en ligne, voir [Éléments de modification en ligne dans une liste dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **Dans la vue Milestone**: vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche lors de l’utilisation de la vue Jalon sur une liste de projets ou un rapport de projet. Pour plus d’informations, voir [Utilisation de la vue Milestone](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **Dans l’en-tête de la tâche**: vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche dans l’en-tête de la tâche. Pour plus d’informations, voir [Modifier les tâches](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)


## Observations relatives à la mise à jour du pourcentage d’achèvement d’une tâche

* Lorsque vous marquez une tâche comme 100 % terminée, l’état de la tâche est mis à jour sur Terminé.
* Les scénarios suivants existent pour les tâches parentes :
   * Vous ne pouvez pas mettre à jour le pourcentage d’achèvement d’une tâche parent à 100 % lorsque le mode d’achèvement du résumé du projet est défini sur Automatique et que les sous-tâches ne sont pas terminées.
   * Vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche parent à 100 % lorsque le mode d’achèvement du résumé du projet est défini sur Manuel et que les sous-tâches sont terminées ou incomplètes.

  Pour plus d’informations, voir [Modification de projets](../manage-projects/edit-projects.md).

## Mettre à jour le pourcentage d&#39;achèvement d&#39;une tâche

1. Accédez à l’une des zones suivantes de Workfront :

   * Une liste de tâches
   * Liste des projets et application de la vue Milestone
   * Une tâche, en accédant à la page de la tâche
1. Recherchez la variable **Pourcentage terminé** pour la tâche dont vous souhaitez mettre à jour le pourcentage.
1. Cliquez dans le champ Pourcentage terminé et saisissez un nombre compris entre 0 et 100.

   Ou

   Cliquez et faites glisser le **Pourcentage terminé** au nombre nécessaire pour indiquer la quantité de la tâche que vous avez effectuée, le cas échéant.

   >[!NOTE]
   >
   >Lorsque vous indiquez que 100 % de la tâche est terminée, l’état de la tâche est également mis à jour pour Terminé.


1. Appuyez sur Entrée du clavier pour enregistrer le pourcentage terminé.

Le pourcentage d’achèvement du projet est également automatiquement mis à jour.

