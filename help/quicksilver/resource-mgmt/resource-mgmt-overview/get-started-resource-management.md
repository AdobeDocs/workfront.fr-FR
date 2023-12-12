---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Prise en main de la gestion des ressources
description: La gestion des ressources vous permet de configurer votre système pour prévoir précisément l’utilisation de vos ressources en fonction de leur disponibilité, de sorte que le travail à faire soit terminé à temps et selon le budget.
author: Alina
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: dfd8dd07e1a88da872550163051e703f6aea5f74
workflow-type: tm+mt
source-wordcount: '1175'
ht-degree: 0%

---

# Prise en main de la gestion des ressources

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

La gestion des ressources vous permet de configurer votre système pour prévoir précisément l’utilisation de vos ressources en fonction de leur disponibilité, de sorte que le travail à faire soit terminé à temps et selon le budget.

## Présentation de la gestion des ressources dans Adobe Workfront

La gestion des ressources fait référence à toutes les activités exécutées par l’administrateur Adobe Workfront, le gestionnaire des ressources et le propriétaire du projet pour planifier (planification des ressources ou des scénarios) et planifier (équilibreur de charge de travail) les ressources d’une organisation et les affecter au travail qui doit être effectué, en tenant compte de leur disponibilité. En outre, la gestion des ressources fait également référence à l’affichage d’informations sur les affectations de ressources prévues et réelles dans une vue de rapport (rapport Utilisation).

Workfront comporte plusieurs ensembles d’outils utilisés pour gérer les ressources. Chaque outil a une portée individuelle. Actuellement, vous pouvez utiliser les outils de gestion des ressources suivants dans Workfront, en fonction de l’étape de gestion des ressources dans laquelle vous vous trouvez :

* Pour planifier l’affectation des ressources à un niveau supérieur, utilisez les outils suivants avant le début du travail réel sur les projets :

   * **Le planificateur de ressources**: vous pouvez utiliser le planificateur de ressources dans la première étape de la gestion des ressources pour planifier l’heure de vos ressources en fonction de leur disponibilité planifiée. Lors de la phase de planification des ressources, vous pouvez organiser les utilisateurs dans les pools de ressources et affecter plusieurs pools de ressources à un projet.

     Pour plus d’informations sur la planification des ressources, voir la section [Planification des ressources dans Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **Planification du scénario**: il s’agit d’une planification des ressources de niveau supérieur qui vous permet de les gérer au cours de plusieurs initiatives qui peuvent s’étendre sur un, trois ou cinq ans et inclure plusieurs projets. Vous pouvez utiliser le meilleur scénario pour tirer le meilleur parti de leur disponibilité et de votre budget.

     Le planificateur de scénario nécessite une licence distincte, en plus de la licence Workfront. Pour plus d’informations sur le planificateur de scénario Workfront, voir [Présentation du planificateur de scénarios](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* Pour planifier ou affecter des ressources à un travail réel (tâches et problèmes), utilisez l’outil suivant :

   * **L’équilibreur de charge de travail**: il s’agit d’une étape inférieure de la gestion des ressources, dans laquelle vous pouvez affecter vos ressources au travail réel (tâches et problèmes) qu’elles doivent effectuer, en fonction du nombre d’heures nécessaires pour les terminer et de leur disponibilité. Avec l’équilibreur de charge de travail, vous pouvez affecter des utilisateurs à un travail réel qui n’est actuellement pas affecté ou affecté à des rôles de tâche.

     Pour plus d’informations sur l’équilibreur Workfront, voir la section [L’équilibreur de charge de travail : index de l’article](../../resource-mgmt/workload-balancer/workload-balancer.md).

<!--

  * **Scheduling** (deprecated <span class="preview">and removed from the Preview environment</span>): Refers to assigning actual work to users by matching the job roles assigned to the tasks and issues with the job roles they can fulfill, or assigning actual work to users on tasks and issues which are currently unassigned. This happens at a lower-level in the process of managing resources, where you can assign your resources to the actual work (tasks and issues) that they must fulfill, according to the hours needed in the project plan to fulfill them.  

     For more information about resource scheduling, see the section [Resource Scheduling](../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

    >[!CAUTION]
    >
    >
    >We are no longer supporting the Resource Scheduling tools and they will be removed from Workfront in **January 2023**. We recommend that you use the Workload Balancer for scheduling your resources. 
    >
    >
    >* For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).
    >
    >
    >* For more information about the timeline for removing the Resource Scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* Pour analyser les affectations prévues, prévues et réelles pour plusieurs projets, utilisez l’outil suivant :

   * **Rapport d’utilisation**: utilisez ce rapport pour afficher l’utilisation des ressources pour les projets. Vous pouvez comparer les affectations prévues, prévues et réelles pour vos projets et leur impact sur le coût et le chiffre d’affaires des projets.

     Pour plus d’informations sur le rapport d’utilisation, voir [Affichage des informations sur l’utilisation des ressources](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Composants du processus de gestion des ressources

>[!NOTE]
>
>La gestion des ressources n’est jamais un processus stagnant dans Workfront. Au fur et à mesure que les plannings de vos projets, la disponibilité de vos utilisateurs ou leurs rôles changent, vous devez continuellement ajuster les informations sur vos ressources, leurs affectations et leurs allocations aux projets, tâches et problèmes.

Le processus de gestion des ressources dans Workfront comprend les étapes suivantes :

* **Configuration**: en tant qu’administrateur système, responsable de ressources ou responsable de projet, vous devez configurer certains champs et objets dans votre instance Workfront avant de gérer vos ressources. Pour plus d’informations sur les conditions préalables requises pour commencer la gestion des ressources dans Workfront, voir la section [Prérequis pour une gestion précise des ressources](#prerequisites-for-accurate-resource-management) dans cet article.\
  Outre les projets comportant des éléments de travail, vous devez configurer les éléments suivants dans Workfront :

   * Utilisateurs\
     Pour plus d’informations sur la création d’utilisateurs, voir l’article [Ajout d’utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * Fonctions\
     Pour plus d’informations sur la création de rôles de tâche, consultez l’article [Création et gestion des rôles de tâche](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * Planifications\
     Pour plus d’informations sur la création de plannings, consultez l’article [Création d’un planning](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * Préférences Projet

     >[!TIP]
     >
     >Seul un administrateur système ou groupe peut modifier les préférences du projet pour votre système ou votre groupe.

     Pour plus d’informations sur la définition des préférences du projet, voir l’article [Configuration des préférences de projet à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * Pools de ressources

     Pour plus d’informations sur la création de pools de ressources, voir [Création de pools de ressources](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * Préférences de gestion des ressources

     En tant que système, vous devez décider comment Workfront calcule la disponibilité de l’utilisateur au niveau du système, que ce soit en utilisant la planification de l’utilisateur ou la planification par défaut de votre système.

     Pour plus d’informations, voir [Configuration des préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Allocation des ressources**: en tant que gestionnaire de ressources ou propriétaire de projet, vous pouvez définir l’allocation des ressources pour vos projets et affecter du travail. Pour cette étape, vous pouvez gérer l’estimation de l’allocation de vos ressources à l’aide du planificateur de ressources ou du planificateur de scénario, et affecter le travail réel aux utilisateurs dans l’équilibreur de charge de travail.

  Pour plus d’informations sur la planification des ressources et l’affectation des tâches, consultez les sections suivantes :

   * [Planification des ressources dans Adobe Workfront](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [Gestionnaire de scénarios Adobe Workfront](../../scenario-planner/scenario-planning.md)
   * [L’équilibreur de charge de travail : index de l’article](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Overview of the Workload Balancer](../workload-balancer/overview-workload-balancer.md). 
-->

* **Analyse**: en tant que responsable des ressources, responsable de projet ou responsable de personnes, consultez le rapport d’utilisation pour comparer les affectations planifiées et budgétées de vos ressources aux affectations réelles. Consultez les informations par heures, coût ou recettes. Pour plus d’informations sur le rapport Utilisation, voir [Affichage des informations sur l’utilisation des ressources](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Accès nécessaire pour afficher et gérer les ressources à l’aide des outils de gestion des ressources dans Workfront

Les utilisateurs suivants ont accès aux outils de gestion des ressources dans Workfront :

Vous devez être l’un des utilisateurs suivants et disposer des droits d’accès et des autorisations suivants pour accéder aux outils de gestion des ressources :

* Administrateur système.
* Un utilisateur disposant d’une licence Plan.

  Un utilisateur disposant d’une licence de travail peut utiliser l’équilibreur de charge de travail d’un projet et gérer les affectations et les affectations.

  Outre le fait d’avoir une licence Work ou supérieure, vous devez disposer des éléments suivants pour utiliser des outils de gestion de ressources spécifiques :

   * Modifier l’accès à la gestion des ressources (non nécessaire pour effectuer des affectations dans l’équilibreur de charge de travail)
   * Modifier l’accès aux données financières pour afficher les informations de coût dans le planificateur de ressources
   * Afficher l’accès aux données financières pour afficher les informations sur les coûts et les recettes dans le rapport d’utilisation (seuls les utilisateurs disposant d’une licence Plan)

* Contribuez à des autorisations ou des autorisations supérieures qui incluent l’option Rendre des affectations sur les projets pour lesquels vous souhaitez gérer des ressources.

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

Pour plus d’informations sur l’accès aux ressources du budget, consultez l’article . [Accès aux ressources du budget](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Pour plus d’informations sur l’accès nécessaire à la gestion des ressources dans l’équilibreur de charge de travail, voir [Accès nécessaire pour gérer les ressources dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## Prérequis pour une gestion précise des ressources  {#prerequisites-for-accurate-resource-management}

Pour pouvoir utiliser efficacement les outils de gestion des ressources de Workfront, vous devez répondre à un ensemble de exigences.

Pour plus d’informations sur les exigences de chaque outil de gestion des ressources dans Workfront, voir :

* La section &quot;Conditions préalables requises pour travailler dans le planificateur de ressources&quot; de l’article [Présentation de Resource Planner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
  <!--remove this at production: * The section "Prerequisites" in the article [Get started with Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).-->
* La section &quot;Bonnes pratiques pour l’utilisation de l’équilibreur de charge de travail&quot; de l’article [Présentation de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Accès aux ressources de budget nécessaires dans Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [Accès nécessaire pour gérer les ressources dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and replaced with the links to each prerequisites instead) </p>
<p> We recommend that the following settings exist before starting to manage resources for your organization: </p>
<ul>
<li> You must have users in the system who have active accounts. </li>
<li> You must assign a Plan or a Worker license to the users whose work allocation you want to manage. <note type="note">
Although you can assign work to a Reviewer or a Requestor, they cannot complete it.
<br>We recommend against assigning work to Reviewers or Requestors. For information about access levels in Workfront, see
<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref" xrefformat="{para}">Access levels overview</a>.
</note></li>
<li> You must have job roles configured in the system.<br>For information about adding job roles to Workfront, see the article <a href="../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" xrefformat="{para}">Create and manage job roles</a>.</li>
<li> (Optional) If you want to budget cost for your work, your job roles and your users must also have rates associated with them.<br></li>
<li> You must associate at least one job role with your users. </li>
<li> You must specify a valid value for the FTE field of all users when you use the User's Schedule instead of The Default Schedule in your Resource Management system preferences. <br>For information about editing users to ensure they have a job role, FTE, or cost associated with them, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" xrefformat="{para}">Edit a user's profile</a>. For information about editing the Resource Management preferences in your system, see <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref" xrefformat="{para}">Configure Resource Management preferences</a>.</li>
<li>You must associate accurate schedules with your users and they should include schedule exceptions.<br>For information about creating and editing schedules, see the article <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref" xrefformat="{para}">Create a schedule</a>.</li>
<li>The Time Off calendar of the users must be up to date. </li>
<li> <p>The following is recommended for the Resource Planner when applying the Project and Role views: </p>
<ul>
<li> <p>You must associate projects with Resource Pools.<br>For information about associating projects with Resource Pools, see <a href="../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-projects-and-templates.md" class="MCXref xref" xrefformat="{para}">Associate resource pools with projects and templates</a>.</p> </li>
</ul> </li>
<li> <p>Your must designate a Resource Manager on your projects and they must have the correct access to budget resources when using the Scheduling tools. </p> <p>For information about the access needed to budget resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref" xrefformat="{para}">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> </li>
<li> <p>You must assign the tasks and issues in your system to job roles, teams, or users.</p> </li>
<li>You must specify a valid value for Planned Hours and Duration for all tasks in your system.<br>For information about Planned Hours, see the article <a href="../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref" xrefformat="{para}">Planned Hours overview</a>.<br>For information about Duration, see the article <a href="../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md" class="MCXref xref" xrefformat="{para}">Overview of Task Duration and Duration Type</a>.</li>
</ul>
</div>
-->
