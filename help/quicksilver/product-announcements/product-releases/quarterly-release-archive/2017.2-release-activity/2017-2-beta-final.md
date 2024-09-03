---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2017.2, version bêta finale
description: Cette page décrit tous les changements les plus récents disponibles dans l’environnement de prévisualisation avec la version 2017.2. La fonctionnalité de cette page a été mise à disposition dans l’environnement de prévisualisation le 28 juin 2017. Elle sera disponible dans l’environnement de production à partir du 26 juillet 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 100%

---

# Activité Version 2017.2, version bêta finale

Cette page décrit tous les changements les plus récents disponibles dans l’environnement de prévisualisation avec la version 2017.2. La fonctionnalité de cette page a été mise à disposition dans l’environnement de prévisualisation le 28 juin 2017. Elle sera disponible dans l’environnement de production à partir du 26 juillet 2017.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour une liste de tous les changements apportés avec la version 2017.2, voir [Vue d’ensemble de l’activité de la version 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La version bêta finale 2017.2 contient des améliorations pour les équipes d’administration Workfront et les autres utilisateurs et utilisatrices :

**Pour les administrateurs et administratrices :**

* [Déterminer la disponibilité de la visionneuse de relecture vidéo HTML5 (ProofHQ et Workfront)](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [Prise en charge des certificats SHA-256 pour SAML 2.0](#support-sha-256-certificates-for-saml-2-0)
* [Saisie semi-automatique pour les attributs de mappage](#type-ahead-for-mapping-attributes)
* [Amélioration de l’API : accès aux allocations des utilisateurs et des utilisatrices](#api-enhancement-access-user-allocations)

**Pour tous les utilisateurs et utilisatrices :**

* [Planificateur de ressources](#resource-planner)
* [Nouvelle zone de planification dans un projet (Team Builder)](#new-scheduling-area-in-a-project-team-builder)
* [Planification des ressources : afficher moins d’éléments par défaut](#resource-scheduling-show-fewer-items-by-default)
* [Planification des ressources : afficher l’indicateur de dépôt et de suraffectation lors du déplacement de tâches et de problèmes](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [Planification des ressources : les affectations aux utilisateurs et utilisatrices ne sont plus arrondies à la demi-heure la plus proche.](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [Exporter le rapport d’utilisation aux formats TSV et PDF](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [2017.2 version bêta finale](#user-calendar-enhancements-in-the-my-work-area%22)
* [2017.2 version bêta finale](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [Le statut de décision de l’épreuve s’affiche dans la zone Mon travail (Workfront)](#proof-decision-displays-in-the-my-work-area-workfront)
* [Visualiser les épreuves Rich Media dans des résolutions prédéfinies (ProofHQ et Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [Visualiser l’URL de sous-pages dans les commentaires sur les épreuves Rich Media (ProofHQ et Workfront)](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [Créer des vues personnalisées à partir de vues standard existantes (ProofHQ)](#create-custom-views-based-on-existing-standard-views-proofhq)
* [Filtrer la zone de rapport (ProofHQ)](#filter-the-reporting-area-proofhq)
* [Afficher les valeurs minimum et maximum dans les rapports (ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq)
* [Notification in-app pour l’approbation de l’épreuve](#in-app-notification-for-proof-approval)
* [Améliorations mobiles](#mobile-improvements)
* [Ajout d’une barre oblique dans les instructions de filtrage pour les valeurs de champ contenant des virgules](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [Taux de facturation multiples](#multiple-billing-rates)
* [Nouveau champ Heures budgétées d’une ressource](#new-resource-budgeted-hour-field)
* [Afficher la fonction d’une personne dans la zone « Affecté à » de la page Détails des tâches et des problèmes](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, consultez la section [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Nouvelle zone de planification dans un projet (Team Builder) {#new-scheduling-area-in-a-project-team-builder}

La zone de planification d’un projet (anciennement appelée Team Builder) a été remaniée avec une interface d’utilisation actualisée et plus intuitive. La nouvelle fonctionnalité de planification est désormais plus proche de la fonctionnalité de planification des ressources actuellement disponible dans d’autres parties de Workfront.

Les améliorations comprennent les éléments suivants :

* Visualiser l’affectation actuelle des ressources pour les personnes membres de l’équipe de projet, ce qui permet de prendre des décisions plus éclairées lors de l’affectation des ressources
* Représentation visuelle de la durée des tâches sur le calendrier de planification
* Filtrer les informations affichées sur le calendrier de planification
* Ajouter et supprimer facilement des personnes de l’équipe de projet, directement à partir de la chronologie de planification

Les fonctionnalités suivantes sont disponibles dans d’autres zones de l’outil lors de la planification des ressources, mais ne sont pas disponibles lors de la planification des ressources dans la zone de planification d’équipe :

* Configurer l’affichage des tâches parent sur la chronologie de planification
* Configurer les noms des projets à afficher sur la chronologie de planification
* Modifier les affectations des utilisateurs et des utilisatrices à l’aide de l’outil Permuter
* Filtrer par portfolios, programmes et projets

Pour plus d’informations sur les fonctionnalités disponibles dans la zone de planification d’équipe, consultez « Commencer à utiliser la planification des ressources ».

## Planification des ressources : afficher moins d’éléments par défaut {#resource-scheduling-show-fewer-items-by-default}

Par défaut, un maximum de 10 éléments de travail par jour est désormais affiché sur la chronologie de planification pour une personne donnée. Vous pouvez développer la liste pour afficher toutes les tâches et tous les problèmes actuellement affectés à cet utilisateur ou à cette utilisatrice.

Cela vous permet de parcourir plus facilement la chronologie de planification lorsque les utilisateurs et les utilisatrices se voient affecter de nombreuses tâches et de nombreux problèmes.

Avant cette modification, l’ensemble des tâches et des problèmes étaient toujours affichés pour tous les utilisateurs et toutes les utilisatrices.

Pour plus d’informations sur l’affectation de tâches et de problèmes aux utilisateurs et aux utilisatrices sur la chronologie de planification, consultez « Affecter manuellement des tâches et des problèmes non affectés dans les zones de planification ».

## Planification des ressources : afficher l’indicateur de dépôt et la surallocation lors du déplacement de tâches et de problèmes {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

Lors de l’affectation d’une tâche ou d’un problème à un utilisateur ou à une utilisatrice sur la chronologie de planification via un glisser-déposer, les informations suivantes s’affichent désormais avant de déposer la tâche ou le problème et de terminer l’affectation :

* Un indicateur de dépôt s’affiche sur la ligne de l’utilisateur ou de l’utilisatrice. Cela vous permet de voir où un élément va être affecté avant de procéder à l’affectation.
* Si les allocations des utilisateurs et des utilisatrices sont activées dans la chronologie de planification, les indicateurs rouges de surallocation s&#39;affichent si l’affectation entraîne une surallocation pour l’utilisateur ou l’utilisatrice.

Avant ces modifications, aucune information n’était affichée avant de déposer la tâche ou le problème.

Pour plus d’informations sur l’affectation de tâches et de problèmes aux utilisateurs et aux utilisatrices sur la chronologie de planification, consultez « Affecter manuellement des tâches et des problèmes non affectés dans les zones de planification ».

## Planification des ressources : les affectations des utilisateurs et utilisatrices ne sont plus arrondies à la demi-heure la plus proche {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

Lorsque plusieurs utilisateurs et utilisatrices sont affectés à une tâche ou à un problème, ou lorsqu’une tâche ou un problème s’étend sur plusieurs jours, Workfront tente de répartir les heures planifiées de manière égale entre les utilisateurs et les utilisatrices et les jours affectés. Les heures sont arrondies par défaut au centième le plus proche (par exemple, 1,33).

Auparavant, lorsque vous modifiez manuellement les heures distribuées, les heures étaient ajustées et arrondies à la demi-heure la plus proche (par exemple, 1,33 était arrondi à 1,5).

Désormais, les heures ne sont plus ajustées et ne sont plus arrondies à la demi-heure la plus proche (par exemple, 1,33 reste 1,33).

## Amélioration de l’API : accès aux allocations des utilisateurs et des utilisatrices {#api-enhancement-access-user-allocations}

Vous pouvez désormais accéder aux allocations des utilisateurs et des utilisatrices via l’API Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## Exporter le rapport d’utilisation aux formats TSV et PDF {#export-the-utilization-report-in-tsv-and-pdf-formats}

Vous pouvez désormais exporter le rapport d’utilisation d’un projet aux formats TSV et PDF, en plus du format XLSX.

Avant cette modification, vous ne pouviez exporter le rapport d’utilisation qu’au format XLSX.

Pour plus d’informations sur l’exportation du rapport d’utilisation, consultez [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans [Vue d’ensemble du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Affichage du statut de décision de l’épreuve dans la zone Mon travail (Workfront) {#proof-decision-displays-in-the-my-work-area-workfront}

Désormais, lorsque vous consultez les approbations de relecture dans l’onglet Mes approbations de votre zone Mon Travail, le statut de décision de l’épreuve est affiché dans votre zone Mon Travail et reste affiché jusqu’à ce que vous cliquiez sur le nouveau bouton Actualiser dans Workfront ou jusqu’à la prochaine actualisation de la page dans le navigateur.

Avant cette modification, rien n’indiquait qu’une décision avait déjà été prise sur l’épreuve, et l’épreuve restait dans l’onglet Mes approbations jusqu&#39;à ce que vous actualisiez le navigateur.

Pour plus d’informations, consultez [Approuver du travail](../../../../review-and-approve-work/manage-approvals/approving-work.md) dans [Approuver du travail](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Visualiser des épreuves de médias riches dans des résolutions prédéfinies (ProofHQ et Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

Dans une version antérieure de l’environnement de prévisualisation, nous avons introduit la possibilité d’ajuster la résolution des épreuves de médias riches, soit en spécifiant une résolution personnalisée, soit en cliquant sur l’image et en la faisant glisser jusqu’à la résolution souhaitée.

Vous pouvez désormais sélectionner des options de résolution prédéfinies pour les téléphones, les tablettes, les ordinateurs portables et les ordinateurs de bureau.

Pour plus d’informations, consultez « Afficher une résolution prédéfinie » dans [Modifier la résolution d’une épreuve interactive dans la visionneuse de relecture](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Afficher l’URL des sous-pages dans les commentaires sur les épreuves de médias riches (ProofHQ et Workfront) {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>Cette fonctionnalité est actuellement disponible dans l’environnement de production.

Désormais, lorsque vous commentez dans une sous-page d’une épreuve de médias riches, l’URL de la sous-page est affichée dans le commentaire.

Avant cette modification, il n’était pas clair à quelle sous-page le commentaire faisait référence.

Pour plus d’informations, consultez les ressources suivantes :

## Déterminer la disponibilité de la visionneuse de relecture vidéo HTML5 (ProofHQ et Workfront) {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

En tant qu’administrateur ou administratrice Workfront dans ProofHQ, vous pouvez déterminer si les utilisateurs et les utilisatrices de votre organisation ont accès à la nouvelle visionneuse de relecture HTML5 pour les épreuves vidéo.

Pour plus d’informations sur la configuration de cette option dans Workfront, voir.

## Créer des vues personnalisées basées sur des vues standard existantes (ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

Vous pouvez désormais créer une vue personnalisée basée sur une vue standard.Les options Colonnes, Tri et Filtres de la vue standard sont incluses par défaut dans la nouvelle vue.

Avant cette modification, pour créer une vue personnalisée, vous deviez créer la vue à partir de zéro. 

Pour plus d&#39;informations, voir [Créer une vue personnalisée](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) dans [Créer et gérer des vues personnalisées dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Filtrer la zone de rapports (ProofHQ) {#filter-the-reporting-area-proofhq}

Par défaut, les données affichées dans l’onglet Rapports comprennent toutes les informations de votre système ProofHQ. Vous pouvez désormais utiliser des filtres pour n’afficher que les informations qui répondent à vos besoins. 

Pour plus d’informations, voir [Filtrer les rapports](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) dans [Exécuter des rapports dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Afficher les valeurs minimales et maximales dans les rapports (ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

Il est désormais possible de configurer l’affichage des valeurs minimales et maximales dans le graphique lors de l’affichage des rapports.

Pour plus d’informations, voir [Afficher des rapports](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) dans [Exécuter des rapports dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Prise en charge des certificats SHA-256 pour SAML 2.0 {#support-sha-256-certificates-for-saml-2-0}

Nous prenons désormais en charge l’algorithme de hachage sécurisé 256 (SHA-256) lors de la configuration de Workfront pour l’authentification unique avec SAML 2.0. Avant cette version, nous ne prenions en charge que l’algorithme de hachage sécurisé 1 (SHA-1).

Pour plus d’informations sur la configuration de Workfront avec SAML 2.0, voir [Configurer Adobe Workfront avec SAML 2.0.](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

## Saisie pour les attributs de mappage {#type-ahead-for-mapping-attributes}

Le type de champ Valeur par défaut de la boîte de dialogue Mappage d’attributs a été mis à jour pour devenir un champ de saisie. Avant cette modification, le type de champ Valeur par défaut était une liste déroulante.

Cette modification s’applique aux protocoles SSO suivants :

* Active Directory
* LDAP
* SAML 2.0

SAML 1.1 ne prend pas en charge le mappage d’attributs.

## Améliorations apportées à l’application mobile {#mobile-improvements}

>[!NOTE]
>
> L’application mobile est publiée indépendamment de l’application principale Workfront. La fonctionnalité décrite dans cette section est disponible depuis le début du mois d’août.

Vous verrez les fonctionnalités supplémentaires suivantes sur les applications mobiles, à la fois pour les plateformes Android et iOS :

* Soumettre des demandes à partir de l’application mobile
* Nouvelle entrée dans la feuille de temps sur l’application mobile
* Modifier les formulaires personnalisés à partir de l’application mobile
* Demandes d’approbation des épreuves sur l’application mobile

Un programme beta public sera mis en place pour certaines de ces fonctionnalités sur la plateforme Android.

Pour plus d’informations sur le programme beta à venir pour les appareils mobiles, voir la page [« Versions beta »](https://support.workfront.com/hc/en-us/sections/115000743248).

Pour plus d’informations sur l’utilisation de l’application mobile Workfront, voir . 

## Barre oblique ajoutée au filtre des instructions pour les valeurs de champ contenant des virgules {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

Lors de la création d’un filtre en mode texte et du filtrage des valeurs de champ contenant des virgules, vous devez ajouter une barre oblique (« / ») avant la virgule qui sépare les valeurs, afin de vous assurer que la valeur est lue comme une option de filtre. Cela s’applique uniquement aux types de champ suivants :

* Listes déroulantes
* Cases d’option
* Cases à cocher

Avant cette modification, vous ne pouviez pas filtrer les champs dont les options contenaient des virgules.

Pour plus d’informations sur cette modification, voir [Vue d’ensemble des filtres](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Multiplier les taux de facturation {#multiple-billing-rates}

Vous pouvez désormais ajouter plusieurs remplacements de taux de facturation pour la même fonction au niveau du projet. Grâce à cette nouvelle fonctionnalité, vous pouvez définir des périodes pour chaque remplacement du taux de facturation. Pendant la période spécifiée, un taux de facturation différent est appliqué à la fonction affectée aux tâches d’un projet. Les taux de facturation sont multipliés par le nombre d’heures consacrées au projet pour calculer les revenus. Les revenus calculés dans la période d’un taux de facturation restent bloqués à ce taux et ne sont pas mis à jour lorsque les taux des fonctions sur le projet sont mis à jour. Dans le cas des revenus réels, aucune heure enregistrée avant le remplacement du taux de facturation ne sera recalculée pour refléter le taux de facturation actuel. Les heures enregistrées avant l’ajout du remplacement du taux de facturation au projet seront associées au taux de facturation de la fonction à ce moment-là.

Avant cette modification, vous ne pouviez remplacer le taux de facturation d’une fonction qu’une seule fois, et les revenus réels étaient recalculés pour refléter le taux de facturation actuel pour toutes les heures enregistrées avant la modification du taux de facturation.

Pour plus d’informations sur les taux de facturation et les revenus, voir [Vue d’ensemble de la facturation et des revenus](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Pour plus d’informations sur le remplacement des taux de facturation pour les fonctions au niveau du projet, voir [Vue d’ensemble du remplacement des taux de facturation des fonctions et du calcul des revenus sur un projet](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Planificateur de ressources {#resource-planner}

Avec cette version, nous introduisons la première phase du planificateur de ressources, qui fait partie de la refonte du nouvel onglet Planification dans la zone Personnes. En utilisant le planificateur de ressources, vous pouvez budgétiser le nombre d’heures attribées aux personnes de vos groupes de ressources dans tous les projets en cours pour lesquels vous êtes gestionnaire de ressources. Dans le planificateur de ressources, vous pouvez consulter les chiffres d’attribution suivants par projet, fonction et personne :

* Heures disponibles
* Heures prévues
* Heures budgétées
* Écart horaire (entre les heures budgétées et le nombre d’heures prévues)
* Différence nette d’heures (entre les heures disponibles et les heures budgétées)

Pour plus d’informations sur l’utilisation du planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Nouveau champ Heures budgétées d’une ressource {#new-resource-budgeted-hour-field}

Pour prendre en charge la nouvelle fonctionnalité de planification et le planificateur de ressources, un nouveau champ a été ajouté à report builder, qui vous permet d’établir un rapport sur les heures budgétées des ressources. Ce champ indique le nombre d’heures budgétées pour une ressource dans le cadre d’un projet. Ce champ n’est pas disponible lors de la budgétisation des ressources à l’aide de la fonctionnalité Planification des ressources héritée.

Pour plus d’informations sur l’utilisation des heures budgétées dans le planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Notification in-app pour l’approbation des épreuves {#in-app-notification-for-proof-approval}

Lorsque vous êtes désigné comme personne approbatrice d’une épreuve, vous recevez une notification in-app sur l’approbation de l’épreuve qui attend votre décision. La notification affiche le texte suivant : `<User name>` souhaite que vous approuviez cette épreuve ». Si les informations relatives à la personne ne sont pas disponibles, la notification devient « Cette épreuve nécessite votre approbation ».

Avant cette amélioration, la seule indication visuelle que vous étiez désigné comme personne approbatrice d’une épreuve était une nouvelle demande d’épreuve dans votre zone Mon travail.

Pour plus d’informations sur les notifications in-app, voir [Afficher et gérer les notifications in-app](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Afficher la fonction d’une personne dans la zone « Affecté à » de la page Détails des tâches et des problèmes {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

Désormais, lorsque vous affichez la page des détails d’une tâche ou d’un problème, une fonction s’affiche sous le nom de la personne cessionnaire dans la zone Affecté à. Cette fonction représente la fonction de la personne qui correspond à l’affectation de fonction de la tâche ou du problème. Si la tâche ou le problème n’est pas affecté à une fonction, la fonction principale de la personne affectée s’affiche.

Avant cette modification, seul le titre de la personne était affiché sous son nom dans la zone Affecté à. 
