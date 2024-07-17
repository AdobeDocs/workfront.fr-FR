---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Vue d’ensemble des informations sur les heures, ETP et les coûts dans les vues Projet et Rôle du planificateur de ressources
description: Vue d’ensemble des informations sur les heures, ETP et les coûts dans les vues Projet et Rôle du planificateur de ressources
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2977'
ht-degree: 2%

---

# Vue d’ensemble des heures, de l’éditeur de texte enrichi et des coûts dans les vues Projet et Rôle du planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

Le budget de vos ressources pour le travail qu’elles doivent accomplir sur un projet est la fonction principale du planificateur de ressources. Vous pouvez afficher le temps disponible de vos ressources et allouer leur temps aux projets auxquels elles sont affectées.

Pour plus d’informations sur la planification des ressources dans le planificateur de ressources, voir [Ressources budgétaires dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

Cet article décrit quelques-uns des concepts clés que vous devez connaître avant de commencer à budgéter vos ressources dans le planificateur de ressources.

## Présentation des ressources de budget

Tenez compte des points suivants lors de la planification des ressources à l’aide du planificateur de ressources :

* Vous pouvez budgétiser l’allocation de vos ressources en spécifiant un montant d’heures, d’éditeur de texte enrichi ou de coûts que vos ressources peuvent utiliser pour terminer le travail sur les projets. Lorsque vous budgétez le temps ou le coût d’une ressource, les heures disponibles, l’éditeur de texte enrichi ou le coût de la ressource diminuent selon le montant budgété. Par conséquent, le montant des heures, de l’éditeur de texte enrichi ou des coûts disponibles pour les projets qui suivent le projet pour lequel vous avez établi un budget diminue pour ces utilisateurs et rôles sur ces projets.

  >[!IMPORTANT]
  >
  >Vous pouvez répartir vos ressources sur une période de 15 ans. Si vous planifiez des ressources pour un projet d’une durée supérieure à 15 ans, les informations de budget peuvent ne pas être exactes.

* Vous pouvez budgéttiser les heures, l’éditeur de texte enrichi ou le coût de vos ressources pour toute période affichée dans le planificateur de ressources, indépendamment de la chronologie du projet. Par exemple, si vous souhaitez indiquer que vos ressources ne seront peut-être pas disponibles dans la chronologie du projet (où elles sont associées aux Heures planifiées), mais qu’elles pourront être disponibles à une autre période, vous pouvez le faire en les budgétisant pour les périodes où les Heures planifiées sont nulles, si c’est le moment où elles deviennent disponibles pour le travail. Vous pouvez modifier manuellement la chronologie du projet pour qu’elle corresponde à la disponibilité de la ressource après cette opération.

  >[!NOTE]
  >
  >Nous vous recommandons de budgétiser manuellement vos heures, votre EPT ou le coût des rôles de tâche ou d’abord celui des utilisateurs. Vous ne pouvez utiliser les options automatiques pour budgéter le temps de vos projets et ressources que lorsque vous êtes certain que le montant des heures planifiées, de l’éditeur de texte enrichi ou du coût doit toujours correspondre à vos heures, à votre ETR ou à votre coût budgété.\
  >Pour plus d’informations sur l’utilisation des options automatiques pour la budgétisation dans le planificateur de ressources, consultez la section &quot;Budget project and ôles automatiquement&quot; de l’article [Révision de la disponibilité et de l’affectation des ressources à l’aide du planificateur de ressources Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* Le budget de l’éditeur de texte enrichi ou des coûts est identique à celui des heures de budget, où Adobe Workfront utilise l’éditeur de texte enrichi et les valeurs des coûts au lieu des heures pour les ressources que vous budgétez.

  Pour plus d’informations sur la façon dont les coûts sont calculés dans le planificateur de ressources, voir [Calculer les coûts dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* L’affectation du budget pour vos ressources dans le planificateur de ressources se fait de la manière suivante :

   * Manuellement

     Ou

   * Automatiquement, en utilisant les options de projet et de rôle dans les vues **Afficher par projet** et **Afficher par rôle**.

  Pour plus d’informations, voir [Ressources de budget dans le planificateur de ressources à l’aide des vues Projet et Rôle](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* Lorsqu’un utilisateur modifie des rôles de tâche, est supprimé, désactivé ou supprimé d’un pool de ressources, les heures budgétisées pour le rôle ne changent pas et elles sont redistribuées aux utilisateurs restants dans le rôle . Si aucun utilisateur n’est plus associé au rôle de tâche, le nombre d’heures budgétisées pour le rôle devient zéro.

Pour plus d’informations sur les options de projet et de rôle, consultez la section [Comprendre les valeurs Hours, FTE et Cost dans le planificateur de ressources](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) de cet article.

## Comprendre les valeurs des heures, de l’ETR et du coût dans le planificateur de ressources {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Avant de budgéter vos ressources et de mettre à jour les informations sur les heures budgétisées dans le planificateur de ressources, vous devez connaître les concepts suivants :

* **Heures planifiées, ETR ou Coût** : le travail qui doit être effectué selon la définition des tâches et des problèmes.
* **Heures disponibles, ETR ou Coût** : durée pendant laquelle les utilisateurs ou les rôles de tâche sont disponibles pour travailler, selon les plannings associés aux utilisateurs.

Ces informations s’affichent dans le planificateur de ressources pour chaque ressource (utilisateur ou rôle) et pour chaque projet.

Pour plus d’informations sur ce qui s’affiche dans les vues Projet et Rôle du projet, reportez-vous à l’article [Présentation de la navigation du planificateur de ressource](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Pour plus d’informations sur la façon dont les coûts sont calculés dans le planificateur de ressources, consultez l’article [Calculer les coûts dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>Le budget par coût est identique au budget par heure ou ETR, mais vous devez comprendre comment Workfront calcule le coût pour le planificateur de ressources.
>
>Pour plus d’informations sur le mode de calcul des coûts dans le planificateur de ressources, consultez l’article [Calculer les coûts dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

Les tableaux suivants affichent les informations d’allocation et de disponibilité qui s’affichent dans le planificateur de ressources lors de l’application de la vue Projet ou Rôle. Vous pouvez afficher ces informations par heures, heure d’été ou coût :

* [Colonne AVL (disponible)](#the-avl-available-column)
* [Colonne PLN (planifiée)](#the-pln-planned-column)
* [Colonne BDG (budgétée)](#the-bdg-budgeted-column)
* [Colonne VAR (variation)](#the-var-variance-column)
* [La colonne NET](#the-net-column)

### La colonne AVL (Disponible) {#the-avl-available-column}

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
   <td> <p>Le total des heures, des EPT ou des coûts pour lesquels tous les utilisateurs du projet sont disponibles pour travailler selon leur planning, pour la période sélectionnée. </p> </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Le total des heures, des EFS ou des coûts pour lesquels tous les utilisateurs associés à ce rôle sont disponibles pour travailler selon leur planning et leur <strong>Pourcentage de disponibilité de l’éditeur de texte enrichi</strong> pour ce rôle spécifique, pour la période sélectionnée. </p> <p>Tenez compte des points suivants : </p> 
    <ul> 
     <li>Si aucun utilisateur n’est associé à un rôle de tâche, la valeur de la fonction Heures disponibles pour le rôle de tâche est zéro. </li> 
     <li>Si un utilisateur est associé à un rôle de tâche par Principal, mais que le <strong>pourcentage de disponibilité de l’éditeur de texte enrichi</strong> pour le rôle est de 0 %, la valeur du rôle de tâche Heures disponibles est zéro.</li> 
     <li>Si l’utilisateur est associé aux autres rôles et que le <strong>pourcentage de disponibilité de l’éditeur de texte enrichi</strong> pour les rôles est de 0 %, les autres rôles ne sont pas répertoriés dans le planificateur de ressources et l’utilisateur s’affiche uniquement sous son rôle de Principal.</li> 
    </ul> <p>Pour plus d’informations sur le <strong>pourcentage de disponibilité de l’éditeur de texte enrichi</strong> pour un rôle de tâche, consultez l’article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Modification du profil d’un utilisateur</a>.</p> <p>Pour plus d’informations sur le mode de calcul de la disponibilité des rôles de tâche dans le planificateur de ressources, voir la section "Calcul des heures disponibles et de l’éditeur de texte enrichi pour un rôle de tâche dans le planificateur de ressources" de l’article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Présentation du calcul des heures et de l’éditeur de texte enrichi pour les utilisateurs et les rôles dans le planificateur de ressources</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Heures, EPT ou coût que l’utilisateur peut utiliser selon son planning pour la période sélectionnée. Ce nombre soustrait les heures associées aux éléments suivants :</p> 
    <ul> 
     <li>exceptions de planification</li> 
     <li>délai d’expiration de l’utilisateur</li> 
     <li>heures budgétisées pour d’autres projets. </li> 
    </ul> <p>La modification des heures disponibles, de l’éditeur de texte enrichi ou du coût pour un utilisateur s’effectue comme suit : </p> 
    <ul> 
     <li>la façon dont leur planification et leur ETR sont calculés en fonction des préférences de gestion des ressources au niveau du système.<br><p>Pour plus d’informations sur le calcul de la disponibilité des utilisateurs et des rôles de travail, consultez l’article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Présentation du calcul des heures et de l’ETR pour les utilisateurs et les rôles dans le planificateur de ressources </a>.</p>
     Pour plus d’informations sur la configuration des préférences de gestion des ressources dans Workfront, voir <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configuration des préférences de gestion des ressources</a></li> 
    </ul> 
    <ul> 
     <li>la <strong>priorité de planification de projet</strong>, si l’utilisateur a un budget de travail.<br>Pour plus d’informations sur la façon dont la priorité de planification des projets affecte les heures disponibles d’un utilisateur, consultez la <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref"> présentation de la navigation du planificateur de ressources </a>. </li> 
    </ul> <p>Si l’utilisateur est programmé pour la désactivation, les heures disponibles, l’éditeur de texte enrichi ou le coût des jours suivant la date de désactivation sont de zéro. <br>Pour plus d’informations sur la désactivation des utilisateurs, consultez l’article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Désactivation ou réactivation d’un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Colonne PLN (planifiée) {#the-pln-planned-column}

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
   <td> <p>Le total des heures planifiées, des EPT ou des coûts de tous les rôles de tâche ou utilisateurs répertoriés sous le projet, y compris dans les sections <strong>Aucun rôle</strong> ou <strong>Aucun utilisateur</strong>, pour la période sélectionnée, et comme affiché dans l’onglet Détails du projet du projet. </p> <p><b>NOTE</b>

Des ajustements manuels des allocations quotidiennes des utilisateurs pourraient modifier la valeur Heures planifiées hebdomadaires, mensuelles ou trimestrielles dans le planificateur de ressources. Vous pouvez ajuster manuellement les affectations quotidiennes des utilisateurs pour les tâches et les problèmes à l’aide de l’équilibreur de charge de travail. Pour plus d’informations, voir <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gérer les affectations des utilisateurs et utilisatrices dans l’équilibreur de charge de travail</a>.</p> </td>
</tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Total des heures planifiées de toutes les tâches affectées au rôle, pendant la période sélectionnée. </p> <p>La section <strong>Aucun rôle</strong> affichera les heures planifiées associées aux tâches non affectées, affectées à des équipes (dont les heures sont répertoriées dans la section <strong>Aucun utilisateur</strong>) ou affectées à des utilisateurs qui ne sont pas associés à un rôle de tâche. </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Heures planifiées de toutes les tâches affectées à l’utilisateur dans un rôle spécifique, pendant la période sélectionnée. </p> <p>La section <strong>Aucun utilisateur</strong> affichera les heures planifiées associées aux tâches non affectées ou affectées à des équipes. </p> </td> 
  </tr> 
 </tbody> 
</table>

Tenez compte des points suivants lors de l’affichage des heures planifiées :

* Bien que vous ne puissiez pas voir les informations sur l’affectation des tâches dans le planificateur de ressources dans les vues Projet et Rôle , le montant des heures planifiées provient des heures planifiées sur les tâches des projets.
* Les Heures planifiées sont répartie de manière égale sur chaque jour au cours de la Durée des tâches, pour chaque ressource qui leur est affectée. La durée de la tâche est basée sur les dates de début et de fin planifiées de la tâche et inclut chaque jour calendaire de cette période.\
  Workfront prend en compte le planning de l’utilisateur ou du projet lors de la distribution des heures planifiées aux utilisateurs ou aux projets. Dans ce cas, les heures planifiées sont réparties de manière égale sur chaque jour au cours de la durée des tâches, à l’exception des week-ends, jours de congé et des exceptions de planification.\
  Si, par exemple, vous affichez le planificateur de ressources par semaine et que vous avez des tâches qui s’étendent sur plusieurs semaines sur des projets, le nombre d’heures planifiées par semaine dépend du nombre de jours de cette semaine qui font partie de la durée de la tâche. Cela fonctionne de la même manière lors de l’affichage du planificateur de ressources par mois ou par trimestre et lorsque les tâches s’étendent sur plusieurs mois ou trimestres.\
  Les jours du week-end, les exceptions de planification et les jours de congé sont exclus de cette distribution.
* Les catégories de tâches suivantes sont incluses dans le calcul des Heures planifiées pour chaque ressource :

   * tâches affectées aux utilisateurs dans les groupes de ressources, les rôles de tâche ou les équipes du projet\
     Si des tâches sont affectées à des équipes, leur attribution apparaît sous les sections **Aucun rôle** et **Aucun utilisateur** . Vous pouvez voir les Heures planifiées associées aux équipes, mais vous ne pouvez pas budgéter les heures, car aucun rôle ni utilisateur n’est associé aux tâches.

   * tâches non affectées

* Les heures planifiées dans le planificateur de ressources n’incluent pas les heures planifiées associées aux éléments suivants :

   * tâches parentes
   * tâches affectées à des utilisateurs sans pool de ressources
   * problèmes, lorsque le paramètre **Inclure les heures à partir des problèmes** est désactivé.

* Les heures planifiées ne s’affichent pas dans le planificateur de ressources si la durée de la tâche est zéro.
* Les heures planifiées associées aux utilisateurs désactivés ne s’affichent pas.

### La colonne BDG (Budget) {#the-bdg-budgeted-column}

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
   <td> <p>Entrée manuelle permettant d’estimer le nombre d’heures, d’EPT ou de coûts du budget pour un projet, pour une période sélectionnée. </p> <p>Dans la vue Projet, les heures que vous allouez au projet sont réparties dans les rôles de tâche répertoriés sous le projet. Le nombre d’heures planifiées pour chaque rôle détermine la manière dont les heures budgétisées sont distribuées aux rôles. Les heures budgétisées sont réparties dans les rôles avec des valeurs d’heures planifiées plus élevées. </p> <p>Dans la vue Rôle, les heures que vous allouez au projet ne sont pas distribuées aux rôles ou aux utilisateurs du projet. </p> </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>Entrée manuelle permettant d’estimer le nombre d’heures que vous consacrez au budget d’un rôle, pour une période sélectionnée. </p> <p>Si aucun utilisateur n’est associé au rôle de tâche, vous ne pouvez pas estimer les heures budgétisées pour le rôle de tâche. </p> <p>Dans la vue Rôle, les heures que vous allouez au rôle sont réparties dans les projets répertoriés sous le rôle . Le montant des heures planifiées de chaque projet détermine la manière dont les heures budgétées sont réparties dans les projets. Les heures budgétisées sont réparties dans les projets avec des valeurs d’heures planifiées plus élevées.</p> <p>Dans la vue Projet, les heures que vous allouez au rôle ne sont pas distribuées aux projets ni aux utilisateurs associés au rôle. </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>Entrée manuelle permettant d’estimer le nombre d’heures que vous consacrez au budget d’un utilisateur, pour une période sélectionnée. </p> <p> <p><b>REMARQUE</b>   Vous pouvez estimer les heures budgétées pour les utilisateurs qui ne sont pas affectés à des tâches, mais qui sont associés à un pool de ressources sur un projet, car ces utilisateurs apparaissent également dans le planificateur de ressources. Toutefois, leurs heures planifiées doivent être nulles si elles ne sont pas affectées à des tâches. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Tenez compte des points suivants lorsque vous utilisez des heures budgétées :

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* Vous ne pouvez budgéter les ressources que si vous disposez des autorisations Modifier de gestion des ressources et des données financières et Gérer les finances sur les projets.

  Pour plus d’informations sur l’accès aux ressources de budget, consultez l’article [Accès aux ressources de budget dans Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Par défaut, les Heures budgétisées du planificateur de ressources sont nulles pour toutes les ressources et pour tous les projets.
* Vous pouvez estimer manuellement les heures budgétées pour les utilisateurs et les rôles, ou vous pouvez utiliser l’un des liens des menus Projet ou Rôle de tâche **Plus** pour les mettre à jour en fonction du nombre d’heures planifiées.\
  Pour plus d’informations sur les options de projet et de rôle, reportez-vous à la section [Présentation des heures, de l’éditeur de texte enrichi et des informations de coût dans les vues Projet et Rôle du planificateur de ressources](#Budget) de cet article.

* La plus petite période pendant laquelle vous pouvez budgéter les heures, l’éditeur de texte enrichi ou le coût est une semaine. Vous ne pouvez pas budgéter les heures, l’éditeur de texte enrichi ou le coût d’une journée.
* Les Heures budgétisées sont réparties de manière égale sur chaque jour au sein de la Durée des tâches, pour chaque ressource qui leur est affectée. La durée de la tâche est basée sur les dates de début et de fin planifiées de la tâche et inclut chaque jour calendaire de cette période.\
  Workfront prend en compte le planning de l’utilisateur ou du projet lors de la distribution des heures budgétaires aux utilisateurs ou aux projets. Dans ce cas, les Heures budgétées sont réparties de manière égale chaque jour dans la Durée des tâches, à l’exception des week-ends, mais aussi des exceptions de délai et de planification.\
  Si, par exemple, vous affichez le planificateur de ressources par semaine et que vous avez des tâches qui s’étendent sur plusieurs semaines, le nombre d’heures budgétisées par semaine dépend du nombre de jours de cette semaine qui font partie de la durée de la tâche. Les jours du week-end sont exclus de cette distribution. Cela fonctionne de la même manière lors de l’affichage du planificateur de ressources par mois ou par trimestre et lorsque les tâches s’étendent sur plusieurs mois ou trimestres.

* Vous pouvez créer des rapports sur les heures budgétisées en sélectionnant Heure budgétée comme objet de rapport pour un nouveau rapport.\
  Pour plus d’informations sur les objets sur lesquels vous pouvez créer des rapports dans Workfront, reportez-vous à la section &quot;Rapport sur les objets&quot; dans l’article [Comprendre les objets dans Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
  Pour plus d’informations sur la création d’un rapport Heure budgétaire, reportez-vous à l’article [Rapport : Heure budgétaire](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* Les heures précédemment budgétées pour les utilisateurs qui ont été ultérieurement désactivés ne s’affichent pas.

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
   <td> <p>L’écart Heure, EPT ou Coût indique si vous disposez de suffisamment d’heures budgétaires pour que le projet atteigne toutes les heures planifiées pour le projet. </p> <p>L’heure du projet, l’ETP ou l’écart de coût sont calculés à l’aide de la formule suivante :</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> <p>L’écart Heure, ETR ou Coût indique si vous disposez de suffisamment d’heures, d’ETR ou de coûts budgétés pour que le rôle puisse accomplir les heures planifiées qui lui sont affectées. </p> <p>L’heure du rôle, l’ETR ou l’écart de coût sont calculés à l’aide de la formule suivante :</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> <p>L’écart Heures, EPT ou Coût indique si vous disposez de suffisamment d’heures budgétaires pour que l’utilisateur puisse accomplir les heures planifiées qui lui sont affectées. </p> <p>L’écart des heures utilisateur, de l’éditeur de texte enrichi ou de coût est calculé à l’aide de la formule suivante :</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Lorsque l’écart Heures, EPT ou Coût s’affiche en rouge, vous avez estimé moins d’heures budgétisées que les heures planifiées du travail réel qui doit être terminé. Dans ce cas, les Heures budgétisées peuvent ne pas suffire à terminer le travail.

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
     <p>Le projet Heures nettes, ETR ou Coût peut afficher l’une des options suivantes : </p> 
     <ul> 
      <li> <p>La différence entre l'heure ou le coût disponible et l'heure ou le coût budgété du projet :</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>La différence entre l’heure ou le coût disponible et l’heure ou le coût planifié du projet, lorsque le paramètre Utiliser les valeurs planifiées (PLN) dans les calculs NET est activé : </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>CONSEIL</b></p>        
  <p>Cette option est appliquée uniquement lorsque vous personnalisez la vue dans la section Afficher les éléments sélectionnés .</p>
  <p>Pour plus d’informations, voir <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Révision de la disponibilité et de l’affectation des ressources à l’aide du planificateur de ressources Adobe Workfront</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Rôle</td> 
   <td> 
    <div> 
     <p>Le rôle Heures nettes, ETR ou Coût peut afficher l’une des options suivantes : </p> 
     <ul> 
      <li> <p>Différence entre le temps ou le coût disponible et le temps ou le coût budgété du rôle :</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>La différence entre le temps ou le coût disponible et le temps ou le coût planifié pour le rôle, lorsque les valeurs Utiliser planifié (PLN) dans le paramètre de calculs NET sont activées :</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>CONSEIL</b> <span>

Cette option est appliquée uniquement lorsque vous personnalisez la vue dans la section Afficher les éléments sélectionnés.</span> </p> <p><span>Pour plus d’informations, voir </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Révision de la disponibilité et de l’allocation des ressources à l’aide du planificateur de ressources Adobe Workfront</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>l’utilisateur ou de l’utilisatrice</td> 
   <td> 
    <div> 
     <p>L’utilisateur Heures réseau, ETR ou Coût peut afficher l’une des options suivantes : </p> 
     <ul> 
      <li> <p>La différence entre l'heure ou le coût disponible et l'heure ou le coût budgété pour l'utilisateur :</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>La différence entre l'heure ou le coût disponible et l'heure ou le coût planifié de l'utilisateur, lorsque les valeurs Utiliser planifié (PLN) dans le paramètre de calcul NET sont activées :</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>CONSEIL</b> <span>

Cette option est appliquée uniquement lorsque vous personnalisez la vue dans la section Afficher les éléments sélectionnés.</span> </p> <p><span>Pour plus d’informations, voir </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Révision de la disponibilité et de l’allocation des ressources à l’aide du planificateur de ressources Adobe Workfront</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Lorsque les heures NETTES, ETR ou Coût s&#39;affichent en rouge, il n&#39;y a pas assez de temps ou de budget disponible pour couvrir soit le budget**, soit l&#39;heure planifiée ou le coût associé au travail. Dans ce cas, les ressources sont surchargées.

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
