---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2017.2, version bêta finale
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2017.2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 28 juin 2017. Il sera disponible dans l’environnement de production le 26 juillet 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 768e9aad-d7e7-4a3c-9f93-926cf588ddc7
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2314'
ht-degree: 1%

---

# Activité Version 2017.2, version bêta finale

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2017.2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 28 juin 2017. Il sera disponible dans l’environnement de production le 26 juillet 2017.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées en 2017.2, consultez la [présentation de l’activité de version 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

La version finale de Beta 2017.2 contient des améliorations à la fois pour les administrateurs de Workfront et pour d’autres utilisateurs :

**Pour les administrateurs :**

* [Déterminer la disponibilité de la visionneuse de vérification vidéo HTML5 (ProofHQ et Workfront)](#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront)
* [Prise en charge des certificats SHA-256 pour SAML 2.0](#support-sha-256-certificates-for-saml-2-0)
* [Type-Ahead pour les attributs de mappage](#type-ahead-for-mapping-attributes)
* [Amélioration de l’API : accès aux affectations des utilisateurs](#api-enhancement-access-user-allocations)

**Pour Tous Les Utilisateurs :**

* [Planificateur de ressources](#resource-planner)
* [Nouvelle zone de planification dans un projet (créateur d’équipes)](#new-scheduling-area-in-a-project-team-builder)
* [Planification des ressources : afficher moins d’éléments par défaut](#resource-scheduling-show-fewer-items-by-default)
* [Planification des ressources : afficher l’indicateur de dépôt et la surallocation lors du glissement de tâches et de problèmes](#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues)
* [Planification des ressources : les affectations des utilisateurs ne sont plus arrondies à la demi-heure la plus proche](#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour)
* [Exporter le rapport d’utilisation au format TSV et PDF](#export-the-utilization-report-in-tsv-and-pdf-formats)
* [Version finale de Beta 2017.2](#user-calendar-enhancements-in-the-my-work-area%22)
* [Version finale de Beta 2017.2](#layout-template-determines-whether-the-new-or-legacy-calendar-displays-in-the-my-work-area)
* [Affichage d’une décision de BAT dans la zone de travail Mon travail (Workfront)](#proof-decision-displays-in-the-my-work-area-workfront)
* [ Afficher les bons à tirer pour les médias riches dans les résolutions de paramètres prédéfinis (BATHQ et Workfront)](#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront)
* [Afficher l’URL vers les sous-pages dans les commentaires sur les bons à tirer de médias riches (ProofHQ et Workfront)](#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront)
* [Créer des vues personnalisées basées sur des vues standard existantes (ProofHQ)](#create-custom-views-based-on-existing-standard-views-proofhq)
* [Filtrer la zone de création de rapports (ProofHQ)](#filter-the-reporting-area-proofhq)
* [Afficher les valeurs minimale et maximale dans les rapports (ProofHQ)](#display-minimum-and-maximum-values-in-reports-proofhq)
* [Notification In-App pour approbation de BAT](#in-app-notification-for-proof-approval)
* [Améliorations mobiles](#mobile-improvements)
* [Barre oblique ajoutée au filtre des instructions pour les valeurs de champ contenant des virgules](#slash-added-to-filter-statements-for-field-values-that-contain-commas)
* [Plusieurs taux de facturation](#multiple-billing-rates)
* [ Nouveau Champ D’Heure Budgété De Ressource ](#new-resource-budgeted-hour-field)
* [Afficher le rôle de la tâche utilisateur dans la zone &quot;Affectée à&quot; de la page Détails pour les tâches et les problèmes](#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues)

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Nouvelle zone de planification dans un projet (créateur d’équipes) {#new-scheduling-area-in-a-project-team-builder}

La zone Planification d’un projet (anciennement appelée Créateur d’équipes) a été repensée avec une interface utilisateur mise à jour et plus intuitive. La nouvelle fonctionnalité de planification correspond désormais davantage à la fonctionnalité de planification des ressources actuellement disponible dans d’autres zones de Workfront.

Les améliorations incluent :

* Affichez les affectations de ressources actuelles pour les membres de l’équipe de projet, ce qui vous permet de prendre des décisions plus éclairées lors des affectations.
* Représentation visuelle des durées de tâche sur la chronologie de planification
* Filtrer les informations affichées dans la chronologie de planification
* Ajoutez et supprimez facilement des utilisateurs de l’équipe de projet, directement depuis la chronologie de planification.

Les fonctionnalités suivantes sont disponibles dans d’autres zones de l’outil lors de la planification des ressources, mais ne sont pas disponibles lors de la planification des ressources dans la zone Planification de l’équipe :

* Configuration des tâches parentes à afficher dans la chronologie de planification
* Configuration des noms de projet à afficher dans la chronologie de planification
* Modification des affectations d’utilisateurs à l’aide de l’outil Swap
* Filtrage par portefeuille, programme et projet

Pour plus d’informations sur les fonctionnalités disponibles dans la zone Planification de l’équipe, voir &quot;Prise en main de la planification des ressources&quot;.

## Planification des ressources : afficher moins d’éléments par défaut {#resource-scheduling-show-fewer-items-by-default}

Par défaut, un maximum de 10 tâches par jour s’affiche désormais dans la chronologie de planification pour un utilisateur donné. Vous pouvez développer la liste pour afficher toutes les tâches et tous les problèmes actuellement affectés à cet utilisateur.

Cela vous permet de parcourir plus facilement la chronologie de planification lorsque de nombreuses tâches et problèmes sont affectés aux utilisateurs.

Avant cette modification, toutes les tâches et tous les problèmes s’affichaient toujours pour tous les utilisateurs.

Pour plus d’informations sur l’affectation de tâches et de problèmes aux utilisateurs dans le planning de planification, voir Affectation manuelle de tâches non affectées et de problèmes dans les zones Planification .

## Planification des ressources : affichez l’indicateur de dépôt et la surallocation lors du glissement de tâches et de problèmes {#resource-scheduling-display-drop-indicator-and-over-allocation-when-dragging-tasks-and-issues}

Lors de l’affectation d’une tâche ou d’un problème à un utilisateur dans la chronologie de planification par glisser-déposer, les informations suivantes s’affichent maintenant avant de publier la tâche ou le problème et de terminer l’affectation :

* Un indicateur de dépôt s’affiche dans la ligne de l’utilisateur. Cela vous permet de voir où un élément est affecté avant d’effectuer l’affectation.
* Si les affectations de l’utilisateur sont activées dans la chronologie de planification, les indicateurs de suraffectation rouges s’affichent si l’exécution de l’affectation entraîne la surallocation de l’utilisateur.

Avant ces modifications, aucune information ne s’affichait avant la publication de la tâche ou du problème.

Pour plus d’informations sur l’affectation de tâches et de problèmes aux utilisateurs dans le planning de planification, voir Affectation manuelle de tâches non affectées et de problèmes dans les zones Planification .

## Planification des ressources : les affectations des utilisateurs ne sont plus arrondies à la demi-heure la plus proche {#resource-scheduling-user-allocations-are-no-longer-rounded-to-the-nearest-half-hour}

Lorsque plusieurs utilisateurs sont affectés à une tâche ou à un problème, ou lorsqu’une tâche ou un problème s’étend sur plusieurs jours, Workfront tente de répartir les heures planifiées uniformément entre les utilisateurs et les jours attribués. Les heures sont arrondies par défaut au centième le plus proche (par exemple, 1,33).

Auparavant, lorsque vous aviez modifié manuellement les heures distribuées, les heures étaient ajustées et arrondies à la demi-heure la plus proche (par exemple, 1,33 est arrondi à 1,5).

Désormais, les heures ne sont plus ajustées et arrondies à la demi-heure la plus proche (par exemple, 1,33 reste 1,33).

## Amélioration de l’API : accès aux affectations des utilisateurs {#api-enhancement-access-user-allocations}

Vous pouvez désormais accéder à l’ombrage de l’affectation des utilisateurs via l’API Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see <a href="../../../../wf-api/api/access-proj-allocation-info-api.md" class="MCXref xref" xrefformat="{para}">Access Project Allocation Information via the API</a>.</p>
-->

## Exporter le rapport Utilisation au format TSV et PDF {#export-the-utilization-report-in-tsv-and-pdf-formats}

Vous pouvez désormais exporter le rapport d’utilisation d’un projet aux formats TSV et PDF, en plus du format XLSX.

Avant cette modification, vous ne pouviez exporter le rapport d’utilisation qu’au format XLSX.

Pour plus d’informations sur l’exportation du rapport d’utilisation, voir [Présentation du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md) dans [Présentation du rapport d’utilisation des ressources](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Affichage d’une décision de preuve dans la zone de travail Mon travail (Workfront) {#proof-decision-displays-in-the-my-work-area-workfront}

Désormais, lorsque vous affichez les validations de vérification dans l’onglet Mes approbations de la zone Mon travail, la décision du BAT s’affiche dans la zone Mon travail et reste jusqu’à ce que vous cliquiez sur le nouveau bouton Actualiser de Workfront ou jusqu’à la prochaine actualisation de la page du navigateur.

Avant cette modification, rien n’indiquait qu’une décision avait déjà été prise sur le BAT et le BAT restait dans l’onglet Mes approbations jusqu’à ce que vous actualisiez le navigateur.

Pour plus d’informations, voir [Valider le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md) dans [Valider le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Affichage des bons à tirer pour les médias riches dans des résolutions de paramètres prédéfinis (BATHQ et Workfront) {#view-rich-media-proofs-in-preset-resolutions-proofhq-and-workfront}

Dans une version antérieure de l’environnement Aperçu, nous avons introduit la possibilité d’ajuster la résolution des BAT de médias riches en spécifiant une résolution personnalisée ou en faisant glisser l’image vers la résolution souhaitée.

Vous pouvez désormais sélectionner parmi les options de résolution prédéfinies de divers téléphones, tablettes, notebooks et ordinateurs de bureau.

Pour plus d’informations, voir &quot;Affichage d’une résolution de paramètre prédéfini&quot; dans [Modification de la résolution du BAT interactif dans la visionneuse de correctifs](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

## Afficher l’URL des sous-pages dans les commentaires sur les bons à tirer du contenu multimédia enrichi (BATHQ et Workfront) {#view-url-to-sub-pages-in-comments-on-rich-media-proofs-proofhq-and-workfront}

>[!NOTE]
>
>Cette fonctionnalité est actuellement disponible dans l’environnement de production.

Désormais, lorsque vous commentez une sous-page dans un BAT multimédia enrichi, l’URL de la sous-page s’affiche sur le commentaire.

Avant cette modification, la sous-page à laquelle faisait référence le commentaire n’était pas claire.

Pour plus d’informations, voir

## Déterminer la disponibilité de la visionneuse de vérification vidéo HTML5 (ProofHQ et Workfront) {#determine-the-availability-of-the-html5-video-proofing-viewer-proofhq-and-workfront}

En tant qu’administrateur Workfront dans BATHQ, vous pouvez déterminer si les utilisateurs de votre entreprise ont accès à la nouvelle visionneuse de vérification de l’HTML5 pour obtenir des bons à tirer.

Pour plus d’informations sur la configuration de cette option dans Workfront, voir .

## Créer des vues personnalisées basées sur des vues standard existantes (ProofHQ) {#create-custom-views-based-on-existing-standard-views-proofhq}

Vous pouvez désormais créer une vue personnalisée basée sur une vue standard. Les options Colonnes, Tri et Filtres de la vue standard sont incluses par défaut dans la nouvelle vue.

Avant cette modification, pour créer une vue personnalisée, vous deviez créer la vue à partir de zéro. 

Pour plus d’informations, voir [Création d’une vue personnalisée](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md#creating) dans [Création et gestion des vues personnalisées dans le BAT Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## Filtrage de la zone de création de rapports (ProofHQ) {#filter-the-reporting-area-proofhq}

Par défaut, les données affichées dans l’onglet Rapports incluent toutes les informations de votre système BATHQ. Vous pouvez désormais utiliser des filtres pour afficher uniquement les informations pertinentes à vos besoins. 

Pour plus d’informations, voir [Filtrage des rapports](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#filtering-reports) dans  [Exécuter des rapports dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Affichage des valeurs minimales et maximales dans les rapports (ProofHQ) {#display-minimum-and-maximum-values-in-reports-proofhq}

Vous pouvez désormais configurer l’affichage des valeurs minimale et maximale dans le graphique lors de l’affichage des rapports.

Pour plus d’informations, voir [Affichage des rapports](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md#viewing-reports) dans  [Exécuter des rapports dans Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/run-reports.md).

## Prise en charge des certificats SHA-256 pour SAML 2.0 {#support-sha-256-certificates-for-saml-2-0}

Nous prenons désormais en charge l’algorithme de hachage sécurisé 256 (SHA-256) lors de la configuration de Workfront pour SSO avec SAML 2.0. Avant cette version, seuls l’algorithme de hachage sécurisé 1 (SHA-1) était pris en charge.

Pour plus d’informations sur la configuration de Workfront avec SAML 2.0, voir [Configuration d’Adobe Workfront avec SAML 2.0](../../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md)

## Type anticipé des attributs de mappage {#type-ahead-for-mapping-attributes}

Le type de champ Valeur par défaut de la boîte de dialogue Mappage des attributs a été mis à jour pour un champ de type avant. Avant cette modification, le type du champ Valeur par défaut était une liste déroulante.

Cette modification s’applique aux protocoles SSO suivants :

* Active Directory
* LDAP
* SAML 2.0

SAML 1.1 ne prend pas en charge le mappage des attributs.

## Améliorations des périphériques mobiles {#mobile-improvements}

>[!NOTE]
>
> L&#39;application mobile est libérée indépendamment de l&#39;application Workfront principale. Les fonctionnalités décrites dans cette section ont été publiées au début du mois d’août.

Les nouvelles fonctionnalités suivantes s’affichent sur les applications mobiles, pour les plateformes Android et iOS :

* Envoi de requêtes depuis l’application mobile
* Nouvelle entrée de la feuille de temps sur l’application mobile
* Modification de formulaires personnalisés à partir de l’application mobile
* Demandes d’approbation de BAT sur l’application mobile

Il y aura un programme bêta public pour certaines de ces fonctionnalités pour la plateforme Android.

Pour plus d’informations sur le programme bêta à venir pour mobile, voir  Page [&quot;Betas&quot;](https://support.workfront.com/hc/en-us/sections/115000743248).

Pour plus d’informations sur l’utilisation de l’application mobile Workfront, voir .  

## Barre oblique ajoutée au filtre des instructions pour les valeurs de champ contenant des virgules {#slash-added-to-filter-statements-for-field-values-that-contain-commas}

Lors de la création d’un filtre en mode texte et du filtrage des valeurs de champ contenant des virgules, vous devez ajouter une barre oblique (&quot;/&quot;) avant la virgule qui sépare les valeurs, afin de vous assurer que la valeur est lue comme une option de filtre. Cela s’applique uniquement aux types de champ suivants :

* Liste déroulante
* Cases d’option
* Cases à cocher

Avant cette modification, vous ne pouviez pas filtrer les champs contenant des virgules.

Pour plus d’informations sur cette modification, voir [Présentation des filtres](../../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Taux de facturation multiples {#multiple-billing-rates}

Vous pouvez désormais ajouter plusieurs remplacements de taux de facturation pour le même rôle de tâche au niveau du projet. Grâce à cette nouvelle fonctionnalité, vous pouvez définir des plages de dates pour chaque remplacement de taux de facturation. Au cours de la période spécifiée, un taux de facturation différent est appliqué au rôle de tâche affecté aux tâches d’un projet. Les taux de facturation sont multipliés par les heures sur le projet pour calculer le chiffre d’affaires. Les recettes calculées dans la période d’un taux de facturation restent verrouillées à ce taux et ne sont pas mises à jour en tant que taux des rôles de tâche lors de la mise à jour du projet. Dans le cas des Recettes réelles, aucune heure enregistrée avant le remplacement du taux de facturation ne sera recalculée pour tenir compte du taux de facturation actuel. Les heures consignées avant l’ajout du remplacement du taux de facturation au projet seront associées au taux de facturation du rôle de tâche à ce moment-là.

Avant cette modification, vous ne pouviez remplacer le taux de facturation d’un rôle de tâche qu’une seule fois, et les Recettes réelles seraient recalculées pour refléter le taux de facturation actuel pour toutes les heures consignées avant que le taux de facturation ne soit modifié.

Pour plus d’informations sur les taux de facturation et les recettes, voir [Présentation de la facturation et des recettes](../../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

Pour plus d’informations sur le remplacement des taux de facturation pour les rôles de tâche au niveau du projet, voir [Présentation du remplacement des taux de facturation des rôles de tâche et calcul des recettes sur un projet](../../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Planificateur de ressources {#resource-planner}

Avec cette version, nous proposons la première phase du planificateur de ressources, qui fait partie de la reconception du nouvel onglet Planification de la zone Personnes. À l’aide du planificateur de ressources, vous pouvez planifier le nombre d’heures alloué par les utilisateurs de vos groupes de ressources dans tous les projets en cours pour lesquels vous êtes le gestionnaire de ressources. Vous pouvez voir les nombres d’attribution suivants par projet, rôle de tâche et par utilisateur, dans le planificateur de ressources :

* Heures disponibles
* Heures prévues
* Heures budgétées
* Ecart horaire (entre les heures budgétisées et les heures planifiées)
* Différence Heure nette (entre les Heures disponibles et les Heures budgétisées)

Pour plus d’informations sur l’utilisation du planificateur de ressources, consultez la [présentation du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Nouveau champ d’heure budgété des ressources {#new-resource-budgeted-hour-field}

Pour prendre en charge la nouvelle fonctionnalité de planification et le planificateur de ressources, un nouveau champ a été ajouté au créateur de rapports, qui vous permet de créer des rapports sur les heures budgétaires de la ressource. Ce champ capture le nombre d’heures prévu pour une ressource dans un projet. Ce champ n’est pas disponible lors de la planification des ressources à l’aide de la fonctionnalité de planification des ressources héritée.

Pour plus d’informations sur l’utilisation des heures budgétées dans le planificateur de ressources, consultez la [présentation du planificateur de ressources](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

## Notification In-App pour approbation de BAT {#in-app-notification-for-proof-approval}

Lorsque vous êtes désigné comme approbateur pour un BAT, vous recevez une notification in-app sur l’approbation du BAT en attendant votre décision. La notification affiche le texte suivant : `<User name>` souhaite que vous approuviez ce BAT&quot;. Si les informations utilisateur ne sont pas disponibles, la notification passe à &quot;Ce BAT nécessite votre approbation&quot;.

Avant cette amélioration, la seule indication visuelle selon laquelle vous étiez désigné comme approbateur sur un BAT était une nouvelle demande de BAT dans votre zone Mon travail.

Pour plus d’informations sur les notifications in-app, voir [Affichage et gestion des notifications in-app](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## Afficher le rôle de la tâche utilisateur dans la zone &quot;Affectée à&quot; de la page Détails pour les tâches et les problèmes {#show-user-job-role-in-assigned-to-area-on-the-details-page-for-tasks-and-issues}

Désormais, lors de l’affichage de la page de détails d’une tâche ou d’un problème, un rôle de tâche s’affiche sous le nom de la personne désignée dans la zone Affectée à . Ce rôle de tâche représente le rôle de tâche de l’utilisateur qui correspond à l’affectation du rôle de tâche de la tâche ou du problème. Si la tâche ou le problème n’est pas assigné à un rôle de tâche, le rôle de tâche principal de l’utilisateur affecté s’affiche.

Avant cette modification, seul le titre de l’utilisateur s’affichait sous le nom de l’utilisateur dans la zone Affecté à . 
