---
title: Remplacement des outils basés sur des Flashs dans Adobe Workfront
description: Remplacement des outils basés sur des Flashs dans Adobe Workfront
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '2705'
ht-degree: 1%

---

# Remplacement des outils basés sur des Flashs dans Adobe Workfront

Nous avons supprimé tous les outils basés sur le Flash d’Adobe Workfront Classic.

Les outils de remplacement basés sur les normes actuelles sont désormais disponibles dans Workfront. Ces modifications s’alignent sur la fin de la prise en charge des produits Flash, comme annoncé par Adobe.

## Dates importantes

Les dates suivantes sont importantes pour le processus de suppression de tous les outils basés sur un Flash dans Workfront :

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **19 novembre 2020**: Tous les outils basés sur des Flashs ont été supprimés de tous les produits Workfront.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## Outils hérités basés sur des Flashs

Les outils répertoriés dans les sections suivantes ont été supprimés du système Workfront et remplacés par de nouvelles solutions.

Pour plus d’informations sur les outils de remplacement, voir [Outils basés sur les Flashs hérités et leurs remplacements](#legacy-flash-based-tools-and-their-replacements) dans cet article.

### Gestion des ressources

* L’onglet Planification des ressources héritées de la zone Personnes et tous les outils de l’onglet, qui comprend les éléments suivants :

   * Gestionnaire du budget des ressources
   * Planificateur de capacités
   * Estimations de ressources
   * Grille des ressources\
      Pour plus d’informations, voir [Planification des ressources dans Adobe Workfront](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* La zone Estimations des ressources héritées de l’analyse de cas d’un projet

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

* Sous-onglet Grille de ressources dans l’onglet Personnel d’un projet
* L’option Utiliser une nouvelle zone de planification dans le sous-onglet Planification de l’onglet Personnel d’un projet supprime l’ancienne zone de planification ou le créateur d’équipes. Dans ce cas, la chronologie de planification s’affiche désormais par défaut.
* Onglet Affectation sous le profil utilisateur

### Rapports

Les fonctions et rapports de création de rapports suivants ont été supprimés :

* Suppression des fonctionnalités de création de rapports :

   * Option Grille de ressources dans un rapport utilisateur
   * Option Gantt héritée dans un rapport de projet ou de tâche\
      Pour plus d’informations, voir [Affichage des informations dans le diagramme de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* Rapports supprimés :

   * Rapport Pool de ressources hérité
   * Rapport des estimations de ressources

   >[!NOTE]
   >
   >Tous les champs hérités accessibles par le biais des rapports ou de l’API (Pool de ressources hérité, Coût budgété hérité, Coût hérité, Heures budgétées héritées, Coût de la main-d’oeuvre budgété hérité, etc.) s’affichent dans divers rapports, mais ne contiennent pas de nouvelles informations.

### Ancien graphique Gantt

* Toutes les vues Gantt héritées des listes de projets et de tâches, ainsi que les options de rapports et de rapports
* Sous-onglets Gantt hérité dans Portfolio et programmes
* Le sous-onglet Gantt hérité dans une liste de tâches de modèle sur un modèle, la vue Gantt héritée dans l’onglet Sous-tâches d’une tâche de modèle et dans un rapport Tâche de modèle

### Relecture

La visionneuse de vérification de l’ancien a été remplacée par la nouvelle visionneuse de vérification de l’intégrité du web et de la bureau pour la plupart des clients. Elle a été supprimée pour tous les clients en novembre 2020.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

Pour plus d’informations, voir les ressources suivantes :

* [Vérifier les bons à tirer dans la visionneuse de tests de Web Proofing](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [Vérification des bons à tirer dans la visionneuse de vérification de l’appli de bureau](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

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

## Outils basés sur les Flashs hérités et leurs remplacements {#legacy-flash-based-tools-and-their-replacements}

Sauf indication contraire, toutes les fonctionnalités héritées ont été remplacées par de nouvelles, comme illustré dans le tableau suivant.

>[!CAUTION]
>
>Les outils hérités basés sur des Flashs ont été supprimés de tous les environnements.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Outils hérités</strong> </p> </th> 
   <th> <p><strong>Nouveaux outils</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Anciens pools de ressources</strong> </p> <p>Les groupes de ressources hérités étaient des groupes ou des collections de rôles de tâche nécessaires en même temps pour la fin d’un projet. Legacy Resource Pools présente un certain nombre de lacunes :</p> 
    <ul> 
     <li> Vous pouviez associer un utilisateur à un pool de ressources hérité, mais il n’était utilisé qu’à des fins de création de rapports. Étant donné que les groupes de ressources hérités fonctionnaient avec des entités de rôle de tâche abstraites, aucune des exceptions de planification et de temps de pause des utilisateurs n’a été prise en compte, ce qui a entraîné des données inexactes sur la disponibilité de la ressource. </li> 
    </ul> 
    <ul> 
     <li>Vous ne pouviez spécifier qu’un seul pool de ressources hérité par projet, ce qui entraînait la prise en charge de plusieurs groupes de ressources hérités ne prenant en charge que le flux de groupes distincts fonctionnant indépendamment les uns des autres et ne partageant jamais de ressources. Dans tous les autres cas, il était recommandé de conserver un pool de ressources hérité qui incluait toutes les ressources du système, ce qui entraînait des problèmes de performances avec un grand nombre de projets et de données.</li> 
    </ul> </td> 
   <td> <p><strong>Pool de ressources</strong> </p> <p>Les nouveaux pools de ressources sont un ensemble d’utilisateurs qui sont nécessaires en même temps pour la fin du projet. Workfront se rend également compte qu’il existe des cas où des utilisateurs spécialisés doivent leur faire consacrer du travail séparément. Pour cette raison, vous pouvez désormais budgéter les utilisateurs au lieu des rôles de tâche. </p> Les avantages du pool de ressources par rapport aux pools de ressources hérités sont les suivants : 
    <ul>
     <li>Comme les pools de ressources sont basés sur les utilisateurs, leurs exceptions de temps d’arrêt et de planification sont déjà prises en compte pour les calculs de disponibilité des utilisateurs et des rôles. Cela se traduit par des données précises et à jour, ce qui permet de prendre des décisions budgétaires correctes et de minimiser la probabilité de changements lorsque le projet est en cours d’exécution.</li>
     <li>Comme il existe désormais un meilleur contrôle sur la disponibilité des ressources et la précision des données, Workfront vous permet d’associer plusieurs groupes de ressources à un projet. Un utilisateur peut également appartenir à plusieurs groupes de ressources s’il dispose de plusieurs compétences pouvant être utilisées simultanément dans plusieurs projets. </li>
    </ul><p>Avec un tel contrôle sur les données, il n’est plus nécessaire d’avoir un seul pool de ressources qui inclut toutes les ressources pour la répartition du budget disponible. En fait, nous ne le recommandons pas. Nous vous recommandons plutôt de diversifier vos groupes de ressources et de n’associer que les groupes de ressources appropriés aux projets.</p><p> Pour plus d’informations sur les pools de ressources, voir <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Présentation des pools de ressources </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gestionnaire du budget des ressources</strong> </p> <p>Vous pouvez utiliser le Gestionnaire du budget des ressources pour spécifier la disponibilité des ressources de rôle de tâche pour plusieurs groupes de ressources. Cependant, en raison des lacunes du pool de ressources hérité, cette fonctionnalité a été rarement utilisée. Lorsqu’elle a été utilisée, elle a forcé les utilisateurs à saisir manuellement la disponibilité des rôles de tâche pour rendre le budget plus précis. Les exceptions de planification et le temps de congé des utilisateurs n’ont pas été pris en compte.</p> </td> 
   <td> <p>Avec le calcul automatique de la disponibilité basé sur les utilisateurs des pools de ressources, le gestionnaire du budget des ressources n’est plus nécessaire. L'outil a été éliminé, ainsi que tous les travaux manuels pour calculer la disponibilité.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimations de ressources</strong> </p> <p>L’onglet Estimations des ressources sous chaque pool de ressources hérité a eu le même objectif que le Gestionnaire du budget des ressources, uniquement dans le contexte d’un pool de ressources hérité. Cet outil présentait les mêmes limites que le Gestionnaire du budget des ressources et les Pools de ressources hérités : données inexactes et saisie manuelle de la disponibilité. </p> </td> 
   <td> <p>Avec le calcul automatique de la disponibilité de l’utilisateur, les estimations de ressources sont devenues obsolètes et ont été supprimées.</p> <p>L’outil est éliminé dans les pools de ressources hérités et dans les estimations de ressources héritées dans l’analyse de cas d’un projet. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Planificateur de capacités</strong> </p> <p>Le gestionnaire de capacités était un outil Workfront permettant de budgéter les ressources et de hiérarchiser les projets dans un pool de ressources hérité, en fonction de la disponibilité des ressources. Étant donné que les données des estimations des ressources et du Gestionnaire du budget des ressources ne sont pas complètes et qu'elles ont fourni les informations pour le responsable du plan de capacité, la hiérarchisation des projets a dû être revu deux fois par rapport à la disponibilité des utilisateurs.</p> <p>L’utilisation d’un seul pool de ressources hérité qui incluait tous les rôles de tâche dans le système était le scénario le plus courant, ce qui entraînait des problèmes de performances lorsque le planificateur de capacité tentait de charger un grand nombre de projets.</p> </td> 
   <td> <p><strong>La vue Projet du planificateur de ressources</strong> </p> <p>Dans la vue basée sur les projets du planificateur de ressources, vous pouvez budgéter les ressources et prioriser les projets de la même manière que vous le faisiez auparavant dans le planificateur de capacité hérité. Contrairement à l’outil hérité, davantage de données sont désormais prises en charge, les informations disponibles étant plus précises en prenant en compte à la fois les heures de service des utilisateurs et les exceptions de planification.</p> <p>Les informations disponibles, prévues et budgétisées sont visibles en un coup d’oeil, de sorte que les gestionnaires de ressources puissent voir à la fois s’il y a suffisamment de personnes pour faire le travail et si les plans de projet dépassent les estimations budgétaires initiales.</p> <p> Pour plus d’informations sur l’utilisation de la vue Projet dans le planificateur de ressources, voir <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Présentation de Resource Planner</a></p> <p><strong>Planification du scénario</strong> </p> <p>Pour la planification des capacités à long terme, la modélisation des scénarios d’hypothèses et la hiérarchisation des priorités, nous avons également introduit le planificateur de scénario Workfront . </p> <p>Le planificateur de scénario n’est disponible que dans la nouvelle expérience Adobe Workfront et nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénario Workfront, voir <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Présentation du planificateur de scénarios</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimations des ressources héritées (analyse de cas)</strong> </p> <p>Vous pouvez utiliser la zone Estimations des ressources héritées de l’Analyse de cas pour budgétiser un certain nombre d’heures et de coûts de travail dans le cadre de la planification du projet et de la demande de ressources. Cette vue n’offrait aucune visibilité sur la disponibilité des ressources, ce qui entraînait des demandes approximatives de ressources et augmentait les chances de travaux de projet rejetés.</p> </td> 
   <td> <p><strong>Budget des ressources (analyse de cas)</strong> </p> <p>La section Budget des ressources sous Analyse de cas offre des fonctionnalités de planification des ressources à l’Analyse de cas, ce qui permet de connaître la disponibilité des utilisateurs et des rôles, ainsi que de planifier au niveau de l’utilisateur. </p> <p> Pour plus d’informations sur la zone Resource Budgeting de l’Analyse de cas, voir <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Présentation des domaines de l’analyse de cas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Rapports d’estimation de ressources</strong> </p> <p>Lorsque vous utilisez les outils hérités pour la gestion des ressources, vous pouvez créer des rapports sur les heures budgétisées et planifiées à partir de l’analyse de cas. Cela vous a permis de créer des rapports de matrice affichant le total des tâches Planifiées et Planifiées pour chaque rôle de tâche au cours d’une période spécifique. Ce rapport n’était pas modifiable et vous n’avez pas pu apporter de modifications au budget de vos ressources en fonction des résultats du rapport. </p> </td> 
   <td> <p><strong>Rapport d’utilisation</strong> </p> <p>Le rapport d’utilisation intégré affiche côte à côte les heures, coûts et recettes planifiées, budgétaires et réelles. </p> <p>Pour plus d’informations sur l’utilisation du rapport Utilisation, voir <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Affichage des informations sur l’utilisation des ressources </a>. </p> 
    <div> 
     <p><strong>Heures budgétisées à rapporter</strong> </p> 
     <p>Créez un rapport pour les heures budgétisées afin de passer en revue les heures budgétisées dans le planificateur de ressources d’un formulaire de rapport. </p> 
     <p>Pour plus d’informations sur les heures budgétées, voir <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossaire de la terminologie Adobe Workfront</a>.</p> 
     <p>Pour plus d’informations sur la création d’un rapport, voir <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Création d’un rapport personnalisé</a>.</p> 
    </div> <p><strong>Vue Rôle du planificateur de ressources</strong> </p> <p>Les heures prévues et planifiées de l’analyse de cas dans les outils de gestion des ressources hérités sont désormais disponibles dans une nouvelle vue native : la vue basée sur le rôle du planificateur de ressources. Cette vue fournit des informations sur les heures disponibles, planifiées et budgétées en un coup d’oeil et vous permet de contrôler et de modifier le budget au même endroit. Cela permet de prendre de meilleures décisions lors de la planification des rôles de haut niveau. </p> <p> Pour plus d’informations sur la planification des ressources dans la vue Rôle du planificateur de ressources, voir la section <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">Utilisation des vues de projet et de rôle pour les ressources de budget </a> dans <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Présentation de Resource Planner</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Grille des ressources</strong> </p> <p>La grille de ressources vous a donné une visibilité sur l’allocation de certains utilisateurs à mesure qu’un projet avance vers la fin. </p> <p>Par exemple, vous pouvez facilement voir quand une personne de votre équipe de projet a fait son travail plus tôt, et quand une personne est tombée en retard, et si elle a été surchargée ou sous-affectée pendant une période donnée. </p> <p>Malheureusement, vous n'avez pas été en mesure d'agir sur l'information dans la même perspective. Pour corriger les problèmes de surallocation, vous avez dû accéder aux projets et y ajuster manuellement les informations sans aucune visibilité sur le résultat de vos actions.</p> </td> 
   <td> <p>La grille de ressources a été remplacée par deux nouveaux outils. Vous pouvez utiliser les outils suivants, selon la phase de planification des ressources dans laquelle vous vous trouvez :</p> 
    <ul> 
     <li> <p><strong>Pour la phase d’analyse :</strong> </p> 
      <ul> 
       <li> <p><strong>L’équilibreur de charge de travail</strong>: Utilisez l’équilibreur de charge de travail pour afficher la charge de travail des utilisateurs à un niveau plus granulaire. Lorsque vous utilisez l’équilibreur de charge de travail, vous pouvez voir quels utilisateurs sont disponibles dans leur charge de travail pour terminer la tâche à temps. Cela inclut les détails des heures de pause et des exceptions de planification. </p> <p>Pour plus d’informations sur l’équilibreur de charge de travail, voir <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Présentation de l’équilibreur de charge de travail</a>.</p> </li> 
       <li> <p><strong>Vue utilisateur du planificateur de ressources</strong><strong>:</strong> Lorsque vous essayez de comprendre à un niveau supérieur les projets auxquels vos utilisateurs sont affectés, utilisez la vue utilisateur du planificateur de ressources. Cela vous permet de voir sur quoi travaillent les utilisateurs, ainsi que leur surallocation et sous-allocation pour une période spécifique. Le planificateur de ressources fournit également une visualisation de l’allocation globale des utilisateurs dans son ensemble, ainsi qu’une visibilité sur les Heures réelles consignées, ce qui s’avère utile pour analyser la progression du travail effectué. </p> <p>Pour plus d’informations sur l’utilisation de la vue utilisateur dans le planificateur de ressources, voir la section <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">Utilisation de la vue utilisateur pour afficher les heures disponibles, planifiées et réelles ou l’éditeur de texte enrichi </a> dans <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Présentation de Resource Planner</a></p> </li> 
      </ul> </li> 
     <li><strong>Pour la phase tactique :</strong> 
      <ul> 
       <li><strong>L’équilibreur de charge de travail</strong> Vous pouvez effectuer les opérations suivantes à l’aide de l’équilibreur de charge de travail : 
        <ul>
         <li>Affectez du travail aux utilisateurs.</li>
         <li>Gérez les affectations des utilisateurs aux tâches. </li>
         <li>Partagez l’équilibreur de charge de travail avec d’autres utilisateurs qui peuvent ne pas avoir de visibilité sur la zone Personnes. Utilisez la fonctionnalité de lien partageable pour partager un lien vers l’équilibreur de charge de travail et l’incorporer dans des tableaux de bord personnalisés. Tous les utilisateurs ayant accès à l’option Afficher les utilisateurs peuvent afficher ces tableaux de bord lorsque vous les partagez.</li>
        </ul><p>L’équilibreur de charge de travail est disponible dans la zone Personnes. </p><p>Pour plus d’informations sur l’équilibreur de charge de travail, voir <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Présentation de l’équilibreur de charge de travail</a>.</p></li> 
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
   <td> <p><strong>Tableau Gantt hérité, Liste des tâches</strong> </p> <p> Le graphique Gantt hérité sur la liste des tâches permet aux utilisateurs de voir visuellement la chronologie du projet et d’effectuer une planification du scénario d’exécution sans avoir à apporter de modifications à la base de données. Le graphique Gantt hérité était basé sur la technologie de Flash, qui présentait des risques pour la sécurité. </p> </td> 
   <td> <p><strong>Graphique de Gantt,</strong> <strong>Liste des tâches</strong></p> <p> Le nouveau diagramme de Gantt basé sur les HTMLS a le même objectif que le diagramme de Gantt hérité. Les utilisateurs peuvent visualiser la chronologie du projet et réaliser une planification du scénario d’exécution sans valider les modifications apportées à la base de données en sélectionnant l’option Enregistrer manuellement dans la barre d’outils de la liste des tâches. </p> <p>Le nouveau diagramme de Gantt est interactif lors de l’utilisation de l’option d’enregistrement automatique que vous pouvez utiliser lorsque vous souhaitez enregistrer automatiquement vos modifications au fur et à mesure. </p> <p>Le nouveau diagramme de Gantt de la liste des tâches repose sur les technologies les plus récentes et est fiable. Ce nouveau diagramme de Gantt se trouve directement dans la liste des tâches et est facilement accessible lorsque vous travaillez sur la liste des tâches sans changer d’onglet ni de vue. </p> <p>Bien que le nouveau graphique Gantt offre les mêmes fonctionnalités que le graphique précédent, il existe des différences de fonctionnalités par rapport au graphique Gantt hérité. </p> <p> Le sous-onglet Gantt hérité d’une liste de tâches de modèle sur un modèle, la vue Gantt héritée de l’onglet Sous-tâches d’une tâche de modèle et le graphique Gantt hérité d’un rapport Tâche de modèle ont également été remplacés par le graphique Gantt basé sur les HTMLS. </p> <p>Si vous utilisez le diagramme de Gantt hérité principalement pour l’affichage simple et les modifications rapides, mais que vous n’utilisez pas le graphique réel, la nouvelle option Planning permet d’apporter rapidement des modifications aux champs de planification clés. Vous pouvez sélectionner Planification de la chronologie au lieu d’enregistrer automatiquement dans la barre d’outils de la liste des tâches.</p> <p>Pour plus d’informations sur l’enregistrement d’une liste de tâches à l’aide de l’option Planification de la chronologie, voir la section "Enregistrer manuellement les modifications dans une liste de tâches lorsque vous sélectionnez l’option Planification de la chronologie" de l’article. <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Editer les tâches dans une liste</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Graphique Gantt hérité pour une liste de projets</strong> </p> <p>Le graphique Gantt hérité sur la liste des projets permet aux utilisateurs d’afficher les projets et leurs tâches en une seule vue. Sans quitter le contexte de la liste des projets, les utilisateurs peuvent afficher les détails sur les tâches d’un projet, ainsi que les dépendances entre les projets. Le graphique Gantt hérité sur la liste des projets était basé sur la technologie de Flash, qui présentait des risques pour la sécurité. </p> </td> 
   <td> <p><strong>Graphique Gantt, liste de projets</strong> </p> <p>Le graphique Gantt basé sur les HTMLS a le même objectif que le graphique Gantt hérité. Les utilisateurs peuvent afficher les projets et leurs tâches dans une vue unique afin d’identifier visuellement les dépendances entre les projets et les tâches. Le graphique Gantt de liste de projets se trouve directement dans la liste des projets. Le nouveau diagramme de Gantt présente une interface moderne et s’appuie sur la technologie la plus récente.</p> <p>Pour plus d’informations sur le diagramme de Gantt de la liste des projets, voir <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Affichage des informations dans le diagramme de Gantt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Partage de boîtes de dialogue pour les rapports, les calendriers et les documents</strong> </p> <p>Lors du partage de rapports, de calendriers et de documents, les boîtes de dialogue utilisées reposaient sur la technologie Flash.</p> </td> 
   <td> <p>L’expérience de partage de rapports, de calendriers et de documents dans Workfront n’a pas changé. Cependant, l’expérience ne dépend plus du Flash.</p> <p>Pour plus d’informations sur le partage de ces éléments, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Présentation des autorisations de partage sur les objets</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Visionneuse de vérification héritée</strong> </p> <p>La visionneuse de vérification héritée était une visionneuse de vérification sur le Web qui fournissait des fonctionnalités de vérification pour les bons à tirer statiques, vidéo et interactifs.</p> </td> 
   <td> <p><strong>Visionneuse de test Web et visionneuse de test de bureau</strong> </p> <p>La visionneuse de test Web fournit des fonctionnalités de vérification pour les bons à tirer statiques et vidéo.</p> <p>La visionneuse de vérification de l’appli de bureau fournit des fonctionnalités de vérification pour les BAT interactifs, en plus de fournir une prise en charge complète des BAT statiques et vidéo.</p> <p>Le format de fichier du SWF n’est plus pris en charge par les principaux fournisseurs et a été remplacé par des bannières HTML5 pour la vérification. </p> <p>Pour plus d’informations sur les différences entre les visionneuses de vérification disponibles, voir <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Présentation des différences entre la visionneuse de test Web et la visionneuse de test de bureau</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
