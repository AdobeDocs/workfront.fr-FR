---
product-area: projects
navigation-topic: update-work-in-a-project
title: Afficher et mettre à jour le pourcentage d'achèvement pour les tâches
description: Vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche afin d’indiquer la progression de la tâche vers son achèvement. La mise à jour du pourcentage terminé pour les événements est similaire à la mise à jour d’une tâche. Cet article décrit comment mettre à jour le pourcentage d’achèvement d’une tâche.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 42%

---

# Afficher et mettre à jour le pourcentage terminé des tâches

<!--Audited: 05/2025-->

Vous pouvez mettre à jour le pourcentage terminé d’une tâche pour indiquer la progression de la tâche vers son achèvement.

La mise à jour du pourcentage terminé pour les événements est similaire à la mise à jour d’une tâche. Cet article décrit comment mettre à jour le pourcentage d’achèvement d’une tâche.

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
   <p>Travail ou supérieur</p>
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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license: Standard</p> 
   Or
   <p>Current license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Zones dans lesquelles vous pouvez mettre à jour le pourcentage terminé d’une tâche

Vous pouvez mettre à jour le pourcentage terminé d’une tâche dans l’un des domaines suivants :

* **Dans une liste de tâches** : vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche lorsque la colonne Pourcentage terminé s’affiche.

  Pour plus d’informations sur la modification en ligne, voir [Modifier en ligne des éléments dans une liste dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **Dans la vue Jalon** : Vous pouvez mettre à jour le pourcentage d&#39;achèvement d&#39;une tâche lors de l&#39;utilisation de la vue Jalon dans une liste de projets ou un rapport de projet.

  >[!TIP]
  >
  >  Vous ne pouvez pas mettre à jour le pourcentage d&#39;achèvement des événements dans la vue Jalon.


  Pour plus d’informations, voir [Utiliser la vue de Jalon](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Dans l’en-tête de la tâche** : vous pouvez mettre à jour le pourcentage d’avancement d’une tâche dans l’en-tête de la tâche.

  ![Mettre à jour le pourcentage dans l’en-tête](assets/nwe-updatetaskpercentinheader-350x54.png)

* **Dans le panneau Résumé d’une tâche** : vous pouvez mettre à jour le pourcentage terminé d’une tâche en haut du panneau Résumé lorsque vous affichez la tâche dans les zones suivantes :

   * Liste ou rapport de tâches
   * Feuille de temps
   * Équilibreur de charge de travail

  ![Mettre à jour le pourcentage dans le résumé de la tâche en surbrillance](assets/update-percent-complete-in-task-summary-highlighted.png)

  Pour plus d’informations, consultez la [Vue d’ensemble du résumé](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md).

* **Accueil** : vous pouvez mettre à jour le pourcentage terminé d’une tâche ou d’un problème à partir du panneau Résumé dans la zone Accueil ou à partir du widget Mon travail.

  Pour plus d’informations, voir [Prise en main de l’Accueil](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

## Considérations relatives à la mise à jour du pourcentage terminé d’une tâche

* Lorsque vous marquez une tâche comme terminée à 100 %, le statut de la tâche devient Terminé. Le statut d&#39;un événement passe à Fermé.
* Terminer une tâche met également à jour le pourcentage d’achèvement du parent et du projet.
* Les scénarios suivants existent pour les tâches et projets parents :
   * Vous ne pouvez pas mettre à jour le pourcentage terminé d’une tâche parent à 100 % lorsque le mode d’achèvement du résumé du projet est défini sur Automatique et que les sous-tâches ne sont pas terminées.
   * Vous pouvez mettre à jour le pourcentage d&#39;achèvement d&#39;une tâche parent ou d&#39;un projet à 100 % lorsque le mode d&#39;achèvement du sommaire du projet est défini sur Manuel et que les sous-tâches sont terminées ou incomplètes.

  Pour plus d’informations, voir [Modifier les projets](../manage-projects/edit-projects.md).

## Mettre à jour le pourcentage terminé d&#39;une tâche

1. Accédez à l’une des zones où vous souhaitez mettre à jour le pourcentage d’avancement d’une tâche.

   Pour plus d’informations, reportez-vous à la section [Zones dans lesquelles vous pouvez mettre à jour le pourcentage d’avancement d’une tâche](#areas-where-you-can-update-the-percent-complete-of-a-task) de cet article.

1. Recherchez le champ **Pourcentage terminé** pour la tâche dont vous souhaitez mettre à jour le pourcentage terminé.

   >[!TIP]
   >
   >Le champ Pourcentage terminé s’affiche toujours en haut du panneau Résumé.

1. Cliquez dans le champ **Pourcentage terminé** et saisissez un nombre compris entre 0 et 100.

   Ou

   Cliquez sur la bulle bleue **Pourcentage terminé** et faites-la glisser jusqu’au nombre nécessaire pour indiquer le nombre de tâches que vous avez terminées, le cas échéant.

   >[!NOTE]
   >
   >    * Vous ne pouvez pas saisir de nombre décimal lorsque vous cliquez dans la bulle Pourcentage terminé.
   >    * Lorsque vous faites glisser la bulle bleue dans le panneau Résumé , le Pourcentage d’achèvement des mises à jour s’incrémente d’un point.
   >
   >    * Lorsque vous faites glisser la bulle bleue dans l’en-tête de la tâche, le Pourcentage terminé est mis à jour par incréments de 5 points.

1. Appuyez sur Entrée sur votre clavier pour enregistrer le pourcentage d’achèvement.

   Le pourcentage d&#39;achèvement du projet ou des tâches parents peut également être mis à jour automatiquement.

   Le statut de la tâche ou de l’événement est également mis à jour.

