---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Activité Publication de fusion Workfront : Semaine du 3 mai 2021'''
description: Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion au cours de la semaine du 3 mai 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 9c2321794c5ba773bfda1d6e9dfda6b8de1a1449
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Activité Publication de fusion Workfront : Semaine du 3 mai 2021

Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion au cours de la semaine du 3 mai 2021.

Pour obtenir la liste de toutes les modifications récentes, voir [Activité Publication de fusion Adobe Workfront](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Pour obtenir la liste des correctifs récents dans Workfront Fusion, reportez-vous à la section [Mises à jour de maintenance de Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) et recherchez toutes les mises à jour intitulées Mise à jour de maintenance de la fusion Workfront.

## Le connecteur Salesforce peut désormais effectuer des recherches à l’aide de SOQL.

Le module Salesforce > Recherche d’enregistrements a désormais la possibilité d’effectuer une recherche à l’aide de SOQL (Salesforce Object Query Language). Vous pouvez également effectuer des recherches à l’aide des options disponibles précédemment (recherches SOSL et simples).

Pour plus d’informations, voir [Modules Salesforce](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## Le nouveau type de connexion dans le connecteur Azure DevOps nécessite moins de portées

Pour améliorer la sécurité, nous avons ajouté un nouveau type de connecteur au connecteur Azure DevOps Workfront Fusion. Désormais, lorsque vous créez une connexion dans un module Azure DevOps, vous pouvez choisir entre deux types de connexions :

* Ops de développement Azure

   Ce nouveau type de connexion limite les portées à celles spécifiquement nécessaires à Workfront Fusion.

* Ops de développement Azure (demander toutes les portées)

   Il s’agit du type de connexion hérité, qui demande toutes les portées disponibles lors d’une connexion à Azure DevOps.

Nous vous recommandons d’utiliser le type de connexion Azure DevOps dans tous vos nouveaux scénarios qui utilisent Azure DevOps. Nous vous recommandons également de modifier les modules Azure DevOps dans vos scénarios existants afin d’utiliser le nouveau type de connexion. Le type de connexion Azure DevOps (Demander toutes les portées) hérité sera bientôt obsolète.

Pour plus d’informations, voir [Modules Azure DevOps](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).
