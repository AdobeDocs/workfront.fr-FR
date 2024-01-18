---
product-area: projects
navigation-topic: update-work-in-a-project
title: Mettre à jour le statut du problème
description: Vous pouvez mettre à jour l’état d’un problème afin d’informer les autres personnes de son état et de son état d’avancement.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 2%

---

# Mettre à jour le statut du problème

<!--Audited: 01/2024-->

Vous pouvez mettre à jour l’état d’un problème afin d’informer les autres personnes de son état et de son état d’avancement.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td> <p>Nouvelle licence : contributeur ou version ultérieure</p>
   Ou
   <p>Licence actuelle : demande ou supérieure</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Modifier l’accès aux problèmes</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations liées au problème</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Statuts des problèmes

Voici les états par défaut des problèmes dans Workfront :

* Nouveau
* En cours
* Réaction en attente
* Suspendu
* Impossible de résoudre
* Rouvert
* Fermé
* Résolu

Votre administrateur Adobe Workfront peut ajouter des états personnalisés pour les problèmes de votre entreprise. Ils peuvent également rendre les états disponibles en fonction du type de problème.

Pour plus d’informations sur les états personnalisés et les types de problèmes, consultez les articles suivants :

* [Création ou modification d’un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [Création de problèmes](../../../manage-work/issues/manage-issues/create-issues.md)

Vous pouvez mettre à jour manuellement les statuts des problèmes ou laisser Workfront les mettre à jour automatiquement lorsque certaines actions ont lieu.

## Mise à jour manuelle de l’état des problèmes

Vous pouvez mettre à jour l’état du problème dans les zones suivantes de Workfront :

* En-tête du problème sur la page de la tâche.
* La boîte de dialogue Modifier le problème, lors de la modification d’un problème.
* La section Détails de la page de problème.
* Dans une liste de problèmes ou un rapport, lorsque le champ Statut est visible dans la vue.
* Dans le panneau Résumé du problème.

Pour mettre à jour manuellement l’état du problème dans l’en-tête du problème :

1. Accédez à un problème pour lequel vous souhaitez mettre à jour l’état.
1. Cliquez sur le bouton **État** dans l’en-tête du problème et sélectionnez un nouvel état.
1. Pour fournir une indication visuelle de la fin du problème, faites glisser ou double-cliquez sur la bulle sous **Pourcentage terminé** dans l’en-tête du problème

   Ou

   Cliquez à l’intérieur de la bulle dans l’en-tête de la question pour entrer un pourcentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Facultatif) Pour fournir des informations supplémentaires sur la mise à jour, effectuez l’une des opérations suivantes :

   * Pour ajouter une note à propos de la mise à jour, accédez au **Mises à jour** et cliquez sur **Nouveau commentaire**, puis saisissez une note.

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Pour avertir certains utilisateurs de la mise à jour, saisissez leurs noms dans le champ **Balisage de personnes ou d’équipes** qui apparaît lorsque vous saisissez un commentaire. Pour plus d’informations, voir [Balisage des autres sur les mises à jour](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Pour mettre à jour la date de validation du problème, cliquez sur **Détails du problème**, puis modifiez la variable **Date de validation** champ . Pour plus d’informations, voir [Modification des problèmes](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).


   >[!IMPORTANT]
   >
   >  Seuls les personnes désignées concernées peuvent mettre à jour la date de validation.



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

## Mettre automatiquement à jour l’état du problème

Workfront met automatiquement à jour l’état existant d’un problème à un état différent lorsque les actions répertoriées dans le tableau ci-dessous se produisent.

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
   <td>Mettre à jour le pourcentage de problèmes terminé à 100 %</td> 
   <td>Nouveau ou en cours</td> 
   <td>Fermé</td> 
  </tr> 
  <tr> 
   <td>Mettre à jour le pourcentage de problèmes terminé de 100 % à un nombre inférieur</td> 
   <td>Fermé </td> 
   <td>En cours</td> 
  </tr> 
  <tr> 
   <td>Mettre à jour l’état d’un objet de résolution associé au problème</td> 
   <td>Divers statuts</td> 
   <td> <p>Divers statuts</p> <p>Pour plus d’informations sur la résolution des objets et sur leur impact sur l’état des problèmes, voir la section "Synchronisation de l’état de l’objet résolvable avec celui de l’objet résolvable" dans l’article . <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Présentation de la résolution et des objets résolvables </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Cliquez sur le bouton Démarrer le problème pour accepter de travailler sur un problème qui vous est assigné.</span> </td> 
   <td><span>Nouveau</span> </td> 
   <td> <p>Tout état associé au bouton Démarrer le problème dans les paramètres de votre équipe d’accueil. </p> <p>Pour plus d’informations sur le remplacement du bouton Travailler dessus par un bouton Démarrer le problème, voir <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Remplacez le bouton Travailler dessus par un bouton Démarrer</a></span><span>.</span> </p> <p>Conseil : Cliquez sur <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">Bouton Annuler</span> après avoir cliqué sur Démarrer le problème, l’état devient Nouveau. </p> </td> 
  </tr> 
 </tbody> 
</table>
