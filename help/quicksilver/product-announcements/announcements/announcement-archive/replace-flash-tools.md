---
title: Remplacement des outils Flash dans Adobe Workfront
description: Remplacement des outils Flash dans Adobe Workfront
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: c80d9b0b7eb2a638af9e0a11ca3038ed99ecf1ee
workflow-type: tm+mt
source-wordcount: '2701'
ht-degree: 100%

---

# Remplacement des outils Flash dans Adobe Workfront

Nous avons supprimé tous les outils Flash d’Adobe Workfront Classic.

De nouveaux outils basés sur les normes actuelles sont désormais disponibles dans Workfront. Ces changements s’inscrivent dans la fin de la prise en charge des produits Flash, comme annoncé par Adobe.

## Dates importantes

Les dates suivantes sont à retenir pour le processus de suppression de tous les outils Flash dans Workfront :

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **19 novembre 2020** : supression des outils Flash de tous les produits Workfront.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## Outils Flash hérités

Les outils répertoriés dans les sections suivantes ont été supprimés du système Workfront et remplacés par de nouvelles solutions.

Pour plus d’informations sur les outils de remplacement, consultez la section [Outils Flashs hérités et leurs héritiers](#legacy-flash-based-tools-and-their-replacements) dans cet article.

### Gestion des ressources

* L’onglet Ancienne planification de ressources de la zone Personnes et tous les outils de l’onglet, qui comprend les éléments suivants :

   * Gestionnaire du budget des ressources
   * Planificateur de capacités
   * Estimations de ressources
   * Grille des ressources\
     Pour plus d’informations, consultez la section [Planifier des ressources : index des articles](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* Zone Anciennes estimations de ressources du business Case d’un projet

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  is displayed in view-only mode
  </MadCap:conditionalText>
  -->

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  For more information, see
  <a href="../../../resource-mgmt/resource-mgmt-overview/migrate-resource-estimates-to-budgeting.md" class="MCXref xref">Migrate from Legacy Resource Estimates to Resource Budgeting </a>
  </MadCap:conditionalText>
  -->

  .

* Sous-onglet Grille des ressources de l’onglet Personnel d’un projet
* L’option Utiliser la zone Nouvel horaire du sous-onglet Planification de l’onglet Personnel d’un projet supprime l’ancienne zone de planification ou Team Builder. Dans ce cas, la chronologie de planification s’affiche désormais par défaut.
* Onglet Affectation sous le profil utilisateur

### Rapports

Les rapports et fonctionnalités de création de rapports suivants ont été supprimés :

* Suppression des fonctionnalités de création de rapports :

   * Option Grille des ressources d’un rapport utilisateur
   * Option Ancien graphique Gantt dans un rapport de projet ou de tâche\
     Pour plus d’informations, consultez la section [Afficher les informations dans le graphique de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* Rapports supprimés :

   * Rapport Ancien groupe de ressources
   * Rapport Estimations de ressources

  >[!NOTE]
  >
  >Tous les anciens champs accessibles par le biais des rapports ou de l’API (ancien groupe de ressources, ancien coût budgété, ancien coût, anciennes heures budgétées, ancien coût budgété de la main-d’oeuvre, etc.) s’affichent dans divers rapports, mais ne contiennent pas de nouvelles informations.

### Ancien graphique Gantt

* Toutes les vues Ancien graphique de Gantt des listes de projets et de tâches, ainsi que les rapports et options de création de rapports
* Sous-onglets Ancien graphique Gantt dans les portfolios et programmes
* Sous-onglet Ancien graphique Gantt dans une liste de tâches de modèle d’un modèle, vue Ancien graphique Gantt de l’onglet Sous-tâches d’une tâche de modèle et dans un rapport Tâche de modèle

### Relecture

L’ancienne visionneuse de relecture a été remplacée par la nouvelle visionneuse de relecture web et de bureau pour la plupart des clientes et clients. Elle a été supprimée pour l’ensemble des personnes en novembre 2020.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

Pour plus d’informations, consultez les ressources suivantes :

* [Réviser les épreuves dans la visionneuse de relecture web](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [Réviser les épreuves dans la visionneuse de relecture de bureau](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/lpv-removed-2018.md" class="MCXref xref">Legacy proofing viewer removed in 2018.3</a> </li>
  -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Additional features to be removed</h3>
<ul>
<li>The Legacy Portfolio Optimizer<br>For more information, see <a href="../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md" class="MCXref xref">Portfolio Optimizer overview</a>.<br></li>
<li>The Legacy financial fields in the Business Case of the project and the Portfolio Optimizer</li>
<li>The dialog boxes used when sharing reports, calendars, and documents no longer rely on Flash-based technology</li>
</ul>
</div>
-->

## Anciens outils Flashs et leurs héritiers {#legacy-flash-based-tools-and-their-replacements}

Sauf indication contraire, toutes les anciennes fonctionnalités ont été remplacées par de nouvelles, comme illustré dans le tableau suivant.

>[!CAUTION]
>
>Les anciens outils Flashs ont été supprimés de tous les environnements.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Anciens outils</strong> </p> </th> 
   <th> <p><strong>Nouveaux outils</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Anciens groupes de ressources</strong> </p> <p>Les anciens groupes de ressources étaient des groupes ou des collections de fonctions nécessaires simultanément pour l’achèvement d’un projet. Les anciens groupes de ressources présentaient un certain nombre d’inconvénients :</p> 
    <ul> 
     <li> Vous pouviez associer un profil utilisateur à un ancien groupe de ressources, mais il n’était utilisé qu’à des fins de création de rapports. Étant donné que les anciens groupes de ressources fonctionnaient avec des entités de fonctions abstraites, aucune des exceptions de planning et aucun des congés des utilisateurs et utilisatrices n’était pris en compte, ce qui renvoyait des données inexactes sur la disponibilité des ressources. </li> 
    </ul> 
    <ul> 
     <li>Vous ne pouviez spécifier qu’un seul ancien groupe de ressources par projet ; plusieurs anciens groupes de ressources ne prenaient ainsi en charge que le flux de groupes distincts fonctionnant indépendamment les uns des autres et ne partageant jamais de ressources. Dans tous les autres cas, il était recommandé de conserver un ancien groupe de ressources qui incluait toutes les ressources du système, ce qui entraînait des problèmes de performances lorsque le nombre de projets et de données était important.</li> 
    </ul> </td> 
   <td> <p><strong>Groupe de ressources</strong> </p> <p>Les nouveaux groupes de ressources constituent une collection d’utilisateurs et d’utilisatrices qui sont nécessaires simultanément pour l’achèvement du projet. Workfront réalise également qu’il existe des cas où des utilisateurs et utilisatrices spécialisés doivent se voir affecter du travail séparément. Pour cette raison, vous pouvez désormais budgéter des utilisateurs et utilisatrices au lieu des fonctions. </p> Les avantages du groupe de ressources par rapport aux anciens groupes de ressources incluent les éléments suivants : 
    <ul>
     <li>Comme les groupes de ressources sont basés sur les utilisateurs et utilisatrices, leurs congés et exceptions de planning sont déjà pris en compte pour les calculs de disponibilité des utilisateurs et utilisatrices et des rôles. Cela se traduit par des données précises et à jour, ce qui permet de prendre des décisions budgétaires correctes et de minimiser la probabilité de changements lorsque le projet est en cours d’exécution.</li>
     <li>Comme il existe désormais un meilleur contrôle sur la disponibilité des ressources et la précision des données, Workfront vous permet d’associer plusieurs groupes de ressources à un projet. Une personne peut également appartenir à plusieurs groupes de ressources si elle dispose de plusieurs compétences pouvant être utilisées simultanément dans plusieurs projets. </li>
    </ul><p>Avec un tel contrôle sur les données, il n’est plus nécessaire d’avoir un seul groupe de ressources qui inclut toutes les ressources pour la répartition du budget disponible. En fait, nous ne le recommandons pas. Nous vous recommandons plutôt de diversifier vos groupes de ressources et de n’associer que les groupes de ressources appropriés aux projets.</p><p> Pour plus d’informations sur les groupes de ressources, voir <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">Vue d’ensemble des groupes de ressources</a>.</p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gestionnaire du budget des ressources</strong> </p> <p>Vous pouvez utiliser le gestionnaire du budget des ressources pour spécifier la disponibilité des ressources de fonction pour plusieurs groupes de ressources. Cependant, en raison des inconvénients de l’ancien groupe de ressources, cette fonctionnalité était rarement utilisée. Lorsqu’elle était utilisée, elle obligeait les utilisateurs et les utilisatrices à saisir manuellement la disponibilité des fonctions pour obtenir une budgétisation plus précise. Les exceptions de planning et les congés des utilisateurs et des utilisatrices n’étaient pas pris en compte.</p> </td> 
   <td> <p>Grâce au calcul automatique de la disponibilité basé sur les utilisateurs et les utilisatrices des groupes de ressources, le gestionnaire du budget des ressources n’est plus nécessaire. L’outil a été supprimé, ainsi que tout le travail manuel de calcul de la disponibilité.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimations de ressources</strong> </p> <p>L’objectif de l’onglet Estimations de ressources sous chaque ancien groupe de ressources était le même que celui du gestionnaire du budget des ressources, dans le cadre d’un ancien groupe de ressources seulement. Cet outil présentait les mêmes limites que le gestionnaire du budget des ressources et les anciens groupes de ressources : données inexactes et saisie manuelle de la disponibilité. </p> </td> 
   <td> <p>Grâce au calcul automatique de la disponibilité de l’utilisateur ou de l’utilisatrice, les estimations de ressources sont devenues obsolètes et ont été supprimées.</p> <p>L’outil est supprimé dans les anciens groupes de ressources et dans les anciennes estimations de ressources dans le business case d’un projet. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Planificateur de capacités</strong> </p> <p>Le planificateur de capacités était un outil Workfront de budgétisation des ressources et de hiérarchisation des projets dans un ancien groupe de ressources en fonction de la disponibilité des ressources. En raison du caractère incomplet des données provenant des estimations de ressources et du gestionnaire du budget des ressources qui fournissaient les informations au planificateur de capacités, la hiérarchisation des projets devait être vérifiée deux fois par rapport à la disponibilité des utilisateurs et des utilisatrices.</p> <p>Le scénario le plus courant consistait à n’utiliser qu’un seul ancien groupe de ressources qui incluait toutes les fonctions du système, ce qui entraînait des problèmes de performances lorsque le planificateur de capacités tentait de charger un grand nombre de projets.</p> </td> 
   <td> <p><strong>Vue Projet du planificateur de ressources</strong> </p> <p>Dans la vue Projet du planificateur de ressources, vous pouvez budgétiser les ressources et hiérarchiser les projets comme que vous le faisiez dans l’ancien planificateur de capacités. Contrairement à l’ancien outil, davantage de données sont désormais prises en charge, les informations disponibles étant plus précises en prenant en compte à la fois les congés des utilisateurs et des utilisatrices et les exceptions de planning.</p> <p>Les informations disponibles, prévues et budgétées sont visibles d’un seul coup d’œil, de sorte que les personnes gestionnaires de ressources puissent voir à la fois s’il y a suffisamment de personnes pour faire le travail et si les plans de projet dépassent les estimations de budget initiales.</p> <p> Pour plus d’informations sur l’utilisation de la vue Projet dans le planificateur de ressources, voir <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Vue d’ensemble du planificateur de ressources</a>.</p> <p><strong>Planificateur de scénarios</strong> </p> <p>Pour la planification des capacités à long terme, la modélisation de scénarios d’hypothèses et la hiérarchisation des priorités, nous avons également introduit le planificateur de scénarios Workfront. </p> <p>Le planificateur de scénarios n’est disponible que dans la nouvelle expérience Adobe Workfront et nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénarios Workfront, voir <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Vue d’ensemble du planificateur de scénarios</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Anciennes estimations de ressources (Business case)</strong> </p> <p>Vous pouviez utiliser la zone Anciennes estimations de ressources du business case pour budgéter un certain nombre d’heures et de coûts de main-d’œuvre dans le cadre de la planification de projet et de la demande de ressources. Cette vue n’offrait aucune visibilité sur la disponibilité des ressources, ce qui entraînait des demandes de ressources approximatives et augmentait le risque de rejet de travail du projet.</p> </td> 
   <td> <p><strong>Établissement du budget de ressources (Business case)</strong> </p> <p>La section Établissement du budget de ressources sous le business case intègre des fonctionnalités du planificateur de ressources dans le business case, offrant ainsi une visibilité sur la disponibilité des utilisateurs et utilisatrices et des rôles, et permettant également de budgéter au niveau de l’utilisateur ou de l’utilisatrice. </p> <p> Pour plus d’informations sur la zone Établissement du budget de ressources du business case, voir <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Vue d’ensemble des zones du business case</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Rapports d’estimation de ressources</strong> </p> <p>Lorsque vous utilisez les outils hérités pour la gestion des ressources, vous pouviez créer des rapports sur les heures budgétées et le nombre d’heures prévues à partir du business case. Cela vous permettait de créer des rapports de matrice affichant le total des tâches budgétées et prévues pour chaque fonction au cours d’une période spécifique. Ce rapport n’était pas modifiable et vous ne pouviez pas apporter de modifications au budget de vos ressources en fonction des résultats du rapport. </p> </td> 
   <td> <p><strong>Rapport d’utilisation</strong> </p> <p>Le rapport d’utilisation intégré affiche côte à côte les heures, coûts et revenus prévus, budgétés et réels. </p> <p>Pour plus d’informations sur l’utilisation du rapport d’utilisation, voir <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Afficher des informations sur l’utilisation des ressources</a>. </p> 
    <div> 
     <p><strong>Heures budgétées sur lesquelles créer un rapport</strong> </p> 
     <p>Créez un rapport des heures budgétées afin de passer en revue les heures budgétées dans le planificateur de ressources d’un formulaire de rapport. </p> 
     <p>Pour plus d’informations sur les heures budgétées, voir <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossaire de la terminologie Adobe Workfront</a>.</p> 
     <p>Pour plus d’informations sur la création d’un rapport, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Créer un rapport personnalisé</a>.</p> 
    </div> <p><strong>Vue Rôle du planificateur de ressources</strong> </p> <p>Les heures budgétées et le nombre d’heures prévues du business case dans les outils de gestion des ressources hérités sont désormais disponibles dans une nouvelle vue native : la vue basée sur le rôle du planificateur de ressources. Cette vue fournit des informations sur les heures disponibles, prévues et budgétées en un coup d’œil et vous permet de contrôler et de modifier le budget au même endroit. Elle permet de prendre de meilleures décisions lors de la planification des fonctions de haut niveau. </p> <p> Pour plus d’informations sur la planification des ressources dans la vue Rôle du planificateur de ressources, voir la section <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">Utiliser les vues de projet et de rôle pour les ressources de budget</a> dans la <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Vue d’ensemble du planificateur de ressources</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Grille des ressources</strong> </p> <p>La grille des ressources vous donnait une visibilité sur l’affectation de certaines personnes à mesure qu’un projet touchait à sa fin. </p> <p>Par exemple, vous pouviez facilement voir qui dans votre équipe de projet avait terminé son travail plus tôt, qui était en retard, ou encore qui connaissait une surcharge ou faisait l’objet d’une sous-affectation pendant une période donnée. </p> <p>Malheureusement, vous ne pouviez pas agir sur ces informations dans la même vue. Pour corriger les problèmes de sur-affectation, vous deviez accéder aux projets et y ajuster manuellement les informations sans aucune visibilité sur le résultat de vos actions.</p> </td> 
   <td> <p>C’est pourquoi la grille des ressources a été remplacée par deux nouveaux outils. Vous pouvez utiliser les outils suivants, selon la phase de planification des ressources dans laquelle vous vous trouvez :</p> 
    <ul> 
     <li> <p><strong>Pour la phase d’analyse :</strong> </p> 
      <ul> 
       <li> <p><strong>Équilibreur de charge de travail</strong> : utilisez l’équilibreur de charge de travail pour afficher la charge de travail des personnes à un niveau plus granulaire. Lorsque vous utilisez l’équilibreur de charge de travail, vous pouvez voir quelles personnes sont disponibles selon leur charge de travail pour terminer la tâche à temps. Cela inclut les détails des congés et des exceptions de planning. </p> <p>Pour plus d’informations sur l’équilibreur de charge de travail, voir <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Vue d’ensemble de l’équilibreur de charge de travail</a>.</p> </li> 
       <li> <p><strong>Vue d’utilisation du planificateur de ressources</strong><strong> :</strong> pour afficher à un niveau supérieur les projets auxquels les personnes sont affectées, utilisez la vue d’utilisation du planificateur de ressources. Cela vous permet de voir sur quoi travaillent les personnes, ainsi que leurs sur-affectations et sous-affectations pour une période spécifique. Le planificateur de ressources fournit également une visualisation de l’affectation globale des personnes dans son ensemble, ainsi qu’une visibilité sur les heures effectives consignées, ce qui permet d’analyser la progression du travail effectué. </p> <p>Pour plus d’informations sur l’utilisation de la vue d’utilisation dans le planificateur de ressources, voir la section <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">Utiliser la vue d’utilisation pour afficher les heures disponibles, prévues, effectives ou en équivalent temps complet</a> dans la <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Vue d’ensemble du planificateur de ressources</a>.</p> </li> 
      </ul> </li> 
     <li><strong>Pour la phase tactique :</strong> 
      <ul> 
       <li><strong>Équilibreur de charge de travail</strong> : vous pouvez effectuer les opérations suivantes à l’aide de l’équilibreur de charge de travail : 
        <ul>
         <li>Affecter du travail aux personnes.</li>
         <li>Gérer les affectations des personnes aux éléments de travail. </li>
         <li>Partager l’équilibreur de charge de travail avec d’autres personnes qui peuvent ne pas avoir de visibilité sur la zone Personnes. Utiliser la fonctionnalité de lien partageable pour partager un lien vers l’équilibreur de charge de travail et l’incorporer dans des tableaux de bord personnalisés. Toutes les personnes ayant accès à la vue des personnes peuvent afficher ces tableaux de bord lorsque vous les partagez.</li>
        </ul><p>L’équilibreur de charge de travail est disponible dans la zone Personnes. </p><p>Pour plus d’informations sur l’équilibreur de charge de travail, voir <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Vue d’ensemble de l’équilibreur de charge de travail</a>.</p></li> 
      </ul> <!--
       <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <li><strong>The Resource Scheduling Areas</strong><strong>:</strong> When assigning your resources to the actual work that must be completed, use the Resource Scheduling areas in the People or Team areas, or at the project level. These areas allow you to visualize and manage the users' workload by day and rectify any problems from one view using the following actions: 
         <ul>
          <li> manual dragging and dropping of tasks to the correct assignee </li>
          <li> automatic assigning of tasks </li>
          <li> bulk swapping assignments </li>
          <li><p>adjusting Planned Hours according to the true availability of users. </p></li>
         </ul><p>These actions provide even more control over managing workload. </p><p> For information about managing user assignments and allocations in the Resource Scheduling areas, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p><p>With this new functionality, the Resource Grid is replaced by the User View of the Resource Planner and the Resource Scheduling areas in the following areas of the application: </p>
         <ul>
          <li>People - the Resource Grid is eliminated along with the Legacy Resource Planning tab.</li>
          <li>Project - the Scheduling area under the Staffing tab of the project is available to Work and Plan license users. They do not have to have Manage access to the project to view this area. </li>
          <li>Reporting - the ability to view User reports in the Resource Grid view is removed. Instead, there is an option to share a URL for the User View of the Resource Planner and embed it in custom dashboards, providing visibility into user utilization to virtually anyone in the system. Any users with access to View users are able to view these dashboards when you share them. </li>
          <li>User - the Allocation tab is eliminated as the same information can be accessed in the User View of the Resource Planner.</li>
         </ul></li> 
       </ul>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Graphique de Gantt hérité, Liste des tâches</strong> </p> <p> Le graphique de Gantt hérité sur la liste des tâches permet aux personnes de voir la chronologie du projet et d’effectuer une planification du scénario d’exécution sans avoir à modifier la base de données. Le graphique de Gantt hérité était basé sur la technologie Flash, qui présentait des risques pour la sécurité. </p> </td> 
   <td> <p><strong>Graphique de Gantt,</strong> <strong>Liste des tâches</strong></p> <p> Le nouveau graphique de Gantt basé sur HTML a le même objectif que le graphique de Gantt hérité. Vous pouvez visualiser la chronologie du projet et réaliser une planification du scénario d’exécution sans valider les modifications apportées à la base de données en sélectionnant l’option Enregistrer manuellement dans la barre d’outils de la liste des tâches. </p> <p>Le nouveau graphique de Gantt est interactif quand vous utilisez l’option d’enregistrement automatique de vos modifications au fur et à mesure. </p> <p>Le nouveau graphique de Gantt de la liste des tâches est fiable, car il repose sur les technologies les plus récentes. Il se trouve directement dans la liste des tâches et est facilement accessible lorsque vous travaillez dessus, puisque vous n’avez pas à changer d’onglet ni de vue. </p> <p>Bien que le nouveau graphique Gantt offre les mêmes fonctionnalités que l’ancien graphique, certaines différences existent toutefois. </p> <p> Le sous-onglet Ancien graphique Gantt d’une liste de tâches de modèle sur un modèle, la vue de l’ancien graphique Gantt de l’onglet Sous-tâches d’une tâche de modèle et l’ancien graphique Gantt d’un rapport Tâche de modèle ont également été remplacés par le graphique de Gantt HTML. </p> <p>Si vous utilisez l’ancien graphique Gantt principalement pour l’affichage simple et les modifications rapides, mais que vous n’utilisez pas le graphique réel, la nouvelle option Planification permet d’apporter rapidement des modifications aux champs de planification clés. Vous pouvez sélectionner Planification chronologique au lieu de l’enregistrement automatiquement dans la barre d’outils de la liste des tâches.</p> <p>Pour plus d’informations sur l’enregistrement d’une liste de tâches à l’aide de l’option Planification chronologique, consultez la section « Enregistrer manuellement les modifications dans une liste de tâches lors de la sélection de l’option Planification chronologique » de l’article <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Modifier les tâches dans une liste</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ancien graphique Gantt pour une liste de projets</strong> </p> <p>L’ancien graphique Gantt sur la liste des projets vous permet d’afficher vos projets et tâches sur un seul écran. Sans quitter le contexte de la liste des projets, vous pouvez afficher les détails des tâches d’un projet, ainsi que les dépendances entre les projets. L’ancien graphique Gantt sur la liste des projets était basé sur la technologie Flash, qui présentait des risques pour la sécurité. </p> </td> 
   <td> <p><strong>Graphique de Gantt, liste de projets</strong> </p> <p>Le graphique de Gantt HTML a le même objectif que l’ancien graphique Gantt. Vous pouvez afficher vos projets et tâches dans une vue unique afin d’identifier visuellement les dépendances entre les projets et les tâches. Le graphique de Gantt de la liste de projets se trouve directement dans la liste des projets. Le nouveau graphique de Gantt présente une interface moderne et repose sur la technologie la plus récente.</p> <p>Pour plus d’informations sur le graphique de Gantt de la liste des projets, consultez la section <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Afficher des informations dans le graphique de Gantt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Partager des boîtes de dialogue pour les rapports, les calendriers et les documents</strong> </p> <p>Lors du partage de rapports, de calendriers et de documents, les boîtes de dialogue utilisées tiraient parti de la technologie Flash.</p> </td> 
   <td> <p>L’expérience de partage de rapports, de calendriers et de documents dans Workfront n’a pas changé. Cependant, celle-ci ne repose plus sur Flash.</p> <p>Pour plus d’informations sur le partage de ces éléments, consultez la section <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Vue d’ensemble des autorisations de partage sur les objets</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Ancienne visionneuse de relecture</strong> </p> <p>L’ancienne visionneuse de relecture était une interface web qui fournissait des fonctionnalités de relecture pour les épreuves statiques, vidéo et interactives.</p> </td> 
   <td> <p><strong>Visionneuse de relecture web et de bureau</strong> </p> <p>La visionneuse de relecture web fournit des fonctionnalités de relecture pour les épreuves statiques et vidéo.</p> <p>La visionneuse de relecture de bureau fournit des fonctionnalités de relecture pour les épreuves interactives, en plus de fournir une prise en charge complète des épreuves statiques et vidéo.</p> <p>Le format de fichier SWF a été abandonné par les principaux fournisseurs et a été remplacé par des bannières HTML5 pour la relecture. </p> <p>Pour plus d’informations sur les différences entre les visionneuses de relecture disponibles, consultez la section <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Vue d’ensemble des différences entre les visionneuses de relecture web et de bureau</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
