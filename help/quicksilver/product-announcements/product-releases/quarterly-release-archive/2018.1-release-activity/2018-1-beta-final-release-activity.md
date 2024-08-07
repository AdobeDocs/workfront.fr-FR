---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.1, version bêta finale
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version finale de Beta 2018.1. Cette fonctionnalité a été rendue disponible dans l’environnement Aperçu le 31 janvier 2018. Il sera disponible dans l’environnement de production en mars 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 1%

---

# Activité Version 2018.1, version bêta finale

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version finale de Beta 2018.1. Cette fonctionnalité a été rendue disponible dans l’environnement Aperçu le 31 janvier 2018. Il sera disponible dans l’environnement de production en mars 2018.

>[!IMPORTANT]
>
> Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.1, voir  [Présentation de l’activité de version 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La version finale de Beta 2018.1 contient des améliorations pour les administrateurs de Workfront et d’autres utilisateurs :

**Pour les administrateurs**

* [Configurer la disponibilité des ressources et les affectations d’utilisateurs à calculer en fonction du calendrier d’utilisation](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**Pour Tous Les Utilisateurs**

* [ Améliorations apportées à l’appareil mobile](#mobile-enhancements)
* [Intégration Jira](#jira-integration)
* [Mise à jour vers la vérification des noms des visionneuses](#update-to-proofing-viewer-names)
* [Modification de la cadence de synchronisation lors de la synchronisation à partir de l’environnement de production de test pour l’aperçu](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [Message d’avertissement s’affiche lorsque la limite de 2 000 éléments est atteinte dans le planificateur de ressources](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## Améliorations apportées à Mobile {#mobile-enhancements}

Les fonctionnalités suivantes seront disponibles dans les boutiques d’applications mobiles début mars 2018 :

* Nouvelle navigation : la page d’accueil de nos applications mobiles a été repensée.
* Accueil sur mobile : notre nouvelle fonctionnalité d’accueil a désormais été mise à jour sur nos applications mobiles.

La nouvelle fonctionnalité est prise en charge pour les plateformes iOS et Android.

## Intégration Jira {#jira-integration}

Vous pouvez désormais lier des problèmes Jira à des tâches ou des problèmes Workfront en installant et en configurant le module complémentaire Workfront pour Jira. Grâce à cette intégration, vos chefs de projet peuvent continuer à travailler dans Workfront, tandis que vos ingénieurs de développement peuvent continuer à travailler dans Jira, tandis que leurs éléments individuels deviennent liés par l’intégration de Workfront à Jira.

Vous pouvez configurer les éléments suivants via cette intégration :

* Définissez des déclencheurs pour les affectations Workfront afin de créer automatiquement des problèmes Jira lorsqu’ils se produisent.
* Liez manuellement les problèmes Jira aux tâches Workfront ou aux problèmes qui ont été créés précédemment.
* Indiquez les champs qui doivent être synchronisés sur les éléments liés dès que l’un des éléments est mis à jour dans l’une des applications.

Le module complémentaire Workfront sera disponible pour les versions On-Premise et On-Demand de Jira. Le module complémentaire est gratuit et sera disponible au téléchargement sur l’Atlassian Marketplace début mars 2018.

Pour plus d’informations sur le module complémentaire Workfront pour Jira, y compris un lien pour le télécharger, voir [Utilisation de Workfront avec Jira.](https://support.workfront.com/hc/en-us/sections/115001130053)

## Mise à jour de la vérification des noms des visionneuses {#update-to-proofing-viewer-names}

Les noms de la visionneuse de vérification d’HTML5 et des visionneuses de vérification d’Flash ont été renommés dans tout le système Workfront. Les noms précédents et mis à jour sont les suivants : 

| **Nom précédent** | **Nom mis à jour** |
|---|---|
| Visionneuse de vérification d’HTML5 | Nouvelle visionneuse de vérification |
| Visionneuse de vérification de Flash | Visionneuse de vérification héritée |

{style="table-layout:auto"}

 Pour plus d’informations sur l’utilisation de la nouvelle visionneuse de vérification, voir [Vérification des bons à tirer dans la visionneuse de vérification.](https://support.workfront.com/hc/en-us/sections/115000275214)

## Configurer la disponibilité des ressources et les affectations d’utilisateurs à calculer en fonction du calendrier d’utilisation {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

L’administrateur de Workfront peut désormais déterminer comment Workfront calcule la disponibilité des ressources et l’allocation des utilisateurs au niveau du système (en tenant compte des heures ainsi que de la disponibilité de l’éditeur de texte enrichi). L’administrateur de Workfront peut configurer la disponibilité des ressources et l’affectation des utilisateurs à calculer à l’aide du planning par défaut ou du planning de l’utilisateur.

Ce paramètre affecte la disponibilité des utilisateurs dans les cas suivants lors de la planification des ressources :

* Lorsque vous autorisez Workfront à affecter automatiquement des ressources, comme décrit dans la section &quot;Affecter manuellement des tâches non affectées et des problèmes dans les zones de planification&quot;.

* Lors de l’affichage des indicateurs d’affectation, comme décrit dans &quot;Gestion des affectations des utilisateurs dans les zones de planification&quot;.

Pour plus d’informations, voir &quot;Configuration de la manière dont Workfront calcule l’heure de la ressource et la disponibilité de l’éditeur de texte enrichi pour la zone de planification&quot;.

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).


## Modification de la cadence de synchronisation lors de la synchronisation à partir de l’environnement de production de test pour la prévisualisation {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>Cette modification entrera en vigueur le 11 février 2018.

Les données de l’environnement de production Workfront Proof sont désormais synchronisées dans l’environnement de prévisualisation Workfront Proof chaque semaine.

Avant cette modification, les données étaient synchronisées chaque mois de l’environnement de production Workfront Proof vers l’environnement de prévisualisation, tandis que les données de l’environnement de production Workfront étaient synchronisées chaque semaine dans l’environnement de prévisualisation Workfront. Cette incohérence provoquait des erreurs de synchronisation lors de l’utilisation de la fonctionnalité de vérification dans l’environnement Workfront Preview. 

Pour plus d’informations, voir [Aperçu de l’environnement de test Sandbox - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md). 

## Message d’avertissement s’affiche lorsque la limite de 2 000 éléments est atteinte dans le planificateur de ressources {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

À l’heure où nous travaillons actuellement à une solution plus permanente pour améliorer les performances du planificateur de ressources, nous avons introduit une limite de 2 000 éléments pour chaque affichage que vous pouvez appliquer au planificateur de ressources :

* La vue utilisateur affiche seulement 2 000 affectations.
* La vue Projet affiche seulement 2 000 projets.
* La vue Rôle affiche seulement 2 000 rôles.

Lorsque le planificateur de ressources tente de charger plus de 2 000 éléments, une notification s’affiche pour vous alerter que seulement 2 000 éléments peuvent être affichés.

Pour plus d’informations sur ces limites et leur impact sur le planificateur de ressources, voir [Limites d’affichage du planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
