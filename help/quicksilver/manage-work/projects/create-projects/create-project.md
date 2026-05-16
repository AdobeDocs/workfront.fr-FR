---
product-area: projects
navigation-topic: create-projects
title: Créer un projet
description: Un projet est une grande unité de travail dans Adobe Workfront. Vous pouvez créer des projets à partir de zéro, utiliser un modèle ou convertir des problèmes ou des tâches en projets.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '1639'
ht-degree: 65%

---

# Créer un projet

<!--remove Preview and Production references-->

<!-- Audited: 110/2025 -->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Les projets représentent une grande quantité de travail à effectuer dans Adobe Workfront.

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
        <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Lorsque vous créez un projet, vous recevez automatiquement les autorisations de gestion du projet.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
        <p>or</p>
        <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project, you automatically receive Manage permissions to the project.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->


## Méthodes de création de projets

Vous pouvez créer un projet dans Workfront à l’aide de l’une des méthodes suivantes :

* Créez un projet à partir de zéro sans utiliser de modèle. Cet article décrit comment créer un projet à partir de zéro.

* Copiez un projet existant.\
  Pour plus d’informations sur la copie d’un projet, voir [ Copier un projet ](../../../manage-work/projects/manage-projects/copy-project.md).

* Utilisez un modèle.\
  Pour plus d’informations sur l’utilisation d’un modèle pour créer un projet, consultez la section [Créer un projet à l’aide d’un modèle](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Importer un projet à partir de Microsoft Project.\
  Pour plus d’informations sur l’import d’un projet à partir de Microsoft Project, consultez la section [Importer un projet à partir de Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importer un projet à l’aide de Kickstarts.

  En tant qu’administrateur ou administratrice Workfront, vous pouvez importer des projets à l’aide d’un Kickstart.

  Pour plus d’informations sur l’import de données à l’aide de Kickstarts dans Workfront, consulter la section [Importer des données dans Adobe Workfront à l’aide d’un modèle de Kickstart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  Pour plus d’informations sur l’import de projets à l’aide de Kickstarts, consultez la section [Scénario Kickstart : préparer simplement l’import de projets et de tâches](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Publiez une initiative à partir d’un scénario dans le Planificateur de scénarios Adobe Workfront.

  Pour plus d’informations sur le planificateur de scénarios Workfront, voir [Vue d’ensemble du planificateur de scénarios](../../../scenario-planner/scenario-planner-overview.md).

  Pour plus d’informations sur la création de projets à partir de la publication d’initiatives, consultez la section [Mettre à jour ou créer des projets en publiant des initiatives dans le planificateur de scénarios](../../../scenario-planner/publish-scenarios-update-projects.md).

* Ajoutez des projets au fur et à mesure que vous les connectez à partir d’un type d’enregistrement dans Workfront Planning.

  Pour plus d’informations sur l’accès à Workfront Planning, voir [Présentation de l’accès](/help/quicksilver/planning/access/access-overview.md).

  Pour plus d’informations sur la création de projets en les ajoutant à des enregistrements, reportez-vous à la section « Créer des projets lors de leur connexion avec des enregistrements de Workfront Planning » de l’article [Créer des objets Workfront à partir de Workfront Planning lorsque vous les connectez à des enregistrements](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)

## Conditions préalables

Avant de commencer, vous devez vous assurer de ce qui suit :

* L’équipe d’administration du système ou de groupes a activé dans la zone de configuration la préférence « Autoriser les utilisateurs et les utilisatrices à créer des projets sans utiliser de modèle ».

  Pour plus d’informations, consultez la section [Configurer des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Nouveaux paramètres par défaut du projet

Lorsque vous créez un projet, Workfront lui applique un ensemble de paramètres par défaut. Par exemple, les modes Statut, Groupe et Planning sont prédéfinis lors de la création d’un projet.

Tenez compte des points suivants :

* En tant qu’équipe d’administration de Workfront ou de groupes, vous avez la possibilité de configurer les paramètres par défaut d’un nouveau projet lors de la configuration des préférences du projet pour votre instance Workfront ou pour un groupe.
* Workfront applique les paramètres du groupe, le cas échéant, avant d’appliquer ceux définis par l’équipe d’administration de Workfront.
* Le statut par défaut d’un nouveau projet correspond à celui défini soit par un administrateur ou une administratrice Workfront dans la zone principale des préférences du projet, soit par un administrateur ou une administratrice de groupes (ou l’administration Workfront) dans la zone des préférences du projet spécifique à ce groupe.

  >[!NOTE]
  >
  >Nous recommandons que le statut par défaut d’un nouveau projet soit Planification. Lorsque vous apportez des modifications au nouveau projet, les notifications ne sont pas envoyées aux utilisateurs et aux utilisatrices à qui le projet a été affecté.
  >
  >Pour plus d’informations sur la configuration du statut et d’autres paramètres par défaut pour un nouveau projet, consultez la section [Configurer des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [Configurer des préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* Les scénarios suivants sont possibles pour la manière dont Workfront définit le groupe et statut d’un nouveau projet :

   * Si vous créez un projet à partir de zéro, le groupe du projet est votre groupe interne.

     Le statut du projet est le statut par défaut dans les préférences du projet de votre groupe interne, le cas échéant, ou de votre instance Workfront. Vous pouvez définir le statut par défaut lors de la création du projet sur n’importe quel statut disponible pour le groupe du projet.

   * Si vous créez un projet à l’aide d’un modèle, les paramètres du modèle prévalent sur ceux définis par l’administrateur ou l’administratrice Workfront ou de groupes.

     Le groupe du nouveau projet est le groupe du modèle. Si le modèle n’est pas associé à un groupe, le groupe du projet est le groupe principal de l’utilisateur ou de l’utilisatrice qui crée le projet.

     Le statut par défaut d’un nouveau projet créé à partir d’un modèle correspond au statut défini par votre administrateur ou administratrice Workfront dans la zone principale Préférences du projet ou par un administrateur ou une administratrice de groupes (ou Workfront) dans la zone Préférences du projet du groupe. Vous pouvez modifier le statut par défaut lors de la création d’un projet à partir d’un modèle, en n’importe quel statut du groupe du projet qui est soit le groupe du modèle, soit le groupe interne de la personne qui crée le projet.

   * Si vous créez un projet en convertissant un problème, le groupe d’un nouveau projet est le groupe du projet existant du problème. Si la personne qui convertit la problème n’a pas accès au projet du problème, ou si le projet du problème ne comporte pas de groupe, le groupe du nouveau projet est le groupe interne de la personne qui convertit le problème.

     Les statuts du nouveau projet correspondent aux statuts du groupe associé au projet, qui est soit le groupe du projet d’origine, soit le groupe principal de la personne qui convertit le problème.

     Si vous utilisez un modèle lors de la création du projet en convertissant le problème, reportez-vous au deuxième scénario ci-dessus pour comprendre quel groupe et quel statut sont appliqués par Workfront au nouveau projet.

* L’emplacement de stockage des documents pour un projet et ses objets enfants (tâches et événements) dépend de ce que l’administrateur Workfront choisit comme valeur par défaut pour les Préférences de stockage dans les Préférences système de la section Configuration. Selon l’emplacement de stockage des documents dans votre instance Workfront, vous pouvez créer les types de projets suivants :

   * Projets de stockage Workfront hérités
   * projets de stockage dans le cloud Adobe.

  Pour plus d’informations, voir [Activer l’espace de stockage dans le cloud Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

  >[!TIP]
  >
  > Votre instance Workfront peut ne pas avoir les deux types de stockage de documents.

* Lorsque vous créez un projet d’espace de stockage dans le cloud Adobe, un dossier de documents portant le même nom que le projet est créé dans la section **Documents** du projet. Après avoir ajouté des tâches au projet, les dossiers portant le nom de la tâche sont ajoutés à la section **Documents** de chaque tâche.

Pour plus d’informations, voir [Présentation de la gestion des documents pour les projets et les objets associés](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).

## Créer entièrement un projet

>[!NOTE]
>
>Si vous créez un projet à l’aide d’un modèle, il est recommandé de consulter également l’article [Créer un projet à l’aide d’un modèle](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur **Projets** et développez **Nouveau projet**.
   * Accédez à un portfolio, puis développez **Nouveau projet**.
   * Accédez à un programme, puis développez **Nouveau projet**.
   * Si vous êtes administrateur ou administratrice de groupes, vous pouvez également créer un projet dans la section Projets d’un groupe que vous gérez. Pour plus d’informations, voir [Créer et modifier des projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![Menu Nouveau projet](assets/new-project-drop-down-with-legacy-storage-option.png)

1. (Conditionnel) Selon le stockage de document utilisé par votre organisation, cliquez sur l’un des éléments suivants :

   * **Nouveau projet**, lorsque l’administrateur Workfront choisit l’un des paramètres suivants : **Espace de stockage dans le cloud Adobe** ou **Workfront hérité**, et qu’il a sélectionné ou non le paramètre **Autoriser l’utilisateur à sélectionner le fournisseur de stockage**.
   * **Nouveau projet (stockage hérité)** lorsque l’administrateur Workfront choisit l’un des paramètres suivants : **Espace de stockage dans le cloud Adobe** ou **Workfront hérité**, et qu’il a également sélectionné le paramètre **Autoriser l’utilisateur à sélectionner le fournisseur de stockage**.

     Cette option s&#39;affiche uniquement lorsque le paramètre **Autoriser l&#39;utilisateur à sélectionner le fournisseur de stockage** est sélectionné dans la zone Configuration.

     Pour plus d’informations, voir [Activer l’espace de stockage dans le cloud Adobe pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

     >[!NOTE]
     >
     >* Lorsque vous créez un projet de stockage dans le cloud Adobe à partir d’un portfolio ou d’un programme de stockage Workfront hérité, le portfolio ou le programme est également converti en objets de stockage dans le cloud Adobe. Tous les autres projets de stockage Workfront hérités du même portefeuille ou programme restent inchangés.
     >* Votre instance Workfront peut ne pas avoir les deux types de stockage de documents.

     Un projet est créé et son nom par défaut suit les schémas suivants, en fonction du Workfront de stockage utilisé pour les documents :

      * `Untitled Project` d’un ancien projet de stockage Workfront.

        Un projet de stockage Workfront hérité affiche une icône **Stockage Workfront hérité** ![Icône de projet de stockage hérité](assets/legacy-storage-project-icon.png) en regard de son nom.

      * `Untitled Project - < Month day, year hour.minute.second >` d’un projet de stockage dans le cloud Adobe

        >[!IMPORTANT]
        >
        >Les projets utilisant l’espace de stockage dans le cloud d’Adobe doivent avoir des noms uniques.


1. Dans l’en-tête du projet, mettez à jour le nom du projet. Appuyez sur Entrée pour enregistrer le nom.

   ![Saisie d’un nom pour le projet](assets/rename-untitled-project.png).

   L’en-tête de la page du projet affiche une vue d’ensemble rapide de l’intégrité et de la progression actuelles d’un projet. Les informations contenues dans l’en-tête du projet changent à mesure que les informations du projet sont mises à jour.

1. Cliquez sur **Commencer à ajouter des tâches**.

   Ou

   Cliquez sur **Nouvelle tâche** pour ajouter des tâches au projet et leur affecter des ressources.

   Pour plus d’informations sur l’ajout de tâches à un projet, voir [Créer des tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Modifiez les détails du projet en cliquant sur le menu **Plus** à droite du nom du projet, dans l’en-tête, puis **Modifier** ![Icône Modifier](assets/qs-edit-icon.png) en regard du nom du projet.

   La zone **Modifier le projet** s’ouvre.

1. Ajoutez des informations sur le projet.

   Pour plus d’informations sur la modification d’un projet, voir [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!TIP]
   >
   >Le statut du projet doit être Planification ou un autre statut qui n&#39;est pas Actuel. Vous pouvez ainsi apporter des modifications au projet sans générer de notifications aux participants du projet.

1. Cliquez sur **Enregistrer** pour enregistrer les modifications.

1. (Facultatif) Après avoir configuré les paramètres du projet et ajouté les tâches, vous pouvez modifier le statut du projet en **Actuel** dans l’en-tête du projet.

   Cela indique que le projet est maintenant prêt à démarrer et que les personnes affectées aux tâches peuvent maintenant commencer à travailler dessus.

   Pour plus d’informations sur les statuts d’un projet, voir [Accéder à la liste des statuts système des projets](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
