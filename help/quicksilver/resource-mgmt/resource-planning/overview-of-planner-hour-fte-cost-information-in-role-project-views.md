---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Vue d’ensemble des heures, des équivalents temps complet et des informations sur les coûts dans les vues Projet et Rôle du planificateur de ressources
description: Vue d’ensemble des heures, des équivalents temps complet et des informations sur les coûts dans les vues Projet et Rôle du planificateur de ressources
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2977'
ht-degree: 100%

---

# Vue d’ensemble des heures, des équivalents temps complet et des informations sur les coûts dans les vues Projet et Rôle du planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

La principale fonction du planificateur de ressources est de budgétiser vos ressources en fonction du travail qu’elles doivent accomplir dans le cadre d’un projet. Vous pouvez visualiser le temps disponible de vos ressources et allouer leur temps aux projets auxquels elles sont affectées.

Pour plus d’informations sur la budgétisation des ressources dans le planificateur de ressources, voir [Budgétiser les ressources dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

Cet article décrit certains des concepts clés que vous devez connaître avant de commencer à budgétiser vos ressources dans le planificateur de ressources.

## Vue d’ensemble de la budgétisation des ressources

Tenez compte des éléments suivants lors de la budgétisation des ressources à l’aide du planificateur de ressources :

* Vous pouvez budgétiser l’allocation de vos ressources en spécifiant un nombre d’heures, d’équivalents temps complet ou de coûts que vos ressources peuvent utiliser pour travailler sur des projets. Lorsque vous budgétisez le temps ou le coût d’une ressource, les heures disponibles, les équivalents temps complet ou le coût de la ressource diminuent du montant budgétisé. Par conséquent, les heures disponibles, les équivalents temps complet ou les montants des coûts pour les projets qui suivent le projet pour lequel vous établissez un budget diminuent pour ces personnes et ces rôles sur ces projets.

  >[!IMPORTANT]
  >
  >Vous pouvez budgétiser vos ressources pour une période de 15 ans. Si vous budgétisez des ressources pour un projet d’une durée supérieure à 15 ans, les informations budgétaires risquent de ne pas être exactes.

* Vous pouvez budgétiser les heures, les équivalents temps complet ou les coûts de vos ressources pour n’importe quelle période affichée dans le planificateur de ressources, indépendamment de la chronologie du projet. Par exemple, si vous souhaitez indiquer que vos ressources peuvent ne pas être disponibles pendant la durée du projet (où elles sont associées à un nombre d’heures prévues), mais qu’elles peuvent être disponibles à un autre moment, vous pouvez le faire en les budgétisant pour des périodes où le nombre d’heures prévues est zéro, si c’est à ce moment-là qu’elles deviennent disponibles pour le travail. Vous pouvez ensuite modifier manuellement la chronologie du projet pour qu’il corresponde à la disponibilité des ressources.

  >[!NOTE]
  >
  >Nous vous recommandons de commencer par budgétiser manuellement les heures, les équivalents temps complet ou les coûts pour les fonctions ou les personnes. Vous pouvez utiliser les options automatiques pour budgétiser le temps de vos projets et de vos ressources uniquement lorsque vous savez que le nombre d’heures prévues, d’équivalents temps complet ou de coûts prévus doit toujours correspondre au nombre d’heures, d’équivalents temps complet ou de coûts budgétisés.\
  >Pour plus d’informations sur l’utilisation des options automatiques de budgétisation dans le planificateur de ressources, voir la section « Budgétiser automatiquement les projets et les rôles » dans l&#39;article [Examiner la disponibilité et l’allocation des ressources à l’aide du planificateur de ressources Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* La budgétisation des équivalents temps complet ou des coûts est identique à la budgétisation des heures, mais Adobe Workfront utilise les valeurs des équivalents temps complet et des coûts au lieu des heures pour les ressources que vous budgétisez.

  Pour plus d’informations sur la manière dont les coûts sont calculés dans le planificateur de ressources, voir [Calculer les coûts dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* La budgétisation des allocations de vos ressources dans le planificateur de ressources s’effectue de la manière suivante :

   * Manuellement

     Ou

   * Automatiquement, en utilisant les options de projet et de rôle dans les vues **Vue par projet** et **Vue par rôle**.

  Pour plus d’informations, voir [Budgétiser des ressources dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* Lorsqu’une personne change de fonction, est supprimée, désactivée ou retirée d’un groupe de ressources, les heures budgétées pour le rôle ne changent pas et sont redistribuées aux personnes restantes dans le rôle. Si personne n’est plus associé à la fonction, les heures budgétées pour le rôle deviennent nulles.

Pour plus d’informations sur les options de projet et de rôle, voir la section [Comprendre les valeurs des heures, des équivalents temps complet et des coûts dans le planificateur de ressources](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) dans cet article.

## Comprendre les valeurs des heures, des équivalents temps complet et des coûts dans le planificateur de ressources {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Avant de budgétiser vos ressources et de mettre à jour les informations relatives aux heures budgétées dans le planificateur de ressources, vous devez vous familiariser avec les concepts suivants :

* **Nombre d’heures prévues, équivalents temps complet ou coût** : le travail qui doit être effectué, tel que défini dans les tâches et les problèmes.
* **Heures disponibles, équivalents temps complet ou coût** : le temps pendant lequel les personnes ou les fonctions sont disponibles pour travailler, selon les horaires associés aux personnes.

Ces informations s’affichent dans le planificateur de ressources pour chaque ressource (personne ou rôle) et pour chaque projet.

Pour plus d’informations sur ce qui s’affiche dans les vues Projet et Rôle du projet, voir l’article [Vue d’ensemble de la navigation dans le planificateur de ressources](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Pour comprendre comment les coûts sont calculés dans le planificateur de ressources, voir l’article [Calculer les coûts dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>La budgétisation par coût est identique à la budgétisation par heures ou équivalents temps complet, mais vous devez comprendre comment Workfront calcule le coût pour le planificateur de ressources.
>
>Pour plus d’informations sur le calcul des coûts dans le planificateur de ressources, voir l’article [Calculer les coûts dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

Les tableaux suivants présentent les informations d’allocation et de disponibilité qui s’affichent dans le planificateur de ressources lors de l’application de la vue Projet ou Rôle. Vous pouvez consulter ces informations par heures, par équivalents temps complet ou par coût :

* [La colonne AVL (disponible)](#the-avl-available-column)
* [La colonne PLN (prévu)](#the-pln-planned-column)
* [La colonne BDG (budgétisée)](#the-bdg-budgeted-column)
* [La colonne VAR (Variance)](#the-var-variance-column)
* [La colonne NET](#the-net-column)

### La colonne AVL (disponible) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché par</strong> </td> 
   <td><strong>Description</strong> </td> 
  </tr> 
  <tr> 
   <td>Projet </td> 
   <td> <p>Le total des heures, des équivalents temps complet ou des coûts pour lesquels toutes les personnes du projet sont disponibles pour travailler selon leur planning, pour la période sélectionnée. </p> </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Le total des heures, des équivalents temps complet ou des coûts pour lesquels toutes les personnes associées à ce rôle sont disponibles pour travailler en fonction de leur planning et de leur <strong>Pourcentage de disponibilité des équivalents temps complet</strong> pour ce rôle spécifique, pour la période sélectionnée. </p> <p>Tenez compte des points suivants : </p> 
    <ul> 
     <li>Si personne n’est associé à une fonction, la valeur des heures disponibles pour la fonction est égale à zéro. </li> 
     <li>Si une personne est associée à une fonction principale, mais que le pourcentage de disponibilité des équivalents temps complet<strong></strong> pour le rôle est de 0 %, la valeur des heures disponibles de la fonction est égale à zéro.</li> 
     <li>Si la personne est associée à d’autres rôles et que le <strong>pourcentage de disponibilité des équivalents temps complet</strong> pour les rôles est de 0 %, les autres rôles ne sont pas répertoriés dans le planificateur de ressources et la personne ne s’affiche que sous son rôle principal.</li> 
    </ul> <p>Pour plus d’informations sur le <strong>Pourcentage de disponibilité des équivalents temps complet</strong> pour une fonction, voir l’article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modifier le profil d’utilisation</a>.</p> <p>Pour plus d’informations sur la manière dont la disponibilité de la fonction est calculée dans le planificateur de ressources, voir la section « Calculer les heures disponibles et les équivalents temps complet pour une fonction dans le planificateur de ressources » dans l’article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Vue d’ensemble du calcul des heures et des équivalents temps complet pour les personnes et les fonctions dans le planificateur de ressources</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Heures, équivalents temps complet ou coûts pour lesquels la personne est disponible pour travailler, selon son planning, pour la période sélectionnée. Ce nombre soustrait les heures associées aux éléments suivants :</p> 
    <ul> 
     <li>exceptions de planning</li> 
     <li>temps de repos de la personne</li> 
     <li>heures budgétées pour d’autres projets. </li> 
    </ul> <p>Les heures disponibles, les équivalents temps complet ou les coûts d’une personne sont modifiés comme suit : </p> 
    <ul> 
     <li>la manière dont leur planning et leur équivalent temps complet sont calculés en fonction des préférences de gestion des ressources au niveau du système.<br><p>Pour plus d’informations sur le calcul de la disponibilité des personnes et des fonctions, voir l’article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Vue d’ensemble du calcul des heures et des équivalents temps complet pour les personnes et les fonctions dans le planificateur de ressources</a>.</p>
     Pour plus d’informations sur la configuration des préférences de gestion des ressources dans Workfront, voir <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurer les préférences de gestion des ressources.</a></li> 
    </ul> 
    <ul> 
     <li>la <strong>priorité de planification de projet</strong>, si la personne est budgétée pour le travail.<br>Pour plus d’informations sur la manière dont la priorité de planification de projet affecte les heures disponibles d’une personne, voir <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Vue d’ensemble de la navigation dans le planificateur de ressources</a>. </li> 
    </ul> <p>Si la désactivation de la personne est programmée, les heures disponibles, les équivalents temps complet ou les coûts pour les jours suivant la date de désactivation sont nuls. <br>Pour plus d’informations sur la désactivation des personnes, voir l’article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactiver ou réactiver une personne</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### La colonne PLN (prévu) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché par</strong> </td> 
   <td><strong>Description</strong> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td> <p>Le total du nombre d’heures prévues, des équivalents temps complet ou des coûts de toutes les fonctions ou personnes répertoriées dans le cadre du projet, y compris dans les sections <strong>Aucun rôle</strong> ou <strong>Aucun utilisateur ou aucune utilisatrice</strong>, pour la période sélectionnée, et tel qu’il est affiché dans l’onglet Détails du projet. </p> <p><b>NOTE</b>

Les ajustements manuels des allocations quotidiennes des personnes peuvent modifier la valeur du nombre d’heures prévues hebdomadaires, mensuelles ou trimestrielles dans le planificateur de ressources. Vous pouvez ajuster manuellement les allocations quotidiennes des personnes pour les tâches et les problèmes à l’aide de l’équilibreur de charge de travail. Pour plus d’informations, voir <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gérer les allocations des personnes dans l’équilibreur de charge de travail</a>.</p> </td>
</tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Le total du nombre d’heures prévues de toutes les tâches affectées au rôle, pendant la période sélectionnée. </p> <p>La section <strong>Aucun rôle</strong> affichera le nombre d’heures prévues associé aux tâches qui sont soit non affectées, soit affectées à des équipes (dont les heures sont répertoriées dans la section <strong>Aucun utilisateur ou aucune utilisatrice</strong>), soit affectées à des personnes qui ne sont pas associées à une fonction. </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Le nombre d’heures prévues de toutes les tâches affectées à la personne dans un rôle spécifique, pendant la période sélectionnée. </p> <p>La section <strong>Aucun utilisateur ou utilisatrice</strong> affichera le nombre d’heures prévues associé aux tâches qui sont soit non affectées, soit affectées à des équipes. </p> </td> 
  </tr> 
 </tbody> 
</table>

Tenez compte des points suivants lors de l’affichage du nombre d’heures prévues :

* Bien que vous ne puissiez pas voir les informations sur les affectations de tâches dans le planificateur de ressources dans les vues Projet et Rôle, le nombre d’heures prévues provient du nombre d’heures prévues sur les tâches dans les projets.
* Les heures prévues sont réparties de manière égale entre chaque jour de la durée des tâches, pour chaque ressource qui y est affectée. La durée de la tâche est basée sur les dates de début et de fin prévues de la tâche et comprend tous les jours calendaires de cette période.\
  Workfront prend en compte le planning de l’utilisateur ou de l’utilisatrice ou du projet lors de la répartition du nombre d’heures prévues entre les utilisateurs et les utilisatrices ou les projets. Dans ce cas, les heures prévues sont réparties de manière égale entre chaque jour de la durée des tâches, à l’exclusion des week-ends, des jours de congé et des exceptions au planning.\
  Si, par exemple, vous affichez le planificateur de ressources par semaine et que vous avez des tâches qui durent plusieurs semaines pour des projets, le nombre d’heures prévues par semaine dépend du nombre de jours de cette semaine qui fait partie de la durée de la tâche. Cela fonctionne de la même manière lors de l’affichage du planificateur de ressources par mois ou par trimestre et lorsque les tâches durent plusieurs mois ou trimestres.\
  Les jours du week-end, les exceptions d’horaire et les jours de congé sont exclus de cette répartition.
* Les catégories de tâches suivantes sont incluses dans le calcul du nombre d’heures prévues pour chaque ressource :

   * les tâches affectées aux personnes dans les groupes de ressources, les fonctions ou les équipes du projet\
     Si des tâches sont affectées à des équipes, leur affectation apparaîtra dans les sections **Aucun rôle** et **Aucun utilisateur ou aucune utilisatrice**. Vous pouvez voir le nombre d’heures prévues associé aux équipes, mais vous ne pouvez pas budgéter les heures, car aucun rôle ni aucunpersonne n’a de tâches affectées.

   * Tâches non affectées

* Le nombre d’heures prévues dans le planificateur de ressources n’inclut pas le nombre d’heures prévues associé aux éléments suivants :

   * Tâches parent
   * Tâches affectées à des utilisateurs et des utilisatrices sans groupes de ressources
   * Problèmes, lorsque le paramètre **Inclure les heures des problèmes** est désactivé.

* Le nombre d’heures prévues ne s’affiche pas dans le planificateur de ressources si la durée de la tâche est nulle.
* Le nombre d’heures prévues associé aux utilisateurs et utilisatrices désactivés ne s’affiche pas.

### Colonne BDG (budgété) {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché par</strong> </td> 
   <td><strong>Description</strong> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td> <p>Entrée manuelle pour estimer le nombre d’heures, l’équivalent temps complet ou les coûts que vous budgétez pour un projet, pour une période sélectionnée. </p> <p>Dans la vue « Projet », les heures que vous budgétez pour le projet sont réparties entre les fonctions répertoriées sous le projet. Le nombre d’heures prévues pour chaque rôle détermine la manière dont les heures budgétées sont réparties entre les rôles. Les rôles ayant le nombre d’heures prévues le plus élevé se voient affecter les heures budgétées. </p> <p>Dans la vue « Rôle », les heures que vous budgétez pour le projet ne sont pas réparties entre les fonctions ou les utilisateurs et les utilisatrices du projet. </p> </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Entrée manuelle pour estimer le nombre d’heures que vous budgétez pour un rôle, pour une période sélectionnée. </p> <p>Si aucune fonction n’est affectée à un utilisateur ou à une utilisatrice, vous ne pouvez pas estimer les heures budgétées pour la fonction. </p> <p>Dans la vue « Rôle », les heures que vous budgétez pour le rôle sont distribuées aux projets répertoriés sous le rôle. Le nombre d’heures prévues pour chaque projet détermine la manière dont les heures budgétées sont réparties entre les projets. Les heures budgétées sont réparties entre les projets dont les valeurs d’heures prévues sont les plus élevées.</p> <p>Dans la vue « Projet », les heures que vous budgétez pour le rôle ne sont pas distribuées aux projets ou aux utilisateurs et utilisatrices à qui le rôle a été affecté. </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Entrée manuelle pour estimer le nombre d’heures que vous budgétez pour un utilisateur ou une utilisatrice, pour une période de temps sélectionnée. </p> <p> <p><b>NOTE</b> : vous pouvez estimer les heures budgétées pour les utilisateurs et les utilisatrices à qui aucune tâche n’est affectée, mais pour qui un groupe de ressources est affecté à un projet, car ces utilisateurs et utilisatrices apparaissent également dans le planificateur de ressources. Le nombre d’heures prévues doit toutefois être égal à zéro si les heures ne sont pas affectées à des tâches. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Tenez compte des éléments suivants lorsque vous utilisez des heures budgétées :

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* Pour budgéter des ressources, vous devez disposer d’un accès en modification à la gestion des ressources et aux données financières, ainsi que d’autorisations de gestion des finances pour les projets.

  Pour plus d’informations sur l’accès nécessaire à la budgétisation des ressources, consultez l’article [Accès nécessaire à la budgétisation des ressources dans Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Par défaut, les heures budgétées dans le planificateur de ressources sont égales à zéro pour toutes les ressources et tous les projets.
* Vous pouvez estimer manuellement les heures budgétées pour les utilisateurs, les utilisatrices et les rôles, ou vous pouvez utiliser l’un des liens dans les menus **Plus** de « Projet » ou « Fonction » pour les mettre à jour selon le nombre d’heures prévues.\
  Pour plus d’informations sur les options de projet et de rôle, consultez dans cet article la section [Vue d’ensemble des informations sur les heures, l’équivalent temps complet et les coûts dans les vues « Projet » et « Rôle » du planificateur de ressources](#Budget).

* La plus petite période pour laquelle vous pouvez budgéter des heures, des coûts ou l’équivalent temps complet est une semaine. Vous ne pouvez pas budgéter des heures, des coûts ou l’équivalent temps complet pour une journée.
* Les heures budgétées sont réparties de manière égale entre chaque jour de la durée des tâches, pour chaque ressource qui y est affectée. La durée de la tâche est basée sur les dates de début et de fin prévues de la tâche et comprend tous les jours calendaires de cette période.\
  Lorsque les heures budgétées leur sont affectées, Workfront prend en compte le planning de l’utilisateur, de l’utilisatrice ou du projet. Dans ce cas, les heures budgétées sont réparties de manière égale entre chaque jour de la durée des tâches, en excluant les week-ends, mais en tenant compte des congés et des exceptions dans le planning.\
  Si vous affichez le planificateur de ressources par semaine, par exemple, et que vous avez des tâches s’étendant sur plusieurs semaines, le nombre d’heures budgétées par semaine dépend du nombre de jours de cette semaine qui correspondent à la durée de la tâche. Les jours de week-end sont exclus de cette répartition. Cela fonctionne de la même manière lors de l’affichage du planificateur de ressources par mois ou par trimestre et lorsque les tâches durent plusieurs mois ou trimestres.

* Vous pouvez établir un rapport sur les heures budgétées en sélectionnant « Heure budgétée » comme objet de rapport pour un nouveau rapport.\
  Pour plus d’informations sur les objets sur lesquels vous pouvez créer des rapports dans Workfront, consultez la section « Rapport sur les objets » dans l’article [Comprendre les objets dans Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
  Pour plus d’informations sur la création d’un rapport sur les heures budgétées, consultez l’article [Rapport : heures budgétées](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* Les heures précédemment budgétées pour les utilisateurs et les utilisatrices dont la désactivation a eu lieu par la suite ne s’affichent pas.

### Colonne VAR (variance) {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché par</strong> </td> 
   <td><strong>Description</strong> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td> <p>La variance d’heures, d’équivalent temps complet ou de coûts indique si vous disposez de suffisamment d’heures budgétées pour le projet afin d’accomplir toutes les heures prévues pour sa réalisation. </p> <p>La variance d’heures, d’équivalent temps complet ou de coûts du projet est calculée à l’aide de la formule suivante :</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>La variance d’heures, d’équivalent temps complet ou de coûts indique si vous disposez de suffisamment d’heures, d’équivalent temps complet ou de coûts budgétés pour que le rôle accomplisse le nombre d’heures prévues qui lui a été affecté. </p> <p>La variance d’heures, d’équivalent temps complet ou de coûts est calculée à l’aide de la formule suivante :</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>La variance d’heures, d’équivalent temps complet ou de coûts indique si vous disposez de suffisamment d’heures budgétées pour que l’utilisateur ou l’utilisatrice puisse accomplir le nombre d’heures prévues qui lui a été affecté. </p> <p>La variance d’heures, d’équivalent temps complet ou de coûts pour les utilisateurs et les utilisatrices est calculée à l’aide de la formule suivante :</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Lorsque la variance d’heures, d’équivalent temps complet ou de coûts s’affiche en rouge, cela signifie que vous avez estimé moins d’heures budgétées que d’heures prévues pour le travail effectif à effectuer. Dans ce cas, les heures budgétées peuvent ne pas être suffisantes pour achever le travail.

### La colonne NET  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Affiché par</strong> </td> 
   <td><strong>Description</strong> </td> 
  </tr> 
  <tr> 
   <td>Projet</td> 
   <td> 
    <div> 
     <p>Les heures, l’équivalent temps complet ou les coûts nets du projet peuvent présenter l’une des caractéristiques suivantes : </p> 
     <ul> 
      <li> <p>Différence entre le temps ou le coût disponible et le temps ou le coût budgété pour le projet :</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>La différence entre le temps ou le coût disponible et le temps ou le coût prévu pour le projet, lorsque le paramètre « Utiliser les valeurs planifiées (PLN) dans les calculs NET » est activé : </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>CONSEIL</b></p>        
  <p>Cette option n’est appliquée que lorsque vous personnalisez l’affichage dans la section « Afficher les éléments sélectionnés ».</p>
  <p>Pour plus d’informations, consultez la section <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Examiner la disponibilité et l’affectation des ressources à l’aide du planificateur de ressources Adobe Workfront.</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> 
    <div> 
     <p>Les rôles « Heures NET », « Équivalent temps complet » ou « Coût » peuvent présenter l’une des caractéristiques suivantes : </p> 
     <ul> 
      <li> <p>La différence entre le temps ou le coût disponible et le temps ou le coût budgété pour le rôle :</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>Différence entre le temps ou le coût disponible et le temps ou le coût prévu pour le rôle, lorsque le paramètre « Utiliser les valeurs planifiées (PLN) dans les calculs NET » est activé :</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>CONSEIL</b> <span>

Cette option n’est appliquée que lorsque vous personnalisez l’affichage dans la section « Afficher les éléments sélectionnés ».</span> </p> <p><span>Pour plus d’informations, consultez la section </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Examiner la disponibilité et l’affectation des ressources à l’aide du planificateur de ressources Adobe Workfront.</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> 
    <div> 
     <p>Les heures NET, l’équivalent temps complet ou le coût de l’utilisateur ou de l’utilisatrice peuvent afficher l’un des éléments suivants : </p> 
     <ul> 
      <li> <p>La différence entre le temps ou le coût disponible et le temps ou le coût budgété pour l’utilisateur ou l’utilisatrice :</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>La différence entre le temps ou le coût disponible et le temps ou le coût prévu pour l’utilisateur ou l’utilisatrice, lorsque le paramètre « Utiliser les valeurs planifiées (PLN) dans les calculs NET » est activé :</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>CONSEIL</b> <span>

Cette option n’est appliquée que lorsque vous personnalisez l’affichage dans la section « Afficher les éléments sélectionnés ».</span> </p> <p><span>Pour plus d’informations, consultez la section </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Examiner la disponibilité et l’affectation des ressources à l’aide du planificateur de ressources Adobe Workfront.</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Lorsque les heures NET, l’équivalent temps complet ou les coûts s’affichent en rouge, cela signifie qu’il n’y a pas assez de temps disponible ou de budget pour couvrir le temps budgété** ou le temps prévu ou les coûts associés au travail. Dans ce cas, les ressources font l’objet d’une affectation trop importante.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the table below is ideal but it does not transfer to Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours, FTE, or Cost)</strong> </td>
<td><strong>Displayed by</strong> </td>
<td><strong>Description</strong> </td>
</tr>
<tr>
<td rowspan="3">AVL <br>(Available Hours, FTE, or Cost)</td>
<td>Project </td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users on the project are available to work according to their schedule, for the time frame selected. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users associated with this role are available to work according to their schedule and their <strong>Percentage of FTE Availability</strong> for that specific role, for the time frame selected. </p> <p>Consider the following: </p>
<ul>
<li>If no user is associated with a job role, then the value for the Available Hours for the job role is zero. </li>
<li>If a user is associated with a Primary Job Role, but the <strong>Percentage of FTE Availability</strong> for the role is 0%, the job role Available Hours value is zero.</li>
<li>If the user is associated with Other Roles and the <strong>Percentage of FTE Availability</strong> for the roles is 0%, the Other Roles are not listed in the Resource Planner and the user displays only under their Primary Role.</li>
</ul> <p>For more information about the <strong>Percentage of FTE Availability</strong> for a job role, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p>For more information about how the job role availability is calculated in the Resource Planner, see the section "Calculate the Available Hours and FTE for a job role in the Resource Planner" in the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>Hours, FTEs, or Cost that the user is available to work, according to their schedule, for the time frame selected. This number subtracts the hours associated with the following:</p>
<ul>
<li>schedule exceptions</li>
<li>time off of the user</li>
<li>hours budgeted for other projects. </li>
</ul> <p>The Available Hours, FTEs, or Cost for a user change according the following: </p>
<ul>
<li>how their schedule and FTE are calculated based on the Resource Management Preferences at the system level.<br>For more information about calculating user and job role availability, see the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</li>
</ul>
<ul>
<li>the <strong>Project Planning Priority</strong>, if the user is budgeted for work.<br>For more information about how Project Planning Priority affects the Available Hours of a user, see <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>. </li>
</ul> <p>If the user is scheduled for deactivation, the Available Hours, FTEs, or Cost for the days after the deactivation date are zero. <br>For more information about deactivating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td>
</tr>
<tr>
<td rowspan="4">PLN <br>(Planned Hours, FTE, or Cost)</td>
<td>Project</td>
<td> <p>The total of the Planned Hours, FTEs, or Cost from all the job roles or users listed under the project, including in the <strong>No Role</strong> or <strong>No User</strong> sections, for the time frame selected, and as displayed in the Project Details tab of the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of the Planned Hours from all the tasks assigned to the role, during the time frame selected. </p> <p>The <strong>No Role</strong> section will show the Planned Hours associated with tasks that are either unassigned, assigned to teams (whose hours are listed in the <strong>No User</strong> section), or assigned to users who are not associated with a job role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Planned Hours from all the tasks assigned to the user in a specific role, during the time frame selected. </p> <p>The <strong>No User</strong> section will show the Planned Hours associated with tasks that are either unassigned or assigned to teams. </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<ul>
<li>Although you cannot see information about task allocations in the Resource Planner in the Project and Role views, the amount of Planned Hours comes from the Planned Hours on the tasks in the projects. </li>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks excluding weekends, time-off days, and schedule exceptions.<br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> The following categories of tasks are included in calculating the Planned Hours for each resource:
<ul>
<li> tasks assigned to users in Resource Pools, job roles, or teams on the project<br>If tasks are assigned to teams, their allocation will appear under <strong>No Role</strong> and <strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </li>
<li> unassigned tasks </li>
</ul></li>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>tasks assigned to users with no Resource Pools</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> </td>
</tr>
<tr>
<td rowspan="4"> BDG <br>(BudgetedHours, FTE, or Cost) </td>
<td>Project</td>
<td> <p>A manual entry to estimate how many hours, FTE, or Cost you budget for a project, for a selected time frame. </p> <p>In the Project view, the hours you budget for the project are distributed to the job roles listed under the project. The amount of Planned Hours for each role determines how the Budgeted Hours are distributed to the roles. The Budgeted Hours are distributed to the roles with higher Planned Hours values. </p> <p>In the Role view, the hours you budget for the project are not distributed to the roles or the users on the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>A manual entry to estimate how many hours you budget for a role, for a selected time frame. </p> <p>If no user is associated with the job role, you cannot estimate the Budgeted Hours for the job role. </p> <p>In the Role view, the hours you budget for the role are distributed to the projects listed under the role. The amount of Planned Hours for each project determines how the Budgeted Hours are distributed to the projects. The Budgeted Hours are distributed to the projects with higher Planned Hours values.</p> <p>In the Project view, the hours you budget for the role are not distributed to the projects or the users associated with the role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>A manual entry to estimate how many hours you budget for a user, for a selected time frame. </p> <p> <note type="note">  You can estimate the Budgeted Hours for users who are not assigned to tasks, but are associated with a Resource Pool on a project because these users also appear in the Resource Planner. Their Planned Hours should be zero, however, if they are not assigned to tasks.
</note> </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when working with Budgeted Hours:</p> <li>
<ul>
<li> <p>You can budget resources only when you have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects.</p> <p>For information about the access needed for budgeting resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this bullet: Duplicated below)</p>
</li>
</ul> </li>
<ul>
<li>By default, the Budgeted Hours in the Resource Planner are zero for all resources and for all the projects.</li>
<li>You can manually estimate the Budgeted Hours for users and roles, or you can use one of the links in the Project or Job Role <strong>More</strong> menus to update them according to the number of Planned Hours.<br>For more information about project and role options, see the section <a href="#Budget" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a> in this article.</li>
<li> The smallest period of time you can budget hours, FTE, or Cost for is a week. You cannot budget hours, FTE, or Cost for a day. </li>
<li> Budgeted Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time. <br>Workfront takes into account the schedule of the user or of the project when distributing Budgeted Hours to users or projects. In this case, Budgeted Hours are equally distributed to each day within the Duration of tasks excluding weekends, but including time-off and schedule exceptions. <br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks, the number of Budgeted Hours per week depends on how many days within that week are part of the task Duration. Weekend days are excluded from this distribution. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters. </li>
<li>You can report on Budgeted Hours, by selecting Budgeted Hour as your report object for a new report.<br>For information about what objects you can report on in Workfront, see the section "Report on objects" in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. <br>For information about building a Budgeted Hour report, see the article <a href="../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</li>
<li>Hours previously budgeted for users who were later deactivated do not display. <br></li>
</ul> </td>
</tr>
<tr>
<td rowspan="4">VAR <br>(Hour, FTE, or ,Cost Variance)</td>
<td>Project</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the project to accomplish all the Planned Hours for the project. </p> <p>The Project Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours, FTE, or Cost for the role to accomplish the Planned Hours assigned to it. </p> <p>The Role Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Hours, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the user to accomplish the Planned Hours assigned to them. </p> <p>The User Hours, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
When the Hours, FTE, or Cost Variance displays in red, you have estimated less Budgeted Hours than the Planned Hours of the actual work that needs to be completed. In this case, the Budgeted Hours might not be enough to complete the work.
</note> </td>
</tr>
<tr>
<td rowspan="4"> NET <br>(Net Hours, FTEs, or Cost) </td>
<td>Project</td>
<td>
<div>
<p>The project Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the project, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>Role</td>
<td>
<div>
<p>The role Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the role:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the role, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span class="preview"><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>User</td>
<td>
<div>
<p>The user Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the user:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the user, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
<span>When the NET Hours,&nbsp;FTE, or Cost display in red, there is not enough Available time or budget to cover either the Budgeted</span> or the Planned time or cost associated with the work. In this case, the resources are overallocated.
</note> </td>
</tr>
</tbody>
</table>
-->
