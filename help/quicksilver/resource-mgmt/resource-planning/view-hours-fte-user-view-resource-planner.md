---
content-type: reference
product-area: resource-management;user-management
navigation-topic: resource-planning
title: Afficher les heures disponibles, prévues et effectives ou le temps complet dans le planificateur de ressources lors de l’utilisation de la vue utilisateur
description: Affichez les heures disponibles, prévues et effectives ou le temps complet dans le planificateur de ressources lors de l’utilisation de la vue utilisateur du planificateur de ressources, par exemple « Planification dans le planificateur de ressources », « Établissement du budget des ressources dans le planificateur de ressources » ou « Gérer les ressources dans le planificateur de ressources », etc. Peut nécessiter une définition à partir d’un autre point de vue.
author: Alina
feature: Resource Management
exl-id: 6b532aa2-435f-4fda-b7ce-abe0a785638f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1739'
ht-degree: 100%

---

# Afficher les heures disponibles, prévues et effectives ou le temps complet dans le planificateur de ressources lors de l’utilisation de la vue utilisateur

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Consider renaming this article (probably split already) to something other than "Planning" in the RP" - maybe "budgeting resources in the RP" or "Managing Resources in the RP." etc... - or might need to be repurposed from another POV?!)</p>
-->

Outre la planification des ressources dans les vues Projet et Rôle, vous pouvez utiliser la vue utilisateur du planificateur de ressources Adobe Workfront pour afficher des informations sur les valeurs Heures prévues, Heures disponibles et Heures effectives ou de temps complet pour les projets et les ressources.

## Vue d’ensemble de la vue utilisateur dans le planificateur de ressources

Tenez compte de ce qui suit lors de l’affichage des heures ou des informations de temps complet dans le planificateur de ressources :

* Vous pouvez afficher les heures disponibles et les heures prévues ou les informations de temps complet des personnes, des fonctions et des projets dans toutes les vues du planificateur de ressources.
* Vous ne pouvez afficher les informations suivantes que dans la vue utilisateur :

   * Différence entre le nombre d’heures prévue ou le temps complet et le nombre d’heures disponibles ou le temps complet. Vous pouvez ensuite budgéter l’affectation de vos personnes en fonction de cette différence dans les vues de projet et de rôle.
   * Heures effectives ou temps complet.

* Vous pouvez afficher la différence entre la personne disponible et le nombre d’heures prévues ou le temps complet sous la forme d’un nombre ou d’un pourcentage dans la vue utilisateur.
* Vous ne pouvez pas afficher les informations dans la vue utilisateur par coût.
* Adobe Workfront renseigne les heures disponibles ou le temps complet en fonction du temps de travail associé aux personnes dans leurs plannings.\
  Les personnes non associées à un planning affichent la disponibilité selon le planning par défaut.\
  Pour plus d’informations sur le planning par défaut, voir [Créer un planning](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* Workfront renseigne le nombre d’heures prévues ou le temps complet à partir du nombre d’heures prévues sur les tâches et les problèmes des projets.
* Workfront renseigne les heures effectives avec le temps effectif consigné dans les tâches et les problèmes par les personnes qui y sont affectées. Cela inclut le temps consigné sur un projet.
* Dans la vue utilisateur, vous pouvez effectuer les opérations suivantes :

   * Développer chaque personne de sorte à afficher la liste des projets auxquels elle est affectée.

     >[!NOTE]
     >
     >Seules les personnes associées aux projets inclus dans les filtres peuvent être développées.

   * Développer chaque projet pour afficher la liste des fonctions que la personne peut remplir sur ces projets.
   * Développer chaque rôle de sorte à afficher la liste des tâches auxquelles la personne est affectée.

  Si aucune fonction n’est associée aux personnes, leurs heures disponibles, prévues et effectives ou leur temps complet sont répertoriés dans la section **Aucun rôle**.\
  Pour plus d’informations sur les champs et les éléments qui s’affichent lors de l’application de la vue utilisateur au planificateur de ressources, voir la section Projet/Rôle/Sélection de la vue utilisateur dans [Vue d’ensemble de la navigation dans le planificateur de ressources](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

## Vue d’ensemble des champs visibles dans la vue utilisateur du planificateur de ressources

Reportez-vous aux tableaux suivants pour comprendre les informations affichées dans la vue utilisateur du planificateur de ressources. Les informations s’affichent en heures ou temps complet.

* [Colonne AVL (disponible)](#the-avl-available-column)
* [Colonne PLN (prévu)](#the-pln-planned-column)
* [Colonne ACT (réel)](#The%C2%A0ACT)
* [Colonne DIF (différence)](#the-dif-difference-column)
* [Colonne % (pourcentage d’attribution des heures prévues)](#the-planned-hours-allocation-percentage-column)

### Colonne AVL (Disponible) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché par</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td>Total des heures disponibles ou temps complet de la personne selon son planning. </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Ces informations ne sont pas disponibles pour le projet lorsque la vue utilisateur est appliquée au planificateur de ressources. </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Total des heures disponibles ou temps complet pour le rôle, en fonction du planning de la personne et du <strong>Pourcentage de disponibilité en temps complet</strong> du rôle.</p> </td> 
  </tr> 
  <tr> 
   <td>Tâche ou problème</td> 
   <td>Ces informations ne sont pas disponibles pour la tâche ou le problème. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le mode de calcul de la disponibilité des personnes et des rôles en fonction du planning de chaque personne et du pourcentage de disponibilité en temps complet, voir [Vue d’ensemble du calcul des heures et du temps complet pour les personnes et les rôles dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

### Colonne PLN (prévu) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché par</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> Total du nombre d’heures prévues ou du temps complet pour toutes les tâches ou problèmes affectés à l’utilisateur ou à l’utilisatrice sur tous les projets.<br><p>Cela inclut les tâches et les problèmes qui sont affectés à l’utilisateur ou à l’utilisatrice, mais qui ne sont associés à aucune fonction, ainsi que les tâches ou les problèmes qui ne font pas partie des projets que vous avez le droit de gérer.</p><p>Lorsque l’affectation des heures des utilisateurs et des utilisatrices a été modifiée à l’aide de l’équilibreur de charge de travail, les données du planificateur de ressources peuvent être affectées si les dates sélectionnées ne contiennent qu’une partie d’une tâche ou d’un problème. Pour plus d’informations sur la modification des affectations pour les utilisateurs et les utilisatrices, consultez la section <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gérer les affectations pour les utilisateurs et les utilisatrices dans l’équilibreur de charge de travail</a>. </p></td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td> Total du nombre d’heures prévues ou de l’équivalent temps complet pour toutes les tâches et problèmes affectés à un utilisateur ou à une utilisatrice spécifique du projet.<br><p>Note : cela n’inclut pas le nombre d’heures prévues ou l’équivalent temps complet des tâches ou des problèmes qui ne sont affectés à personne. </p></td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Total du nombre d’heures prévues ou de l’équivalent temps complet pour toutes les tâches et tous les problèmes affectés à un utilisateur ou à une utilisatrice dans ce rôle pour le projet.</p> <p> <p>Note : cela n’inclut pas le nombre d’heures prévues ou l’équivalent temps complet des tâches ou des problèmes qui sont affectés à ce rôle mais ne sont affectés à personne dans ce rôle. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Tâche ou problème</td> 
   <td>Nombre d’heures prévues ou équivalent temps complet associé à la tâche ou au problème du projet.</td> 
  </tr> 
 </tbody> 
</table>

Tenez compte des points suivants lors de l’affichage du nombre d’heures prévues :

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this is a snippet converted to text because there are difference from project/ role views and the user view (users with no pools DO show in user view)</p>
-->

* Le nombre d’heures prévues est réparti de manière égale sur chaque jour dans la durée des tâches et des problèmes pour chaque ressource qui lui est affectée. La durée de la tâche ou du problème est basée sur les dates de début et de fin prévues et inclut chaque jour calendaire de cette période.\
  Workfront prend en compte le planning de l’utilisateur ou de l’utilisatrice ou du projet lors de la répartition du nombre d’heures prévues entre les utilisateurs et les utilisatrices ou les projets. Dans ce cas, le nombre d’heures prévues est réparti de manière égale entre chaque jour dans la durée des tâches ou des problèmes, à l’exception des week-ends, jours de congé et des exceptions d’horaire.

  Si, par exemple, vous affichez le planificateur de ressources par semaine et que vous avez des tâches qui durent plusieurs semaines pour des projets, le nombre d’heures prévues par semaine dépend du nombre de jours de cette semaine qui fait partie de la durée de la tâche. Cela fonctionne de la même manière lors de l’affichage du planificateur de ressources par mois ou par trimestre et lorsque les tâches durent plusieurs mois ou trimestres.\
  Les jours du week-end, les exceptions d’horaire et les jours de congé sont exclus de cette répartition.

* Les catégories de tâches suivantes sont incluses dans le calcul du nombre d’heures prévues pour chaque ressource :

   * Tâches affectées aux utilisateurs et utilisatrices dans les groupes de ressources, les fonctions ou les équipes du projet.

     >[!TIP]
     >
     >Si des tâches sont affectées à des équipes, leur affectation apparaît sous les sections **Aucun rôle** et **Aucune personne**. Vous pouvez voir le nombre d’heures prévues associé aux équipes, mais vous ne pouvez pas budgéter les heures, car aucun rôle ni aucunpersonne n’a de tâches affectées.

* Le nombre d’heures prévues dans le planificateur de ressources n’inclut pas le nombre d’heures prévues associé aux éléments suivants :

   * Tâches parent
   * Tâches non affectées
   * Problèmes, lorsque le paramètre **Inclure les heures des problèmes** est désactivé.

* Le nombre d’heure prévues ne s’affiche pas dans le planificateur de ressources si la durée de la tâche ou du problème est nulle.
* Le nombre d’heures prévues associé aux utilisateurs et utilisatrices désactivés ne s’affiche pas.

Pour plus d’informations sur le nombre d’heures prévues et le temps complet dans le planificateur de ressources, consultez la section [Vue d’ensemble des heures, de l’équivalent temps complet et des coûts dans les vues de projet et de rôle du planificateur de ressources](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

### Colonne ACT (Réel)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché par</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice </td> 
   <td> <p>Temps consigné par l’utilisateur ou l’utilisatrice concernant l’ensemble des tâches et problèmes affectés.</p> <p>Cela inclut les éléments suivants :</p> 
    <ul> 
     <li>Tâches et problèmes affectés à l’utilisateur ou l’utilisatrice, mais qui ne sont pas associés à une fonction.</li> 
     <li>Tâches et problèmes qui ne concernent pas les projets pour lesquels vous avez accès à l’option de gestion. </li> 
    </ul> <p>Cela inclut le temps consigné pour le projet uniquement lorsque des tâches ou des problèmes sur ce projet sont affectés à un utilisateur ou une utilisatrice.  </p> </td> 
  </tr> 
  <tr> 
   <td>Projet </td> 
   <td> <p>Temps consigné par l’utilisateur ou l’utilisatrice concernant l’ensemble des tâches et problèmes affectés.</p> <p>Cela inclut tout le temps directement consigné dans le projet.</p> <p>Cela ne comprend pas les éléments suivants :</p> 
    <ul> 
     <li> <p>Temps consigné pour les tâches et problèmes pour lesquels aucune affectation d’utilisateur ou d’utilisatrice n’a été faite. </p> </li> 
     <li> <p>Temps consigné pour les tâches parent. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Temps consigné par l’utilisateur ou par l’utilisatrice dans ce rôle concernant l’ensemble des tâches et problèmes affectés. </p> <p>Cela ne comprend pas les éléments suivants :</p> 
    <ul> 
     <li>Heures consignées pour les tâches et problèmes affectés à ce rôle, mais pas pour cet utilisateur ou cette utilisatrice occupant ce rôle.</li> 
     <li>Heures consignées directement pour le projet ou les tâches parent. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Tâche ou problème </td> 
   <td> <p>Heures consignées pour les tâches et problèmes par la personne qui leur est également affectée. </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Les heures consignées s’affichent dans le délai correspondant à la Date d’entrée de l’entrée d’heure, quel que soit le délai de la tâche, du problème ou du projet dont les heures sont consignées.

Pour plus d’informations sur les heures effectives, voir [Afficher les heures effectives](../../manage-work/tasks/task-information/actual-hours.md).

### Colonne DIF (Différence) {#the-dif-difference-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché par</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Différence entre le nombre d’heures disponibles et prévues ou le temps complet de l’utilisateur ou de l’utilisatrice. </p> <p>La différence d’heure ou de temps complet est calculée à l’aide de la formule suivante :</p> <p><code style="font-style: normal;">User Hour or FTE Difference = User Available Hours or FTE - User Planned Hours or FTE</code> </p> <p> <p>Remarque : si la valeur s’affiche en chiffres rouges négatifs, l’utilisateur ou l’utilisatrice est en suraffectation. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Ces informations ne sont pas disponibles pour le projet. </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Différence entre les heures disponibles et prévues ou le temps complet de la fonction. </p> <p>La différence d’heure ou de temps complet est calculée à l’aide de la formule suivante :</p> <p><code style="font-style: normal;">Role Hour or FTE Difference = Role Available Hours or FTE - Role Planned Hours or FTE</code> </p> <p> <p>Remarque : si la valeur est affichée en chiffres rouges négatifs, le rôle est en suraffectation. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Tâche ou problème</td> 
   <td>Ces informations ne sont pas disponibles pour la tâche, le problème ou le projet. </td> 
  </tr> 
 </tbody> 
</table>

### Colonne % (pourcentage d’attribution des heures prévues) {#the-planned-hours-allocation-percentage-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché par</strong> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Attribution des heures prévues ou du temps complet en pourcentage des heures disponibles. Le pourcentage d’attribution des heures prévues est calculé à l’aide de la formule suivante :</p> <p><code style="font-style: normal;">User Planned Hours Allocation Percentage = (User Planned Hours/ User Available Hours) * 100</code> </p> <p>Le même calcul est utilisé pour les valeurs du temps complet. </p> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td>Ces informations ne sont pas disponibles pour le projet lors de l’application de la vue <strong>Afficher par utilisateur et utilisatrice</strong> sur le planificateur de ressources.</td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> Attribution des heures prévues ou du temps complet en pourcentage des heures disponibles. <p>Le pourcentage d’attribution des heures prévues est calculé à l’aide de la formule suivante :</p><p><code style="font-style: normal;">Role Planned Hours Allocation Percentage = (Role Planned Hours/ Role Available Hours) * 100</code></p><p>Le même calcul est utilisé pour les valeurs du temps complet.</p></td> 
  </tr> 
  <tr> 
   <td>Tâche ou problème</td> 
   <td>Ces informations ne sont pas disponibles pour la tâche, le problème ou le projet. </td> 
  </tr> 
 </tbody> 
</table>

Si la valeur des heures prévues ou du temps complet est de zéro, le pourcentage d’attribution est de 0 %. Si la valeur des heures disponibles ou du temps complet est de zéro, le pourcentage d’attribution ne peut pas être calculé.

Pour plus d’informations sur les heures prévues et le temps complet, ainsi que sur leur affichage dans le planificateur de ressources, voir [Établir le budget des ressources dans le planificateur de ressources à l’aide des vues de projet et de rôle](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

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
