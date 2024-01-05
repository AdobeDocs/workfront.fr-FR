---
product-area: projects
navigation-topic: create-projects
title: Création de lignes de base de projet
description: Une ligne de base est un instantané de projet qui représente des éléments d’information clés inclus dans le plan initial du projet ou à tout moment pendant la durée du projet.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: bec625b70b39fec9f9a6d4f7b48023702de43675
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Création de lignes de base de projet

<!-- Audited: 12/2023 -->

Une ligne de base est un instantané de projet qui représente des éléments d’information clés inclus dans le plan initial du projet ou à tout moment pendant la durée du projet.

Vous pouvez utiliser la ligne de base pour comparer ces informations du plan actuel au plan d’origine ou à tout autre moment dans le temps, afin d’identifier les tâches problématiques, les changements d’étendue et d’autres tendances au fil du temps.

## Exigences d’accès

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
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
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
    <td><p>Nouveau : Standard</p>
        <p>ou</p>
        <p>Actuel : formule </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès</td> 
   <td> <p>Modifier l’accès aux projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Affichage des autorisations pour le projet ou version ultérieure pour afficher les lignes de base</p> <p>Gérer les autorisations du projet pour créer des lignes de base</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Observations relatives à l’utilisation des lignes de base

* Vous pouvez capturer plusieurs fois un instantané de la progression d’un projet au cours de sa durée de vie, créant ainsi plusieurs lignes de base.
* Vous pouvez afficher les informations incluses dans les lignes de base d’un projet en créant une ligne de base ou en créant un rapport de ligne de base.
* Lorsque vous créez une ligne de base, les informations de tâche sont également capturées sur les tâches de base de cette ligne de base.
* Vous pouvez afficher les informations des tâches de base en créant un rapport Tâche de ligne de base .

>[!IMPORTANT]
>
>Une ligne de base prend un instantané du nom, des dates et des informations financières du projet. La ligne de base n’inclut pas les valeurs des champs personnalisés du projet. Pour plus d’informations sur les informations financières incluses dans la ligne de base, voir [Finances du projet incluses dans les lignes de base du projet](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Création d’une ligne de base

Vous pouvez créer une ligne de base comme suit :

* **Automatiquement**: votre administrateur Workfront ou un administrateur de groupe définit les préférences de projet pour que Workfront crée automatiquement une ligne de base lorsqu’un projet devient actuel. Lorsque ce paramètre est activé, une ligne de base est créée lorsque l’état du projet devient Actuel. Lorsque ce paramètre n’est pas activé, vous devez créer manuellement des lignes de base.

  Pour plus d’informations sur la configuration des préférences de projet et la configuration de la création automatique de la ligne de base, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!CAUTION]
  >
  >L’activation de ce paramètre crée automatiquement une ligne de base pour un projet chaque fois qu’un état de projet passe à Actuel. La première ligne de base créée est la ligne par défaut. Vous devez créer manuellement toutes les autres lignes de base pendant la durée du projet .

* **Manuellement**: vous pouvez créer de nouvelles lignes de base pour le projet au fur et à mesure que le projet progresse. Vous pouvez ensuite comparer des lignes de base pour voir l’évolution du projet au fil du temps.

Pour créer une ligne de base :

1. Accédez à un projet.
1. Dans le panneau de gauche, cliquez sur **Lignes de base**.

   Ou

   Cliquez sur **Afficher plus**, puis cliquez sur **Lignes de base**.

   ![Section de base sur le projet](assets/baselines-section-on-project-with-header.png)

1. Cliquez sur **Nouvelle ligne de base.**
1. Indiquez le nom de la ligne de base.
1. (Facultatif) S’il s’agit de la première ligne de base, vous pouvez la choisir comme valeur par défaut.
1. Cliquer sur **Enregistrer**.

   Par défaut, les informations suivantes s’affichent sur la ligne de base que vous avez créée :

   * Nom de la ligne de base
   * Date d’entrée de ligne de base
   * Date de début planifiée du projet lorsque la ligne de base a été créée
   * Date de début prévue du projet lorsque la ligne de base a été créée
   * Durée réelle du projet lors de la création de la ligne de base
   * % Terminé du projet lorsque la ligne de base a été créée
   * Indicateur de ligne de base par défaut qui indique si une ligne de base est la ligne de base par défaut du projet.

     >[!TIP]
     >
     >Vous ne pouvez pas afficher les informations de deux lignes de base en même temps dans la même vue ou dans le même rapport. Vous pouvez uniquement afficher les informations d’une ligne de base donnée et de la ligne de base par défaut dans le même rapport. Vous pouvez modifier la ligne de base que vous considérez comme la ligne de base par défaut à tout moment pendant la durée du projet.

1. (Facultatif) Cliquez sur le **Affichage** , puis créez une vue ou modifiez la vue actuelle pour ajouter des champs à la vue et comparer des informations supplémentaires entre les lignes de base. Pour plus d’informations, voir [Création ou modification de vues dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Création d’un rapport de ligne de base ou de tâche de ligne de base

Pour afficher des informations de base, vous pouvez également créer un rapport de ligne de base ou de tâche de ligne de base. Vous pouvez ainsi afficher un nombre indéfini de champs relatifs aux lignes de base ou aux tâches de base pour les comparer dans une vue.

>[!TIP]
>
>Vous devez créer une ligne de base avant de pouvoir créer un rapport de ligne de base ou de tâche de ligne de base.

Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Nous vous recommandons d’ajouter un regroupement Nom de projet à votre rapport Tâche de ligne de base ou Tâche de ligne de base afin de faciliter la lecture.

Pour plus d’informations sur la création d’un groupement, voir [Création de groupes dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).
