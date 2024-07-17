---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Vue d’ensemble du planificateur de ressources
description: Vous pouvez estimer et budgéter l’allocation de vos ressources aux projets auxquels elles sont affectées et prévoir leur disponibilité pour un travail futur à l’aide du planificateur de ressources.
author: Alina
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: 1c8d9a62f5582b0dbc3c72b5881bb5d8f0b790ba
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 1%

---

# Vue d’ensemble du planificateur de ressources

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

Vous pouvez estimer et budgéter l’allocation de vos ressources aux projets auxquels elles sont affectées et prévoir leur disponibilité pour un travail futur à l’aide du planificateur de ressources.

Pour une présentation générale de la planification des ressources dans Adobe Workfront, consultez l’article [Prise en main de la planification des ressources](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Vue d’ensemble du planificateur de ressources

Vous pouvez utiliser le planificateur de ressources pour comprendre facilement la disponibilité des utilisateurs et des rôles de tâche, ainsi que le temps planifié nécessaire pour terminer le travail sur les projets. Vous pouvez ensuite décider comment allouer vos utilisateurs et leurs rôles de travail sur les projets auxquels ils sont affectés en fonction de leur temps disponible.

>[!IMPORTANT]
>
>Vous ne pouvez pas utiliser le planificateur de ressources pour affecter le travail réel (tâches et problèmes) aux utilisateurs. Vous pouvez uniquement estimer le temps nécessaire aux utilisateurs ou aux rôles de tâche pour terminer un projet, quelles que soient les tâches et les problèmes auxquels ils sont affectés.\
>Pour affecter un travail réel aux utilisateurs, vous devez utiliser l’équilibreur de charge de travail. Pour plus d’informations sur l’équilibreur de charge de travail, consultez la [présentation de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Vous pouvez afficher les informations dans le planificateur de ressources à l’aide de trois vues distinctes. Vous pouvez utiliser chaque vue pour réaliser l’un des objectifs suivants :

* Pour estimer le temps ou le coût de vos ressources pour le travail qui doit être accompli à l’aide des vues Projet et Rôle . Il s’agit de l’objectif principal du planificateur de ressources.\
  Pour plus d’informations sur la planification dans le planificateur de ressources, consultez l’article [Ressources de budget dans le planificateur de ressources à l’aide des vues Projet et Rôle](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* Pour afficher les informations suivantes à l’aide de la vue Utilisateur :

   * La disponibilité de vos utilisateurs selon leur planning
   * Le temps prévu pour terminer le travail conformément au plan du projet.
   * La durée pendant laquelle les utilisateurs se sont déjà connectés aux tâches réelles

  Pour plus d’informations sur l’affichage des heures disponibles, planifiées et réelles ou de l’éditeur de texte enrichi pour les utilisateurs dans le planificateur de ressources, consultez l’article [Afficher les heures disponibles, planifiées et réelles ou l’éditeur de texte enrichi dans le planificateur de ressources lors de l’utilisation de la vue utilisateur](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## Considérations relatives au planificateur de ressources

* Vous pouvez hiérarchiser les projets sur lesquels vous travaillez et répartir vos ressources en fonction de leur priorité afin de vous assurer que les ressources sont d’abord allouées aux projets les plus importants.

  Pour plus d’informations sur la hiérarchisation des projets dans le planificateur de ressources, voir [Hiérarchisation des projets dans le planificateur de ressources](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* Vous pouvez afficher des informations sur les heures, l’éditeur de texte enrichi et les coûts à partir des tâches et des problèmes des projets.

  >[!NOTE]
  >
  >Les tâches et les problèmes ne s’affichent pas dans le planificateur de ressources. Toutefois, les informations sur les heures, l’ETP et les coûts des allocations de ressources sur les tâches s’affichent dans le planificateur de ressources sous forme de nombre total pour le projet.

* Les informations sur l’heure, l’éditeur de texte enrichi et les coûts des tâches parents sont exclues des projets qui s’affichent dans le planificateur de ressources. Nous vous recommandons d’affecter des ressources uniquement aux tâches enfants si vous souhaitez gérer le temps ou le coût de ces ressources dans le planificateur de ressources.

  Pour plus d’informations sur les tâches parentes, voir les articles suivants :

   * [Présentation des tâches](../../manage-work/tasks/task-information/tasks-overview.md)
   * [Créer des sous-tâches](../../manage-work/tasks/create-tasks/create-subtasks.md)

  >[!TIP]
  >
  >Les tâches parentes affichent le total des heures et des coûts des tâches pour enfants. Pour cette raison, le comptage des heures, de l’éditeur de texte enrichi et du coût des tâches enfants et des tâches parentes compterait deux fois ces montants. C’est pourquoi les informations de la tâche parente sont exclues du planificateur de ressources.

* Vous ne pouvez pas gérer l’affectation des équipes sur les projets pour lesquels elles ont des tâches ou des problèmes dans le planificateur de ressources.
* Vous pouvez budgétiser des ressources pour plusieurs projets à la fois à l’aide du planificateur de ressources ou pour un seul projet à l’aide de la zone Budget des ressources de l’Analyse de cas. Les informations que vous budgétisez pour un projet s’affichent également dans le planificateur de ressources.

  Pour plus d’informations sur la façon de budgéter les ressources pour un seul projet, consultez l’article [Ressources budgétaires dans l’analyse de cas ](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

  Pour plus d’informations sur la manière dont vous pouvez budgéter les ressources dans le planificateur de ressources pour plusieurs projets à la fois, consultez la section &quot;Ressources budgétaires dans le planificateur de ressources&quot; de l’article [Ressources budgétaires dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## Conditions préalables pour travailler dans le planificateur de ressources {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

Pour utiliser correctement le planificateur de ressources pour budgéter vos ressources, vous devez d’abord vous assurer que vous, vos projets et vos tâches remplissez un ensemble de conditions préalables. Ces conditions préalables sont obligatoires pour afficher les informations correctes dans le planificateur de ressources et pour gérer correctement vos ressources.

>[!IMPORTANT]
>
>Si l’une des conditions préalables suivantes est manquante, vous constaterez peut-être que certaines informations sur l’allocation ou la disponibilité des ressources sont manquantes ou ont une valeur nulle.\
>Pour plus d’informations sur la raison pour laquelle les champs ne contiennent pas de données ou n’ont aucune valeur, passez la souris sur les champs.

![](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>Les conditions préalables suivantes ne sont requises que lors de l’affichage du planificateur de ressources par projet ou par rôle de tâche ou lors de la planification des ressources dans le cas d’affaires d’un projet.

Les types de prérequis suivants sont requis pour la fonctionnalité correcte du planificateur de ressources lors de son affichage par projet ou par rôle :

* [Conditions préalables requises pour l’utilisateur](#user-prerequisites)
* [Prérequis du projet](#project-prerequisites)
* [Tâches et problèmes préalables](#tasks-and-issues-prerequisites)
* [Conditions préalables au niveau système](#system-level-prerequisites)

### Conditions préalables requises pour les utilisateurs {#user-prerequisites}

Assurez-vous que la configuration utilisateur suivante existe avant de commencer à utiliser le planificateur de ressources :

* Vous disposez d’un accès correct aux ressources du budget.

  Pour plus d’informations sur l’accès aux ressources du budget, consultez l’article [Accès aux ressources du budget dans Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Les utilisateurs affectés à des tâches sont ajoutés aux pools de ressources associés au projet.

  Pour plus d’informations sur l’ajout d’utilisateurs aux pools de ressources, voir [Association des pools de ressources aux utilisateurs](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

  >[!NOTE]
  >
  >Lorsque des utilisateurs ne sont pas ajoutés aux pools de ressources, les scénarios suivants peuvent exister :
  >
  >   
  >   
  >   * Les utilisateurs n’apparaissent pas dans le planificateur de ressources, bien qu’ils puissent être affectés à des tâches sur les projets.
  >   * Si les tâches auxquelles elles sont associées comportent des heures planifiées, ces heures n’apparaissent pas pour le projet dans le planificateur de ressources, sauf si l’utilisateur est également associé à un rôle de tâche pour ces tâches.
  >   * Si les utilisateurs sont associés à un rôle de tâche sur une tâche du projet, les heures planifiées s’affichent dans le planificateur de ressources pour le rôle de tâche, mais le rôle de tâche ne peut pas être budgété.
  >   
  >

* Les utilisateurs affectés aux pools de tâches et de ressources doivent être associés à des planifications et des rôles de tâche.

  Pour plus d’informations sur l’association de planifications et de rôles de tâche avec les utilisateurs, voir [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Les utilisateurs qui ne sont pas associés à un planning mais qui se trouvent dans le pool de ressources du projet ne peuvent pas être inclus dans le budget du planificateur de ressources.

* Pour obtenir des informations précises sur les heures disponibles, assurez-vous que les planifications associées à vos utilisateurs disposent des exceptions de planification et du délai d’expiration mis à jour.

  >[!NOTE]
  >
  >Si un utilisateur n’est pas associé à une planification, la planification par défaut de votre système Workfront est associée à l’utilisateur par défaut, aux fins du planificateur de ressources.

  Pour plus d’informations sur la création de plannings, consultez l’article [Créer un planning](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Si vous souhaitez répartir les ressources par coût, vous devez associer les rôles de tâche à coût/heure. les taux. Le coût associé aux rôles de tâche affectés aux utilisateurs dans vos pools de ressources est utilisé pour calculer le coût de la main-d’oeuvre budgété et le coût budgété du projet.\
  Pour plus d’informations sur l’association de rôles de tâche avec des taux, consultez l’article [Créer et gérer des rôles de tâche](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
  Pour plus d’informations sur le calcul du coût de la main-d’oeuvre budgétisée, consultez l’article [ Comprendre le coût de la main-d’oeuvre et les heures budgétisées pour les projets](../../manage-work/projects/project-finances/budgeted-labor-cost.md).\
  Pour plus d’informations sur le calcul du coût budgété, consultez l’article [Calculer le coût budgété](../../manage-work/projects/project-finances/budgeted-cost.md).

### Conditions préalables du projet {#project-prerequisites}

Assurez-vous que la configuration de projet suivante existe avant de commencer à utiliser le planificateur de ressources :

* Vos projets sont associés à des pools de ressources.\
  Pour plus d’informations sur l’ajout de pools de ressources aux projets, voir [Association des pools de ressources aux projets et aux modèles](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

  >[!IMPORTANT]
  >
  >Les projets sans pools de ressources n’affichent pas les informations Heure planifiée ou Affectations dans le planificateur de ressources.

### Tâches et problèmes préalables {#tasks-and-issues-prerequisites}

Bien que vous ne puissiez pas afficher les tâches et les problèmes dans le planificateur de ressources, leurs informations sont transférées vers les projets qui s’affichent dans le planificateur de ressources .

Assurez-vous que la tâche et la configuration de problème suivantes existent avant de démarrer les ressources de budget dans le planificateur de ressources :

* Les tâches ou problèmes relatifs aux projets pour lesquels vous budgétisez des ressources sont affectés à l’une de ces entités :

   * Utilisateurs des pools de ressources du projet qui sont également associés aux rôles de tâche
   * Fonctions

  >[!NOTE]
  >
  >Les heures planifiées des tâches et problèmes affectés aux rôles de tâche s’affichent dans le planificateur de ressources, mais ces heures ne peuvent pas être budgétées, sauf si un utilisateur associé au rôle de tâche est répertorié dans un pool de ressources associé au projet.

* Vous ne devez pas affecter de tâches parentes aux utilisateurs ou aux rôles.

  Pour afficher les informations sur l’heure dans le planificateur de ressources pour les utilisateurs ou les rôles associés aux tâches parents, vous devez également les affecter aux tâches enfants. Le planificateur de ressources n’affiche pas les informations des tâches parents.

* Les tâches et les problèmes ont une valeur pour les heures planifiées qui est supérieure à zéro.
* Les tâches et les problèmes ont une valeur pour leur durée supérieure à zéro.
* Les dates prévues des problèmes sont dans le calendrier du projet.

### Conditions préalables au niveau système {#system-level-prerequisites}

Vous devez comprendre comment votre instance de Workfront calcule la disponibilité de l’utilisateur en fonction des préférences de gestion des ressources de votre système. Workfront peut calculer la disponibilité de l’utilisateur à l’aide du planning de l’utilisateur tel que défini dans sa page Profil utilisateur ou dans la Planification par défaut de votre système.

![](assets/resource-management-preferences-section-in-setup-350x89.png)

Votre administrateur Workfront configure vos préférences de gestion des ressources.

Pour plus d’informations, voir [Configurer les préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Localiser le planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

Vous pouvez localiser le planificateur de ressources dans deux zones de Workfront, selon que vous souhaitez budgéter vos ressources pour plusieurs projets ou pour un seul projet.

Pour plus d’informations sur la localisation du planificateur de ressources, voir [Localisation du planificateur de ressources](../../resource-mgmt/resource-planning/locate-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(this is drafted and moved to its own article: locate-resource-planner) </p>
<p>Ensure that all prerequisites are met before starting to use the Resource Planner. This way, you ensure that the Resource Planner displays the correct information before you start budgeting your resources.<br>For information about the prerequisites that must be met before you can start using the Resource Planner, see the <a href="#prerequisites-for-working-in-the-resource-planner" class="MCXref xref">Prerequisites for working in the Resource Planner</a> section in this article. </p>
<p>You can locate the Resource Planner in two areas of Workfront, depending on whether you want to budget your resources for multiple projects, or for just one project.</p>
<ul>
<li><a href="#use-the-resource-planner-for-multiple-projects" class="MCXref xref">Use the Resource Planner for multiple projects</a> </li>
<li> <p><a href="#use-the-resource-planner-for-one-project" class="MCXref xref">Use the Resource Planner for one project</a> </p> </li>
</ul>
<p><strong>Use the Resource Planner for multiple projects</strong></p>
<p>When using the Resource Planner for multiple projects, the allocation numbers for your resources represent numbers across multiple projects. </p>
<p>To access the  Planner section  in the  Resourcing area: </p>
<ol>
<li value="1">  Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.  </li>
<li value="2"> <p>  Click <strong>Resourcing</strong>. The Resource Planner displays by default.  For information about budgeting resources in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> <p> <img src="assets/qs-resource-management-area-with-planner-as-default-350x152.png" style="width: 350;height: 152;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">  Hover over the left panel, and click <strong>Resource Pools</strong>. <br>For information about creating new resource pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md" class="MCXref xref">Create resource pools</a>.</li>
</ol>
<p><strong>Use the Resource Planner for one project</strong></p>
<p>When using the Resource Planner for one project, the allocation numbers for your resources represent numbers for the selected project. </p>
<ol>
<li value="1"> <p>Go to a project you want to budget resources for.</p> </li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Business Case</strong> in the left panel.</p> </li>
<li value="3"> <p>Scroll to the <strong>Resource Budgeting</strong> section of the Business Case.</p> </li>
<li value="4"> <p>Click <strong>Edit Resource Budgeting</strong> to add resource pools to your project and start budgeting your resources. </p> <note type="tip">
You can only add a resource pool in the Resource Budgeting area of the Business Case when the project has no resource pools associated with it. When the project already has a resource pool, the users in the pool and their job roles display in the Resource Budgeting area by default.
</note> <p> <img src="assets/resource-budgeting-area-on-project-350x70.png" style="width: 350;height: 70;"> </p> <p>For information about budgeting resources for one project, see the article <a href="../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md" class="MCXref xref">Budget resources in the Business Case</a>.</p> </li>
</ol>
</div>
-->

## Les zones du planificateur de ressources

Vous pouvez afficher les informations suivantes ou effectuer les actions suivantes dans le planificateur de ressources :

* Informations sur les ressources affectées à vos projets dans le planificateur de ressources dans un calendrier général.
* Suraffectation ou sous-utilisation de vos ressources dans le planificateur de ressources.
* Planifiez vos ressources de manière manuelle ou automatique.

Pour plus d’informations sur les zones qui s’affichent dans le planificateur de ressources et sur la configuration des informations qui s’affichent dans ces zones, consultez l’article [Présentation de la navigation du planificateur de ressources](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Limites de l’affichage des informations dans le planificateur de ressources

Pour améliorer les performances, Workfront limite la quantité d’éléments que vous pouvez afficher dans le planificateur de ressources.

Pour plus d’informations sur ces limites, consultez l’article [Limites d’affichage du planificateur de ressources](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md) .

## Calcul de l’éditeur de texte enrichi dans le planificateur de ressources

Vous pouvez afficher les valeurs de disponibilité, d’affectation et de planification dans le planificateur de ressources sous Heures, ETR ou Coût.

Pour plus d’informations sur la modification des informations que vous affichez dans le planificateur de ressources, consultez la section [Affichage des informations par heure, ETR ou coût](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) de l’article [Révision de la disponibilité et de l’allocation des ressources à l’aide du planificateur de ressources Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

Pour plus d’informations sur le calcul des heures et de l’ETR pour les utilisateurs et les rôles dans Workfront, consultez l’article [Présentation du calcul des heures et de l’ETR pour les utilisateurs et les rôles dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Calcul des coûts dans le planificateur de ressources

Vous devez disposer des autorisations Afficher l’accès aux données financières et Afficher le financement sur les projets pour afficher les informations par coût dans le planificateur de ressources.

Outre l’affichage des valeurs de disponibilité, d’affectation et planifiées dans le planificateur de ressources dans les heures et l’éditeur de texte enrichi, vous pouvez également les afficher par coût.

>[!TIP]
>
>Vous devez associer vos utilisateurs et vos rôles de tâche aux taux de coût par heure afin d’afficher les informations par coûts dans le planificateur de ressources.

Pour plus d’informations sur l’association des taux de coût par heure avec les rôles de tâche, consultez l’article [Créer et gérer des rôles de tâche](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
Pour plus d’informations sur l’association des taux de coût par heure avec les utilisateurs, consultez l’article [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Tenez compte des points suivants lors de l’affichage des informations par coût dans le planificateur de ressources :

* Le coût de chaque type d’heures (planifiée, disponible, budgétée, réelle pour les utilisateurs, les rôles ou les projets) est calculé à l’aide d’un autre Taux de coût.
* Le coût planifié est affecté par le type de coût des tâches sur les projets.
* Lors de l’application de la vue utilisateur au planificateur de ressources, vous ne pouvez pas afficher les informations d’affectation et de disponibilité par coût.

Pour plus d’informations sur la façon dont les coûts sont calculés dans le planificateur de ressources pour les utilisateurs et les rôles, consultez l’article [Calculer les coûts dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Use the User View to view Available, Planned, and Actual Hours or FTE </h2>
<p>(this information is repeated from above where it exists in shorter form. Drafted to simplify the amount of info of this article.) </p>
<p>You can use the User View of the Resource Planner to display information about the Planned, Available, and Actual Hours or FTE values for projects and resources. </p>
<p>For information about using the Resource Planner to review the Available, Planned, and Actual Hours and FTE for resources, see the article <a href="../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md" class="MCXref xref">View Available, Planned, and Actual Hours or FTE in the Resource Planner when using the User view</a>.</p>
<p><strong>Use the Project and Role Views to budget resources </strong></p>
<p> The main function of the Resource Planner is to budget your resources for the work that needs to be completed on the projects that you can manage. </p>
<p> You can budget your resources only if you apply the <strong>View by Project</strong> or <strong>View by Role</strong> views to the Resource Planner.</p>
<p>For information about budgeting resources using the Project and Role views in the Resource Planner, see the article <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md"><a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a></a>.</p>
</div>
-->

## Filtrer des informations dans le planificateur de ressources

Vous pouvez réduire le nombre de projets, de rôles ou d’utilisateurs qui s’affichent dans le planificateur de ressources en créant un filtre.\
Pour plus d’informations, voir l’article [Filtrer les informations dans le planificateur de ressources](../../resource-mgmt/resource-planning/filter-resource-planner.md).
