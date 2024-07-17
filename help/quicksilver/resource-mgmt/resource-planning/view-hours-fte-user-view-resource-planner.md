---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: Afficher les heures disponibles, prévues et effectives ou ETP dans le planificateur de ressources lors de l’utilisation de la vue Utilisateur ou utilisatrice
description: Afficher les heures disponibles, planifiées et réelles ou l’éditeur de texte enrichi dans le planificateur de ressources lors de l’utilisation de l’affichage des utilisateurs dans le programme de recherche (RP), par exemple "budget des ressources dans le programme de recherche" ou "Gestion des ressources dans le programme de recherche". etc.. - ou peut nécessiter une réutilisation à partir d’un autre POV?!)"
author: Alina
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1739'
ht-degree: 3%

---

# Afficher les heures disponibles, prévues et effectives ou ETP dans le planificateur de ressources lors de l’utilisation de la vue Utilisateur ou utilisatrice

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

Outre la planification des ressources dans les vues Projet et Rôle, vous pouvez utiliser la vue Utilisateur du planificateur de ressources Adobe Workfront pour afficher des informations sur les valeurs Heures prévues, Disponibles et Réelles ou ETR pour les projets et les ressources.

## Vue d’ensemble de l’utilisateur dans le planificateur de ressources

Tenez compte de ce qui suit lors de l’affichage des informations Heures ou ETR dans le planificateur de ressources :

* Vous pouvez afficher les heures disponibles et planifiées ou les informations de l’éditeur de texte enrichi pour les utilisateurs, les rôles de tâche et les projets dans toutes les vues du planificateur de ressources.
* Vous ne pouvez afficher les informations suivantes que dans la vue Utilisateur :

   * Différence entre le nombre d’heures planifiées ou l’ETR et le nombre d’heures disponibles ou d’ETR. Vous pouvez ensuite budgéter l’allocation de vos utilisateurs en fonction de cette différence dans les vues Projet et Rôle .
   * Heures réelles ou ETR.

* Vous pouvez afficher la différence entre l’utilisateur disponible et le nombre d’heures planifiées ou l’éditeur de texte enrichi sous la forme d’un nombre ou d’un pourcentage dans la vue Utilisateur.
* Vous ne pouvez pas afficher les informations dans la vue Utilisateur par coût.
* Adobe Workfront renseigne les heures disponibles ou l’éditeur de texte enrichi en fonction du temps de travail associé aux utilisateurs dans leurs plannings.\
  Les utilisateurs non associés à un planning affichent la disponibilité selon le planning par défaut.\
  Pour plus d’informations sur la planification par défaut, voir [Création d’une planification](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfront renseigne les informations Heures planifiées ou ETR à partir des Heures planifiées sur les tâches et les problèmes des projets.
* Workfront renseigne la valeur Heures réelles avec le temps réel consigné dans les tâches et les problèmes par les utilisateurs qui leur sont affectés. Cela inclut le temps de connexion à un projet.
* Dans la vue Utilisateur, vous pouvez effectuer les opérations suivantes :

   * Développez chaque utilisateur pour afficher la liste des projets auxquels cet utilisateur est affecté.

     >[!NOTE]
     >
     >Seuls les utilisateurs associés aux projets inclus dans les filtres peuvent être développés.

   * Développez chaque projet pour afficher la liste des rôles de tâche que l’utilisateur peut remplir sur ces projets.
   * Développez chaque rôle pour afficher la liste des tâches auxquelles l’utilisateur est affecté.

  Si aucun rôle de travail n’est associé aux utilisateurs, leurs heures disponibles, planifiées et réelles ou leur éditeur de texte enrichi sont répertoriées dans la section **Aucun rôle** .\
  Pour plus d’informations sur les champs et les éléments qui s’affichent lors de l’application de la vue Utilisateur au planificateur de ressources, voir la section &quot;Projet/Rôle/Sélection de la vue utilisateur&quot; dans la [présentation de la navigation du planificateur de ressources](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Présentation des champs visibles dans la vue utilisateur du planificateur de ressources

Reportez-vous aux tableaux suivants pour comprendre les informations affichées dans la vue Utilisateur du planificateur de ressources. Les informations s’affichent dans les valeurs Heures ou ETR.

* [Colonne AVL (disponible)](#the-avl-available-column)
* [Colonne PLN (planifiée)](#the-pln-planned-column)
* [Colonne ACT (Réel)](#The%C2%A0ACT)
* [Colonne DIF (Différence)](#the-dif-difference-column)
* [Colonne % (Pourcentage d’affectation des heures planifiées)](#the-planned-hours-allocation-percentage-column)

### La colonne AVL (Disponible) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché Par</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td>Total des heures disponibles ou de l’éditeur de texte enrichi pour l’utilisateur selon son planning. </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Ces informations ne sont pas disponibles pour le projet lorsque la vue Utilisateur est appliquée au planificateur de ressources. </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Total des heures disponibles ou de l’éditeur de texte enrichi pour le rôle, en fonction du planning de l’utilisateur et du <strong>pourcentage de disponibilité de l’éditeur de texte enrichi</strong> du rôle.</p> </td> 
  </tr> 
  <tr> 
   <td>Tâche ou problème</td> 
   <td>Ces informations ne sont pas disponibles pour la tâche ou le problème. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le mode de calcul de la disponibilité des utilisateurs et des rôles en fonction du planning de l’utilisateur et du pourcentage de disponibilité de l’éditeur de texte enrichi du rôle, voir [Présentation du calcul des heures et de l’éditeur de texte enrichi pour les utilisateurs et les rôles dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### Colonne PLN (planifiée) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché Par</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> Total des heures planifiées ou de l’éditeur de texte enrichi pour toutes les tâches ou tous les problèmes affectés à l’utilisateur sur tous les projets.<br><p>Cela inclut les tâches et les problèmes qui sont affectés à l’utilisateur, mais qui ne sont associés à aucun rôle de tâche, ainsi que les tâches ou les problèmes qui ne se trouvent pas sur les projets que vous avez accès à Gérer.</p><p>Lorsque l’allocation utilisateur des heures a été modifiée à l’aide de l’équilibreur de charge de travail, les données du planificateur de ressource peuvent être affectées si les dates sélectionnées ne contiennent qu’une partie d’une tâche ou d’un problème. Pour plus d’informations sur la modification des attributions pour les utilisateurs, voir <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gestion des affectations des utilisateurs dans l’équilibreur de charge de travail</a> . </p></td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td> Total des heures planifiées ou de l’éditeur de texte enrichi de toutes les tâches et problèmes affectés à un utilisateur spécifique du projet.<br><p>Remarque : Cela n’inclut pas les heures planifiées ou l’éditeur de texte enrichi des tâches ou des problèmes qui ne sont attribués à aucun utilisateur. </p></td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Total des heures planifiées ou de l’éditeur de texte enrichi de toutes les tâches et problèmes affectés à l’utilisateur dans ce rôle sur le projet.</p> <p> <p>Remarque : Cela n’inclut pas les heures planifiées ou l’éditeur de texte enrichi des tâches ou des problèmes affectés à ce rôle, mais pas à cet utilisateur dans ce rôle. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Tâche ou problème</td> 
   <td>Heures planifiées ou ETR associées à la tâche ou au problème du projet.</td> 
  </tr> 
 </tbody> 
</table>

Tenez compte des points suivants lors de l’affichage des heures planifiées :

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* Les Heures planifiées sont réparties de manière égale à chaque jour dans la Durée des tâches et des problèmes pour chaque ressource qui leur est affectée. La durée de la tâche ou du problème est basée sur les dates de début et de fin planifiées et inclut chaque jour calendaire de cette période.\
  Workfront prend en compte le planning de l’utilisateur ou du projet lors de la distribution des heures planifiées aux utilisateurs ou aux projets. Dans ce cas, les heures planifiées sont réparties de manière égale entre chaque jour dans la Durée des tâches ou des problèmes, à l’exception des week-ends, jours de congé et des exceptions de planification.

  Si, par exemple, vous affichez le planificateur de ressources par semaine et que vous avez des tâches qui s’étendent sur plusieurs semaines sur des projets, le nombre d’heures planifiées par semaine dépend du nombre de jours de cette semaine qui font partie de la durée de la tâche. Cela fonctionne de la même manière lors de l’affichage du planificateur de ressources par mois ou par trimestre et lorsque les tâches s’étendent sur plusieurs mois ou trimestres.\
  Les jours du week-end, les exceptions de planification et les jours de congé sont exclus de cette distribution.

* Les catégories de tâches suivantes sont incluses dans le calcul des Heures planifiées pour chaque ressource :

   * tâches affectées aux utilisateurs dans les groupes de ressources, les rôles de tâche ou les équipes du projet.

     >[!TIP]
     >
     >Si des tâches sont affectées à des équipes, leur attribution apparaît sous les sections **Aucun rôle** et **Aucun utilisateur** . Vous pouvez voir les Heures planifiées associées aux équipes, mais vous ne pouvez pas budgéter les heures, car aucun rôle ni utilisateur n’est associé aux tâches.

* Les heures planifiées dans le planificateur de ressources n’incluent pas les heures planifiées associées aux éléments suivants :

   * tâches parentes
   * tâches non affectées
   * problèmes, lorsque le paramètre **Inclure les heures à partir des problèmes** est désactivé.

* Les heures planifiées ne s’affichent pas dans le planificateur de ressources si la durée de la tâche ou du problème est nulle.
* Les heures planifiées associées aux utilisateurs désactivés ne s’affichent pas.

Pour plus d’informations sur les heures planifiées et l’éditeur de texte enrichi dans le planificateur de ressources, voir [Aperçu des heures, de l’éditeur de texte enrichi et des informations sur les coûts dans les vues Projet et Rôle du planificateur de ressources](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### La colonne ACT (Réel)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché Par</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice </td> 
   <td> <p>Heure consignée par l’utilisateur sur toutes les tâches ou tous les problèmes qui lui sont affectés.</p> <p>Cela inclut les éléments suivants :</p> 
    <ul> 
     <li>Tâches et problèmes affectés à l’utilisateur, mais non associés à un rôle de tâche.</li> 
     <li>Tâches et problèmes qui ne concernent pas les projets pour lesquels vous avez accès à l’option Gérer . </li> 
    </ul> <p>Cela inclut le temps de connexion au projet uniquement lorsque l’utilisateur est affecté à des tâches ou à des problèmes sur ce projet.  </p> </td> 
  </tr> 
  <tr> 
   <td>Projet </td> 
   <td> <p>Heure consignée par l’utilisateur pour toutes les tâches et tous les problèmes qui lui sont affectés sur le projet.</p> <p>Cela inclut le moment où ils se sont connectés directement au projet.</p> <p>Cela ne comprend pas les éléments suivants :</p> 
    <ul> 
     <li> <p>Heure de connexion aux tâches et problèmes qui ne sont attribués à aucun utilisateur. </p> </li> 
     <li> <p>Heure de connexion aux tâches parentes. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Heure de connexion à toutes les tâches ou problèmes affectés à l’utilisateur dans ce rôle. </p> <p>Cela ne comprend pas les éléments suivants :</p> 
    <ul> 
     <li>Heure de connexion aux tâches et problèmes affectés à ce rôle, mais pas à cet utilisateur dans ce rôle.</li> 
     <li>Heure de connexion directe au projet ou aux tâches parentes. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Tâche ou problème </td> 
   <td> <p>Heure de connexion aux tâches et problèmes par l’utilisateur qui lui est également affecté. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>L’heure consignée s’affiche dans la période correspondant à la Date d’entrée de l’heure, quelle que soit la période de la tâche, du problème ou du projet où les heures sont consignées.

Pour plus d’informations sur les heures réelles, voir [Afficher les heures réelles](../../manage-work/tasks/task-information/actual-hours.md).

### Colonne DIF (Différence) {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché Par</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Différence entre les heures disponibles et planifiées ou l’ETR de l’utilisateur. </p> <p>La différence Heure ou ETR est calculée à l’aide de la formule suivante :</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>Remarque : Si la valeur s’affiche en chiffres rouges négatifs, l’utilisateur est surchargé. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Ces informations ne sont pas disponibles pour le projet. </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Différence entre les heures disponibles et planifiées ou l’éditeur de texte enrichi du rôle de tâche. </p> <p>La différence Heure ou ETR est calculée à l’aide de la formule suivante :</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>Remarque : Si la valeur est affichée en chiffres rouges négatifs, le rôle est suralloué. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Tâche ou problème</td> 
   <td>Ces informations ne sont pas disponibles pour la tâche, le problème ou le projet. </td> 
  </tr> 
 </tbody> 
</table>

### Colonne % (Pourcentage d’affectation des heures planifiées) {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché Par</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Allocation des heures planifiées ou de l’éditeur de texte enrichi en pourcentage des heures disponibles. Le pourcentage de l’allocation des heures planifiées est calculé à l’aide de la formule suivante :</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>Le même calcul est utilisé pour les valeurs de l’éditeur de texte enrichi. </p> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Ces informations ne sont pas disponibles pour le projet lors de l’application de la vue <strong>Vue par l’utilisateur</strong> au planificateur de ressources.</td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> Allocation des heures planifiées ou de l’éditeur de texte enrichi en pourcentage des heures disponibles. <p>Le pourcentage de l’allocation des heures planifiées est calculé à l’aide de la formule suivante :</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>Le même calcul est utilisé pour les valeurs de l’éditeur de texte enrichi.</p></td> 
  </tr> 
  <tr> 
   <td>Tâche ou problème</td> 
   <td>Ces informations ne sont pas disponibles pour la tâche, le problème ou le projet. </td> 
  </tr> 
 </tbody> 
</table>

Si la valeur de l’heure planifiée ou de l’éditeur de texte enrichi est zéro, le pourcentage d’allocation est de 0 %. Si la valeur de l’heure disponible ou de l’éditeur de texte enrichi est égale à zéro, le pourcentage d’allocation ne peut pas être calculé.

Pour plus d’informations sur les heures planifiées et l’éditeur de texte enrichi, ainsi que sur leur affichage dans le planificateur de ressources, voir [Ressources de budget dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this table is ideal but it does not render in Markdown) </p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours or FTE)</strong> </td>
<td><strong>Displayed By</strong> </td>
<td> <p><strong>Description</strong> </p> </td>
</tr>
<tr>
<td rowspan="5">AVL <br>(Available Hours or FTE)</td>
<td>User</td>
<td>The total of Available Hours or FTE for the user according to their schedule. </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the User view to the Resource Planner. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Available Hours or FTE for the role according to the schedule of the user and the <strong>Percentage of FTE Availability</strong> of the role.</p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project.</td>
</tr>
<tr>
<td colspan="2"> <p colspan="2">For more information about how user and role availability is calculated based on the schedule of the user and the Percentage of FTE Availability of the role, see <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">PLN <br>(Planned Hours or FTE)</td>
<td>User</td>
<td> The total of Planned Hours or FTE from all the tasks or issues assigned to the user on all the projects.<br><p>This includes tasks and issues that are assigned to the user but not associated with any job role and tasks or issues that are not on projects that you have access to Manage.</p><p>When the user allocation for hours has been modified using the Workload Balancer, the data in the Resource Planner can be affected if the dates selected contain only a portion of a task or issue. For information about modifying allocations for users, see <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a> . </p></td>
</tr>
<tr>
<td>Project</td>
<td> The total of Planned Hours or FTE from all the tasks and issues assigned to a specific user on the project.<br><note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are not assigned to any users.
</note></td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Planned Hours or FTE from all the tasks and issues assigned to the user in this role on the project.</p> <p> <note type="note">
This does not include the Planned Hours or FTE from tasks or issues that are assigned to this role but not to this user in this role.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>The Planned Hours or FTE associated with the task or the issue on the project.</td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view))</p>
<ul>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks and issues , for each resource assigned to them. The task or issue Duration is based on their Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks or issues excluding weekends, time-off days, and schedule exceptions.</p> <p>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> <p>The following categories of tasks are included in calculating the Planned Hours for each resource: </p>
<ul>
<li> <p> tasks assigned to users in Resource Pools, job roles, or teams on the project.</p> <note type="tip">
If tasks are assigned to teams, their allocation will appear under
<strong>No Role</strong> and
<strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks.
</note> </li>
</ul> </li>
</ul>
<ul>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>unassigned tasks</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task or issue Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> <p>For more information about Planned Hours and FTE in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td rowspan="5">ACT<br>(Actual Hours or FTE) </td>
<td>User </td>
<td> <p>The time logged by the user on all the tasks or issues assigned to them.</p> <p>This includes the following:</p>
<ul>
<li>Tasks and issues that are assigned to the user but not associated with any job role.</li>
<li>Tasks and issues that are not on projects for which you have access to Manage.. </li>
</ul> <p>This does not include time logged directly on the project or on parent tasks. </p> </td>
</tr>
<tr>
<td>Project </td>
<td> <p>The time logged by the user on all the tasks and issues assigned to them on the project.</p> <p>This includes any time that they logged directly on the project.</p> <p>This does not include the following:</p>
<ul>
<li> <p>Time logged on tasks and issues that are not assigned to any users. </p> </li>
<li> <p>Time logged on parent tasks. </p> </li>
</ul> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The time logged on all the tasks or issues assigned to the user in this role. </p> <p>This does not include the following:</p>
<ul>
<li>Time logged on tasks and issues assigned to this role but not to this user in this role.<em> </em></li>
<li>Time logged directly on the project or parent tasks. </li>
</ul> </td>
</tr>
<tr>
<td>Task or Issue </td>
<td> <p>The time logged on tasks and issues by the user who is also assigned to them. </p> </td>
</tr>
<tr>
<td colspan="2"> <p> <note type="important">
The time logged is displayed in the timeframe corresponding to the Entry Date of the hour entry, regardless of the timeframe of the task, issue, or project where the hours are logged.
</note> </p> <p>For more information about Actual Hours, see <a href="../../manage-work/tasks/task-information/actual-hours.md" class="MCXref xref">View Actual Hours</a></p> </td>
</tr>
<tr>
<td rowspan="4">DIF <br>(Hour or FTE Difference) <br><br></td>
<td>User</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the user. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <note type="note">
If the value displays in negative red numbers, the user is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project. </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The difference between the Available and Planned Hours or FTE of the job role. </p> <p>The Hour or FTE difference is calculated using the following formula:</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <note type="note">
If the value is displayed in negative red numbers, the role is overallocated.
</note> </p> </td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td rowspan="5">Planned Hours or FTE Allocation Percentage (%)</td>
<td>User</td>
<td> <p>The allocation of the Planned Hours or FTE as a percentage of the Available Hours. The percentage of the Planned Hours Allocation is calculated using the following formula:</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>The same calculation is used for FTE values. </p> </td>
</tr>
<tr>
<td>Project</td>
<td>This information is not available for the Project when applying the <strong>View by User</strong> view to the Resource Planner.</td>
</tr>
<tr>
<td>Role</td>
<td> The allocation of the Planned Hours or FTE as a percentage of the Available Hours. <p>The percentage of the Planned Hours Allocation is calculated using the following formula:</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>The same calculation is used for FTE values.</p></td>
</tr>
<tr>
<td>Task or Issue</td>
<td>This information is not available for the Task, Issue, or Project. </td>
</tr>
<tr>
<td colspan="2"> <p> If the value of the Planned Hours or FTE is zero, the Percentage Allocation is 0%. If the value of the Available Hours or FTE is zero, the Percentage Allocation cannot be calculated. </p> <p>For more information about Planned Hours and FTE and how they are displayed in the Resource Planner, see <a href="../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md" class="MCXref xref">Budget resources in the Resource Planner using the Project and Role views</a>. </p> </td>
</tr>
</tbody>
</table>
-->
