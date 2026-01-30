---
product-area: projects
navigation-topic: update-work-in-a-project
title: Mettre à jour le statut de l'événement
description: Vous pouvez mettre à jour le statut d’un problème pour informer les autres personnes de son état d’avancement et de son évolution.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 97%

---

# Mettre à jour le statut du problème

<!--Audited: 01/2024-->

Vous pouvez mettre à jour le statut d’un problème pour informer les autres personnes de son état d’avancement et de son évolution.

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
   <td> <p>Contributeur ou version ultérieure</p>
   <p>Requête ou supérieure</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations liées aux problèmes</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>New: Contributor or higher</p>
   Or
   <p>Current: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Statuts des problèmes

Les statuts par défaut des problèmes dans Workfront sont les suivants :

* Nouveau
* En cours
* En attente de feedback
* Suspendu
* Impossible de résoudre
* Rouvert
* Fermé
* Résolu

Votre équipe d’administration Adobe Workfront peut ajouter des statuts personnalisés pour les problèmes de votre organisation. Elle peut également rendre les statuts disponibles en fonction du type de problème.

Pour plus d’informations sur les statuts personnalisés et les types de problèmes, voir les articles suivants :

* [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [Créer des problèmes](../../../manage-work/issues/manage-issues/create-issues.md)

Vous pouvez mettre à jour les statuts des problèmes manuellement ou laisser Workfront les mettre à jour automatiquement lorsque certaines actions ont lieu.

## Mettre à jour manuellement le statut du problème

Vous pouvez mettre à jour le statut du problème dans les zones suivantes de Workfront :

* L’en-tête du problème sur la page de la tâche.
* La zone Modifier le problème, lors de la modification d’un problème.
* La section Détails de la page du problème.
* Dans une liste de problèmes ou un rapport, lorsque le champ Statut est visible dans la vue.
* Dans le panneau Résumé du problème.

Pour mettre à jour manuellement le statut du problème dans l’en-tête du problème, procédez comme suit :

1. Accédez à un problème dont vous souhaitez mettre à jour le statut.
1. Cliquez sur le champ **Statut** dans l’en-tête du problème et sélectionnez un nouveau statut.
1. Pour obtenir une indication visuelle de l’avancement du problème, faites glisser la bulle située sous **Pourcentage terminé** dans l’en-tête du problème ou double-cliquez dessus.

   Ou

   Cliquez à l’intérieur de la bulle, dans l’en-tête du problème, pour saisir un pourcentage.

   ![Mettre à jour le pourcentage de tâche terminé dans l’en-tête](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Facultatif) Effectuez l’une des opérations suivantes pour fournir des informations supplémentaires sur la mise à jour :

   * Pour ajouter une note à propos de la mise à jour, accédez à la section **Mises à jour**, cliquez sur **Nouveau commentaire**, puis saisissez une note.

     ![Boîte de message de flux de mise à jour du problème](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Pour informer certaines personnes de la mise à jour, saisissez leur nom dans le champ **Taguer des personnes ou des équipes** qui s’affiche lorsque vous saisissez un commentaire. Pour plus d’informations, voir la section [Mentionner d’autres personnes sur les mises à jour](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Pour mettre à jour la date d’engagement du problème, cliquez sur **Détails du problème**, puis modifiez le champ **Date d’engagement**. Pour plus d’informations, voir [Modifier des problèmes](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).


   >[!IMPORTANT]
   >
   >  Seules les personnes à qui des problèmes sont affectés peuvent mettre à jour la date d’engagement.



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![Issue status expanded in header](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![Update task percent in header](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

## Mettre à jour automatiquement le statut du problème

Workfront met automatiquement à jour le statut actuel d’un problème avec un statut différent lorsque les actions énumérées dans le tableau ci-dessous se produisent.

>[!NOTE]
>
>Les statuts présentés dans le tableau suivant sont des statuts système par défaut. Votre équipe d’administration Workfront ou une équipe d’administration de groupe peut renommer les statuts de votre instance Workfront. Pour plus d’informations sur la création et la gestion des statuts dans Workfront, voir [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Action</b></td> 
   <td><b>Statut d’origine</b></td> 
   <td><b>Nouveau statut</b></td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le pourcentage terminé du problème à 100 %</td> 
   <td>Nouveau ou en cours</td> 
   <td>Fermé</td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le pourcentage terminé du problème de 100 % à un nombre inférieur</td> 
   <td>Fermé </td> 
   <td>En cours</td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le statut d’un objet de résolution associé au problème</td> 
   <td>Divers statuts</td> 
   <td> <p>Divers statuts</p> <p>Pour plus d’informations sur les objets de résolution et sur leur incidence sur le statut des problèmes, voir la section « Synchroniser le statut de l’objet résolvable avec celui de l’objet de résolution » dans l’article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Vue d’ensemble des objets résolvables et de résolution</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Cliquez sur le bouton Démarrer le problème pour accepter de travailler sur un problème qui vous a été attribué.</span> </td> 
   <td><span>Nouveau</span> </td> 
   <td> <p>Tout statut associé au bouton Démarrer le problème dans vos paramètres de l’équipe principale. </p> <p>Pour plus d’informations sur le remplacement du bouton Travailler sur cette tâche par un bouton Démarrer le problème, voir la section <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Remplacer le bouton Travailler sur cette tâche par un bouton Démarrer</a></span><span>.</span> </p> <p>Astuce : le fait de cliquer sur <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">le bouton Annuler</span> après avoir cliqué sur Démarrer le problème rétablit le statut sur Nouveau. </p> </td> 
  </tr> 
 </tbody> 
</table>
