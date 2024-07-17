---
product-area: projects
navigation-topic: create-projects
title: Créer un projet
description: Un projet est une grande unité de travail dans Adobe Workfront. Vous pouvez créer des projets à partir de zéro, utiliser un modèle ou convertir des problèmes ou des tâches en projets.
author: Alina
feature: Work Management
exl-id: d4e28fa6-25f9-4765-b051-8960c8873d5a
source-git-commit: f9afe7c8f04777dd547ea1e202e7844bdfd3518e
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 18%

---

# Créer un projet

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is linked from the UI from the Projects global nav section in classic. Do not change/ remove)</p>
-->

<!-- Audited: 12/2023 -->

Les projets représentent une grande quantité de travail à faire dans Adobe Workfront.

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

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouvelle : standard</p>
        <p>ou</p>
        <p>Actuelle : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Modifier l’accès aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Lorsque vous créez un projet, vous recevez automatiquement les autorisations de gestion du projet.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Méthodes de création de projets

Vous pouvez créer un projet dans Workfront à l’aide de l’une des méthodes suivantes :

* Créez un projet à partir de zéro sans utiliser de modèle. Cet article décrit comment créer entièrement un projet.

* Copiez un projet existant.\
  Pour plus d’informations sur la copie d’un projet, voir [Copier un projet](../../../manage-work/projects/manage-projects/copy-project.md).

* Utilisez un modèle.\
  Pour plus d’informations sur l’utilisation d’un modèle pour créer un projet, voir [Création d’un projet à l’aide d’un modèle](../../../manage-work/projects/create-projects/create-project-from-template.md).

* Importez un projet à partir du projet Microsoft.\
  Pour plus d’informations sur l’importation d’un projet à partir de MS Project, voir [Importation d’un projet à partir de Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

* Importez un projet à l’aide de lancements.

  En tant qu’administrateur de Workfront, vous pouvez importer des projets à l’aide d’un démarrage rapide.

  Pour plus d’informations sur l’importation de données à l’aide de lancements dans Workfront, voir [Importation de données dans Adobe Workfront à l’aide d’un modèle de démarrage rapide](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

  Pour plus d’informations sur l’importation de projets à l’aide de lancements, voir [Scénario de démarrage : préparation simple de l’importation de projets et de tâches](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-simple-project-task-import-prep.md).

* Publish une initiative à partir d’un scénario dans le planificateur de scénario Adobe Workfront. Le planificateur de scénario nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénario Workfront, consultez la [présentation du planificateur de scénario](../../../scenario-planner/scenario-planner-overview.md). Pour plus d’informations sur la création de projets à partir d’initiatives de publication, voir [Mise à jour ou création de projets en publiant des initiatives dans le planificateur de scénario](../../../scenario-planner/publish-scenarios-update-projects.md).

## Conditions préalables

Avant de commencer, vous devez vous assurer que :

* L’administrateur du système ou du groupe a activé la préférence &quot;Autoriser les utilisateurs à créer des projets sans utiliser de modèle&quot; dans la zone Configuration.

  Pour plus d’informations, voir [Configurer les préférences du projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Paramètres par défaut du projet

Lorsque vous créez un projet, Workfront lui applique un ensemble de paramètres par défaut. Par exemple, les modes État, Groupe et Planification sont prédéfinis lors de la création d’un projet.

Tenez compte des points suivants :

* En tant qu’administrateur Workfront ou administrateur de groupe, vous pouvez configurer les paramètres par défaut d’un nouveau projet lors de la configuration des préférences du projet pour l’ensemble de votre instance Workfront ou pour un groupe.
* Workfront applique les paramètres du groupe, le cas échéant, avant d’appliquer ceux définis par l’administrateur Workfront.
* L’état par défaut d’un nouveau projet correspond à l’état défini par votre administrateur Workfront dans la zone principale Préférences du projet ou par un administrateur de groupe (ou un administrateur Workfront) dans la zone Préférences du projet pour un groupe.

  >[!NOTE]
  >
  >Nous vous recommandons de spécifier l’état par défaut d’un nouveau projet, à savoir Planification. Lorsque vous apportez des modifications au nouveau projet, les notifications ne sont pas envoyées aux utilisateurs affectés au projet.
  >
  >Pour plus d’informations sur la configuration de l’état par défaut et d’autres paramètres par défaut pour un nouveau projet, voir [ Configuration des préférences du projet à l’échelle du système ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) ou [ Configuration des préférences du projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

* Les scénarios suivants existent pour la manière dont Workfront définit le groupe et l’état d’un nouveau projet :

   * Si vous créez un projet à partir de zéro, le groupe du projet est votre groupe d’accueil.

     L’état du projet est l’état par défaut dans les préférences du projet de votre groupe d’accueil, le cas échéant, ou de votre instance Workfront. Vous pouvez définir l’état par défaut lors de la création du projet sur n’importe quel état disponible pour le groupe du projet.

   * Si vous créez un projet à l’aide d’un modèle, les paramètres du modèle prévalent sur ceux définis par l’administrateur Workfront ou de groupe.

     Le groupe du nouveau projet est le groupe du modèle. Si le modèle n’est pas associé à un groupe, le groupe du projet est le groupe principal de l’utilisateur ou de l’utilisatrice qui crée le projet.

     L’état par défaut d’un nouveau projet créé à partir d’un modèle correspond à l’état défini par votre administrateur Workfront dans la zone principale Préférences du projet ou par un administrateur de groupe (ou un administrateur Workfront) dans la zone Préférences du projet du groupe. Vous pouvez modifier l’état par défaut lors de la création d’un projet à partir d’un modèle, en n’importe quel état du Groupe du projet qui est soit le Groupe du modèle, soit le Groupe d’accueil de l’utilisateur qui crée le projet.

   * Si vous créez un projet en convertissant une publication, le groupe d’un nouveau projet est le groupe du projet existant du problème. Si l’utilisateur qui convertit la publication n’a pas accès au projet de la publication ou si le projet de la publication ne comporte pas de groupe, le groupe du nouveau projet est le groupe d’accueil de l’utilisateur qui convertit la publication.

     Les statuts du nouveau projet correspondent aux états du groupe associé au projet, qui est soit le Groupe du projet d’origine, soit le Groupe d’accueil de l’utilisateur qui convertit le problème.

     Si vous utilisez un modèle lors de la création du projet en convertissant le problème, reportez-vous au deuxième scénario ci-dessus pour comprendre quel groupe et quel Workfront d’état s’appliquent au nouveau projet.

## Créer entièrement un projet

>[!NOTE]
>
>Si vous créez un projet à l’aide d’un modèle, nous vous recommandons de voir également l’article [Créer un projet à l’aide d’un modèle](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).


1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche. Cliquez sur **Projets**, puis développez **Nouveau projet**.
   * Accédez à un portfolio, puis développez **Nouveau projet**.
   * Accédez à un programme, puis développez **Nouveau projet**.
   * Si vous êtes administrateur ou administratrice de groupes, vous pouvez également créer un projet dans la section Projets d’un groupe que vous gérez. Pour plus d’informations, voir [Créer et modifier des projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

   ![Nouveau menu Projet](assets/new-project-dropdown-nwe-350x358.png)

1. Cliquez sur **Nouveau projet** dans le menu pour créer un projet à partir de zéro.
1. Saisissez le nom du projet. Appuyez sur Entrée pour enregistrer le nom.

   ![Saisissez un nom pour le projet](assets/rename-untitled-project.png)

   L’en-tête de la page du projet affiche un aperçu rapide de l’état actuel et de la progression d’un projet. Les informations contenues dans l’en-tête du projet changent à mesure que les informations du projet sont mises à jour.

1. Cliquez sur **Commencer à ajouter des tâches**.

   Ou

   Cliquez sur **Nouvelle tâche** pour ajouter des tâches au projet et leur affecter des ressources.

   Pour plus d’informations sur l’ajout de tâches à un projet, voir [Créer des tâches dans un projet](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

1. Modifiez les détails du projet en cliquant sur le menu **Plus** , puis sur **Modifier** ![](assets/qs-edit-icon.png) en regard du nom du projet.

   La boîte de dialogue **Modifier le projet** s’ouvre.

   Pour plus d’informations sur la modification d’un projet, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

1. (Facultatif) Après avoir configuré les paramètres du projet et ajouté les tâches, vous pouvez modifier l’état du projet en **Actuel**.

   Cela indique que le projet est maintenant prêt à démarrer et que les utilisateurs affectés aux tâches peuvent maintenant commencer à travailler dessus.

   Pour plus d’informations sur les états du projet, voir [Accès à la liste des états du projet système](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md).
