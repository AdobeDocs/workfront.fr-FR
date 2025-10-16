---
content-type: overview
product-area: resource-management
navigation-topic: resource-management-overview
title: Prise en main de la gestion des ressources
description: La gestion des ressources vous permet de configurer votre système pour prévoir précisément l’utilisation de vos ressources en fonction de leur disponibilité, de sorte que le travail soit terminé en respectant le délai et le budget.
author: Lisa
feature: Resource Management
exl-id: b10ef503-60ea-4450-b63e-b2918e9bcc11
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 96%

---

# Commencer avec la gestion des ressources

<!-- Audited: 12/2023 -->

<!--
<p>(NOTE: DO NOT DELETE THIS ARTICLE. MANY ARTICLES MENTIONING RES MANAGEMENT ARE AND STILL SHOULD / WILL BE LINKED TO IT.) </p>
<p>(NOTE: Alina: ***As functionality is removed from Legacy and added to Res Planning - this will be continually updated: remove the Legacy Res Planning when that functionality is removed from the system.) </p>
</div>
-->

La gestion des ressources vous permet de configurer votre système pour prévoir précisément l’utilisation de vos ressources en fonction de leur disponibilité, de sorte que le travail soit terminé en respectant le délai et le budget.

## Vue d’ensemble de la gestion des ressources dans Adobe Workfront

La gestion des ressources fait référence à toutes les activités exécutées par l’administrateur ou l’aministratrice Adobe Workfront, la personne en charge de la gestion des ressources et la personne propriétaire du projet pour planifier les ressources d’une organisation (planification des ressources, des scénarios et équilibreur de charge de travail) et les affecter au travail qui doit être effectué, en tenant compte de leur disponibilité. En outre, la gestion des ressources fait également référence aux informations sur les affectations de ressources prévues et effectives dans une vue de rapport (rapport d’utilisation).

Workfront comporte plusieurs ensembles d’outils utilisés pour gérer les ressources. Chaque outil a une portée individuelle. Actuellement, vous pouvez utiliser les outils de gestion des ressources suivants dans Workfront, en fonction de votre étape de gestion des ressources actuelle :

* Pour planifier l’affectation des ressources à un niveau supérieur, utilisez les outils suivants avant le début du travail effectif sur les projets :

   * **Planificateur de ressources** : vous pouvez utiliser le planificateur de ressources dans la première étape de la gestion des ressources pour planifier l’heure d’utilisation de vos ressources en fonction de leur disponibilité prévue. Lors de la phase de planification des ressources, vous pouvez organiser les personnes dans des groupes de ressources et affecter plusieurs groupes de ressources à un projet.

     Pour plus d’informations sur la planification des ressources, voir [Planification des ressources : index des articles](../../resource-mgmt/resource-planning/resource-planning-overview.md).

   * **Planification de scénarios** : il s’agit d’une planification des ressources de niveau supérieur qui vous permet de les gérer dans le cadre de multiples initiatives qui peuvent s’étendre sur un, trois ou cinq ans et inclure plusieurs projets. Vous pouvez utiliser le meilleur scénario pour maximiser leur disponibilité et respecter votre budget.

     Le planificateur de scénarios nécessite une licence distincte, en plus de la licence Workfront. Pour plus d’informations sur le planificateur de scénarios Workfront, consultez [Vue d’ensemble du planificateur de scénarios](../../scenario-planner/scenario-planner-overview.md).

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when more functionality is added, maybe we add that we recommend to start here if this is available for them?!) </p>   
     -->

* Pour planifier ou affecter des ressources à un travail effectif (tâches et problèmes), utilisez l’outil suivant :

   * **Équilibreur de charge de travail** : il s’agit d’une étape inférieure de la gestion des ressources, dans laquelle vous pouvez affecter vos ressources au travail effectif (tâches et problèmes) qu’elles doivent faire, en fonction du nombre d’heures nécessaires pour le terminer et de leur disponibilité. Avec l’équilibreur de charge de travail, vous pouvez affecter des utilisateurs et des utilisatrices à un travail effectif qui n’est actuellement pas affecté ou affecté à certains rôles

     Pour plus d’informations sur l’équilibreur Workfront, consultez [Équilibreur de charge de travail : index des articles](../../resource-mgmt/workload-balancer/workload-balancer.md).

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
* Pour analyser les affectations budgétées, prévues et effectives pour plusieurs projets, utilisez l’outil suivant :

   * **Rapport d’utilisation** : utilisez ce rapport pour afficher l’utilisation des ressources pour les projets. Vous pouvez comparer les affectations budgétées, prévues et effectives pour vos projets et leur impact sur le coût et le chiffre d’affaires des projets.

     Pour plus d’informations sur le rapport d’utilisation, consultez [Afficher des informations sur l’utilisation des ressources](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Composants du processus de gestion des ressources

>[!NOTE]
>
>La gestion des ressources n’est jamais un processus stagnant dans Workfront. Au fur et à mesure que les plannings de vos projets, la disponibilité de vos utilisateurs et utilisatrices ou leurs rôles changent, vous devez continuellement ajuster les informations sur vos ressources, leurs affectations et leurs allocations aux projets, tâches et problèmes.

Le processus de gestion des ressources dans Workfront comprend les étapes suivantes :

* **Configuration** : en tant qu’administrateur ou administratrice système, personne responsable de ressources ou de projet, vous devez configurer certains champs et objets dans votre instance Workfront avant de gérer vos ressources. Pour plus d’informations sur les conditions préalables requises pour commencer la gestion des ressources dans Workfront, consultez la section [Conditions préalables pour une gestion précise des ressources](#prerequisites-for-accurate-resource-management) dans cet article.\
  Outre les projets comportant des éléments de travail, vous devez configurer les éléments suivants dans Workfront :

   * Utilisateurs\
     Pour plus d’informations sur la création d’utilisateurs et d’utilisatrices, voir l’article [Ajouter des utilisateurs et utilisatrices](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   * Fonctions\
     Pour plus d’informations sur la création de fonctions, consultez l’article [Créer et gérer des fonctions](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

   * Planifications\
     Pour plus d’informations sur la création de plannings, consultez l’article [Créer un planning](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * Préférences Projet

     >[!TIP]
     >
     >Seulement un administrateur ou une administratrice système ou de groupes peut modifier les préférences du projet pour votre système ou votre groupe.

     Pour plus d’informations sur la définition des préférences du projet, voir l’article [Configurer les préférences de projet à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * Pools de ressources

     Pour plus d’informations sur la création de groupes de ressources, voir [Créer des groupes de ressources](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

   * Préférences de gestion des ressources

     En tant que système, vous devez décider comment Workfront calcule la disponibilité des utilisateurs et utilisatrices au niveau du système, que ce soit en utilisant leur planning ou le planning par défaut de votre système.

     Pour plus d’informations, voir [Configurer les préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Allocation des ressources** : en tant que personne gestionnaire de ressources ou propriétaire de projet, vous pouvez définir l’allocation des ressources pour vos projets et attribuer le travail. Pour cette étape, vous pouvez gérer l’estimation de l’allocation de vos ressources à l’aide du planificateur de ressources ou du planificateur de scénarios, et attribuer le travail réel aux utilisateurs et utilisatrices dans l’équilibreur de charge de travail.

  Pour plus d’informations sur la planification des ressources et l’affectation du travail, consultez les sections suivantes :

   * [Planification des ressources : index des articles](../../resource-mgmt/resource-planning/resource-planning-overview.md)
   * [[!DNL Adobe Workfront Scenario Planner] : index des articles](../../scenario-planner/scenario-planning.md)
   * [Équilibreur de charge de travail : index des articles](../../resource-mgmt/workload-balancer/workload-balancer.md)

<!--
* **Resource scheduling**: After generally planning for resources to use on your projects at a high level, you can start assigning work items (tasks and issues) to users based on their job roles using the Workload Balancer.

  For more information, see [Workload Balancer overview](../workload-balancer/overview-workload-balancer.md). 
-->

* **Analyse** : en tant que personne reponsable de la gestion des ressources, propriétaire du projet ou responsable du personnel, vous devez examiner le rapport d’utilisation pour comprendre comment les affectations budgétées et prévues de vos ressources se comparent aux affectations réelles. Examinez les informations par heures, par coûts ou par revenus. Pour plus d’informations sur le rapport d’utilisation, consultez la section [Afficher les informations d’utilisation des ressources](../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Accès nécessaire pour afficher et gérer les ressources à l’aide des outils de gestion des ressources dans Workfront

Les types d’utilisateurs et d’utilisatrices suivants ont accès aux outils de gestion des ressources dans Workfront :

Pour accéder aux outils de gestion des ressources, vous devez appartenir à l’un des types d’utilisateurs et d’utilisatrices suivants et disposer des accès et autorisations présentés ci-dessous :

* Personne responsable de l’administration du système.
* Utilisateur disposant d’une licence Standard ou Plan.

  Un utilisateur ou une utilisatrice disposant d’une licence Travail peut utiliser l’équilibreur de charge de travail d’un projet et gérer les affectations et les allocations.

  Outre une licence de travail ou supérieure (ou une licence standard), vous devez disposer des éléments suivants pour utiliser des outils de gestion des ressources spécifiques :

   * Modifier l’accès à la gestion des ressources (non nécessaire pour effectuer des affectations dans l’équilibreur de charge de travail)
   * Modifier l’accès aux données financières pour afficher les informations sur les coûts dans le planificateur de ressources
   * Afficher l’accès aux données financières pour visualiser les informations sur les coûts et les revenus dans le rapport d’utilisation (uniquement pour les utilisateurs et les utilisatrices disposant d’une licence Plan).

* Autorisations de contribution ou de niveau supérieur qui incluent « Créer des affectations » sur les projets dont vous souhaitez gérer les ressources.

<!--
* Designated as a Resource Manager for projects to use the Scheduling tool (the Scheduling tool is deprecated).

  >[!TIP]
  >
  >You do not have to be a Resource Manager to use the Resource Planner, Scenario Planner, or the Workload Balancer. 
-->

Pour plus d’informations sur l’accès nécessaire à l’établissement d’un budget de ressources, consultez l’article [Accès nécessaire pour établir un budget de ressources](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Pour plus d’informations sur l’accès nécessaire à la gestion des ressources dans l’équilibreur de charge de travail, consultez la section [Accès nécessaire pour gérer les ressources dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

## Conditions préalables à une gestion précise des ressources  {#prerequisites-for-accurate-resource-management}

Vous devez remplir un certain nombre de conditions avant de pouvoir utiliser efficacement les outils de gestion des ressources dans Workfront.

Pour plus d’informations sur les conditions préalables pour chaque outil de gestion des ressources dans Workfront, consultez les sections suivantes :

* La section [Conditions préalables pour travailler dans le planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planner.md#prerequisites-for-working-in-the-resource-planner) dans l’article [Vue d’ensemble du planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planner.md).
* La section [Bonnes pratiques pour l’utilisation de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/overview-workload-balancer.md#best-practices-for-using-the-workload-balancer) dans l’article [Vue d’ensemble de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
* [Accès nécessaire à l’établissement d’un budget de ressources dans Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).
* [Accès nécessaire à la gestion des ressources dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

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
