---
content-type: overview;how-to-procedural
product-area: projects;user-management
navigation-topic: assign-tasks
title: Vue d’ensemble des affectations intelligentes
description: Lors de la gestion des affectations de tâches et de problèmes, vous pouvez utiliser des affectations intelligentes pour identifier la personne la plus apte à effectuer le travail. Les affectations intelligentes sont des suggestions qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources en fonction d’un algorithme qui détermine la ressource la plus appropriée pour la tâche.
author: Alina
feature: Work Management
exl-id: 8d17eff6-5ff0-4985-b575-4934a3bb7c0b
source-git-commit: 758dae749d324326857a330c8a23954764e68fd1
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 82%

---

# Vue d’ensemble des affectations intelligentes

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elles sont disponibles uniquement dans l’environnement de prévisualisation pour toutes les clientes et tous les clients ou dans l’environnement de production pour les clientes et les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activer ou désactiver le versions rapides pour votre entreprise](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Pour plus d’informations sur la version actuelle, voir [Vue d’ensemble de la version du quatrième trimestre 2024](/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-release-overview.md).</span>

Lors de la gestion des tâches et des affectations de problèmes, vous pouvez utiliser des affectations intelligentes pour identifier la meilleure ressource pour effectuer le travail. Les affectations intelligentes sont des suggestions qu’Adobe Workfront vous présente lorsque vous affectez des tâches à des ressources en fonction d’un algorithme qui détermine la ressource la plus appropriée pour la tâche. Les affectations intelligentes peuvent être des personnes, des rôles de tâche ou des équipes.

>[!NOTE]
>
>Lors de la suggestion de personnes, les affectations intelligentes ne prennent pas en compte leur disponibilité. Toutefois, leur disponibilité en fonction de leurs plannings affecte les dates prévues et prévisionnelles des tâches et des problèmes lorsqu’elles sont affectées. Pour plus d’informations sur les plannings, voir l’article [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Cet article contient des informations générales sur les affectations intelligentes. Pour plus d’informations sur l’utilisation d’affectations intelligentes pour affecter des tâches et des problèmes aux personnes, voir [Créer des affectations intelligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md).

## Vue d’ensemble des affectations intelligentes

Tenez compte des points suivants lorsque vous utilisez des affectations intelligentes :

* <span class="preview">L’algorithme fonctionne indépendamment pour les tâches et les problèmes. Cela signifie que la liste des utilisateurs suggérés pour les problèmes peut différer de celle des utilisateurs suggérés pour une tâche, car Workfront crée les listes en fonction de critères relatifs aux problèmes et aux tâches séparément. </span>
<!--not sure this is accurate: * Smart assignments do not recommend job roles or teams. Instead, they are suggestions of users who are best fit to complete a task or an issue. -->
* Les affectations suggérées sont toujours des utilisateurs, des rôles de tâche ou des équipes actifs.
* La ressource répertoriée en premier doit correspondre le mieux à la tâche.

## Rechercher les suggestions d’affectation intelligente

Vous pouvez afficher des affectations intelligentes dans les zones suivantes où vous pouvez affecter des tâches ou des problèmes :

* Liste de problèmes ou rapport dans la colonne Affectations

  ![](assets/smart-assignments-issue-list.png)

* <span class="preview">Une liste de tâches ou un rapport dans la colonne Affectations</span>

  ![](assets/smart-assignments-task-list.png)

* <span class="preview">En-tête de tâche dans le champ Affectations</span>

  ![](assets/smart-assignments-task-header-nwe-350x302.png)

* En-tête de problème dans le champ Affectations

  ![](assets/smart-assignments-issue-header.png)

* Panneau Résumé de la tâche ou du problème dans la zone Affectations

  ![](assets/issue-assignments-summary-panel.png)

* <span class="preview">Champ Affectations de la zone Nouvelle tâche lors de l’ajout d’une tâche à un projet</span>

  ![](assets/smart-assignments-new-task-modal.png)

<!--this is not possible in the new home  - we have Summary there: 
* The Assignments field for an item listed in the Home area, when you open a task or issue

  ![](assets/smart-assignments-in-home-nwe-350x216.png)
-->

* <span class="preview">Équilibreur de charge de travail dans la zone Affecté à lorsque vous affectez une tâche ou un problème</span>

  ![](assets/smart-assignments-workload-balancer-bulk-assignments.png)


## Critères des affectations intelligentes

Les affectations intelligentes diffèrent selon qu’il s’agit de tâches ou de problèmes.

### Critères d’affectation intelligente des tâches

Le calcul des affectations intelligentes de tâche fonctionne en <span class="preview">deux phases qui utilisent deux algorithmes différents.</span>

<span class="preview">Selon l’algorithme qui trouve l’affectation dynamique, les affectations sont répertoriées sous deux sections distinctes dans le champ Affectations.</span> Pour plus d’informations, voir [Effectuer des affectations dynamiques](/help/quicksilver/manage-work/tasks/assign-tasks/make-smart-assignments.md).

![](assets/smart-assignments-task-list.png)

<div class="preview">

#### Première phase de calcul des affectations intelligentes pour les tâches

Lors de la première phase de calcul des affectations intelligentes, Workfront calcule un score de similarité pour chaque affectation.

>[!NOTE]
>
>La première phase du calcul des affectations intelligentes ne s’applique pas aux tâches suivantes :
>
>* Affectations en masse dans l’équilibreur de charge de travail
>* Cartes connectées sur des panoramas


Le calcul du score de similarité et l’ordre dans lequel les affectations sont répertoriées prennent en compte les éléments suivants :

* Un score de 100 % est attribué à une affectation existante où les noms de la tâche, du projet et du portfolio sont identiques à la tâche que vous essayez d’affecter. Les noms de projet et de portfolio de la tâche d’une affectation existante doivent également correspondre au projet et au portfolio de la tâche que vous essayez d’affecter.

* Si seulement certaines de ces informations provenant d’autres affectations correspondent sur les tâches existantes, le score peut être inférieur à 100 %.

  Par exemple, si vous attribuez une tâche appelée « Ma seconde tâche » sur un projet appelé « Mon projet » dans un portfolio appelé « Mon portfolio » et que vous avez une tâche existante appelée « Ma tâche » dans un autre projet appelé « Mon projet » dans un portfolio appelé « Mon portfolio », la personne affectée à « Ma tâche » peut obtenir un score de 95 %, car le nom de la tâche existante et la tâche que vous essayez d’affecter sont similaires, mais pas identiques.

  >[!TIP]
  >
  >  Workfront recherche des correspondances uniquement dans les champs Nom des tâches, des projets et des portfolios.

* Une affectation pourrait obtenir un score plus élevé lorsqu’elles sont affectées à de nombreuses tâches du système portant des noms similaires. Par exemple, si une équipe appelée « Développement » est affectée à 50 % des tâches du système contenant « IA » dans le nom et que vous attribuez désormais une autre tâche avec « IA » dans le nom, le score de l’équipe « Développement » est plus élevé. Dans ce cas, les noms des projets et des portfolios ne revêtent pas un caractère aussi important.

* En tenant compte de ce système de notation, les 7 premières suggestions sont répertoriées comme des affectations intelligentes, dans l’ordre décroissant de leurs scores. Les affectations dont les scores sont inférieurs à 40 % ne s’affichent pas.

* Si plusieurs affectations ont des scores identiques, ils s’affichent dans l’ordre de la date à laquelle les affectations ont été effectuées, à partir de la date la plus récente.

  Par exemple, si Rémy a été affecté à une tâche similaire plus tôt aujourd’hui et qu’Ingrid a été affectée à une tâche similaire il y a deux jours, Rémy s’affiche en premier.

* Les affectations identifiées dans cette phase sont répertoriées dans la section    **Affectations proposées** du champ Affectations pour les tâches.

* S’il n’existe aucune correspondance utilisant ce calcul, la deuxième phase des affectations intelligentes commence, qui est calculée à l’aide d’un autre algorithme.

</div>

#### Deuxième phase de calcul de l’affectation intelligente pour les tâches

Si la première étape des affectations intelligentes de tâche n’a trouvé aucune correspondance, Workfront calcule les affectations intelligentes pour les tâches de la même manière qu’il les calcule pour les problèmes.

Pour plus d’informations, voir la section [Critères d’affectation intelligente pour les tâches et les problèmes](#smart-assignments-criteria-for-tasks-and-issues) de cet article.

Les affectations identifiées au cours de cette phase sont répertoriées dans les sections **Utilisateurs et équipes**, **Affectations de rôles de tâche** et <span class="preview">**Taux des rôles de carte**</span> du champ Affectations. <span class="preview">Pour plus d’informations sur les cartes de taux, voir [Gestion des cartes de taux](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)</span>. <!--keep the rate cards roles in yellow after the release of assignments to Prod-->

### Critères d’affectation intelligente pour les tâches et les problèmes


>[!NOTE]
>
>Les critères suivants s’appliquent aux tâches uniquement lorsque la première phase du calcul d’affectation dynamique de tâche n’a trouvé aucune correspondance. Pour plus d’informations, voir la section [Première phase de calcul de l’affectation intelligente pour les tâches](#first-phase-of-smart-assignment-calculation-for-tasks) de cet article. Par défaut, les critères suivants s’appliquent toujours aux problèmes.

![](assets/smart-assignments-issue-header.png)

Les personnes sont recommandées dans la liste déroulante Affectations intelligentes en fonction d’une combinaison des critères suivants (répertoriés dans l’ordre du plus important au moins important) :

1. Personnes affectées à d’autres tâches au cours des 30 derniers jours par la personne donnant l’affectation. Les 50 premiers utilisateurs qui correspondent à ce critère s’affichent. La personne qui est la plus souvent affectée s’affiche en premier.

2. Si l’élément de travail est affecté à une équipe ou à un rôle, la liste des personnes suggérées est filtrée en tenant compte des affectations existantes ci-dessous. Dans ce cas, seules les personnes suivantes s’affichent dans la liste des suggestions :

   * Personnes dont l’équipe principale est l’équipe affectée à l’élément de travail.
   * Personnes dont le rôle principal est le rôle affecté à l’élément de travail.

>[!TIP]
>
>* Si aucun rôle ou équipe n’est affecté à la tâche ou au problème, Workfront affiche toutes les personnes affectées au cours des 30 derniers jours, jusqu’à 50 personnes.
>
>* Si vous n’avez effectué aucune affectation au cours des 30 derniers jours, seules les personnes appartenant à l’équipe affectée ou ayant le rôle affecté à l’élément de travail s’affichent dans la liste des affectations intelligentes.



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
