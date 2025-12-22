---
product-area: projects
navigation-topic: create-tasks
title: Création de tâches dans un projet
description: Vous ne pouvez créer des tâches dans un projet qu’après avoir créé le projet.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 57%

---

# Créer des tâches dans un projet

<!-- Audited: 10/2024 -->

Vous pouvez créer des tâches dans Adobe Workfront des manières suivantes :

* Créez entièrement une tâche dans un projet, une fois le projet créé.

  Après avoir créé un projet, vous pouvez ajouter des tâches et les modifier pour organiser le plan du projet. Pour en savoir plus sur la création d’un projet, voir [Créer un projet](../../../manage-work/projects/create-projects/create-project.md).

* Créez des tâches en ajoutant un modèle à un projet.

  Pour plus d’informations, voir [Joindre un modèle à un projet](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Créez des tâches personnelles et déplacez-les vers un projet.

  Vous pouvez créer des tâches personnelles en effectuant l’une des opérations suivantes :

   * Créer une demande de travail ad hoc et l’envoyer à un utilisateur
   * Création d’une tâche dans la zone d’Accueil

  Pour plus d&#39;informations sur la création de tâches personnelles ne faisant pas partie d&#39;un projet, voir [Créer des tâches personnelles](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

  Vous pouvez déplacer des tâches personnelles vers un projet et elles deviennent des tâches de travail.

Cet article décrit comment créer des tâches à partir de zéro et comment déplacer des tâches personnelles vers un projet.

Vous pouvez également créer des tâches de la manière suivante :

* En copiant ou en dupliquant des tâches existantes. Pour plus d’informations, voir [Copier et dupliquer des tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* En déplaçant les tâches d’un projet à un autre. Pour plus d’informations, voir [Déplacer des tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

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
   <p>Travail ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux tâches et aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribuer pour le projet avec la capacité d’ajouter des tâches ou autorisations supérieures</p> 
   <p>Lorsque vous créez une tâche, vous recevez automatiquement des autorisations de gestion de la tâche.</p> 
    </td> 
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
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license</p> </td> 
   <td><p>Standard</p> 
   <p>Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects. </a></p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Créer des tâches dans un projet

La création de tâches dans un projet est similaire à la création de tâches sur un modèle. Vous pouvez suivre les étapes décrites ci-dessous lors de l’ajout de tâches de modèle à un modèle.

Pour créer des tâches dans un projet :

1. Accédez au projet dans lequel vous souhaitez créer une tâche.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. (Conditionnel) Si vous affichez actuellement la liste des tâches dans une vue Agile, cliquez sur l’icône **Vue Liste** ![](assets/list-view-in-agile-view-for-tasks.png) dans le coin supérieur droit pour afficher la liste des tâches.
1. (Facultatif) Cliquez sur l’icône **Mode Plan** ![](assets/nwe-plan-mode-icon-task-list.png) et sélectionnez **Enregistrement manuel**, puis sélectionnez **Standard** ou **Planification chronologique**. Cette opération désactive l’option **Enregistrement automatique** qui est activée par défaut.

   ![Sélectionner Enregistrement manuel](assets/manual-save-option.png)

   >[!TIP]
   >
   >Vous pouvez annuler vos modifications lorsque vous sélectionnez Enregistrement manuel.

1. Créez une nouvelle tâche en effectuant l’une des opérations suivantes :

   * Cliquez sur **Nouvelle tâche** en haut de la liste de tâches.
   * Cliquez sur **Ajouter d’autres tâches** en bas de la liste de tâches.

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (Conditionnel) Si vous avez cliqué sur **Nouvelle tâche** procédez comme suit :

   1. Spécifiez l’un des champs de la liste limitée de champs dans la zone **Nouvelle tâche**, puis cliquez sur **Créer une tâche** si vous souhaitez créer rapidement une tâche.

      Ou

      Pour mettre à jour tous les champs de la tâche, cliquez sur **Plus d’options** pour ouvrir la boîte de dialogue **Créer une tâche**.

      ![](assets/nwe-create-task-small-screen-350x272.png)

      La boîte de dialogue **Créer une tâche** s’ouvre.

      ![](assets/create-task-larger-box-nwe-350x244.png)


      >[!NOTE]
      >
      >Selon la manière dont votre administrateur ou administratrice Workfront configure notre modèle de mise en page, les champs de la boîte de dialogue Créer une tâche peuvent afficher différents champs dans votre environnement. Pour plus d’informations, voir [Personnaliser la vue Détails à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. Spécifiez les informations des zones suivantes dans le panneau de gauche de la boîte de dialogue Créer une tâche :

      * Nom de la tâche
      * Vue d’ensemble
      * Affectations
      * Formulaires personnalisés
      * Finances
      * Paramètres

        Pour plus d’informations sur la définition de tous les champs liés à une tâche, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   1. (Le cas échéant et facultatif) Si vous souhaitez que la tâche soit récurrente, mettez à jour le champ **Fréquence de périodicité**. Pour plus d’informations sur la création de tâches récurrentes, voir [Créer des tâches récurrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Facultatif) Cliquez sur **Documents** dans le panneau de gauche pour joindre un document à la nouvelle tâche, puis sur **Ajouter ou lier des fichiers** pour ajouter un document à la tâche à partir de votre ordinateur, d’un autre service ou pour lier des documents et des dossiers à partir de votre ordinateur ou d’un autre service.

1. (Le cas échéant) Si vous avez cliqué sur **Ajouter des tâches** à l’étape 5, commencez à saisir les informations de la tâche en les modifiant en ligne, puis appuyez sur Entrée.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Nous vous recommandons d’utiliser cette option, en particulier lors de l’ajout de plusieurs tâches à la liste.

   ![](assets/add-more-tasks-inline.png)

1. (Le cas échéant) Utilisez l’une des méthodes suivantes :

   * Si vous avez cliqué sur **Nouvelle tâche** à l’étape 5, cliquez sur **Créer la tâche** pour enregistrer vos modifications et ajouter la nouvelle tâche à votre projet.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * Si vous avez cliqué sur **Ajouter des tâches** à l’étape 5, procédez comme suit :

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. Cliquez n’importe où dans le navigateur pour soumettre les modifications ou appuyez sur Entrée.
      1. (Facultatif) Dans la liste des tâches, sélectionnez la tâche que vous venez de créer, puis cliquez sur **Retrait**.

         Cela fait de la nouvelle tâche un enfant ou une sous-tâche de la tâche précédente.

         Pour plus d&#39;informations sur les tâches enfants, reportez-vous à la section « Créer des sous-tâches à partir de la section Tâches subordonnées » de l&#39;article [Créer des sous-tâches](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

      1. (Le cas échéant) Si vous avez désactivé l’option **Enregistrement automatique** après avoir appuyé sur **Ajouter des tâches**, vous pouvez effectuer les opérations suivantes :

         * Cliquez sur **Annuler la modification** à tout moment pour annuler votre dernière modification, ou sur **Annuler** pour annuler toutes les modifications que vous avez apportées à la liste des tâches.
         * Si vous avez cliqué précédemment sur **Annuler la modification**, cliquez sur **Rétablir** pour appliquer à nouveau la dernière modification que vous avez annulée.
         * Cliquez sur **Enregistrer** pour enregistrer vos modifications de la liste des tâches.
   1. (Facultatif) Dans une liste de tâches, cliquez sur la section **Prédécesseur** pour ajouter des prédécesseurs à la tâche. Pour plus d&#39;informations, voir [Créer une relation de prédécesseur à l&#39;aide de la zone Prédécesseurs](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
   1. (Facultatif) Dans une liste de tâches, cliquez sur la section **Sous-tâches** pour ajouter des tâches enfants. Pour plus d’informations, voir [Créer des sous-tâches](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

## Créer des tâches en déplaçant une tâche personnelle vers un projet

1. (Sous condition) Assurez-vous que vous ou d’autres utilisateurs avez créé des tâches personnelles.

   Pour plus d’informations, voir [Créer des tâches personnelles](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).
1. Créez un filtre de tâche personnel et appliquez-le à un rapport ou à une liste de tâches.

   Pour plus d’informations, voir [Filtrer : tâches personnelles](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md).

   ![](assets/personal-tasks-report.png)
1. Cliquez sur le nom d&#39;une tâche dans le rapport personnel des tâches pour l&#39;ouvrir.

   Workfront enregistre les tâches personnelles dans un projet personnel non répertorié toujours nommé selon ce modèle : « &lt; Nom complet de l’utilisateur > Tâches de . Par exemple, un projet personnel peut être nommé « Tâches de Rick ».

1. Sur la page de la tâche, cliquez sur le **** Plus![](assets/more-icon.png), puis sur **Déplacer**. Pour plus d’informations sur le déplacement de tâches, voir [Déplacer des tâches](/help/quicksilver/manage-work/tasks/manage-tasks/move-tasks.md).

   Une fois que vous avez déplacé la tâche, elle s’affiche dans le projet que vous avez sélectionné. La chronologie du projet peut être affectée par la chronologie de la nouvelle tâche.
