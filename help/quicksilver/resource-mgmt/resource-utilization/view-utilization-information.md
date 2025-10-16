---
product-area: resource-management
navigation-topic: resource-utilization
title: Afficher les informations sur l'utilisation des ressources
description: Vous pouvez voir l’utilisation de vos ressources dans le rapport d’utilisation.
author: Lisa
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '7259'
ht-degree: 99%

---

# Afficher des informations sur l’utilisation des ressources {#view-resource-utilization-information}

>[!CONTEXTUALHELP]
>id="wf-resourcing-utilization"
>title="Rapport d’utilisation"
>abstract="Le rapport d’utilisation vous permet d’afficher la progression, le coût ou les revenus d’un projet, d’un programme ou d’un portfolio dans un seul rapport. Vous pouvez également comparer les revenus aux coûts."

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

Vous pouvez voir l’utilisation de vos ressources dans le rapport d’utilisation.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Vazgen's response about these hours ie below and he asked us to NOT document them:</p>
<p>It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours.</p>
<p>In some cases, like for Planned Hours, it takes them from Assignments</p>
<p>But Budgeted Hours come from projects.</p>
<p>And Actual Hours are their own object - Hour)</p>
</div>
-->

<!--
<p style="color: #dc143c;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This report displays information about the assignments on work items for projects in your environment, like Planned, Actual, and Budgeted Hours, FTE, or Cost.&nbsp;These are hours,&nbsp;FTE, or costs associated with the assignments and not with the tasks and issues themselves.(PRIVATE NOTE:&nbsp;Vazgen's response about these hours: It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours. In some cases, like for Planned Hours, it takes them from Assignments; But Budgeted Hours come from projects. And Actual Hours are their own object - Hour.)</p>
-->

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <tr> 
   <td>Package Adobe Workfront</td> 
   <td><p>Tous</p></td>
  </tr> 
  <tr> 
   <td>Licence Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès Affichage ou niveau supérieur aux éléments suivants :</p> 
    <ul> 
     <li> <p>Gestion des ressources </p> </li> 
     <li> <p>Projets</p> </li> 
     <li> <p>Portefeuilles</p> </li> 
     <li> <p>Programmes</p> </li> 
     <li> <p>Données financières, si vous souhaitez afficher les informations par coût</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Autorisations d’objet</td> 
   <td> <p>Accès Affichage aux projets, portfolios et programmes pour accéder à la section Utilisation dans la zone Ressources</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>Accès Gestion à un projet pour accéder à la section Utilisation du projet</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Prerequisites for accessing utilization information</h2>
<p>(NOTE: drafted, replaced with above table)</p>
<p>To access utilization information as described in this section, ensure that the following conditions are met:</p>
<ul>
<li>You have at least&nbsp;View access to the project, program, or portfolio for which you want to view the utilization information.</li>
<li>Your Workfront administrator must grant you at least View access to&nbsp;Financial&nbsp;Data in your Access Level to be able to view cost and revenue information in the Utilization report. The Workfront administrator must enable both View Role Billing & Cost Rates as well as View User Billing &&nbsp;Cost Rates when they grant you the View access to Financial Data. For information about granting access to&nbsp;Financial&nbsp;Data, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. </li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;drafted. No longer the case.) </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Reporting area. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Resourcing area. </p>
</li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is available by default in the Reporting area if the system administrator has not assigned a custom layout template to you. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is available by default in the Resourcing area if the system administrator has not assigned a custom layout template to you. </p>
</li>
</ul>
</div>
-->

## Vue d’ensemble du rapport d’utilisation {#overview-of-the-utilization-report}

Le rapport d’utilisation vous permet d’afficher la progression, le coût ou les revenus d’un projet, d’un programme ou d’un portfolio dans un seul rapport. Vous pouvez également comparer les revenus aux coûts.

Vous pouvez consulter le rapport d’utilisation dans la zone Ressource afin d’afficher l’utilisation sur plusieurs projets. Vous pouvez également le consulter à l’échelle d’un projet pour afficher l’utilisation pour les ressources individuelles (fonctions et utilisateurs ou utilisatrices) associées à ce projet.

Pour plus d’informations sur l’accès et l’utilisation du rapport d’utilisation, voir la section [Suivre la progression, le coût et les revenus à l’aide du rapport d’utilisation](#track-progress-cost-and-revenue-with-the-utilization-report) dans cet article.

### Suivre les heures (progression) {#track-hours-progress}

Vous pouvez suivre la progression en comparant les heures prévues et budgétées aux heures effectives.

Lors du suivi de la progression d’un projet, d’un programme ou d’un portfolio, la progression par rapport aux tâches et aux problèmes est incluse dans le rapport d’utilisation.

Les informations suivantes sont disponibles dans le rapport d’utilisation lors du suivi des heures :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Titre de colonne lors de l’affichage des heures</strong> </th> 
   <th><strong>Fonction</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Heures budgétées</strong> </td> 
   <td scope="col"> <p>Le nombre total d’heures budgétées sur les projets inclus. Vous pouvez afficher le total des heures budgétées pour la durée totale des projets inclus ou afficher le total des heures budgétées uniquement pour la période spécifiée (vous pouvez indiquer une semaine ou un mois spécifique). </p> <p>Les heures budgétées sont renseignées à partir des informations disponibles dans la zone Établissement du budget de ressources du business case ou du planificateur de ressources<em>.</em></p> <p>Les heures budgétées apparaissent dans le rapport d’utilisation dans l’une des lignes suivantes :</p> 
    <ul> 
     <li> Les heures budgétées sont résumées par fonction et par personne individuelle dans le rapport d’utilisation, comme suit : <br><strong>Personne individuelle :</strong> les heures budgétées sont résumées pour chaque personne dans le rapport d’utilisation. Ces heures budgétées sont associées aux tâches et problèmes auxquels la personne est affectée sur les projets inclus. (Vous pouvez développer la ligne de la fonction correspondante pour afficher la liste des personnes ayant cette fonction.)<br><strong>Fonction :</strong> les heures budgétées sont résumées par fonction dans le rapport d’utilisation.<br>Les heures budgétées apparaissent dans une fonction particulière en tant que résultat de l’un des scénarios suivants :
     <ul>
     <li>La fonction est définie comme la fonction principale de la personne affectée à la tâche ou au problème auquel les heures budgétées sont associées. </li> 
       <li>Lorsque vous affichez des informations d’utilisation pour un seul projet, la fonction de la personne à laquelle les heures sont affectées est utilisée, qu’il n’y ait aucune affectation sur la tâche ou le problème, qu’une autre personne soit affectée sans affectation de fonction, qu’une autre personne soit affectée avec une fonction différente ou qu’une autre équipe soit affectée.</li> 
       <li>Lorsque vous affichez des informations d’utilisation pour plusieurs projets, programmes ou portfolios, la fonction de la personne à laquelle les heures sont affectées n’est utilisée que lorsque la fonction est affectée à une tâche ou à un problème dans un projet. </li> 
       <li>La fonction est attribuée à la tâche ou au problème auquel sont associées les heures budgétées, et la personne affectée à la tâche ou au problème n’a pas de fonction définie dans le système.</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>Heures non allouées</strong> : les heures budgétées s’affichent dans le rapport d’utilisation de la section Heures non allouées lorsque les heures budgétées sont associées à une tâche ou à un problème et qu’aucune personne ou aucun rôle n’est affecté(e) à la tâche ou au problème.<br>Cette section s’affiche uniquement lorsque des heures sur le projet correspondent à cette description et lors de l’affichage du rapport d’utilisation par ou à partir d’un projet. </p> <p>Cette section s’affiche uniquement lorsque des heures sur le projet correspondent à cette description et lors de l’affichage du rapport d’utilisation par ou à partir d’un projet. </p> </li> 
    </ul> <p>Pour plus d’informations sur les heures budgétées, voir <a href="/help/quicksilver/manage-work/projects/project-finances/budgeted-labor-cost.md#locate-the-budgeted-hours-of-a-project">Rechercher les heures budgétées d’un projet</a> dans <a href="/help/quicksilver/manage-work/projects/project-finances/budgeted-labor-cost.md">Comprendre le coût budgété de la main-d’œuvre et les heures budgétées pour les projets</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Nombre d’heures prévues</strong> </td> 
   <td scope="col">
<p>
Nombre d’heures prévues sur les projets inclus associés aux affectations pour chaque tâche et chaque problème. Vous pouvez afficher le nombre total d’heures prévues de toutes les affectations sur le projet pour la durée totale des projets inclus ou afficher le nombre total d’heures prévues uniquement pour la période spécifiée (une semaine ou un mois spécifique).
</p>
<p>
<strong>CONSEIL</strong>
</p>
<p>
Le nombre d’heures prévues des éléments dont la durée est de 0 n’est pas pris en compte. 
</p>
<p>
Le nombre d’heures prévues dans le rapport d’utilisation tient compte du fait que les heures prévues ont été réaffectées pendant toute la durée d’une tâche ou d’un problème. 
</p>
<p>
Lorsque l’affectation quotidienne des heures a été modifiée à l’aide de l’équilibreur de charge de travail, les données du rapport d’utilisation peuvent être affectées si les dates sélectionnées dans le rapport d’utilisation contiennent seulement une partie de la durée d’une tâche ou d’un problème. 
</p>
<p>
Pour plus d’informations sur la modification des affectations, voir <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">Gestion des affectations dans l’équilibreur de charge de travail</a>.


</p>
<p>
Le nombre d’heures prévues est indiqué dans le rapport d’utilisation de l’une des lignes suivantes :
</p>
<ul>

<li>Le nombre d’heures prévues est résumé par fonction et par personne dans le rapport d’utilisation, comme suit : 
<ul>

<li><strong>Personne individuelle</strong> : le nombre d’heures prévues est résumé pour chaque personne dans le rapport d’utilisation. Ce nombre d’heures prévues est associé aux tâches et aux problèmes auxquels la personne est affectée sur les projets inclus. (Vous pouvez développer la ligne de la fonction correspondante pour afficher la liste des personnes ayant cette fonction.)

<li><strong>Fonction</strong> : le nombre d’heures prévues est résumé par fonction dans le rapport d’utilisation d’un seul projet.<br>Le nombre d’heures prévues apparaît dans une fonction particulière en tant que résultat de l’un des scénarios suivants :  
<ul>

<li>La fonction est définie comme la fonction principale de la personne affectée à la tâche ou au problème auquel le nombre d’heures prévues est associé.

<li>Lorsque vous affichez les informations d’utilisation d’un seul projet, les heures associées à une fonction ne s’affichent pas pour la fonction dans les scénarios suivants :   
<ul>

<li>Il n’y a pas d’affectation de la tâche ou du problème.

<li>Une personne est affectée sans fonction.

<li>Une personne se voit attribuer une fonction différente.

<li>Une équipe est affectée à la tâche ou au problème.
</li>   
</ul>

<li>Lorsque vous affichez des informations d’utilisation pour plusieurs projets, programmes ou portfolios, la fonction de la personne à laquelle les heures sont affectées n’est utilisée que lorsque la fonction est affectée à une tâche ou à un problème dans un projet. Les heures de fonction ne s’affichent pas séparément lors de l’affichage du rapport d’utilisation de plusieurs projets.

<li>La fonction est attribuée à la tâche ou au problème associés au nombre d’heures prévues. La personne affectée à la tâche ou au problème n’a pas de fonction définie dans le système.
</li>  
</ul>

<li><strong>Heures non allouées</strong> : le nombre d’heures prévues s’affiche dans le rapport d’utilisation de la section Heures non allouées lorsque le nombre d’heures prévues est associé à une tâche ou à un problème et qu’aucune personne ou aucun ou rôle n’est attribué à la tâche ou au problème. Cette section s’affiche uniquement lorsque des heures sur le projet correspondent à cette description et lors de l’affichage du rapport d’utilisation pour un seul projet. <br>Pour plus d’informations sur le nombre d’heures prévues, voir <a href="../../manage-work/tasks/task-information/planned-hours.md">Vue d’ensemble du nombre d’heures prévues</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Heures effectives</strong> </td> 
   <td> <p> Nombre total d’heures consigné pour les tâches, les problèmes <span>et le projet</span> pour les projets inclus. Vous pouvez afficher le nombre total d’heures effectives pour la durée totale des projets inclus ou afficher le nombre total d’heures effectives uniquement pour la période spécifiée (une semaine ou un mois spécifique). </p> <p><strong>Avertissement :</strong> le rapport d’utilisation inclut les heures enregistrées dans le projet, les tâches enfants, les problèmes et les tâches parents qui ont au moins une affectation. Il n’inclut pas les heures consacrées aux tâches parents sans affectation. Nous vous recommandons de ne pas utiliser de tâches parents comme tâches de travail et d’affecter uniquement des tâches enfants à vos ressources. </p> <p>Les heures effectives sont indiquées dans le rapport d’utilisation de l’une des lignes suivantes :</p> 
    <ul> 
     <li> Les heures effectives sont résumées par fonction et par personne dans le rapport d’utilisation d’un projet, comme suit :<br><strong>Personne individuelle :</strong> les heures effectives s’affichent dans le rapport d’utilisation de la ligne de la personne qui a consigné les heures. (Vous pouvez développer la ligne de la fonction correspondante pour afficher la liste des personnes disposant de cette fonction et ayant des heures consignées.)<br><strong>Fonction :</strong> les heures effectives consignées par les personnes associées à ces rôles sont résumées dans le rapport d’utilisation de la ligne de la fonction correspondante.<br>Les heures effectives apparaîssent dans une fonction particulière en tant que résultat de l’un des scénarios suivants : 
      <ul> 
       <li>La fonction est définie comme fonction principale de la personne qui a consigné les heures.</li> 
       <li>Il n’y a pas d’affectation de la tâche ou du problème.</li> 
       <li>Une autre personne est affectée sans fonction.</li> 
       <li>Une autre personne se voit attribuer une fonction différente.</li> 
       <li> <p>Une équipe est affectée.</p> </li> 
      </ul></li>  
     <p>Si la personne qui consigne les heures n’a pas de fonction associée à son profil, la fonction utilisée pour le rapport d’utilisation est celle affectée à la tâche ou au problème où les heures sont consignées, ou encore la fonction associée à la personne propriétaire principale de la tâche ou du problème. </p> 
     <li><strong>Autres heures :</strong> les heures effectives s’affichent dans le rapport d’utilisation de la section Autres heures, dans la ligne de la personne qui a consigné les heures.<br>Les heures s’affichent dans cette section lorsque la personne qui a consigné les heures n’a pas de fonction définie dans le système.<br>Cette section s’affiche uniquement lorsque des heures indiquées dans le projet correspondent à cette description. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Écart budgété (concernant les heures)</strong> </td> 
   <td> <p>Total des heures budgétées moins le total des heures effectives dans les projets inclus. Vous pouvez afficher l’écart budgété total pour la durée totale des projets inclus ou vous pouvez afficher l’écart budgété total uniquement pour la période spécifiée (vous pouvez indiquer une semaine ou un mois spécifique). </p> <p>Si la valeur est positive, elle s’affiche en vert. Cela indique que le total des heures budgétisées est supérieur aux heures effectives.</p> <p>Si la valeur est négative, elle s’affiche en rouge. Cela indique que le total des heures budgétisées est inférieur aux heures effectives.</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Écart prévu (concernant les heures)</strong> </td> 
   <td> <p>Nombre total d’heures prévues moins le nombre total d’heures effectives dans les projets inclus. Vous pouvez afficher l’écart prévu total pour la durée totale des projets inclus ou l’écart prévu total uniquement pour la période spécifiée (vous pouvez indiqueer une semaine ou un mois spécifique).</p> <p>Si la valeur est positive, elle s’affiche en vert. Cela indique que le total des heures prévues est supérieur aux heures effectives.</p> <p>Si la valeur est négative, elle s’affiche en rouge. Cela indique que le total des heures prévues est inférieur aux heures effectives.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Suivi des coûts {#track-cost}

Vous pouvez effectuer un suivi des coûts en comparant le coût budgété et le coût prévu aux coûts réels.

Lors du suivi des coûts d’un projet, d’un programme ou d’un portfolio, les informations du rapport d’utilisation proviennent des tâches. Les informations sur les coûts des tâches sont toujours disponibles dans le rapport d’utilisation. Le coût des tâches est calculé en fonction du type de coût de la tâche. Pour plus d’informations sur le type de coût des tâches, voir [Méthode de calcul des types de coûts par Workfront pour les tâches](/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-cost-types-for-tasks) dans [Suivi des coûts](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

Vous pouvez afficher les informations de coût dans le rapport d’utilisation de la façon suivante :

* Pour une semaine donnée ou un mois donné, ou pour le projet, programme ou portfolio global
* Par rôle ou par personne, pour les projets

La devise indiquée dans le rapport d’utilisation est déterminée par la devise définie dans le projet. Pour plus d’informations sur l’ajustement de la devise d’un projet, consultez [Modification de la devise du projet](../../manage-work/projects/project-finances/change-project-currency.md).

Les informations suivantes sont disponibles dans le rapport d’utilisation lors du suivi des coûts :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Titre de la colonne lors de l’affichage des coûts</strong> </th> 
   <th> <p><strong>Fonction</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Coût budgété</strong> </td> 
   <td scope="col"> <p>Coût budgété des projets inclus. Vous pouvez afficher le coût total budgété pour la durée totale des projets inclus ou afficher le coût total budgété pour la période spécifiée uniquement (vous pouvez spécifier une semaine ou un mois spécifique).</p> <p>Comme le coût budgété dans le rapport d’utilisation est axé sur le coût par rôle, le calcul est le même que le coût budgété de la main-d’oeuvre dans d’autres zones de Workfront. Pour plus d’informations sur le mode de calcul du coût budgété de la main-d’œuvre, consultez <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Comprendre le coût budgésé de la main-d’œuvre et les heures budgétées pour les projets</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Coût prévu</strong> </td> 
   <td scope="col"> <p>Coût prévu total des projets inclus. Vous pouvez afficher les coûts prévus totaux pour la durée totale des projets inclus ou afficher le coût prévu total pour la période spécifiée uniquement (vous pouvez spécifier une semaine ou un mois spécifique).</p> <p>Notez que pour les vues hebdomadaire, mensuelle et trimestrielle, les coûts prévus sont calculés en moyenne sur la période choisie lorsque les taux de dépenses des fonctions ou des utilisateurs et utilisatrices sont à la date effective.</p><p>Pour plus d’informations sur le mode de calcul du coût prévu du projet, voir <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-planned-budgeted-and-actual-costs">Comment Workfront calcule les coûts prévus, budgétés et réels</a> dans <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md">Suivi des coûts</a>.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"><strong>Coût réel</strong> </td> 
   <td scope="col"> <p>Les coûts réels totaux sur les projets inclus. Vous pouvez afficher les coûts réels totaux pour toute la durée de vie des projets inclus ou afficher les coûts réels totaux uniquement pour la période spécifiée (vous pouvez spécifier une semaine ou un mois spécifique).</p> <p>Pour plus d’informations sur le mode de calcul du coût réel du projet, voir <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md#how-workfront-calculates-planned-budgeted-and-actual-costs">Comment Workfront calcule les coûts prévus, budgétés et réels</a> dans <a href="/help/quicksilver/manage-work/projects/project-finances/track-costs.md">Suivi des coûts</a>.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Variance budgétée (concernant les coûts)</strong> </td> 
   <td scope="col"> <p>Coût budgété total moins le coût réel total dans les projets inclus. Vous pouvez afficher l’écart budgété total pour la durée totale des projets inclus ou vous pouvez afficher l’écart budgété total uniquement pour la période spécifiée (vous pouvez indiquer une semaine ou un mois spécifique).</p> <p>Si la valeur est positive, elle s’affiche en vert. Cela indique que le coût budgété total est supérieur au coût réel.</p> <p>Si la valeur est négative, elle s’affiche en rouge. Cela indique que le coût budgété total est inférieur au coût réel.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Variance prévue (concernant les coûts)</strong> </td> 
   <td> <p>Le coût prévu total moins le coût réel total des projets inclus. Vous pouvez afficher l’écart prévu total pour la durée totale des projets inclus ou l’écart prévu total uniquement pour la période spécifiée (vous pouvez indiqueer une semaine ou un mois spécifique). </p> <p>Si la valeur est positive, elle s’affiche en vert. Cela indique que le coût prévu total est supérieur au coût réel.</p> <p>Si la valeur est négative, elle s’affiche en rouge. Cela indique que le coût prévu total est inférieur au coût réel.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Suivre les revenus {#track-revenue}

Vous pouvez effectuer le suivi des revenus en comparant les revenus budgétés et prévus aux revenus réels.

Lors du suivi des revenus d’un projet, d’un programme ou d’un portfolio, seul les revenus provenant de tâches sont inclus dans le rapport d’utilisation.

Les informations contenues dans le tableau suivant sont disponibles dans le rapport d’utilisation lors du suivi des revenus.

Pour plus d’informations sur les champs spécifiques et sur la façon dont Workfront les calcule, reportez-vous également aux sections [Suivre les coûts](../../manage-work/projects/project-finances/track-costs.md) et [Vue d’ensemble de la facturation et des revenus](../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Titre de colonne lors de l’affichage des revenus</strong> </th> 
   <th> <strong>Fonction</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Revenu budgété</strong> </td> 
   <td scope="col"> <p>Le nombre total d’heures budgétées multiplié par le taux de facturation de la fonction pour les projets inclus. Vous pouvez afficher le revenu budgété total pour la durée totale des projets inclus ou afficher le revenu budgété total uniquement pour la période spécifiée (vous pouvez indiquer la semaine ou le mois de votre choix).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Revenus prévus</strong> </td> 
   <td scope="col"> <p>La zone Revenus prévus du rapport d’utilisation affiche les revenus correspondant au nombre d’heures prévues affectées aux ressources des tâches du projet.</p> <p>Dans le rapport d’utilisation, Workfront calcule les revenus prévus du projet à l’aide de la formule suivante :</p> <p><code>Project Planned Revenue = SUM (All Tasks Planned Revenue)</code> </p> 
   <p><b>NOTE</b>
   <p>Les revenus prévus du projet qui s’affichent dans le rapport d’utilisation diffèrent des revenus prévus qui s’affichent dans la zone Détails du projet et dans les rapports sur le projet. </p> <p>La zone Revenus prévus dans les détails du projet reflète les revenus de la tâche ainsi que les revenus fixes du projet. La zone Revenus prévus du rapport d’utilisation affiche les revenus prévus pour les tâches du projet uniquement. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>Si le projet comporte une tâche de 10 heures, affectée à une personne externe au taux horaire de 20 $ et que le projet a des revenus fixes de 100 $, le rapport d’utilisation affiche 200 $ pour les revenus prévus (les revenus prévus associés aux heures de la tâche). La section Détails du projet affiche 300 $ (les revenus prévus de la tâche et les revenus fixes du projet). </p> 
     </div> <p>Pour plus d’informations sur les revenus prévus pour les tâches et les projets en dehors du rapport d’utilisation, consultez la <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Vue d’ensemble de la facturation et des revenus</a>.</p> </p> <p>Dans le rapport d’utilisation, le mode de calcul et d’affichage des revenus prévus pour les projets inclus prend en compte le type de revenu défini sur la tâche. </p> <p>Selon le type de revenu de chaque tâche du projet, les scénarios suivants existent : </p> <p><strong>Revenus fixes :</strong> quelles que soient les affectations de la tâche, les revenus de celle-ci sont toujours calculés à l’aide du montant fixe spécifié pour la tâche.</p> <p><b>IMPORTANT</b>

Contrairement à d’autres zones de Workfront, le rapport d’utilisation calcule les revenus prévus pour les tâches de revenus fixes en divisant les revenus fixes de manière égale par le nombre d’heures prévues de la tâche. </p> <p>Prenons l’exemple d’une tâche affichant des revenus de 200 $. Si la tâche comporte 4 heures prévues, chaque heure correspond à 50 $. Ce montant est réparti au niveau de la personne et de la fonction. Cette répartition est propre au rapport d’utilisation.</p> <p><b>NOTE</b>

Si vous avez une tâche de revenus fixes et qu’il n’y a pas d’heures prévues pour la tâche, les revenus ne s’affichent pas dans le rapport d’utilisation, car il n’existe aucun moyen de les répartir en heures. Si la tâche comporte des heures prévues, des revenus fixes et aucune affectation, les revenus s’affichent sous la forme de revenus non affectés. </p> <p><strong>Rôle par heure :</strong> les revenus de la tâche sont calculés à l’aide du taux de facturation défini pour un rôle spécifique, multiplié par le nombre d’heures prévues pour ce rôle. Workfront utilise la formule suivante :</p> <p><code>Revenus prévus du rôle par heure = SOMME(heures prévues du rôle sur toutes les tâches) * taux de facturation du rôle</code></p><p><b>NOTE :</b> le taux de facturation horaire dans la formule prend en compte toute modification du taux en vigueur à la date.</p>   <p><strong>Personne, par heure :</strong> les revenus de la tâche sont calculés selon le taux de facturation défini pour une personne donnée, multiplié par le nombre d’heures prévues pour cette personne. Workfront utilise la formule suivante :</p> <p><code>Revenus prévus de la personne par heure = SOMME(heures prévues de la personne sur toutes les tâches) * taux de facturation de la personne</code> </p> <p><b>REMARQUE :</b> le taux de facturation horaire dans la formule prend en compte toute modification du taux en vigueur à la date.</p> <p><b>Rôle par heure ou Personne, par heure plus fixe</b> </p> <p><b>IMPORTANT</b>

Contrairement à d’autres zones de Workfront, le rapport d’utilisation calcule les revenus prévus en divisant les revenus fixes de manière égale par le nombre d’heures prévues de la tâche. </p> <p>Les cas suivants existent : </p>
<ul>
<li> <p><strong>Rôle par heure plus fixe :</strong> le revenu de la tâche est calculé à l’aide du taux de facturation défini pour un rôle spécifique, multiplié par le nombre d’heures prévues associées au rôle. En outre, un montant fixe spécifié sur la tâche est ajouté au taux du rôle. Workfront utilise la formule suivante :</p> <p><code>Revenus prévus de rôle par heure plus fixe = [SOMME(Heures prévues du rôle sur toutes les tâches) * Taux de facturation du rôle] + SOMME(Limite ou montant fixe de la tâche / Heures prévues de la tâche)</code> </p> </li>
<li> <p><strong>Personne, par heure plus fixe :</strong> taux de facturation défini pour une personne spécifique, multiplié par le nombre d’heures prévues de la tâche de cette personne. En outre, un montant fixe spécifié dans la tâche est ajouté au taux de la personne. Workfront utilise la formule suivante :</p> <p><code>Revenus prévus de personne, par heure plus fixe = [SOMME(Heures prévues de la personne sur toutes les tâches) * Taux de facturation de la personne] + SOMME(Limite ou montant fixe de la tâche / Heures prévues de la tâche)</code> </p> </li>
</ul> <p><b>Rôle par heure avec limite ou personne, par heure avec limite</b> </p> <p><b>IMPORTANT</b>

Contrairement à d’autres zones de Workfront, si les revenus prévus dépassent la limite, le montant par rapport au montant de la limite est considéré comme des revenus fixes. Les revenus prévus sont calculés en divisant équitablement les revenus fixes par le nombre d’heures prévues sur la tâche, puis en y ajoutant le montant de la limite et les revenus par heure du rôle ou de la personne.<br></p> <p>Les cas suivants existent : </p>
<ul>
<li> <p><strong>Rôle par heure avec limite :</strong> les tâches sont facturées toutes les heures comme dans l’option Rôle par heure, mais vous pouvez spécifier un montant maximal. Workfront utilise la formule suivante :</p> <p><code>Revenus prévus de rôle par heure avec limite = [SOMME(Heures prévues du rôle sur toutes les tâches et tous les problèmes) * Taux de facturation du rôle] + Montant de limite de la tâche + SOMME(Montant par rapport au montant de limite / Heures prévues de la tâche)</code> </p> </li>
<li> <p><strong>Personne, par heure avec limite :</strong> les tâches sont facturées toutes les heures comme dans Personne, par heure, mais vous pouvez spécifier un montant de limite maximal. Workfront utilise la formule suivante : </p> <p><code>Revenus prévus de Personne, par heure avec limite = [SOMME(Heures prévues de la personne pour toutes les tâches) * Taux de facturation de la personne] + Montant de limite maximal de la tâche + SOMME(Montant par rapport au montant de limite / Heures prévues de la tâche)</code> </p> </li>
</ul> <p>Pour plus d’informations sur le rôle ou la personne pris(e) en compte lors du calcul des revenus prévus, consultez <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Vue d’ensemble de la facturation et des revenus</a>.</p> </td>
</tr> 
  <tr> 
   <td><strong>Revenus réels</strong> </td>
   <td> <p>Les revenus réels correspondent au revenu associé aux heures effectives des tâches et du projet. Pour plus d’informations sur les revenus réels, consultez <a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#track-revenue-amounts">Suivre les montants de revenu</a> dans <a href="/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md">Vue d’ensemble de la facturation et des revenus</a>.</p>

<p>La manière selon laquelle le rapport d’utilisation calcule les revenus réels pour les projets inclus varie en fonction du type de revenu défini sur la tâche, comme suit :</p> <p><strong>Revenus fixes :</strong> quelles que soient les affectations de tâche, le revenu de la tâche est toujours calculé à l’aide du montant fixe spécifié sur la tâche.</p> <p><b>IMPORTANT</b>

Contrairement à d’autres zones de Workfront, le rapport d’utilisation calcule les revenus réels en divisant équitablement les revenus fixes par le nombre d’heures consignées sur la tâche. </p> <p> </p> <p>Par exemple, les revenus réels d’une tâche sont de 200 $. Si la tâche comporte 4 heures effectives, chaque heure équivaudrait à 50 $. Cette répartition se fait au niveau de l’utilisateur ou l’utilisatrice et du rôle. Cette répartition est propre au rapport d’utilisation.</p> <p><b>REMARQUE</b>

Si vous avez une tâche de revenus fixes et qu’il n’y a pas d’heures effectives sur la tâche, les revenus réels n’apparaissent pas dans le rapport d’utilisation, car il n’existe aucun moyen de répartir les heures. </p> <p><strong>Rôle par heure :</strong> le revenu de la tâche est calculé à l’aide du taux de facturation défini pour un rôle spécifique, multiplié par le nombre d’heures effectives.</p> <p>Workfront utilise la formule suivante :</p> <p><code>Revenus réels de rôle par heure = SOMME(Heures effectives du rôle sur toutes les tâches) * Taux de facturation du rôle</code> </p> <p><b>NOTE :</b> le taux de facturation par heure dans la formule prend en compte toute modification apportée à la date d’entrée en vigueur du taux.</p> <p><strong>Personne, par heure :</strong> le revenu de la tâche est calculé à l’aide du taux de facturation défini pour une personne spécifique, multiplié par le nombre d’heures enregistrées sur la tâche par cette personne. Workfront utilise la formule suivante :</p> <p><code>Revenus réels de personne, par heure = SOMME(Heures effectives de la personne sur toutes les tâches) * Taux de facturation de la personne</code></p> <p><b>NOTE :</b> le taux de facturation par heure dans la formule prend en compte toute modification apportée à la date d’entrée en vigueur du taux.</p> <p><b>Rôle par heure plus fixe ou personne, par heure plus fixe</b> </p> <p><b>IMPORTANT</b>

Contrairement à d’autres zones de Workfront, le rapport d’utilisation calcule les revenus réels en divisant équitablement les revenus fixes par le nombre d’heures consignées sur la tâche. </p> <p>Les cas suivants existent : </p>
<ul>
<li> <p><strong>Rôle par heure plus fixe :</strong> taux de facturation défini pour un rôle spécifique, multiplié par le nombre d’heures enregistrées sur la tâche par une personne disposant de ce rôle. En outre, un montant fixe spécifié sur la tâche est ajouté au taux du rôle. </p> <p>Workfront utilise la formule suivante :</p> <p><code>Revenus réels de rôle par heure plus fixe = [SOMME(Heures effectives du rôle sur toutes les tâches) * Taux de facturation du rôle] + SOMME(Limite ou montant fixe de la tâche / Heures effectives de la tâche)</code> </p> </li>
<li> <p><strong>Personne, par heure plus fixe :</strong> taux de facturation défini pour une personne spécifique, multiplié par le nombre d’heures consignées pour la tâche par cette personne. En outre, un montant fixe spécifié dans la tâche est ajouté au taux de la personne. </p> <p>Workfront utilise la formule suivante :</p> <p><code>Revenus réels de la personne, par heure plus fixe = [SOMME(Heures effectives du rôle sur toutes les tâches) * Taux de facturation de la personne] + SOMME(Montant limite ou fixe de la tâche / Heures de la personne de la tâche)</code> </p> </li>
</ul> <p><b>Rôle par heure avec limite ou personne, par heure avec limite</b> </p> <p><b>IMPORTANT</b>

Contrairement à d’autres zones de Workfront, si les revenus prévus dépassent la limite, le montant par rapport au montant de la limite est considéré comme des revenus fixes. Les revenus prévus sont calculés en divisant équitablement les revenus fixes par le nombre d’heures prévues sur la tâche, puis en y ajoutant le montant de la limite et les revenus par heure du rôle ou de la personne.<br></p> <p>Les cas suivants existent :</p>
<ul>
<li> <p><strong>Rôle par heure avec limite :</strong> les tâches sont facturées toutes les heures comme dans l’option Rôle par heure, mais vous pouvez spécifier un montant maximal. Workfront utilise la formule suivante :</p> <p><code>Revenus réels du rôle, par heure et avec limite = [SOMME(heures effectives du rôle sur toutes les tâches et tous les problèmes) * Taux de facturation du rôle] + Montant de limite maximal de la tâche + SOMME(Montant supérieur au montant maximal / Heures effectives de la tâche).</code></p> </li>
<li> <p><strong>Personne, par heure avec limite :</strong> les tâches sont facturées toutes les heures comme dans l’option Personne, par heure, mais vous pouvez spécifier un montant maximal.</p> <p> Workfront utilise la formule suivante :</p> <p><code>Revenus réels de la personne, par heure avec limite = [SOMME(Heures effectives du rôle sur toutes les tâches et tous les problèmes) * Taux de facturation de la personne] + Montant de limite maximal de la tâche + SOMME(Montant supérieur au montant maximal / Heures effectives de la tâche)</code> </p> </li>
</ul>
<p><strong>Revenus du projet</strong> : les revenus pour les heures consignées dans le projet sont calculés en tenant compte du montant de la facturation par heure pour la fonction principale de la personne qui consigne l’heure. Il n’est pas recommandé de consigner les heures consacrées au projet. </p>
<p><b>NOTE</b>

Si la personne n’est pas associé à une fonction ou si la facturation par heure du rôle principal est égale à zéro, Workfront calcule les revenus réels à l’aide du montant de la facturation par heure pour la personne. Si le profil d’utilisateur ou d’utilisatrice ne comporte pas de montant de facturation par heure, les revenus réels sont nuls. </p>
</td> 
  </tr> 
  <tr> 
   <td><strong>Variance budgétée (concernant les revenus)</strong> </td> 
   <td> <p>Les revenus réels totaux moins le revenu budgété sur les projets inclus.<br>Vous pouvez afficher la variance budgétée totale pour la durée totale des projets inclus ou vous pouvez afficher la variance budgétée totale uniquement pour la période spécifiée (vous pouvez indiquer une semaine ou un mois spécifique).</p> <p>Si la valeur est positive, elle s’affiche en vert. Cela indique que le total du revenu budgété est supérieur aux revenus réels.</p> <p>Si la valeur est négative, elle s’affiche en rouge. Cela indique que le revenu budgété total est inférieur aux revenus réels.</p> </td>
  </tr> 
  <tr> 
   <td><strong>Variance prévue (concernant les revenus)</strong> </td> 
   <td> <p>Revenus réels totaux moins les revenus prévus totaux pour les projets inclus.<br>Vous pouvez afficher la variance prévue totale pour la durée totale des projets inclus ou la variance prévue totale uniquement pour la période spécifiée (vous pouvez indiquer une semaine ou un mois spécifique). </p> <p>Si la valeur est positive, elle s’affiche en vert. Cela indique que les revenus prévus totaux sont supérieurs aux revenus réels.</p> <p>Si la valeur est négative, elle s’affiche en rouge. Cela indique que le total des revenus prévus est inférieur aux revenus réels.</p> </td>
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### Comparer les revenus aux coûts prévus et réels {#compare-revenue-against-planned-and-actual-costs}

Vous pouvez visualiser le coût prévu ou réel en regard des revenus prévus. La marge (%) est également affichée (la marge est calculée comme suit : revenus - coût / revenus).

Les informations suivantes sont disponibles dans le rapport d’utilisation lors de la comparaison des revenus par rapport aux coûts prévus et réels :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Titre de colonne lors de l’affichage des revenus et du coût (prévus)</strong> </th> 
   <th> <strong>Fonction</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Coût prévu</strong> </td> 
   <td scope="col"> Coût prévu total des projets inclus. Vous pouvez afficher les coûts prévus totaux pour la durée totale des projets inclus ou afficher le coût prévu total pour la période spécifiée uniquement (vous pouvez spécifier une semaine ou un mois spécifique). </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Revenus prévus</strong> </td> 
   <td scope="col"> <p>Les revenus prévus correspondent aux revenus pour les heures prévues des tâches. </p> <p>Le mode de calcul et d’affichage du rapport d’utilisation des revenus pour les projets inclus varie en fonction du type de revenu défini sur la tâche, comme décrit dans la section <a href="#track-revenue" class="MCXref xref">Suivre les revenus</a> dans cet article.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Marge</strong> </td> 
   <td scope="col"> <p>Le pourcentage de marge est calculé comme suit :</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>NOTE</b>

Si les revenus prévus sont nuls, la marge l’est également. </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>Titre de colonne lors de l’affichage du revenu par rapport au coût (réels)</strong> </p>  </td> 
   <td scope="col"><p><strong>Fonction</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Coût réel</strong> </td> 
   <td scope="col"> <p>Les coûts réels totaux sur les projets inclus. Vous pouvez afficher les coûts réels totaux pour toute la durée de vie des projets inclus ou afficher les coûts réels totaux uniquement pour la période spécifiée (vous pouvez spécifier une semaine ou un mois spécifique).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Revenus réels</strong> </td> 
   <td> <p>Les revenus réels correspondent au revenu associé aux heures effectives des tâches.</p> <p>Les revenus réels n’apparaissent dans le rapport d’utilisation qu’une fois la tâche marquée comme Terminé (ou dont le statut est Terminé).</p> <p>La manière selon laquelle le rapport d’utilisation calcule les revenus réels pour les projets inclus varie en fonction du type de revenu défini sur la tâche, comme décrit dans la section <a href="#track-revenue" class="MCXref xref">Suivre le revenu</a> de cet article. </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Marge</strong> </td> 
   <td> <p>Le pourcentage de marge est calculé comme suit :</p> <p>Revenus réels - Coût réel / Revenus réels * 100. </p> <p><b>NOTE</b>

Si les revenus réels sont de 0, la marge affichée est de 0. </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## Suivre la progression, le coût et le revenu avec le rapport d’utilisation {#track-progress-cost-and-revenue-with-the-utilization-report}

Vous pouvez suivre la progression ou le coût d’un projet, d’un programme ou d’un portfolio.

Vous pouvez afficher des informations sur le rapport d’utilisation pour une semaine ou un mois spécifique, ou pour la toute la durée de vie des projets.

Pour suivre la progression ou le coût d’un ou de plusieurs projets avec un rapport d’utilisation :

1. Effectuez l’une des opérations suivantes, selon que vous affichez les informations d’utilisation d’un projet individuel, de plusieurs projets, d’un programme ou d’un portfolio :

   * Pour afficher les informations d’utilisation d’un seul projet :

      1. Accédez au projet pour lequel vous souhaitez afficher des informations d’utilisation, puis cliquez sur **Utilisation** dans le panneau de gauche.
      1. Les informations d’utilisation s’affichent automatiquement lors de l’affichage d’un projet individuel, et l’application d’un filtre n’est pas obligatoire.\
         Si vous souhaitez filtrer le rapport d’utilisation, vous pouvez appliquer un filtre, puis cliquer sur **Exécuter**.\
         Pour plus d’informations sur le filtrage du rapport d’utilisation, consultez [Filtrer les informations d’utilisation](#filter-utilization-information) dans cet article.\
         Les informations d’utilisation s’affichent pour les utilisateurs et utilisatrices et les rôles individuels (les utilisateurs et utilisatrices sont regroupés dans le rôle qui leur est associé).

   * Pour afficher les informations d’utilisation de plusieurs projets :

     {{step1-to-utilization-report}}

      1. Appliquez un filtre au rapport d’utilisation, puis cliquez sur **Exécuter**.
Vous devez spécifier un ou plusieurs projets dans le filtre avant d’exécuter le rapport d’utilisation. Pour plus d’informations sur le filtrage du rapport d’utilisation, consultez [Filtrer les informations d’utilisation](#filter-utilization-information) dans cet article.\
         Les informations d’utilisation s’affichent pour les rôles et les projets individuels (les rôles sont regroupés dans le projet qui leur est associé).

   * Pour afficher les informations d’utilisation d’un programme :

     {{step1-to-utilization-report}}

      1. Cliquez sur **Afficher** > **Programmes**.
      1. Appliquez un filtre au rapport d’utilisation, puis cliquez sur **Exécuter**.\
         Vous devez spécifier un ou plusieurs programmes dans le filtre avant d’exécuter le rapport d’utilisation. Pour plus d’informations sur le filtrage du rapport d’utilisation, consultez [Filtrer les informations d’utilisation](#filter-utilization-information) dans cet article.\
         Les informations d’utilisation s’affichent pour les projets et programmes individuels (les projets sont regroupés dans le programme qui leur est associé).

   * Pour afficher les informations d’utilisation d’un portfolio :

     {{step1-to-utilization-report}}

      1. Cliquez sur **Afficher** > **Portfolios**.
      1. Appliquez un filtre du rapport d’utilisation, puis cliquez sur **Exécuter**.\
         Vous devez spécifier un ou plusieurs portfolios dans le filtre avant d’exécuter le rapport d’utilisation. Pour plus d’informations sur le filtrage du rapport d’utilisation, consultez [Filtrer les informations d’utilisation](#filter-utilization-information) dans cet article.\
         Les informations d’utilisation s’affichent pour les projets, programmes et portfolios individuels (les projets sont regroupés dans le programme qui leur est associé et les programmes sont regroupés dans le portfolio qui leur est associé).

1. Dans le coin supérieur droit du rapport d’utilisation, cliquez sur **Afficher**, puis sélectionnez l’une des options suivantes dans le menu :

   * **Coût**
   * **Heures**
   * **Revenu**
   * **Comparatif revenus/coûts (prévus)**
   * **Comparatif revenus/coûts (réels)**

   L’option sélectionnée détermine les colonnes et les informations disponibles dans le rapport.
   ![Options d’affichage](assets/utilization-view-dropdown.png)

1. (Facultatif) Sélectionnez la période pour laquelle les informations d’utilisation s’affichent. Vous pouvez afficher les informations d’une semaine ou d’un mois spécifique à gauche de la colonne **Général**. Les informations relatives au projet, au programme ou au portfolio global sont toujours affichées dans la colonne **Général**.\
   Pour plus d’informations, voir [Ajuster la période pour laquelle les informations sont affichées](#adjust-the-date-range-for-which-information-is-displayed) dans cet article.

1. (Facultatif) Cliquez sur le titre d’une colonne pour trier le rapport d’utilisation en fonction des informations qu’elle contient. Le tri ne fonctionne que lorsque vous incluez plusieurs éléments dans votre rapport. Vous pouvez, par exemple, trier les résultats de votre rapport lorsque vous observez plusieurs projets (ou portfolios ou programmes). Vous ne pouvez pas trier les résultats lorsque vous ne vous intéressez qu’à un seul projet (ou à un seul portfolio ou un seul programme) à la fois.
1. Utilisez les informations de la section [Vue d’ensemble du rapport d’utilisation](#overview-of-the-utilization-report) dans cet article pour en savoir plus sur chaque colonne du rapport d’utilisation.

## Informations sur l’utilisation des filtres {#filter-utilization-information}

Vous pouvez filtrer le contenu affiché dans un rapport d’utilisation sur un projet. Vous pouvez filtrer par tâches, problèmes, rôles et données personnalisées. Lorsque vous appliquez un filtre, le rapport d’utilisation contient des informations basées sur les critères que vous sélectionnez.

Vous pouvez créer un filtre ou en appliquer un que vous avez déjà créé.

### Créer ou modifier un filtre {#create-or-modify-a-filter}

Lorsque vous créez un filtre, les utilisateurs et utilisatrices de Workfront ayant accès au rapport d’utilisation ont également accès au filtre que vous créez. De même, lorsque vous modifiez un filtre existant, celui-ci est modifié pour les utilisateurs et utilisatrices ayant accès au rapport d’utilisation.

Pour créer et modifier un filtre :

1. Ouvrez le rapport Utilisation.
Pour ce faire, voir [Suivre la progression, les coûts et les revenus à l’aide du rapport Utilisation](#track-progress-cost-and-revenue-with-the-utilization-report).

1. Cliquez sur l’icône **Filtrer** pour afficher les options de filtrage.
1. (Le cas échéant) Pour modifier un filtre existant, cliquez sur le menu déroulant **Filtrer**, puis sélectionnez le filtre à modifier.
1. Indiquez les informations suivantes pour créer ou modifier le filtre :

   * **Portfolios :** commencez à saisir le nom du portfolio qui contient les informations à inclure dans le rapport d’utilisation, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.\
     Répétez cette procédure pour inclure des informations provenant de plusieurs portfolios dans le rapport d’utilisation.\
     Pour inclure tous les portfolios de votre système dans votre filtre, cliquez sur **Tout ajouter**. (Cette option est disponible uniquement si votre système contient moins de 10 portfolios.)

   * **Programmes :** commencez à saisir le nom du programme contenant les informations à inclure dans le rapport d’utilisation, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.\
     Répétez cette procédure pour inclure des informations provenant de plusieurs tâches dans le rapport d’utilisation.\
     Si vous avez déjà désigné des portfolios dans le filtre, le programme que vous spécifiez doit provenir des portfolios déjà inclus dans le filtre. Dans le cas contraire, les données du programme ne sont pas incluses dans le rapport d’utilisation.\
     Pour inclure tous les programmes de votre système dans votre filtre, cliquez sur **Tout ajouter**. (Cette option est disponible uniquement si votre système comporte moins de 20 programmes.)

   * **Projets :** commencez à saisir le nom du projet contenant les informations à inclure dans le rapport d’utilisation, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.\
     Répétez cette procédure pour inclure des informations provenant de plusieurs projets dans le rapport d’utilisation.\
     Si vous avez déjà désigné des portfolios ou des programmes dans le filtre, le projet que vous spécifiez doit provenir de l’un des portfolios ou programmes déjà inclus dans le filtre. Dans le cas contraire, les données du projet ne sont pas incluses dans le rapport d’utilisation.\
     Pour inclure tous les projets de votre système dans votre filtre, cliquez sur **Tout ajouter**. (Cette option est disponible uniquement si votre système contient moins de 250 projets.)

   * **Tâches :** commencez à saisir le nom de la tâche qui contient les informations à inclure dans le rapport d’utilisation, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.\
     Répétez cette procédure pour inclure des informations provenant de plusieurs tâches dans le rapport d’utilisation.\
     Si vous avez déjà désigné des portfolios, programmes ou projets dans le filtre, la tâche que vous spécifiez doit provenir de l’un des portfolios, programmes ou projets déjà inclus dans le filtre. Dans le cas contraire, les données de la tâche ne sont pas incluses dans le rapport d’utilisation.

   * **Problèmes :** commencez à saisir le nom du problème qui contient les informations à inclure dans le rapport d’utilisation, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante.\
     Répétez cette procédure pour inclure des informations provenant de plusieurs problèmes dans le rapport d’utilisation.\
     Si vous avez déjà désigné des portfolios, programmes ou projets dans le filtre, le problème que vous spécifiez doit provenir de l’un des portfolios, programmes ou projets déjà inclus dans le filtre. Dans le cas contraire, les données du problème ne sont pas incluses dans le rapport d’utilisation.\
     Les informations sur les coûts des problèmes ne sont pas toujours incluses dans le rapport d’utilisation. Pour plus d’informations sur le moment où les informations sur les coût des problèmes sont incluses dans le rapport d’utilisation, voir [Suivre la progression, les coûts et les revenus à l’aide du rapport d’utilisation](#track-progress-cost-and-revenue-with-the-utilization-report) dans cet article.

   * **Rôles :** commencez à saisir le nom du rôle que vous souhaitez représenter dans le rapport d’utilisation, puis cliquez sur le nom lorsqu’il apparaît dans la liste déroulante. Répétez cette procédure pour inclure des rôles supplémentaires.
Le rapport d’utilisation ne contient des informations que sur les rôles que vous spécifiez. Par exemple, une tâche contient 10 heures effectives. Six d’entre elles proviennent d’un rôle de conception et quatre d’un rôle de développement. Si vous filtrez le rapport d’utilisation par rôle pour la conception, les quatre heures qui proviennent du rôle de développement sont exclues du rapport.

   * **Ajouter une règle de filtre :** cliquez sur **Ajouter une règle de filtre**, cliquez dans le champ de texte, puis commencez à saisir le nom du champ sur lequel vous souhaitez filtrer les données. Si le champ est disponible, il est renseigné pour chaque objet auquel il peut être associé. Cliquez sur le nom du champ pour l’ajouter au filtre.

     >[!IMPORTANT]
     >
     >Vous devez saisir le nom du champ et non le libellé du champ. Le libellé du champ s’affiche sur un formulaire personnalisé associé à un objet. Pour plus d’informations sur la différence entre le libellé et le nom d’un champ personnalisé, voir [Création d’un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

     Pour plus d’informations sur les champs que vous voyez dans les colonnes, consultez [Glossaire de la terminologie Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).\
     Sélectionnez les modificateurs de filtre et de condition pour le filtre. Les modificateurs disponibles sont décrits dans [Modificateurs de filtre et de condition](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Pour créer un filtre, cliquez sur **Enregistrer le filtre**.\
   Ou\
   Pour modifier un filtre existant, cliquez sur la flèche en regard du bouton **Enregistrer le filtre**, puis cliquez sur **Enregistrer un nouveau filtre**.
Dans le champ **Nom du filtre**, saisissez le nom du filtre, puis cliquez sur **Enregistrer**.
La zone Utilisation est filtrée avec les informations que vous avez incluses dans le filtre.

### Appliquer un filtre enregistré {#apply-a-saved-filter}

1. Ouvrez le rapport Utilisation.
Pour ce faire, consultez [Suivre la progression, le coût et le revenu avec le rapport d’utilisation](#track-progress-cost-and-revenue-with-the-utilization-report).

1. Cliquez sur **Filtres enregistrés**, puis sélectionnez le filtre à appliquer dans la liste déroulante.

### Dupliquer un filtre {#duplicate-a-filter}

1. Ouvrez le rapport Utilisation.
Pour ce faire, consultez [Suivre la progression, le coût et le revenu avec le rapport d’utilisation](#track-progress-cost-and-revenue-with-the-utilization-report).

1. Cliquez sur **Filtres enregistrés**, pointez sur le filtre à dupliquer, puis cliquez sur l’icône **Dupliquer**.

   ![Icône Dupliquer](assets/utilization-filter-duplicate.png)

   La boîte de dialogue Dupliquer le filtre s’affiche.

1. Dans le champ **Nom du filtre**, saisissez le nom du nouveau filtre, puis cliquez sur **Enregistrer**.

### Renommer un filtre {#rename-a-filter}

Lorsque vous renommez un filtre, tous les utilisateurs et utilisatrices de Workfront ayant accès au rapport d’utilisation voient le nouveau nom que vous avez saisi.

Pour renommer un filtre :

1. Ouvrez le rapport Utilisation.
Pour ce faire, consultez [Suivre la progression, le coût et le revenu avec le rapport d’utilisation](#track-progress-cost-and-revenue-with-the-utilization-report).

1. Cliquez sur **Filtres enregistrés**, pointez sur le filtre à renommer, puis cliquez sur l’icône **Renommer**.

   ![Icône Renommer le filtre](assets/utilization-filter-rename.png)

   La boîte de dialogue Renommer le filtre s’affiche.

1. Dans le champ **Nom du filtre**, saisissez le nom du nouveau filtre, puis cliquez sur **Enregistrer**.

### Supprimer un filtre {#delete-a-filter}

Lorsque vous supprimez un filtre, celui-ci est supprimé pour tous les utilisateurs et utilisatrices de Workfront ayant accès au rapport d’utilisation.

Pour supprimer un filtre :

1. Ouvrez le rapport Utilisation.
Pour ce faire, consultez [Suivre la progression, le coût et le revenu avec le rapport d’utilisation](#track-progress-cost-and-revenue-with-the-utilization-report).

1. Cliquez sur **Filtres enregistrés**, pointez sur le filtre à supprimer, puis cliquez sur l’icône **Supprimer**.

   ![Icône Supprimer](assets/utilization-filter-delete.png)

1. Cliquez sur **Supprimer** lorsqu’on vous invite à confirmer la suppression du filtre.

## Régler la période d’affichage des informations {#adjust-the-date-range-for-which-information-is-displayed}

Vous pouvez régler la période pour laquelle les informations d’utilisation s’affichent. Vous pouvez sélectionner une date passée ou future. Les modifications que vous apportez ne sont visibles que par vous.

1. Ouvrez le rapport Utilisation.
Pour plus d’informations, voir [Suivre la progression, le coût et les revenus à l’aide du rapport d’utilisation](#track-progress-cost-and-revenue-with-the-utilization-report).

1. Cliquez sur la période en regard du bouton **Exporter**.

   La semaine en cours est sélectionnée par défaut.

1. Choisissez l’une des options suivantes :

   * **Semaine :** sélectionnez cette option pour sélectionner une semaine donnée (du dimanche au samedi).
   * **Mois :** Sélectionnez cette option pour sélectionner un mois donné.

   La période sélectionnée s’affiche dans le rapport d’utilisation, à gauche de la colonne **Général**.\
   Workfront se souvient si vous souhaitez afficher une semaine ou un mois. La prochaine fois que vous accéderez au rapport d’utilisation, la semaine ou le mois en cours s’affichera, selon l’option sélectionnée.

## Exporter des informations d’utilisation

Vous pouvez exporter des informations d’utilisation pour un projet, un programme ou un portfolio à partir de Workfront. Les informations ne peuvent être exportées que dans les formats XLSX, TSV et PDF.

Lorsqu’ils sont consultés dans Microsoft Excel, les nombres négatifs sont affichés entre parenthèses.

Pour exporter des informations d’utilisation :

1. Ouvrez le rapport Utilisation.
Pour plus d’informations, voir [Suivre la progression, le coût et les revenus à l’aide du rapport d’utilisation](#track-progress-cost-and-revenue-with-the-utilization-report).

1. Cliquez sur **Exporter** dans le coin supérieur gauche du rapport.

1. Sélectionnez l’une des options suivantes :

   * **PDF :** exporte le rapport au format PDF. Ce format est recommandé si vous envisagez d’imprimer le rapport.\
     Sélectionnez **Lettre - Portrait**, **Lettre - Paysage**, ou **Autres tailles** (propose des options pour l’export dans les formats Légal (8,5x14 pouces), Ledger (11x17 pouces) et A4).
Selon le système d’exploitation que vous utilisez, vous avez la possibilité d’ouvrir ou d’enregistrer le fichier. Ouvrez le fichier avec l’application associée ou enregistrez-le sur votre ordinateur.

   * **Excel :** exporte le rapport au format XLSX. Ce format est recommandé si vous envisagez d’analyser les données en profondeur dans Excel.
Selon le système d’exploitation que vous utilisez, vous avez la possibilité d’ouvrir ou d’enregistrer le fichier. Ouvrez le fichier avec l’application associée ou enregistrez-le sur votre ordinateur.

   * **Délimité par des tabulations :** exporte le rapport au format TSV. Il s’agit du format recommandé si vous envisagez d’importer les données dans un logiciel tiers en vue d’une analyse plus approfondie.
Selon le système d’exploitation que vous utilisez, vous avez la possibilité d’ouvrir ou d’enregistrer le fichier. Ouvrez le fichier avec l’application associée ou enregistrez-le sur votre ordinateur.

1. Lisez les informations de l’article [Exporter des données](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) pour comprendre comment utiliser le fichier exporté.

## Afficher des informations d’utilisation dans un graphique

Vous pouvez visualiser les données du rapport d’utilisation sous forme de graphique.

1. Ouvrez le rapport Utilisation.
Pour plus d’informations, voir [Suivre la progression, le coût et les revenus à l’aide du rapport d’utilisation](#track-progress-cost-and-revenue-with-the-utilization-report).

1. Dans le coin supérieur droit du rapport d’utilisation, cliquez sur l’icône **Graphique**.

   ![Icône de graphique](assets/utilization-chart.png)

   Le rapport d’utilisation est affiché sous forme de graphique.

1. (Facultatif) Configurez le graphique pour afficher Projets, Programmes ou Portfolios en sélectionnant l’option appropriée dans le menu déroulant **Affichage**.
1. (Facultatif) Placez la souris sur un point spécifique du rapport pour afficher les données correspondant à ce point dans le temps.

   ![Pointage sur un point de données](assets/utilization-chart-hover.png)

1. (Facultatif) Ajustez les filtres pour modifier les informations affichées dans le graphique. Pour plus d’informations sur l’ajustement des filtres, voir [Filtrer des informations d’utilisation](#filter-utilization-information) dans cet article.
1. (Facultatif) Configurez la période du rapport graphique, comme décrit dans la section [Ajuster la période pour laquelle les informations sont affichées](#adjust-the-date-range-for-which-information-is-displayed) dans cet article.
