---
product-area: templates
navigation-topic: templates-navigation-topic
title: Créer un modèle de projet
description: Vous pouvez créer et supprimer des modèles à partir de la zone Modèles. Lorsque vous créez un modèle, vous pouvez saisir les informations pour toutes les tâches et pour les paramètres de votre futur projet. Ces informations seront ensuite transférées à tout projet que vous créerez à partir du modèle.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 46133f435c665dd82d134f18d0b5de4e70bab7d7
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 59%

---

# Créer un modèle de projet

<!-- Audited: 10/2025 -->

Vous pouvez créer et supprimer des modèles à partir de la zone Modèles. Lorsque vous créez un modèle, vous pouvez saisir les informations pour toutes les tâches et pour les paramètres de votre futur projet. Ces informations seront ensuite transférées à tout projet que vous créerez à partir du modèle.

>[!NOTE]
>
>Un modèle et ses tâches n’ont pas de dates réelles, mais plutôt une indication du jour (à partir duquel le futur projet pourrait démarrer) où une tâche pourrait démarrer et du jour où la tâche doit s’achever. Lors de l’utilisation de modèles pour créer les futurs projets, les projets recevront des dates réelles. Pour plus d’informations, voir [Créer un projet](../create-projects/create-project.md).


Vous pouvez créer un modèle des manières suivantes :

* En partant de zéro, comme décrit dans cet article.
* À partir de projets existants, en enregistrant un projet en tant que modèle.

  Pour plus d’informations sur la création de modèles à partir de projets existants, voir [Enregistrer un projet en tant que modèle](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* En le copiant à partir d’un autre modèle.

  Pour plus d’informations sur la copie d’un modèle existant, voir [Copier un modèle de projet](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* En important des plans directeurs. Vous devez être un administrateur ou une administratrice Workfront pour importer des plans directeurs. Pour plus d’informations, voir [Configurer un plan directeur](../../../administration-and-setup/blueprints/configure-template-package.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard </p><p>Plan</p> <p>Vous devez être un administrateur ou une administratrice système pour importer des modèles à partir de plans directeurs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux modèles</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Par défaut, vous avez le droit de gérer les modèles que vous créez.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Créer un modèle

{{step1-to-templates}}

1. Cliquez sur **Nouveau modèle**.

   Le modèle est sans titre.

   ![Nouveau modèle](assets/create-template-nwe-2022-350x102.png)

1. Spécifiez un nom pour le nouveau modèle dans l’en-tête du modèle, puis appuyez sur **Entrée.**
1. Cliquez sur la section **Tâches du modèle** dans le panneau de gauche.
1. Cliquez sur **Commencer à ajouter des tâches de modèles** pour ajouter des tâches en ligne

   Ou

   Cliquez sur **Nouvelle tâche de modèle** pour commencer à ajouter des tâches à votre modèle dans la zone **Nouvelle tâche de modèle**.

   ![Nouvelle zone de tâche de modèle](assets/new-template-task-box.png)

   <!--<span class="preview">The Create Template Task opens in the new experience.</span>-->

   <!--
   1. <span class="preview">(Conditional) Using the new experience, update information in the following areas in the **Create Template Task** box:</span>
   <div class="preview">
   * Template Task Name
   * Overview
   * Assignments
   * Finance
   * Custom Forms
   * Documents
   * Settings 
   </div>
   1. Click **Save**
   Or (*******remove the 1. from the step below and continue with those steps here*********)
   1. (Optional) Click **Switch back to old experience** at the bottom of the **Create Template Task** box.
   The **New Template Task** opens. (************add screen shot***********)-->

1. Mettez à jour les informations dans les zones suivantes de la zone **Nouvelle tâche de modèle** :

   * Vue d’ensemble
   * Finances
   * Paramètres
   * Affectations
   * Formulaires personnalisés
   * Joindre le document

     La mise à jour des informations d’une tâche de modèle est similaire à la modification des tâches d’un projet. Pour plus d&#39;informations, voir [Modifier les tâches](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md). <!--should this be relinked at preview/ prod release to say it's the same as Edit template tasks??-->

   >[!NOTE]
   >
   >Vous ne pouvez pas ajouter de tâches récurrentes à un modèle.

1. Cliquez sur l’une des options suivantes :

   * **Enregistrer la tâche de modèle** pour enregistrer la tâche de modèle en cours et ferme la boîte de dialogue Nouvelle tâche de modèle.
   * **Enregistrer la tâche de modèle et en démarrer une autre** pour enregistrer la tâche de modèle en cours et ouvrir une autre boîte de dialogue Nouvelle tâche de modèle pour ajouter une autre tâche.
   * **Annuler** pour fermer la boîte sans enregistrer la tâche de modèle.
1. (Facultatif) Après avoir ajouté les tâches de modèle, dans la section Tâches de modèle, cliquez sur l’icône **Diagramme de Gantt** dans le coin supérieur droit de la Liste des tâches pour afficher une représentation visuelle de la liste des tâches du modèle.

   >[!TIP]
   >
   >Vous ne pouvez pas modifier les tâches directement à partir de ce graphique de Gantt.

1. Pour ajouter des informations à votre nouveau modèle, cliquez sur le menu **Plus** ![icône Plus](assets/more-icon.png) à gauche du nom du modèle dans l’en-tête, puis cliquez sur **Modifier**.

   Pour plus d’informations sur la modification d’un modèle, voir [Modifier les modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

   >[!NOTE]
   >
   >   L’association d’un modèle de projet à un groupe (ou son absence) affecte la manière dont les préférences du projet, de la tâche et du problème déterminent certains paramètres du modèle.
   >
   >Pour plus d’informations, reportez-vous à la section « Application des préférences aux modèles et aux tâches de modèles » de l’article [Création et modification de modèles de projet d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

1. Cliquer sur **Enregistrer**.
1. (Facultatif) Ajoutez les éléments suivants au modèle

   * Documents
   * Risques
   * Processus d’approbation
   * Taux de facturation
   * Frais
   * Détails de la file d&#39;attente
   * Groupes de sujets et rubriques de file d’attente

1. (Facultatif) Ajoutez les éléments suivants aux tâches dans le modèle :

   * Documents
   * Frais
   * Approbations

   Pour plus d’informations, reportez-vous à la section « Ajouter d’autres éléments à un modèle » de l’article [&#x200B; Modifier les modèles de projet &#x200B;](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).




