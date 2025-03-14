---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Présentation du planificateur des ressources
description: Grâce au planificateur de ressources, vous pouvez estimer et budgéter l’affectation de vos ressources aux projets et prévoir leur disponibilité pour des travaux futurs.
author: Lisa
feature: Resource Management
exl-id: 06cd2226-f94d-4b6a-8692-6d35210782f2
source-git-commit: 696d656816a4c1c2edef4347567b2fc553f489f7
workflow-type: tm+mt
source-wordcount: '2113'
ht-degree: 98%

---

# Vue d’ensemble du planificateur de ressources {#resource-planner-overview}

>[!CONTEXTUALHELP]
>id="wf-resourcing-planner"
>title="Planificateur de ressources"
>abstract="Vous pouvez utiliser le planificateur de ressources pour estimer et budgéter l&#39;allocation de vos ressources aux projets auxquels elles sont affectées, et prévoir leur disponibilité pour un travail futur."

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: this used to be the beginning of Planning in the Resource Planner - consider restructuring it further? Merging some of this information with information about Understanding Navigation in the RP?!)</p>
-->

Grâce au planificateur de ressources, vous pouvez estimer et budgéter l’affectation de vos ressources aux projets et prévoir leur disponibilité pour des travaux futurs.

Pour une vue d’ensemble générale de la planification des ressources dans Adobe Workfront, reportez-vous à l’article [Prise en main de la planification des ressources](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Vue d’ensemble du planificateur de ressources

Le planificateur de ressources vous permet de visualiser aisément la disponibilité des utilisateurs et des utilisatrices, des fonctions et le temps prévu pour terminer les projets. Vous pouvez ensuite décider comment affecter vos utilisateurs et utilisatrices ainsi que leurs fonctions sur les projets qui leur sont affectés en fonction de leur temps disponible.

>[!IMPORTANT]
>
>Vous ne pouvez pas utiliser le planificateur de ressources pour affecter le travail réel (tâches et problèmes) aux utilisateurs et aux utilisatrices. Vous pouvez uniquement estimer le temps nécessaire aux utilisateurs et aux utilisatrices ou aux fonctions pour terminer un projet, quels que soient les tâches et les problèmes qui leur sont affectés.\
>Pour affecter un travail réel aux utilisateurs et aux utilisatrices, vous devez utiliser l’équilibreur de charge de travail. Pour plus d’informations sur l’équilibreur de charge de travail, consultez la section [Vue d’ensemble de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Vous pouvez afficher les informations dans le planificateur de ressources à l’aide de trois vues distinctes. Vous pouvez utiliser chaque vue pour réaliser l’un des objectifs suivants :

* Pour estimer le temps ou le coût de vos ressources pour le travail qui doit être accompli à l’aide des vues « Projet » et « Rôle ». Il s’agit de l’objectif principal du planificateur de ressources.\
  Pour plus d’informations sur l’établissement d’un budget dans le planificateur de ressources, consultez l’article [Établir un budget de ressources dans le planificateur de ressources à l’aide des vues « Projet » et « Rôle »](../resource-planning/budget-resources-project-role-views-resource-planner.md).

* Pour afficher les informations suivantes à l’aide de la vue « Utilisateur ou utilisatrice », procédez comme suit :

   * Disponibilité de vos utilisateurs et de vos utilisatrices selon leur planning
   * Durée prévue pour terminer le travail conformément au plan du projet
   * Durée que les utilisateurs et les utilisatrices ont déjà consignée pour les éléments de travail réel

  Pour plus d’informations sur l’affichage des heures disponibles, prévues et effectives ou de l’équivalent temps complet pour les utilisateurs et les utilisatrices dans le planificateur de ressources, consultez l’article [Afficher les heures disponibles, prévues et effectives ou l’équivalent temps complet dans le planificateur de ressources lors de l’utilisation de la vue des utilisateurs et des utilisatrices](../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md#using).

## Considérations du planificateur de ressources

* Vous pouvez hiérarchiser les projets sur lesquels vous travaillez et répartir vos ressources en fonction de leur priorité afin de vous assurer que les ressources sont d’abord affectées aux projets les plus importants.

  Pour plus d’informations sur le classement des projets par priorité dans le planificateur de ressources, consultez la section [Hiérarchiser les projets dans le planificateur de ressources](../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* Vous pouvez afficher des informations sur les heures, l’équivalent temps complet et les coûts à partir des tâches et des problèmes des projets.

  >[!NOTE]
  >
  >Les tâches et les problèmes ne s’affichent pas dans le planificateur de ressources. Toutefois, les informations sur les heures, l’équivalent temps complet et les coûts des affectations de ressources sur les tâches s’affichent dans le planificateur de ressources sous forme de nombre total pour le projet.

* Les informations sur les heures, l’équivalent temps complet et les coûts des tâches parent sont exclues des projets qui s’affichent dans le planificateur de ressources. Nous vous recommandons d’affecter des ressources uniquement aux tâches enfant si vous souhaitez gérer le temps ou le coût de ces ressources dans le planificateur de ressources.

  Pour plus d’informations sur les tâches parent, consultez les articles suivants :

   * [Vue d’ensemble des tâches](../../manage-work/tasks/task-information/tasks-overview.md)
   * [Créer des sous-tâches](../../manage-work/tasks/create-tasks/create-subtasks.md)

  >[!TIP]
  >
  >Les tâches parent affichent le total des heures et des coûts des tâches enfant. Pour cette raison, le comptage des heures, de l’équivalent temps complet et du coût des tâches enfant et des tâches parent compterait deux fois ces montants. C’est pourquoi les informations de la tâche parent sont exclues du planificateur de ressources.

* Vous ne pouvez pas gérer l’affectation des équipes sur les projets pour lesquels elles ont des tâches ou des problèmes dans le planificateur de ressources.
* Vous pouvez budgéter des ressources pour plusieurs projets à la fois à l’aide du planificateur de ressources ou pour un seul projet à l’aide de la zone « Établissement du budget de ressources» du business case. Les informations que vous budgétez pour un projet s’affichent également dans le planificateur de ressources.

  Pour plus d’informations sur l’établissement du budget de ressources pour un seul projet, consultez l’article [Établissement du budget de ressources dans le business case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

  Pour plus d’informations sur la manière dont vous pouvez établir un budget de ressources dans le planificateur de ressources pour plusieurs projets à la fois, reportez-vous à la section « Établir un budget de ressources dans le planificateur de ressources » de l’article [Établir un budget de ressources dans le planificateur de ressources à l’aide des vues « Projet » et « Rôle »](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

## Conditions préalables pour travailler dans le planificateur de ressources {#prerequisites-for-working-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(<b>THIS SECTION IS LINKED TO ALL RES PLANNING ARTICLES. DO NOT RENAME OF DELETE THIS!</b> - do NOT ADD the variable here, because it might break this link!)</p>
-->

Afin de bien utiliser le planificateur de ressources pour établir un budget de ressources, il est nécessaire de vérifier au préalable que vous, vos projets et vos tâches respectez un ensemble de conditions préalables. Ces conditions préalables sont obligatoires pour afficher les informations correctes dans le planificateur de ressources et pour gérer correctement vos ressources.

>[!IMPORTANT]
>
>Si l’une des conditions préalables suivantes est manquante, vous constaterez peut-être que certaines informations sur l’affectation ou la disponibilité des ressources sont manquantes ou ont une valeur nulle.\
>Pour plus d’informations sur la raison pour laquelle les champs ne contiennent pas de données ou n’ont aucune valeur, pointez la souris sur les champs.

![Aucun utilisateur avec ce rôle](assets/no-users-with-this-role-in-the-res-pool-350x57.png)

>[!NOTE]
>
>Les conditions préalables suivantes ne sont requises que lors de l’affichage du planificateur de ressources par projet ou par fonction ou lors de l’établissement d’un budget de ressources dans le business case d’un projet.

Les types de conditions préalables suivants sont nécessaires au bon fonctionnement du planificateur de ressources lorsqu’il est affiché par projet ou par rôle :

* [Conditions préalables requises pour les utilisateurs et les utilisatrices](#user-prerequisites)
* [Conditions préalables du projet](#project-prerequisites)
* [Conditions préalables pour les tâches et problèmes](#tasks-and-issues-prerequisites)
* [Conditions préalables au niveau du système](#system-level-prerequisites)

### Conditions préalables pour les utilisateurs et utilisatrices {#user-prerequisites}

Assurez-vous que la configuration utilisateur ou utilisatrice suivante existe avant de commencer à utiliser le planificateur de ressources :

* Vous disposez d’un accès correct pour budgétiser les ressources.

  Pour plus d’informations sur l’accès requis pour budgétiser les ressources, consultez l’article [Accès requis pour budgétiser les ressources dans Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Les personnes affectées à des tâches sont ajoutées aux groupes de ressources associés au projet.

  Pour plus d’informations sur l’ajout de personnes aux groupes de ressources, voir [Associer des groupes de ressources à des utilisateurs et utilisatrices](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

  >[!NOTE]
  >
  >Lorsque des personnes ne sont pas ajoutées à des groupes de ressources, les scénarios suivants peuvent se produire :
  >
  >   
  >   
  >   * Les personnes n’apparaissent pas dans le planificateur de ressources, bien qu’elles puissent être affectées à des tâches sur les projets.
  >   * Si les tâches auxquelles elles sont associées comportent un nombre d’heures prévues, ces heures n’apparaissent pas pour le projet dans le planificateur de ressources, sauf si la personne est également associée à une fonction pour ces tâches.
  >   * Si les personnes sont associées à une fonction sur une tâche du projet, le nombre d’heures prévues s’affiche dans le planificateur de ressources pour la fonction, mais la fonction ne peut pas être budgétée.
  >   
  >

* Les personnes affectées aux groupes de tâches et de ressources doivent avoir des plannings et des fonctions associés dans leur profil.

  Pour plus d’informations sur l’association de plannings et de fonctions à des personnes, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Les personnes qui ne sont pas associées à un planning mais qui se trouvent dans le groupe de ressources du projet ne peuvent pas être budgétées dans le planificateur de ressources.

* Pour obtenir des informations précises sur les heures disponibles, assurez-vous que les exceptions et les congés des plannings associés à vos utilisateurs et utilisatrices sont mis à jour.

  >[!NOTE]
  >
  >Si une personne n’est pas associée à un planning, le planning par défaut de votre système Workfront est associé à l’utilisateur ou l’utilisatrice par défaut, aux fins du planificateur de ressources.

  Pour plus d’informations sur la création de plannings, voir l’article [Créer un planning](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Si vous souhaitez répartir les ressources par coût, vous devez associer les fonctions aux taux de coût/heure . Le coût associé aux fonctions affectées aux personnes dans vos groupes de ressources est utilisé pour calculer le coût budgété de la main-d’œuvre et le coût budgété du projet.\
  Pour plus d’informations sur l’association de fonctions à des taux, consultez l’article [Créer et gérer des fonctions](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
  Pour plus d’informations sur le calcul du coût budgété de la main-d’œuvre, consultez l’article [Comprendre le coût bugété de la main-d’œuvre et les heures budgétées pour les projets](../../manage-work/projects/project-finances/budgeted-labor-cost.md).\
  Pour plus d’informations sur le calcul du coût budgété, voir l’article [Calculer le coût budgété](../../manage-work/projects/project-finances/budgeted-cost.md).

### Conditions préalables pour le projet {#project-prerequisites}

Assurez-vous que la configuration de projet suivante existe avant de commencer à utiliser le planificateur de ressources :

* Vos projets sont associés à des groupes de ressources.\
  Pour plus d’informations sur l’ajout de groupes de ressources à des projets, voir [Associer des groupes de ressources à des projets et modèles](../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md).

  >[!IMPORTANT]
  >
  >Les projets sans groupes de ressources n’affichent pas les informations sur le nombre d’heures prévues ou les affectations dans le planificateur de ressources.

### Conditions préalables pour les tâches et problèmes {#tasks-and-issues-prerequisites}

Bien que vous ne puissiez pas afficher les tâches et les problèmes dans le planificateur de ressources, leurs informations sont transférées vers les projets qui s’affichent dans le planificateur de ressources.

Assurez-vous que la configuration de tâche et de problème suivante existe avant de démarrer la budgétisation des ressources dans le planificateur de ressources :

* Les tâches ou problèmes sur les projets pour lesquels vous budgetisez des ressources sont affectés à l’une de ces entités :

   * Personnes des groupes de ressources du projet qui sont également associées à des fonctions
   * Fonctions

  >[!NOTE]
  >
  >Le nombre d’heures prévues des tâches et problèmes affectés aux fonctions s’affichent dans le planificateur de ressources, mais ces heures ne peuvent pas être budgétées, sauf si une personne associée à la fonction est répertoriée dans un groupe de ressources associé au projet.

* Vous ne devez pas affecter de tâches parent aux personnes ou aux fonctions.

  Pour afficher les informations sur les heures dans le planificateur de ressources pour les personnes ou les rôles associés aux tâches parent, vous devez également affecter ces derniers aux tâches enfant. Le planificateur de ressources n’affiche pas les informations des tâches parent.

* La valeur du nombre d’heures prévues pour les tâches et les problèmes est supérieure à zéro.
* La valeur de la durée des tâches et des problèmes est supérieure à zéro.
* Les dates prévues des problèmes sont dans la chronologie du projet.

### Conditions préalables au niveau du système {#system-level-prerequisites}

Vous devez comprendre comment votre instance de Workfront calcule la disponibilité de la personne en fonction des préférences de gestion des ressources de votre système. Workfront peut calculer la disponibilité de la personne à l’aide de son planning tel que défini dans sa page Profil utilisateur ou dans le planning par défaut de votre système.

![Préférences de gestion](assets/resource-management-preferences-section-in-setup-350x89.png)

Votre administrateur ou administratrice Workfront configure vos préférences de gestion des ressources.

Pour plus d’informations, voir [Configurer les préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Rechercher le planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This became another standalone article; drfat this section here when article is live.)</p>
-->

Vous pouvez localiser le planificateur de ressources dans deux zones de Workfront, selon que vous souhaitez établir le budget de vos ressources pour un ou plusieurs projets.

Pour plus d’informations sur la localisation du planificateur de ressources, voir [Localiser le planificateur de ressources](../../resource-mgmt/resource-planning/locate-resource-planner.md).

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

## Zones du planificateur de ressources

Vous pouvez afficher les informations suivantes ou effectuer les actions suivantes dans le planificateur de ressources :

* Informations sur les ressources affectées à vos projets dans le planificateur de ressources dans une chronologie générale.
* Surallocation ou sous-utilisation de vos ressources dans le planificateur de ressources.
* Budgétez vos ressources de manière manuelle ou automatique.

Pour plus d’informations sur les zones affichées dans le planificateur de ressources et sur la configuration des informations affichées dans ces zones, consultez l’article [Vue d’ensemble de la navigation dans le planificateur de ressources](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Limitations de l’affichage des informations dans le planificateur de ressources

Pour améliorer les performances, Workfront limite la quantité d’éléments affichés dans le planificateur de ressources.

Pour plus d’informations sur ces limitations, consultez l’article [Limitations d’affichage du planificateur de ressources](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

## Calculer l’équivalent temps complet dans le planificateur de ressources

Vous pouvez afficher les valeurs de disponibilité, d’affectation et de planification dans le planificateur de ressources par heures, équivalent temps complet ou coût.

Pour plus d’informations sur la modification des informations affichées dans le planificateur de ressources, consultez la section [Afficher les informations par heure, équivalent temps complet ou coût](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#display-by-hour-or-fte-menu) dans l’article [Vérifier la disponibilité et l’affectation des ressources à l’aide du planificateur de ressources d’Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

Pour plus d’informations sur le calcul des heures et de l’équivalent temps complet pour les personnes et les rôles dans Workfront, consultez l’article [Vue d’ensemble du calcul des heures et de l’équivalent temps complet pour les personnes et les rôles dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

## Calculer des coûts dans le planificateur de ressources

Vous devez disposer des autorisations Afficher pour les données financières et Afficher pour les finances pour les projets pour afficher les informations par coût dans le planificateur de ressources.

Vous pouvez afficher les valeurs de disponibilité, d’affectation et de planification dans le planificateur de ressources par heures, équivalent temps complet et coût.

>[!TIP]
>
>Vous devez associer les personnes et les fonctions aux taux Coûts par heure afin d’afficher les informations par coûts dans le planificateur de ressources.

Pour plus d’informations sur l’association de fonctions à des taux de coût par heure, consultez l’article [Créer et gérer des fonctions](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).\
Pour plus d’informations sur l’association de personnes à des taux de coût par heure, consultez l’article [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Tenez compte des éléments suivants lorsque vous affichez des informations par coût dans le planificateur de ressources :

* Le coût de chaque type d’heures (prévues, disponibles, budgétées, effectives pour les personnes, les rôles ou les projets) est calculé à l’aide d’un autre taux de dépenses.
* Le coût prévu est affecté par le type de coût des tâches des projets.
* Lors de l’application de la vue Utilisateur ou utilisatrice au planificateur de ressources, vous ne pouvez pas afficher les informations d’affectation et de disponibilité par coût.

Pour plus d’informations sur le calcul des coûts dans le planificateur de ressources pour les personnes et les rôles, consultez l’article [Calculer les coûts dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

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

## Filtrer les informations dans le planificateur de ressources

Vous pouvez réduire le nombre de projets, de rôles ou de personnes qui s’affichent dans le planificateur de ressources en créant un filtre.\
Pour plus d’informations, consultez l’article [Filtrer les informations dans le planificateur de ressources](../../resource-mgmt/resource-planning/filter-resource-planner.md).
