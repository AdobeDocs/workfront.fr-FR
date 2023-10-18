---
product-area: projects
navigation-topic: update-work-in-a-project
title: Afficher et mettre à jour le pourcentage d’achèvement pour les tâches
description: Vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche pour indiquer l’avancement de la tâche vers son achèvement.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Afficher et mettre à jour le pourcentage d’achèvement pour les tâches

Vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche pour indiquer l’avancement de la tâche vers son achèvement.

## Conditions d’accès

<!--drafted for P&P:

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
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Vous devez disposer des accès suivants pour mettre à jour manuellement les tâches :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour la tâche</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.


## Zones dans lesquelles vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche

Vous pouvez mettre à jour le pourcentage de réalisation d’une tâche dans l’un des domaines suivants :

* **Dans une liste de tâches**: vous pouvez mettre à jour le pourcentage de fin d’une tâche lorsque la colonne Pourcentage de fin est affichée.\
  Pour plus d’informations sur la modification en ligne, voir [Éléments de modification en ligne dans une liste dans Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **Dans la vue Milestone**: vous pouvez mettre à jour le pourcentage d’achèvement d’une tâche lors de l’utilisation de la vue Jalon sur une liste de projets ou un rapport de projet. Pour plus d’informations, voir [Utilisation de la vue Milestone](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Lorsque vous mettez à jour la tâche**: vous pouvez mettre à jour l’option Pourcentage d’achèvement d’une tâche lors de l’ajout d’une mise à jour à la tâche.

  >[!IMPORTANT]
  >
  >Cette option s’affiche uniquement une fois que vous avez activé l’option Afficher le pourcentage terminé .\
  >Pour activer la barre de mise à jour du pourcentage d’achèvement des tâches, procédez comme suit :
  >
  >1. Accédez au **Principal** menu>votre nom>**Plus** en regard de votre nom >**Modifier** > sélectionner **Afficher le pourcentage terminé à l’état de mise à jour**.\
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >

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

   Cliquez et faites glisser le **Pourcentage terminé** au nombre nécessaire pour indiquer la partie de la tâche que vous avez effectuée.

   >[!NOTE]
   >
   >Lorsque vous indiquez que 100 % de la tâche est terminée, l’état de la tâche est également mis à jour pour Terminé.


1. Appuyez sur Entrée du clavier pour enregistrer le pourcentage terminé.

