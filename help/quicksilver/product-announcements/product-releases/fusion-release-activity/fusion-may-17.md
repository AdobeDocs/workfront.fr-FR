---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Activité Publication de fusion Workfront : semaine du 17 mai 2021"
description: Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion durant la semaine du 17 mai 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 930c335e-2c88-41af-983f-82be790c1a4b
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 12%

---

# Activité Publication de fusion Workfront : semaine du 17 mai 2021

Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion durant la semaine du 17 mai 2021.

Pour obtenir la liste de toutes les modifications récentes, voir [Activité de publication d’Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Pour obtenir la liste des correctifs récents dans Workfront Fusion, reportez-vous à la page [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html?lang=fr) et recherchez toutes les mises à jour intitulées Mise à jour de maintenance de Workfront Fusion.

## Copie de modules dans des scénarios Workfront Fusion

Pour faciliter l’utilisation de vos scénarios de fusion Workfront, nous avons rendu possible la copie et le collage des modules. Vous pouvez désormais copier un module ou un groupe de modules et les coller dans le même scénario ou dans un autre. La copie des modules conserve les valeurs de champ dans ce module.

Pour plus d’informations, voir [Copie de modules ou de scénarios dans Adobe Workfront Fusion](../../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

## Sélection de plusieurs modules dans un scénario Workfront Fusion

Désormais, lors de la modification d’un scénario, vous pouvez sélectionner plusieurs modules à la fois. Vous pouvez ensuite exécuter des actions en bloc sur les modules sélectionnés.

* Copier
* Déplacer
* Supprimer

La copie et le déplacement des modules conservent les valeurs des modules et toutes les lignes reliant les modules.

Pour plus d’informations sur la modification des scénarios, voir [Création d’un scénario dans Adobe Workfront Fusion](../../../workfront-fusion/scenarios/create-a-scenario.md).

## Les modules conservent désormais les informations non enregistrées.

Pour faciliter la création de scénarios, nous avons rendu possible la conservation des valeurs de champ par les modules lorsqu’elles ne sont pas ciblées. Désormais, lorsque vous cliquez en dehors d’un module sans l’enregistrer, puis que vous y revenez, les champs affichent les valeurs saisies précédemment. Lorsque le module est fermé, il affiche un indicateur indiquant qu’il existe des champs non enregistrés.

## Le connecteur Azure AD gère désormais séparément les enregistrements nouveaux et mis à jour

Les nouveaux enregistrements et mises à jour des enregistrements existants sont désormais gérés par des modules distincts.

* Pour rechercher de nouveaux enregistrements, vous pouvez utiliser le module de déclenchement Enregistrements de contrôle . Ce module ne recherche plus les enregistrements mis à jour.
* Pour obtenir des enregistrements mis à jour, vous pouvez utiliser le nouveau module Delta Utilisateurs/groupes de recherche . Ce module renvoie des enregistrements nouveaux, mis à jour et supprimés.

Pour plus d’informations, voir [Modules Azure Active Directory](../../../workfront-fusion/apps-and-their-modules/azure-ad-modules.md).
