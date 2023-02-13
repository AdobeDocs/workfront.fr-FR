---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Activité Publication de fusion Workfront : Semaine du 17 mai 2021'''
description: Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion au cours de la semaine du 17 mai 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 930c335e-2c88-41af-983f-82be790c1a4b
hidefromtoc: true
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Activité Publication de fusion Workfront : semaine du 17 mai 2021

Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion au cours de la semaine du 17 mai 2021.

Pour obtenir la liste de toutes les modifications récentes, voir [Activité Publication de fusion Adobe Workfront](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Pour obtenir la liste des correctifs récents dans Workfront Fusion, reportez-vous à la section [Mises à jour de maintenance de Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) et recherchez toutes les mises à jour intitulées Mise à jour de maintenance de la fusion Workfront.

## Copie de modules dans des scénarios Workfront Fusion

Pour faciliter l’utilisation de vos scénarios de fusion Workfront, nous avons rendu possible la copie et le collage des modules. Vous pouvez désormais copier un module ou un groupe de modules et les coller dans le même scénario ou dans un autre. La copie des modules conserve les valeurs de champ dans ce module.

Pour plus d’informations, voir [Copie de modules ou de scénarios dans Adobe Workfront Fusion](../../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

## Sélection de plusieurs modules dans un scénario Workfront Fusion

Désormais, lorsque vous modifiez un scénario, vous pouvez sélectionner plusieurs modules à la fois. Vous pouvez ensuite exécuter des actions en bloc sur les modules sélectionnés.

* Copier
* Déplacer
* Supprimer

La copie et le déplacement des modules conservent les valeurs des modules et toutes les lignes reliant les modules.

Pour plus d’informations sur la modification de scénarios, voir [Création d’un scénario dans Adobe Workfront Fusion](../../../workfront-fusion/scenarios/create-a-scenario.md).

## Les modules conservent désormais les informations non enregistrées.

Pour faciliter la création de scénarios, nous avons rendu possible la conservation des valeurs de champ par les modules lorsqu’elles ne sont pas ciblées. Désormais, lorsque vous cliquez en dehors d’un module sans l’enregistrer, puis que vous y revenez, les champs affichent les valeurs saisies précédemment. Lorsque le module est fermé, il affiche un indicateur indiquant qu’il existe des champs non enregistrés.

## Le connecteur Azure AD gère désormais séparément les enregistrements nouveaux et mis à jour

Les nouveaux enregistrements et mises à jour des enregistrements existants sont désormais gérés par des modules distincts.

* Pour rechercher de nouveaux enregistrements, vous pouvez utiliser le module de déclenchement Enregistrements de contrôle . Ce module ne recherche plus les enregistrements mis à jour.
* Pour obtenir des enregistrements mis à jour, vous pouvez utiliser le nouveau module Delta Utilisateurs/groupes de recherche . Ce module renvoie des enregistrements nouveaux, mis à jour et supprimés.

Pour plus d’informations, voir [Modules Azure Principale Directory](../../../workfront-fusion/apps-and-their-modules/azure-ad-modules.md).
