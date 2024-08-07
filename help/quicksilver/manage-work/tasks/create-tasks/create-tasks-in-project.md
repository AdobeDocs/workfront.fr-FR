---
product-area: projects
navigation-topic: create-tasks
title: Créer des tâches dans un projet
description: Vous ne pouvez créer des tâches dans un projet qu’après avoir créé le projet.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 11%

---

# Créer des tâches dans un projet

<!-- Audited: 1/2024 -->

Vous ne pouvez créer des tâches dans un projet qu’après avoir créé le projet.

Par exemple, après avoir créé un projet, vous pouvez ajouter des tâches et les modifier pour organiser le plan du projet. Pour plus d’informations sur la création d’un projet, voir [Création d’un projet](../../../manage-work/projects/create-projects/create-project.md).

Pour plus d’informations sur la création de tâches personnelles qui ne font pas partie d’un projet, reportez-vous à la section [Créer une tâche personnelle](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task) de l’article [Créer des tâches à partir de la zone d’accueil](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

Cet article décrit comment créer des tâches à partir de zéro. Vous pouvez également créer des tâches de la manière suivante :

* En copiant ou en dupliquant des tâches existantes. Pour plus d’informations, voir [Copier et dupliquer les tâches](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* En déplaçant les tâches d’un projet à un autre. Pour plus d’informations, voir [Déplacer les tâches](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Licence Adobe Workfront</p> </td> 
   <td><p>Actuellement : Travail ou licence supérieure</p> 
   Ou
   <p>Nouvelle : standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux tâches et aux projets</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations Contribute pour le projet avec possibilité d’ajouter des tâches ou plus</p> <p>Lorsque vous créez une tâche, vous recevez automatiquement les autorisations Gérer pour la tâche.</p> <p> Pour plus d’informations sur les autorisations de tâche, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Partager une tâche </a>. </p> <p>Pour plus d'informations sur la demande d'autorisations supplémentaires, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d'accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer des tâches dans un projet

1. Accédez au projet dans lequel vous souhaitez créer une tâche.
1. Cliquez sur **Tâches** dans le panneau de gauche.
1. (Conditionnel) Si vous affichez actuellement la liste des tâches dans une vue agile, cliquez sur l’icône **Mode Liste** ![](assets/list-view-in-agile-view-for-tasks.png) dans le coin supérieur droit pour afficher la liste des tâches.
1. (Facultatif) Cliquez sur l’icône **Mode Plan** ![](assets/nwe-plan-mode-icon-task-list.png) et sélectionnez **Enregistrement manuel**, puis sélectionnez **Standard** ou **Planning**. Cette opération désactive l’option **Enregistrement automatique** activée par défaut.

   ![Sélectionner l’enregistrement manuel](assets/manual-save-option.png)

   >[!TIP]
   >
   >Vous pouvez annuler vos modifications lorsque vous sélectionnez Enregistrer manuellement.

1. Créez une nouvelle tâche en effectuant l’une des opérations suivantes :

   * Cliquez sur **Nouvelle tâche** en haut de la liste des tâches.
   * Cliquez sur **Ajouter d’autres tâches** au bas de la liste des tâches.

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (Conditionnel) Si vous avez cliqué sur **Nouvelle tâche**, procédez comme suit :

   1. Spécifiez l’un des champs de la liste limitée des champs dans la zone **Nouvelle tâche**, puis cliquez sur **Créer une tâche** si vous souhaitez créer rapidement une tâche.

      Ou

      Pour mettre à jour tous les champs de la tâche, cliquez sur **Plus d’options** pour ouvrir la boîte de dialogue **Créer une tâche**.

      ![](assets/nwe-create-task-small-screen-350x272.png)

      La zone **Créer une tâche** s’ouvre.

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >Selon la manière dont votre administrateur Workfront configure notre modèle de mise en page, les champs de la zone Créer une tâche peuvent afficher différents champs dans votre environnement. Pour plus d’informations, voir [Personnaliser la vue Détails à l’aide d’un modèle de disposition](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. Spécifiez les informations des zones suivantes dans le panneau de gauche de la zone Créer une tâche :

      * Nom de la tâche
      * Vue d’ensemble
      * Affectations
      * Formulaires personnalisés
      * Finances
      * Paramètres

        Pour plus d’informations sur la définition de tous les champs liés à une tâche, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   1. (Conditionnel et facultatif) Si vous souhaitez que la tâche soit récurrente, mettez à jour le champ **Fréquence de périodicité** . Pour plus d’informations sur la création de tâches récurrentes, voir [Créer des tâches récurrentes](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Facultatif) Cliquez sur **Documents** dans le panneau de gauche pour joindre un document à la nouvelle tâche, puis cliquez sur **Ajouter ou lier des fichiers** pour ajouter un document à la tâche depuis votre ordinateur, un autre service, ou pour lier des documents et des dossiers depuis votre ordinateur ou un autre service.

1. (Conditionnel) Si vous avez cliqué sur **Ajouter d’autres tâches** à l’étape 5, commencez à saisir les informations de la tâche à l’aide de la modification en ligne, puis appuyez sur Entrée.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Nous vous recommandons d’utiliser cette option, en particulier lors de l’ajout de plusieurs tâches à la liste.

   ![](assets/add-more-tasks-inline.png)

1. (Le cas échéant) Effectuez l’une des opérations suivantes :

   * Si vous avez cliqué sur **Nouvelle tâche** à l’étape 5, cliquez sur **Créer une tâche** pour enregistrer vos modifications et ajouter la nouvelle tâche à votre projet.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * Si vous avez cliqué sur **Ajouter d’autres tâches** à l’étape 5, procédez comme suit :

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. Cliquez n’importe où dans le navigateur pour envoyer les modifications ou appuyez sur Entrée.
      1. (Facultatif) Dans la liste des tâches, sélectionnez la tâche nouvellement créée, puis cliquez sur **Retrait**.

         Cela fait de la nouvelle tâche un enfant ou une sous-tâche de la tâche précédente.

         Pour plus d’informations sur les tâches enfants, voir [Créer des sous-tâches](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

      1. (Conditionnel) Si vous avez désactivé l’option **Enregistrement automatique** après avoir appuyé sur **Ajouter d’autres tâches**, vous pouvez effectuer les opérations suivantes :

         * Cliquez à tout moment sur **Annuler** pour annuler votre dernière modification ou sur **Annuler** pour annuler toutes les modifications apportées à la liste des tâches.
         * Si vous avez précédemment cliqué sur **Annuler**, cliquez sur **Rétablir** pour appliquer à nouveau la dernière modification que vous avez annulée.
         * Cliquez sur **Enregistrer** pour enregistrer vos modifications dans la liste des tâches.
