---
product-area: projects
navigation-topic: create-tasks
title: Création de tâches dans un projet
description: Vous ne pouvez créer des tâches dans un projet qu’après avoir créé le projet.
author: Alina
feature: Work Management
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: f8d596121f90d4f0c57e65cc415d1df87c14730c
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 1%

---

# Création de tâches dans un projet

Vous ne pouvez créer des tâches dans un projet qu’après avoir créé le projet.

Par exemple, après avoir créé un projet, vous pouvez ajouter des tâches et les modifier pour organiser le plan du projet. Pour plus d’informations sur la création d’un projet, voir [Création d’un projet](../../../manage-work/projects/create-projects/create-project.md).

Pour plus d’informations sur la création de tâches personnelles qui ne figurent pas dans un projet, voir la section &quot;Créer une tâche personnelle&quot; de l’article. [Création d’éléments de travail à partir de la zone Accueil](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

Cet article décrit comment créer entièrement des tâches. Vous pouvez également créer des tâches de la manière suivante :

* En copiant ou en dupliquant des tâches existantes. Pour plus d’informations, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* En déplaçant les tâches d’un projet à un autre. Pour plus d’informations, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Exigences d’accès

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td><p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Licence Adobe Workfront*</p> </td> 
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur l’accès aux tâches, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Accorder l’accès aux tâches</a>. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Attribuez des autorisations au projet avec la possibilité d’ajouter des tâches ou plus.</p> <p>Lorsque vous créez une tâche, vous recevez automatiquement les autorisations Gérer pour la tâche.</p> <p> Pour plus d’informations sur les autorisations de tâche, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Partage d’une tâche </a>. </p> <p>Pour plus d’informations sur la demande d’autorisations supplémentaires, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Création de tâches dans un projet

1. Accédez au projet dans lequel vous souhaitez créer une tâche.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. (Conditionnel) Si vous affichez actuellement la liste des tâches dans une vue agile, cliquez sur le bouton **Mode Liste** icon ![](assets/list-view-in-agile-view-for-tasks.png) dans le coin supérieur droit pour afficher la liste des tâches.
1. (Facultatif) Cliquez sur le **Mode Plan** icon ![](assets/nwe-plan-mode-icon-task-list.png) et sélectionnez **Enregistrement manuel**, puis sélectionnez **Standard** ou **Planification de la chronologie**. Cette opération désactive la fonction **Enregistrement automatique** qui est activée par défaut.

   ![](assets/nwe-autosave-off-manual-highlighted-350x58.png)

   >[!TIP]
   >
   >Vous pouvez annuler vos modifications lorsque vous sélectionnez Enregistrer manuellement.

1. Créez une tâche en effectuant l’une des opérations suivantes :

   * Cliquez sur **Nouvelle tâche** en haut de la liste des tâches
   * Cliquez sur **Ajout de tâches** en bas de la liste des tâches

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (Conditionnel) Si vous avez cliqué sur **Nouvelle tâche** procédez comme suit :

   1. Spécifiez l’un des champs de la liste limitée des champs dans la variable **Nouvelle tâche** , puis cliquez sur **Créer une tâche** si vous souhaitez créer rapidement une tâche.

      Ou

      Pour mettre à jour tous les champs de la tâche, cliquez sur **Plus d’options** pour ouvrir le **Créer une tâche** de la boîte.

      ![](assets/nwe-create-task-small-screen-350x272.png)

      Le **Créer une tâche** s’ouvre.

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >Selon la manière dont votre administrateur Workfront configure notre modèle de mise en page, les champs de la zone Créer une tâche peuvent afficher différents champs dans votre environnement. Pour plus d’informations, voir [Personnalisation de la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. Spécifiez les informations des zones suivantes dans le panneau de gauche de la zone Créer une tâche :

      * Nom de la tâche
      * Vue d’ensemble
      * Affectations
      * Formulaires personnalisés
      * Finances
      * Paramètres

        Pour plus d’informations sur la définition de tous les champs liés à une tâche, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   1. (Conditionnel et facultatif) Si vous souhaitez que la tâche soit récurrente, mettez à jour la variable **Fréquence de périodicité** champ . Pour plus d’informations sur la création de tâches récurrentes, voir [Créer des tâches récurrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Facultatif) Cliquez sur **Documents** dans le panneau de gauche pour joindre un document à la nouvelle tâche, puis cliquez sur **Ajouter ou lier des fichiers** pour ajouter un document à la tâche à partir de votre ordinateur, d’un autre service ou pour lier des documents et des dossiers à partir de votre ordinateur ou d’un autre service.

1. (Conditionnel) Si vous avez cliqué sur **Ajout de tâches** à l’étape 5, commencez à saisir les informations de la tâche en les éditant en ligne, puis appuyez sur Entrée.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Nous vous recommandons d’utiliser cette option, en particulier lors de l’ajout de plusieurs tâches à la liste.

   ![](assets/ctp4-350x26.png)

1. (Conditionnel) Effectuez l’une des opérations suivantes :

   * Si vous avez cliqué **Nouvelle tâche** à l’étape 5, cliquez sur **Créer une tâche** pour enregistrer vos modifications et ajouter la nouvelle tâche à votre projet.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * Si vous avez cliqué **Ajout de tâches** à l’étape 5, procédez comme suit :

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. Cliquez n’importe où dans le navigateur pour envoyer les modifications ou appuyez sur Entrée.
      1. (Facultatif) Dans la liste des tâches, sélectionnez la tâche nouvellement créée, puis cliquez sur **Retrait**.

         Cela fait de la nouvelle tâche un enfant ou une sous-tâche de la tâche précédente.

         Pour plus d’informations sur les tâches pour enfants, voir [Présentation des tâches](../../../manage-work/tasks/task-information/tasks-overview.md).

      1. (Conditionnel) Si vous avez désactivé la variable **Enregistrement automatique** option après avoir appuyé **Ajout de tâches**, vous pouvez effectuer les opérations suivantes :

         * Cliquez sur **Annuler** à tout moment pour annuler votre dernière modification, ou **Annuler** pour annuler toutes les modifications que vous avez apportées à la liste des tâches.
         * Si vous avez cliqué précédemment **Annuler**, cliquez sur **Rétablir** pour appliquer à nouveau la dernière modification que vous avez annulée.
         * Cliquez sur **Enregistrer** pour enregistrer vos modifications dans la liste des tâches.
