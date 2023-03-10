---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Présentation des affectations intelligentes
description: Lors de la gestion des tâches et des affectations de problèmes, vous pouvez utiliser des affectations intelligentes pour identifier le meilleur utilisateur à effectuer le travail. Les affectations intelligentes sont des suggestions qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources en fonction d’un algorithme qui détermine la ressource la plus appropriée pour la tâche.
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 7e220e496aff2675910416bd86e3ddf7b9231afa
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Présentation des affectations intelligentes

Lors de la gestion des tâches et des affectations de problèmes, vous pouvez utiliser des affectations intelligentes pour identifier le meilleur utilisateur à effectuer le travail. Les affectations intelligentes sont des suggestions qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources en fonction d’un algorithme qui détermine la ressource la plus appropriée pour la tâche.

>[!NOTE]
>
>Les affectations intelligentes ne prennent pas en compte la disponibilité de l’utilisateur. Toutefois, leur disponibilité en fonction de leurs plannings affecte les Dates prévues et prévues des tâches et des problèmes lorsqu’elles sont affectées. Pour plus d’informations sur les plannings, voir l’article [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Cet article contient des informations générales sur les affectations intelligentes. Pour plus d’informations sur l’utilisation d’affectations intelligentes pour affecter des tâches et des problèmes aux utilisateurs, voir [Rendre des affectations intelligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## Présentation des affectations intelligentes

Tenez compte des points suivants lorsque vous utilisez des affectations intelligentes :

* L’algorithme fonctionne indépendamment pour les tâches et les problèmes. Cela signifie que la liste des utilisateurs suggérés pour les problèmes peut différer de celle des utilisateurs suggérés pour une tâche, car Workfront crée les listes en fonction de critères relatifs aux problèmes et aux tâches séparément.
* Les affectations intelligentes ne recommandent pas les rôles ou les équipes de travail. Il s’agit plutôt de suggestions d’utilisateurs qui sont les mieux à même d’effectuer une tâche ou un problème.
* Les affectations suggérées sont toujours des utilisateurs principaux.
* L’utilisateur répertorié en premier doit correspondre le mieux à la tâche.

## Recherche de suggestions d’affectation dynamique

Vous pouvez afficher des affectations intelligentes dans les zones suivantes où vous pouvez affecter des tâches ou des problèmes :

* une tâche, une liste de problèmes ou un rapport ;

   ![](assets/smart-assignments-task-list-nwe-350x280.png)

* Un en-tête de tâche ou de problème

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

* Panneau Résumé de la tâche ou du problème

   ![](assets/smart-assignments-summary-panel-nwe-350x332.png)

* Le champ Affectations pour un élément répertorié dans la zone Accueil

   ![](assets/smart-assignments-in-home-nwe-350x216.png)


<!--removed for scheduling deprecation: 

* Resource Scheduling

  ![](assets/smart-assignments-scheduling-350x219.png)

  >[!CAUTION]
  >
  >Resource Scheduling is a deprecated feature. For more information, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).

-->
* Équilibreur de charge de travail

   ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## Critères d’attribution intelligente

Les affectations intelligentes affichent les 50 premières recommandations basées sur un algorithme propriétaire.

Les utilisateurs sont recommandés dans la liste déroulante Affectations intelligentes en fonction d’une combinaison des critères suivants (répertoriés dans l’ordre du plus important au moins important) :

* Utilisateurs affectés à d’autres tâches au cours des 30 derniers jours par l’utilisateur effectuant l’affectation. Les 50 premiers utilisateurs qui correspondent à ce critère s’affichent. L’utilisateur qui est le plus souvent affecté s’affiche en premier.

   Si l’élément de travail est attribué à une équipe ou à un rôle, la liste des utilisateurs suggérés est filtrée en tenant compte des affectations existantes ci-dessous. Dans ce cas, seuls les utilisateurs suivants s’affichent dans la liste des suggestions :

   * Utilisateurs dont l’équipe d’accueil est l’équipe affectée à l’élément de travail.
   * Utilisateurs dont le rôle Principal est le rôle attribué à l’élément de travail.

      >[!TIP]
      >
      >* If <!--you're not part of any team and --> si aucun rôle ou équipe n’est affecté à la tâche ou au problème, Workfront affiche tous les utilisateurs affectés au cours des 30 derniers jours, jusqu’à 50 utilisateurs.
      >* Si vous n’avez effectué aucune affectation au cours des 30 derniers jours, seuls les utilisateurs appartenant à l’équipe affectée ou ayant le rôle affecté à l’élément de travail s’affichent dans la liste des affectations intelligentes.


<!--the commented out piece in the tip above was live before but I am not totally sure that smart assignments look at your team. I think they look JUST at the team/ role assigned to the work item; see this help site request for more info: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/62fd222200037eb87572c5b6ad6bf53e/overview -->
<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h3>Smart assignments criteria for the Production environment</h3>
<p>(NOTE: drafted,this was the case BEFORE we updated the logic in the WB - with the 21.4 release)</p>
</div>
<p>Smart assignments display on tasks and issues when the following conditions are met:</p>
<ul>
<li>The task or issue is subordinate to a parent task or issue that has a user, team, or job role currently assigned. </li>
</ul>
<p>Smart assignments display the top twenty recommendations based on a proprietary algorithm that uses your own team information.</p>
<p>Users are recommended in the smart assignments drop-down list based on a combination of the following criteria (listed in order from most important to least important):</p>
<ul>
<li>The user has the team assigned to the task or issue designated as their Home Team</li>
<li>The user is also assigned to the parent task</li>
<li>The user has the same primary job role as is currently assigned to the task or issue</li>
<li>The user has the team assigned to the parent task or issue designated as their Home Team</li>
<li>The user is associated with the same primary job role currently assigned to the parent task</li>
<li>The user is a member of the same team as the user who assigned the task or issue and the team is designated as their Home Team</li>
<li>The user is a member of the same Home Group as the user who is assigning the task or issue</li>
<li>The user has the same primary job role as the user who is assigning the task or issue.</li>
</ul>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Make smart assignments</h2>
<p>(NOTE:&nbsp;this was moved to its own article: make-smart-assignments.) </p>
<p>Smart assignments are available in most locations where you can make assignments in Workfront.</p>
<p>You can use smart assignments on tasks and issues that have previously been assigned to a job role or a team.</p> <note type="note">
You must have a Plan or a Work license and have at least Contribute permissions to a task or an issue to be able to make assignments to the task or the issue. You must have the Make Assignments option enabled in your permission level to make assignments.
</note>
<p>To use smart assignments:</p>
<ol>
<li value="1">Navigate to an issue or a task and click one of the following fields to edit them: <br>
<ul>
<li><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">The <strong>Assignments</strong> field in the task or issue header</p></li>
<li>The <strong>Assignments</strong> field of a task or issue list using in-line editing in a task or issue list. </li>
<li>The <strong>Assignee</strong> field after you have clicked <strong>Advanced</strong> from a task or an issue. </li>
</ul></li>
<li value="2"> <p>Place your cursor in the assignment field, and wait for two seconds, then the <strong>Suggestions</strong> list is displayed.</p> <p>Users displayed in this list are the smart assignment suggestions for the task or the issue.<br></p> <p> <img src="assets/nwe-smart-assignment-suggestions-350x160.png" style="width: 350;height: 160;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3"> <p>Select the user in the recommendations list by clicking their name. </p> <p>If there are no suggestions, the suggestion list does not open.</p> </li>
<li value="4">(Optional) If you do not want to use one of the recommended users from the smart assignments list, start typing the name of the desired user and select the name when it appears in the list.</li>
<li value="5">Click <strong>Enter</strong> to make the assignment. </li>
</ol>
</div>
-->
