---
content-type: release-notes
navigation-topic: product-releases-archive
title: Fonctionnalités disponibles dans l’environnement d’aperçu en 2016
description: Les fonctionnalités suivantes ont été rendues disponibles dans l’environnement Aperçu en 2016. Ces fonctionnalités doivent être publiées dans l’environnement de production avec la version R1.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 08e0bd72-5979-449e-9fb2-c4d45f51119e
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 1%

---

# Fonctionnalités disponibles dans l’environnement d’aperçu en 2016

Les fonctionnalités suivantes ont été rendues disponibles dans l’environnement Aperçu en 2016. Ces fonctionnalités doivent être publiées dans l’environnement de production avec la version R1.

## Amélioration de la planification des ressources

>[!NOTE]
>
>Les outils de planification des ressources ont été abandonnés et supprimés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Présentation de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Vous pouvez désormais afficher toutes les tâches sur les projets pour lesquels vous êtes le gestionnaire de ressources, ce qui vous permet d’être plus informé lors de la prise de décisions de planification.

Pour des informations générales sur les outils disponibles pour la planification des ressources, voir &quot;Prise en main de la planification des ressources&quot;.

Pour ajuster les informations affichées dans la chronologie de la planification, créez un filtre, comme décrit dans la section &quot;Filtrer les informations dans la zone Planification&quot;.

Outre l’affichage des tâches sur les projets dont vous êtes responsable, vous pouvez utiliser la chronologie de planification pour apporter des modifications aux affectations de ressources. Pour plus d’informations sur la gestion des affectations d’utilisateurs dans la chronologie de planification, voir Affectation manuelle de tâches non affectées et de problèmes dans les zones Planification .

## Gestion des affectations des utilisateurs dans la chronologie de planification

Désormais, lorsque vous planifiez des ressources à l’aide des nouveaux outils de planification des ressources, vous pouvez déterminer comment les heures planifiées d’une tâche ou d’un problème sont attribuées aux utilisateurs. Vous pouvez diviser les heures par jours dans la durée de la tâche et entre les utilisateurs affectés.

Pour plus d’informations, voir &quot;Gestion des affectations d’utilisateurs dans les zones de planification&quot;.

## Les affectations d’utilisateurs sont désactivées par défaut

L’ombrage de l’affectation des utilisateurs sur la chronologie de planification lors de la planification des ressources est désormais désactivé par défaut.

Auparavant, l’ombrage d’affectation s’affichait par défaut et ne pouvait pas être désactivé.

Pour plus d’informations sur l’activation des options d’affectation des utilisateurs, voir
&quot;Gestion des affectations utilisateur dans les zones de planification&quot;.

## Modèle de mise en page Détermine si le calendrier nouveau ou hérité s’affiche dans la zone de travail Mon travail

**Aperçu d’un environnement de test : 7 décembre 2016 ; accès anticipé : 14 décembre 2016** 

Le nouveau calendrier s’affiche par défaut dans la zone Mon travail lorsqu’aucun modèle de mise en page n’est appliqué.

Si vous le souhaitez, vous pouvez configurer le calendrier hérité à afficher dans la zone Mon travail en appliquant un modèle de mise en page à la zone Mon travail configurée pour afficher uniquement la date de validation sur les tâches et les problèmes.

Lors de l’utilisation du calendrier hérité dans la zone Mon travail, seule la tâche à laquelle vous vous êtes engagé s’affiche.

Pour configurer Workfront de manière à afficher le nouveau calendrier dans la zone Mon travail lorsqu’un modèle de mise en page est appliqué, configurez le modèle de mise en page de sorte qu’il affiche la date d’achèvement planifiée pour les tâches et les problèmes, puis attribuez ce modèle de mise en page aux utilisateurs appropriés.

Pour plus d’informations sur la configuration du modèle de mise en page, voir [Créer et gérer des modèles de mise en page](../../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md#customizing-my-work) dans [Créer et gérer des modèles de mise en page](../../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

## Outlook 365 Beta

**Beta : À déterminer ; Disponibilité publique : à déterminer**

Vous pouvez utiliser Workfront depuis Outlook pour Office 365, comme décrit dans les sections suivantes :

* [Configuration d’Adobe Workfront pour Outlook](../../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)
* &quot;Mise à jour d’un élément existant à partir d’un courrier électronique avec Outlook 365&quot;

## Réorganiser les colonnes dans n’importe quelle liste par glisser-déposer

**Accès anticipé : 20 février 2016**

Vous pouvez modifier l’ordre des colonnes dans n’importe quelle liste en faisant glisser une colonne d’un emplacement et en la déposant dans un autre.

Cela s’avère particulièrement utile lorsque vous affichez simultanément le diagramme de Gantt et le mode Liste, et que la colonne que vous souhaitez afficher ne s’affiche pas sur le côté gauche de la page. 

Pour plus d’informations, voir [ Modifier la largeur et l’ordre des colonnes](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)

## Représentation mise à jour de la liste des tableaux de bord

Désormais, lorsque vous affichez une liste de tableaux de bord, l’apparence est plus moderne et évolutive.

Pour plus d’informations sur les tableaux de bord, voir [Création d’un tableau de bord](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)

## Contrôle de l’accès à Forms personnalisé

**Aperçu de l’environnement de test : 23 janvier 2016**

Vous pouvez désormais contrôler qui a accès à un formulaire personnalisé en accordant l’accès à des utilisateurs, équipes, rôles, groupes ou entreprises individuels. 

Avant cette modification, vous ne pouviez accorder l’accès qu’aux groupes.

## Intégration à Adobe Creative Cloud

**Module complémentaire disponible pour téléchargement : avril 2016**

L’extension Workfront pour Adobe Creative Cloud est conçue pour vous permettre d’enregistrer et d’exporter des ressources que vous créez dans le Creative Cloud vers Workfront, ce qui accélère le processus d’approbation et de révision.
