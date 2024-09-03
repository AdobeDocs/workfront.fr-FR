---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité de la version bêta finale 2018.1
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation avec la version bêta finale 2018.1. Cette fonctionnalité est disponible dans l’environnement de prévisualisation depuis le 31 janvier 2018. Elles seront disponibles dans l’environnement de production en mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 100%

---

# Activité de la version bêta finale 2018.1

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation avec la version bêta finale 2018.1.Cette fonctionnalité est disponible dans l’environnement de prévisualisation depuis le 31 janvier 2018. Elles seront disponibles dans l’environnement de production en mars 2018.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant d’être disponibles dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées dans la version 2018.1, consultez [Vue d’ensemble de l’activité de la version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La version bêta finale 2018.1 contient des améliorations pour les administrateurs et administratrices Workfront ainsi que pour les autres utilisateurs et utilisatrices :

**Pour les administrateurs et administratrices**

* [Configurer la disponibilité des ressources et les affectations des utilisateurs et des utilisatrices à calculer en fonction de leur planning](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**Pour tous les utilisateurs et utilisatrices**

* [Améliorations mobiles](#mobile-enhancements)
* [Intégration Jira](#jira-integration)
* [Mettre à jour les noms de la visionneuse de relecture](#update-to-proofing-viewer-names)
* [Modification de la cadence de synchronisation lors de la synchronisation depuis l’environnement de production de relecture pour la prévisualisation](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [Un message d’avertissement s’affiche lorsque la limite de 2 000 éléments est atteinte dans le planificateur de ressources](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## Améliorations mobiles {#mobile-enhancements}

Les fonctionnalités suivantes seront disponibles dans les boutiques d’applications mobiles début mars 2018 :

* Nouvelle navigation : la page d’accueil de nos applications mobiles a été repensée.
* Accueil sur mobile : notre nouvelle fonctionnalité d’accueil a aussi été mise à jour sur nos applications mobiles.

La nouvelle fonctionnalité est prise en charge pour les plateformes iOS et Android.

## Intégration Jira {#jira-integration}

Vous pouvez désormais lier des problèmes Jira à des tâches ou des problèmes Workfront en installant et en configurant le module complémentaire Workfront pour Jira. Grâce à cette intégration, les personnes responsables de vos projets peuvent continuer à travailler dans Workfront, tandis que vos ingénieures et ingénieurs de développement peuvent continuer à travailler dans Jira et leurs éléments individuels deviennent liés via l’intégration de Workfront à Jira.

Vous pouvez configurer les éléments suivants via cette intégration :

* Définissez des déclencheurs pour les affectations Workfront afin de créer automatiquement des problèmes Jira lorsqu’ils se produisent.
* Liez manuellement les problèmes Jira aux tâches Workfront ou aux problèmes qui ont été créés précédemment.
* Indiquez les champs qui doivent être synchronisés sur les éléments liés dès que l’un des éléments est mis à jour dans l’une des applications.

Le module complémentaire Workfront sera disponible pour les versions sur site et à la demande de Jira. Le module complémentaire est gratuit et sera disponible au téléchargement sur l’Atlassian Marketplace début mars 2018.

Pour plus d’informations sur le module complémentaire Workfront pour Jira, y compris un lien de téléchargement, voir [Utiliser Workfront avec Jira.](https://support.workfront.com/hc/fr-fr/sections/115001130053)

## Mise à jour des noms de la visionneuse de relecture {#update-to-proofing-viewer-names}

Les noms de la visionneuse de relecture HTML5 et des visionneuses de relecture Flash ont été modifiés dans tout le système Workfront. Les noms précédents et mis à jour sont les suivants :

| **Nom précédent** | **Nom mis à jour** |
|---|---|
| Visionneuse de relecture HTML5 | Nouvelle visionneuse de relecture |
| Visionneuse de relecture Flash | Visionneuse de relecture héritée |

{style="table-layout:auto"}

Pour plus d’informations sur l’utilisation de la nouvelle visionneuse de relecture, voir [Relecture des épreuves dans la visionneuse de relecture.](https://support.workfront.com/hc/fr-fr/sections/115000275214)

## Configurer la disponibilité des ressources et les affectations des utilisateurs et des utilisatrices à calculer en fonction de leur planning {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

L’administrateur ou l’administratrice Workfront peut désormais déterminer la façon dont Workfront calcule la disponibilité des ressources et l’affectation des utilisateurs et utilisatrices au niveau du système (en tenant compte des heures ainsi que de la disponibilité de l’ETC). L’administrateur ou administratrice Workfront peut configurer la disponibilité des ressources et l’affectation des utilisateurs et utilisatrices à calculer à l’aide du planning par défaut ou du planning de l’utilisateur ou de l’utilisatrice.

Ce paramètre affecte la disponibilité des utilisateurs et utilisatrices dans les cas suivants lors de la planification des ressources :

* Lorsque vous autorisez Workfront à affecter automatiquement des ressources, tel que décrit dans « Affecter manuellement des tâches et des problèmes non affectées dans les zones de planification ».

* Lors de l’affichage des indicateurs d’affectation, tel que décrit dans « Gérer les affectations de personnes dans les zones de planification ».

Pour plus d’informations, voir « Configurer la manière dont Workfront calcule l’heure de la ressource et la disponibilité ETC pour la zone de planification ».

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).


## Modification de la cadence de synchronisation à partir de l’environnement de production de relecture pour la prévisualisation {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>Cette modification est entrée en vigueur le 11 février 2018.

Les données de l’environnement de production d’épreuve Workfront sont désormais synchronisées dans l’environnement de prévisualisation d’épreuve Workfront chaque semaine.

Avant cette modification, les données étaient synchronisées chaque mois de l’environnement de production d’épreuve Workfront vers l’environnement de prévisualisation, tandis que les données de l’environnement de production Workfront étaient synchronisées chaque semaine dans l’environnement de prévisualisation Workfront. Cette incohérence provoquait des erreurs de synchronisation lors de l’utilisation de la fonctionnalité de relecture dans l’environnement d’aperçu Workfront. 

Pour plus d’informations, voir [Prévisualiser l’environnement de test Sandbox - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).

## Un message d’avertissement s’affiche lorsque la limite de 2 000 éléments est atteinte dans le planificateur de ressources {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

Comme nous travaillons actuellement à une solution plus permanente pour améliorer les performances du planificateur de ressources, nous avons introduit une limite de 2 000 éléments pour chaque vue que vous pouvez appliquer au planificateur de ressources :

* La vue Utilisateurs et utilisatrices affiche seulement 2 000 affectations.
* La vue Projet affiche seulement 2 000 projets.
* La vue Rôle affiche seulement 2 000 rôles.

Lorsque le planificateur de ressources tente de charger plus de 2 000 éléments, une notification s’affiche pour vous avertir que seuls 2 000 éléments peuvent être affichés.

Pour plus d’informations sur ces limites et leur impact sur le planificateur de ressources, voir [Limites d’affichage du planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
