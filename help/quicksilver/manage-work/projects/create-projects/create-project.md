---
product-area: projects
navigation-topic: create-projects
title: Créer un projet
description: Un projet est une grande unité de travail dans Adobe Workfront. Vous pouvez créer des projets à partir de zéro, utiliser un modèle ou convertir des problèmes ou des tâches en projets.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: a00776ecd9f8dc14b9dce14ce9463c2bb709a363
workflow-type: tm+mt
source-wordcount: '1263'
ht-degree: 92%

---

# Créer un projet

<!--remove Preview and Production references-->

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Les projets représentent une grande quantité de travail à effectuer dans Adobe Workfront.

## Conditions d’accès

<!--drafted for P&P - replace table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Nouveau : Standard</p>
        <p>ou</p>
        <p>Actuel : formule </p> </td> 
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

* Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Méthodes de création de projets

Vous pouvez créer un projet dans Workfront à l’aide de l’une des méthodes suivantes :

* Créez un projet à partir de zéro sans utiliser de modèle. Cet article décrit comment créer un projet à partir de zéro.

* Copiez un projet existant.\
  Pour plus d’informations sur la copie d’un projet, consultez la section [Copier un projet](../../../manage-work/projects/manage-projects/copy-project.md).

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

## Créer entièrement un projet

>[!NOTE]
>
>Si vous créez un projet à l’aide d’un modèle, il est recommandé de consulter également l’article [Créer un projet à l’aide d’un modèle](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).


1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche. Cliquez sur **Projets**, puis développez **Nouveau projet**.
   * Accédez à un portfolio, puis développez **Nouveau projet**.
   * Accédez à un programme, puis développez **Nouveau projet**.
   * Si vous êtes administrateur ou administratrice de groupes, vous pouvez également créer un projet dans la section Projets d’un groupe que vous gérez. Pour plus d’informations, voir [Créer et modifier les projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![Menu Nouveau projet](assets/new-project-dropdown-nwe-350x358.png)

1. Cliquez sur **Nouveau projet** dans le menu pour créer un projet à partir de zéro.
1. Saisissez le nom du projet. Appuyez sur Entrée pour enregistrer le nom.

   ![Saisie d’un nom pour le projet](assets/rename-untitled-project.png).

   L’en-tête de la page du projet affiche une vue d’ensemble rapide de l’intégrité et de la progression actuelles d’un projet. Les informations contenues dans l’en-tête du projet changent à mesure que les informations du projet sont mises à jour.

1. Cliquez sur **Commencer à ajouter des tâches**.

   Ou

   Cliquez sur **Nouvelle tâche** pour ajouter des tâches au projet et leur affecter des ressources.

   Pour plus d’informations sur l’ajout de tâches à un projet, voir [Créer des tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Modifiez les détails du projet en cliquant sur le menu **Plus** puis sur **Modifier** ![Icône Modifier](assets/qs-edit-icon.png) en regard du nom du projet.

   La boîte de dialogue **Modifier le projet** s’ouvre.

   Pour plus d’informations sur la modification d’un projet, voir [Modifier des projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Facultatif) Après avoir configuré les paramètres du projet et ajouté les tâches, vous pouvez modifier le statut du projet en **Actuel**.

   Cela indique que le projet est maintenant prêt à démarrer et que les personnes affectées aux tâches peuvent maintenant commencer à travailler dessus.

   Pour plus d’informations sur les statuts d’un projet, voir [Accéder à la liste des statuts système des projets](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
