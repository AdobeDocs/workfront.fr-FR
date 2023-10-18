---
product-area: projects
navigation-topic: update-work-in-a-project
title: Mettre à jour le statut des tâches
description: Vous pouvez mettre à jour l’état d’une tâche pour informer les autres personnes sur l’emplacement de la tâche (et sur le projet global) et son état d’avancement.
author: Alina
feature: Work Management
exl-id: e1efc676-e110-486e-91dc-f521421575e8
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 1%

---

# Mettre à jour le statut des tâches

Vous pouvez mettre à jour l’état d’une tâche pour informer les autres personnes sur l’emplacement de la tâche (et sur le projet global) et son état d’avancement.

Les états par défaut sont Nouveau, En cours et Terminé. Votre administrateur Adobe Workfront peut ajouter des statuts personnalisés à votre organisation. Pour plus d’informations, voir [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Vous pouvez mettre à jour manuellement les états des tâches ou laisser Workfront les mettre à jour automatiquement lorsque certaines actions ont lieu.

## Exigences d’accès

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

## Observations relatives à la mise à jour de l’état des tâches

* Lorsque vous marquez une tâche comme terminée, le pourcentage d’achèvement de la tâche passe à 100 %.
* Les scénarios suivants existent pour les tâches parentes :
   * Vous ne pouvez pas mettre à jour l’état d’une tâche parente sur Terminé lorsque le mode d’achèvement du résumé du projet est défini sur Automatique et que les sous-tâches ne sont pas terminées.
   * Vous pouvez mettre à jour l’état d’une tâche parente sur Terminé lorsque le mode d’achèvement du résumé du projet est défini sur Manuel et que les sous-tâches sont terminées ou incomplètes.

  Pour plus d’informations, voir [Modification de projets](../manage-projects/edit-projects.md).

## Mise à jour manuelle de l’état de la tâche

Lorsque vous mettez à jour l’état d’une tâche, vous pouvez également saisir une explication sur le nouvel état et modifier d’autres informations sur la tâche, telles que la date d’échéance.

1. Accédez à une tâche à laquelle vous êtes affecté et pour laquelle vous souhaitez mettre à jour l’état.
1. Cliquez sur le bouton **État** dans l’en-tête de la tâche et sélectionnez un nouvel état.
1. (Facultatif) Pour fournir des informations supplémentaires sur la mise à jour, effectuez l’une des opérations suivantes, puis cliquez sur **Mettre à jour** ou, si la tâche a la propriété **Terminer** état, cliquez sur **Terminé :**

   * Pour ajouter une note à propos de la mise à jour, accédez au **Mises à jour** zone et clic **Démarrer une nouvelle mise à jour**, puis saisissez votre note.

   * Pour avertir certains utilisateurs de la mise à jour, saisissez leurs noms dans le champ **Notifier** qui s’affiche lorsque vous saisissez une note à propos de la mise à jour. Pour plus d’informations, voir [Balisage des autres sur les mises à jour](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Pour mettre à jour la condition de la tâche, cliquez sur **Sélectionner la condition** à droite du **Notifier** (elles s’affichent lorsque vous tapez une note sur la mise à jour), puis sélectionnez la condition qui reflète le mieux la condition actuelle de la tâche.

   * Pour mettre à jour la date de validation de la tâche, développez la variable **Date de validation** du calendrier déroulant, puis sélectionnez une nouvelle date de validation.
   * Pour fournir une indication visuelle de la fin de la tâche, faites glisser la bulle sous Pourcentage terminé ou double-cliquez dessus pour saisir une valeur de pourcentage.\
     ![](assets/drag-the-progress-bar-350x155.png)

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
   <td>Action</td> 
   <td>État d’origine</td> 
   <td>Nouveau statut</td> 
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
