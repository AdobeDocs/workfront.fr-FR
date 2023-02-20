---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Présentation de l’affectation de travail dans l’équilibreur de charge de travail
description: En tant que gestionnaire de ressources, vous pouvez utiliser l’équilibreur de charge de travail Adobe Workfront pour afficher les tâches qui n’ont pas encore été affectées aux utilisateurs et leur affecter ces éléments.
author: Alina
feature: Resource Management
exl-id: 98779b67-b975-4501-8426-63e255b1d7df
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 0%

---

# Présentation de l’affectation de travail dans l’équilibreur de charge de travail

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu .</span>

En tant que gestionnaire de ressources, vous pouvez utiliser l’équilibreur de charge de travail Adobe Workfront pour afficher les tâches qui n’ont pas encore été affectées aux utilisateurs et leur affecter ces éléments.

Pour obtenir des informations générales sur l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Vous pouvez affecter des tâches (tâches et problèmes) aux utilisateurs dans d’autres zones de Workfront. Cependant, en utilisant l’équilibreur de charge de travail, vous pouvez facilement comprendre la disponibilité des utilisateurs et voir clairement tous les autres éléments auxquels ils sont affectés avant de leur assigner plus de travail.

Pour plus d’informations sur l’affectation de tâches dans d’autres zones de Workfront, reportez-vous aux articles suivants :

* [Affecter des tâches](../../manage-work/tasks/assign-tasks/assign-tasks.md)
* [Attribuer des problèmes](../../manage-work/issues/manage-issues/assign-issues.md)

## Disponibilité des utilisateurs dans l’équilibreur de charge de travail

Vous pouvez affecter du travail dans l’équilibreur de charge de travail afin qu’il corresponde à l’heure disponible pour les utilisateurs. Pour vous assurer que vous attribuez le bon volume de travail et non sur-affectez l’utilisateur, le total des heures planifiées des tâches affectées à l’utilisateur doit correspondre aux affectations quotidiennes ou hebdomadaires de l’utilisateur.

Vous devez comprendre comment Workfront calcule l’heure disponible pour un utilisateur.

Workfront utilise les informations suivantes pour calculer la capacité de l’utilisateur dans l’équilibreur de charge de travail :

* Les Préférences De Gestion Des Ressources. L’administrateur de Workfront détermine le mode de calcul de l’heure disponible pour le système en sélectionnant d’utiliser l’une des options suivantes dans la zone Resource Management de la section Configuration :

   * Planification par défaut du système Workfront et de l’éditeur de texte enrichi de l’utilisateur.
   * Planification de l’utilisateur, comme indiqué dans la zone Profil utilisateur .

      Cela calcule la disponibilité quotidienne et hebdomadaire de l’utilisateur. Toutes les exceptions de planification sur le planning sélectionné sont répercutées dans la capacité de l’utilisateur dans l’équilibreur de charge de travail.
   Pour plus d’informations, voir [Configuration des préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

   Pour plus d’informations sur les plannings, voir [Création d’un planning](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

* Le temps de congé de l’utilisateur. Cela indique les jours que l’utilisateur prévoit de décoller.

   Pour plus d’informations, voir [Configuration du temps de pause personnel dans Adobe Workfront](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).
<div class="preview">
* Temps de travail de l’utilisateur. Cela indique le pourcentage de temps de l’éditeur de texte enrichi que l’utilisateur est disponible pour effectuer des tâches réelles liées au projet, sans compter les frais généraux. Définissez la valeur Durée du travail sur 1 pour indiquer que l’utilisateur est disponible pour le travail lié au projet et qu’il dispose de son équivalent à temps plein.
</div>

## Affecter un travail dans l’équilibreur de charge

Vous pouvez affecter des tâches qui n’ont pas encore été affectées à un utilisateur ou réaffecter des éléments qui ont été affectés à des utilisateurs dans l’équilibreur de charge de travail.

Vous pouvez affecter le travail dans l’équilibreur de charge de travail de la manière suivante :

* Un élément à la fois en attribuant manuellement chaque élément.

   Vous pouvez effectuer des affectations avancées lors de l’attribution manuelle d’éléments, une par une.

   Pour plus d’informations, voir [Affectation manuelle du travail à l’aide de l’équilibreur de charge](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

* Un élément à la fois, en faisant glisser et en déposant des tâches sur l’utilisateur qui doit être affecté.

   Pour plus d’informations, voir [Affectez un travail à l’équilibreur de charge de travail en le faisant glisser et en le déposant](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

* Plusieurs éléments à la fois, à l’aide de l’option Affectations en bloc . Vous pouvez définir des règles en fonction desquelles les éléments sont affectés à plusieurs utilisateurs à la fois.

   Pour plus d’informations, voir [Affectation du travail en masse à l’aide de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

Pour plus d’informations sur l’annulation de l’affectation d’une tâche, voir [Annulation de l’affectation du travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

## Zones d’affectation dans l’équilibreur de charge de travail

Vous pouvez affecter du travail aux utilisateurs à l’aide de l’équilibreur de charge de travail dans la zone Ressource, au niveau du projet ou au niveau de l’équipe. Pour plus d’informations sur l’emplacement de l’équilibreur de charge de travail dans Workfront, voir [Localisation de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

L’équilibreur de charge de travail comporte deux zones où vous pouvez afficher les tâches :

* **Travail non attribué**: affiche les éléments qui ne sont pas affectés aux utilisateurs.
* **Travail attribué**: affiche les éléments affectés aux utilisateurs.

Le tableau suivant décrit les éléments qui s’affichent dans chaque zone en fonction de leurs affectations :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Type d’affectation</strong> </td> 
   <td colspan="2"><strong>Zones dans lesquelles les affectations sont visibles</strong> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td>Travail non affecté </td> 
   <td>Travail affecté </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span style="font-weight: normal;">Élément non attribué</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Équipe</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span data-mc-edit-date="2020-04-08T15:57:40.7175506-04:00" data-mc-editor="alinawilson" data-mc-comment="Drafted because role only is not displayed; first it will be displayed in Unassigned - 20.2 beta" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:24:04.5189150-05:00">Rôle</span> </td> 
   <td><span>✔</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rôle et équipe</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Utilisateur</td> 
   <td> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Utilisateur et équipe</td> 
   <td> <p> </p> </td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>Utilisateur, rôle et équipe</td> 
   <td>✔*</td> 
   <td>✔**</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Utilisateur et rôle</p> </td> 
   <td><span data-mc-edit-date="2019-11-15T13:37:42.5435254-05:00" data-mc-editor="alinawilson" data-mc-comment="drafted because it's not in the Unassigned" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2019-11-15T13:37:33.3097484-05:00">✔</span>*</td> 
   <td>✔**</td> 
  </tr> 
 </tbody> 
</table>

&#42;Lorsqu’un élément de travail est attribué à un utilisateur et à un rôle, il s’affiche dans la zone de travail Non affecté uniquement lorsque le rôle est le cessionnaire Principal.

&#42;&#42;Lorsqu’un élément de travail est attribué à un utilisateur et à une autre entité, il s’affiche dans la zone de travail Affecté uniquement lorsque l’utilisateur est le cessionnaire Principal.

Pour plus d’informations sur les zones Non assignées et Affectées de l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Considérations relatives à plusieurs affectations pour les rôles de tâche, les équipes et les utilisateurs

Tenez compte des points suivants lorsque vous affectez plusieurs ressources à une tâche :

* Les utilisateurs peuvent avoir plusieurs rôles de tâche associés à leur profil. Pour plus d’informations sur l’association d’utilisateurs à des rôles de tâche, voir [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Les tâches ou les problèmes sont généralement affectés en premier à un ou plusieurs rôles de tâche ou à une équipe. Lorsque les projets sont prêts à démarrer, ils doivent peut-être également être affectés aux utilisateurs.\
   Si une tâche ou un problème est assigné à un ou plusieurs rôles, puis que vous affectez également un utilisateur, Adobe Workfront décide quel rôle de tâche associer à l’utilisateur supplémentaire (le cas échéant) selon les règles suivantes :

   * Si un seul rôle de tâche est attribué et qu’il correspond au rôle Principal de l’utilisateur, la tâche ou le problème est affecté uniquement à l’utilisateur qui remplit son rôle Principal.
   * Si plusieurs rôles sont affectés et qu’au moins un des rôles correspond aux rôles secondaires de l’utilisateur, la tâche ou le problème est alors assigné à l’utilisateur qui remplit l’un de ses Autres rôles — que Workfront sélectionne au hasard s’il existe plusieurs correspondances — ainsi que les rôles supplémentaires affectés.
   * Si un ou plusieurs rôles de tâche sont affectés et qu’il n’y a aucune correspondance avec les rôles de l’utilisateur, la tâche ou le problème est affecté à la fois au rôle ou aux rôles ainsi qu’à l’utilisateur.

* Si une tâche ou un problème est assigné à une équipe et que vous affectez également un utilisateur, la tâche ou le problème reste assigné à l’équipe et à l’utilisateur.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2 data-mc-conditions="QuicksilverOrClassic.Quicksilver"> Manually assign one item at a time</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Moved manual assignment and drag-and-drop to their own articles) </p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items</p> <p>Or</p> <p>Go to the <strong>Assigned Work</strong> area and expand the name of a user to view the work items assigned to them.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area. You can only reassign issues already assigned to users in the Assigned Work area. Otherwise,</span> you can assign issues from a list or at the issue level. For information, see
<a href="../../manage-work/issues/manage-issues/assign-issues.md" class="MCXref xref">Assign issues</a>.
</note> </li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> on the bar of a work item, then click <strong>Assign this to</strong>. </p> <p> <img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"> </p> <note type="tip">
<p><span>You can also use the following shortcuts to assign tasks or issues:</span> </p>
<ul>
<li><span>In Windows: CTRL+click the task or issue bar.</span> </li>
<li><span>In&nbsp;Mac: CMD+click the task or issue bar.</span> </li>
</ul>
</note> </li>
<li value="4"> <p>Start typing the name of a user, job role, or team that you want to assign to the item in the <strong>Search people, role or teams</strong> field, select it when it displays in the list, then click&nbsp;<strong>Save</strong>. </p> <p> <img src="assets/assignments-box-wb.png"> </p> <p>This assigns or reassigns the work item to the specified assignees.</p> <p>If you assign an item to just a team or a job role, the item displays only in the Unassigned Work area. You must assign work items to users in order to display them in the Assigned Work area of the Workload Balancer.</p> <note type="tip">
<p>You can assign multiple users or job roles, and you can assign only one team. <span>You can assign only active users, <span>job roles</span>, and teams.</span></p>
<p><span>If a user, <span>job role</span>, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:</span> </p>
<ul>
<li> <p><span>Reassign the work item to active resources.</span> </p> </li>
<li> <p><span>Associate the users in a deactivated team with an active team and reassign the work item to the active team.</span> </p> </li>
</ul>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>.</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol>
<div data-mc-conditions="QuicksilverOrClassic.Quicksilver">
<h2>Assign an item by dragging and dropping</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider retitling this to "Assign one item at a time by dragging and dropping" when bulk assignments will come???)&nbsp;</p>
<p>You can assign an item from the Unassigned Work area to a user, or you can reassign an already assigned item to another user in the Assigned Work area.</p>
<ol>
<li value="1">Go to the Workload Balancer.</li>
<li value="2"> <p>Go to the <strong>Unassigned Work</strong> area and apply a filter to view work items.</p> <note type="important">
<span>You cannot view and assign issues from the Unassigned Work area.</span>
</note> </li>
<li value="3"> <p>Click the bar of a work item that indicates either the planned or the projected timeline and drag it over the name of a user in the <strong>Assigned</strong> area.</p> <p>The user you hover over to drop the work item to is highlighted.</p> <note type="tip">
The Planned Hours for the user you're hovering over update in real time with the number of daily Planned Hours from the work item, to indicate what the impact of adding a new item might be to their overall allocation.
</note> <p> <img src="assets/drag-drop-item-from-unassigned-to-assigned-wb-nwe-350x152.png" style="width: 350;height: 152;"> </p> </li>
<li value="4"> <p>When you are ready, drop the selected work item in the same line as the user's name in the Assigned Area. The item is assigned and the allocated Planned Hours are updated for the user with the new hours from the work item.</p> <note type="tip">
<p>If you enabled Group by Project in the Settings area, the assigned task displays under the corresponding project. If the setting is disabled, the assigned task displays in the user area. </p>
<p>The item displays according to the Workload Balancer criteria for sorting work items.&nbsp;For more information, see <a href="../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigate the Workload Balancer</a>.</p>
</note> </li>
<li value="5"> <p>(Optional) Click the <strong>Show allocations icon</strong> <img src="assets/show-allocations-icon-small.png">, then click the <strong>More menu</strong> <img src="assets/qs-more-menu.png"> > <strong>Edit allocations</strong>. (NOTE: make sure these are still called this, and that the icon has not changed)</p> <p>Or</p> <p>Double-click a daily or weekly allocation to modify the amount of time the user is allocated to the work item.</p> <p>For information about modifying user allocations in the Workload Balancer, see the "Modify user allocations"&nbsp;section in the article <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Manage user allocations in the Workload Balancer</a>.</p> </li>
</ol> 
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Assign items in bulk</h2>
<p>(NOTE: This is also a separate article. Should we keep this section or the separate article?) </p>
</div>
<p>&nbsp;</p>
</div>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Unassign work items in the Workload Balancer</h2>
<p>(NOTE: moved this section to a new article. Draft here at release to preview) </p>
<p>You can either unassign items from users and move them to the Unassigned Work area, or reassign them to other users. </p>
<p>To unassign work items from users: </p>
<ol>
<li value="1">In the Workload Balancer, go to the <strong>Assigned Work</strong> area and expand a user.</li>
<li value="2">Do 
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
one of
</MadCap:conditionalText>
the following:
<ul>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Find the item you want to unassign in a user's area, click it, drag and drop it in the Unassigned area or in another user's area. </p></li>
<li><p>Click the <strong>More</strong> icon <img src="assets/more-icon-task-list.png"> to the right of the name of a work item, click&nbsp;<strong>Assign this to</strong> , then remove the name of the entities assigned to the work item or enter another name and click&nbsp;<strong>Save</strong>.</p><p><img src="assets/workload-balancer-assign-this-to-link-from-task-350x117.png" style="width: 350;height: 117;"></p></li>
</ul><p>The item displays in the Unassigned Work area if it matches the filtering criteria for that area and it is not assigned to any users or it displays in the user area if it is assigned to that user. </p><note type="tip">
Unassigned issues do not display in the Unassigned area.
</note><p>For information about filtering information in the Workload Balancer, see <a href="../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md" class="MCXref xref">Manage filters in the Workload Balancer</a>. </p></li>
</ol>
</div>
-->
