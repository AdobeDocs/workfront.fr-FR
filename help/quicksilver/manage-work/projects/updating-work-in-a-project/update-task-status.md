---
product-area: projects
navigation-topic: update-work-in-a-project
title: Mettre à jour le statut des tâches
description: Vous pouvez mettre à jour l’état d’une tâche pour informer les autres personnes sur l’emplacement de la tâche (et sur le projet global) et son état d’avancement.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 1%

---

# Mettre à jour le statut des tâches

Vous pouvez mettre à jour l’état d’une tâche pour informer les autres personnes sur l’emplacement de la tâche (et sur le projet global) et son état d’avancement.

Les états par défaut sont Nouveau, En cours et Terminé. Votre administrateur Adobe Workfront peut ajouter des statuts personnalisés à votre organisation. Pour plus d’informations, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Vous pouvez mettre à jour manuellement les états des tâches ou laisser Workfront les mettre à jour automatiquement lorsque certaines actions ont lieu.

## Exigences d’accès

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
   <td> <p>Nouveau : Standard</p> 
   Ou
   <p>Actuel : travail ou plus élevé</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Modifier l’accès aux tâches</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations pour la tâche</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Observations relatives à la mise à jour de l’état des tâches

* Lorsque vous marquez une tâche comme terminée, le pourcentage d’achèvement de la tâche passe à 100 %.
* Les scénarios suivants existent pour les tâches parentes :
   * Vous ne pouvez pas mettre à jour l’état d’une tâche parente sur Terminé lorsque le mode d’achèvement du résumé du projet est défini sur Automatique et que les sous-tâches ne sont pas terminées.
   * Vous pouvez mettre à jour l’état d’une tâche parente sur Terminé lorsque le mode d’achèvement du résumé du projet est défini sur Manuel et que les sous-tâches sont terminées ou incomplètes.

  Pour plus d’informations, voir [Modification de projets](../manage-projects/edit-projects.md).

## Mise à jour manuelle de l’état de la tâche

Vous pouvez mettre à jour l’état de la tâche dans les zones suivantes de Workfront :

* En-tête de la tâche sur la page de la tâche.
* La boîte de dialogue Modifier la tâche, lors de la modification d’une tâche.
* La section Détails de la tâche de la page de la tâche.
* Dans une liste de tâches ou un rapport, lorsque le champ Statut est visible dans la vue.
* Dans le panneau Résumé de la tâche.

Pour mettre à jour manuellement l’état de la tâche dans l’en-tête de la tâche :

1. Accédez à une tâche pour laquelle vous souhaitez mettre à jour l&#39;état.
1. Cliquez sur le bouton **État** dans l’en-tête de la tâche et sélectionnez un nouvel état.
1. Pour fournir une indication visuelle de la fin de la tâche, faites glisser ou double-cliquez sur la bulle sous **Pourcentage terminé** dans l’en-tête de la tâche

   Ou

   Cliquez à l’intérieur de la bulle dans l’en-tête de la tâche pour saisir un pourcentage.

   ![](assets/percent-complete-status-widgets-task-header.png)

1. (Facultatif) Pour fournir des informations supplémentaires sur la mise à jour, effectuez l’une des opérations suivantes :

   * Pour ajouter une note à propos de la mise à jour, accédez au **Mises à jour** et cliquez sur **Nouveau commentaire**, puis saisissez une note.

     ![](assets/add-update-to-task.png)

   * Pour avertir certains utilisateurs de la mise à jour, saisissez leurs noms dans le champ **Balisage de personnes ou d’équipes** qui apparaît lorsque vous saisissez un commentaire. Pour plus d’informations, voir [Balisage des autres sur les mises à jour](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Pour mettre à jour la date de validation de la tâche, cliquez sur **Détails de la tâche**, puis modifiez la variable **Date de validation** champ . Pour plus d’informations, voir [Modifier les tâches](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).


   >[!IMPORTANT]
   >
   >  Seuls les cessionnaires des tâches peuvent mettre à jour la date de validation.

<!--old functionality in old commenting: 

1. Go to a task that you are assigned to for which you want to update the status.
1. Click the **Status** field in the task header and select a new status. 
1. (Optional) Do any of the following to provide additional information about the update, then click **Update** or, if the task has the **Complete** status, click **Done:**

   * To add a note about the update, go to the **Updates** area and click **Start a new update**, then type your note.  

   * To notify certain users about the update, type their names in the **Notify** box that appears when you type a note about the update. For more information, see [Tag others on updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md). 
   * To update the condition of the task, click **Select Condition** to the right of the **Notify** box (these appear when you type a note about the update), then select the condition that best reflects the current condition of the task.
   
   * To update the Commit Date of the task, expand the **Commit Date** drop-down calendar, and select a new Commit Date. 
   * To provide a visual indication of task completion, drag the bubble under Percent Complete or double-click it to enter a percent value.   
     ![](assets/drag-the-progress-bar-350x155.png)-->

## Mettre automatiquement à jour l’état de la tâche

Workfront met automatiquement à jour l’état existant d’une tâche vers un état différent lorsque les actions répertoriées dans le tableau ci-dessous se produisent.

>[!NOTE]
>
>Les états dans le tableau suivant sont les états système par défaut. Votre administrateur Workfront ou un administrateur de groupe peut renommer les états de votre instance de Workfront. Pour plus d’informations sur la création et la gestion des états dans Workfront, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Action</b></td> 
   <td><b>État d’origine</b></td> 
   <td><b>Nouveau statut</b></td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le pourcentage de la tâche terminé à 100 %</td> 
   <td>Nouveau ou en cours</td> 
   <td>Terminé</td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le pourcentage de tâches terminé de 100 % à un nombre inférieur</td> 
   <td>Terminé</td> 
   <td>En cours</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Cliquez sur le bouton Démarrer la tâche pour accepter de travailler sur une tâche qui vous est assignée.</span> </td> 
   <td><span>Nouveau</span> </td> 
   <td> <p>Tout état associé au bouton Démarrer la tâche dans les paramètres de votre équipe d’accueil.</p> <p>Pour plus d’informations sur le remplacement du bouton Travailler dessus par un bouton Démarrer la tâche, voir <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Remplacez le bouton Travailler dessus par un bouton Démarrer</a></span>.</p> <p>Conseil : <span>Cliquer</span> <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">Bouton Annuler</span>après avoir cliqué sur Démarrer la tâche, l’état devient Nouveau. </p> </td> 
  </tr> 
 </tbody> 
</table>
