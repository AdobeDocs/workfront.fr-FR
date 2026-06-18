---
product-area: templates
navigation-topic: templates-navigation-topic
title: Créer un modèle de projet
description: Vous pouvez créer et supprimer des modèles à partir de la zone Modèles. Lorsque vous créez un modèle, vous pouvez saisir les informations pour toutes les tâches et pour les paramètres de votre futur projet. Ces informations seront ensuite transférées à tout projet que vous créerez à partir du modèle.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/JqR-bwIq1AVMOMz3aTWIKoiPep1VQ6IaONbbuDJ1AiA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1e6380b0422efdd98449ab1e74cadb4f330917f1
workflow-type: tm+mt
source-wordcount: 790
ht-degree: 48%

---

# Créer un modèle de projet

<!-- Audited: 10/2025 -->

<!--remove all instances of new/ old experience and redo the steps when the toggle is removed-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

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
   <td role="rowheader">Package Adobe Workfront</td> 
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

<!--
Old:
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
</table>
-->

## Créer un modèle

{{step1-to-templates}}

1. Cliquez sur **Nouveau modèle**.

1. (Conditionnel) Selon le stockage de document utilisé par votre organisation, cliquez sur l’un des éléments suivants :

   * **Nouveau modèle**, lorsque l’administrateur Workfront choisit l’un des paramètres suivants : **Espace de stockage dans le cloud Adobe** ou **Workfront hérité**, et qu’il a sélectionné ou non le paramètre **Autoriser l’utilisateur à sélectionner le fournisseur de stockage**.
   * **Nouveau modèle (stockage hérité)** lorsque l’administrateur Workfront choisit l’un des paramètres suivants : **Espace de stockage dans le cloud Adobe** ou **Workfront hérité**, et qu’il a également sélectionné le paramètre **Autoriser l’utilisateur à sélectionner le fournisseur de stockage**.

     Cette option s&#39;affiche uniquement lorsque le paramètre **Autoriser l&#39;utilisateur à sélectionner le fournisseur de stockage** est sélectionné dans la zone Configuration.

     Pour plus d’informations, voir [Activer l’espace de stockage dans le cloud Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

     Un modèle est créé et son nom par défaut suit les schémas suivants, en fonction du Workfront de stockage utilisé pour les documents :

      * **Modèle sans titre** pour un modèle de stockage Workfront.

        Un modèle de stockage Workfront hérité affiche une icône **Stockage Workfront hérité** ![Icône de projet de stockage hérité](assets/legacy-storage-project-icon.png) en regard de son nom.

      * **Modèle sans titre - &lt; Jour du mois, année heure.minute.seconde >** pour un modèle de stockage dans le cloud Adobe

        >[!IMPORTANT]
        >
        >Les modèles utilisant le stockage Adobe doivent avoir des noms uniques.

   ![Nouveau modèle](assets/create-template-nwe-2022-350x102.png)

1. Spécifiez un nom pour le nouveau modèle dans l’en-tête du modèle, puis appuyez sur **Entrée.**
1. Cliquez sur la section **Tâches du modèle** dans le panneau de gauche.
1. Cliquez sur **Commencer à ajouter des tâches de modèles** pour ajouter des tâches en ligne

   Ou

   Cliquez sur **Nouvelle tâche de modèle** pour commencer à ajouter des tâches à votre modèle dans la zone **Nouvelle tâche de modèle**.

   La zone **Créer une tâche de modèle** s&#39;ouvre lorsque vous cliquez sur **Nouvelle tâche de modèle**.

   ![Nouvelle expérience pour la nouvelle tâche de modèle](assets/new-template-task-box-unshimmed.png)

1. (Conditionnel) Mettez à jour les informations dans les zones suivantes de la zone **Créer une tâche de modèle** :

   * Nom de tâche de modèle
   * Vue d’ensemble
   * Affectations
   * Finances
   * Formulaires personnalisés
   * Documents
   * Paramètres

   La mise à jour des informations pour une tâche de modèle est similaire à la modification des tâches de modèle.

   Pour plus d’informations, voir [Modifier les tâches de modèle](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-template-task.md).

   >[!NOTE]
   >
   >Vous ne pouvez pas ajouter de tâches récurrentes à un modèle.

1. Cliquez sur **Créer une tâche de modèle**.

1. (Facultatif) Après avoir ajouté les tâches de modèle, dans la section **Tâches de modèles**, cliquez sur l’icône **Graphique Gantt** ![Icône Gantt](assets/gantt-icon.png) dans le coin supérieur droit de la liste des tâches pour afficher une représentation visuelle de la liste des tâches du modèle.

   >[!TIP]
   >
   >Vous ne pouvez pas modifier les tâches directement à partir d&#39;un modèle de tâche Diagramme de Gantt.

1. Pour ajouter des informations à votre nouveau modèle, cliquez sur le menu **Plus** ![icône Plus](assets/more-icon.png) à droite du nom du modèle dans l’en-tête, puis cliquez sur **Modifier**.

   Pour plus d’informations sur la modification d’un modèle, voir [Modifier les modèles de projet](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

   >[!NOTE]
   >
   >L’association d’un modèle de projet à un groupe (ou son absence) affecte la manière dont les préférences du projet, de la tâche et du problème déterminent certains paramètres du modèle.
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




