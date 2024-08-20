---
product-area: dashboards
navigation-topic: creating-and-managing-dashboards
title: Présentation des tableaux de bord de canevas
description: Vous pouvez créer des tableaux de bord Canevas qui intègrent des visualisations Canevas de rapports aux rapports traditionnels et offrent de nouvelles options de mise en page.
author: Nolan
feature: Reports and Dashboards
hidefromtoc: true
hide: true
exl-id: b02ca181-e3c3-41e9-ab45-b1b606909127
source-git-commit: 9f975b2128e4ead84ccef8cda30dcb9f29f96e25
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Présentation des tableaux de bord de canevas

<!-- Audited: 12/2023 -->

Les tableaux de bord de canevas, une fonctionnalité en cours de développement pour les tableaux de bord, offre une nouvelle option pour créer des tableaux de bord efficaces dans Workfront. Les tableaux de bord du canevas de rapports permettent d’inclure facilement des visualisations du canevas de rapports dans les rapports existants, offrant ainsi plus de flexibilité et de nouvelles options de mise en page.

Cette fonctionnalité est en cours de développement et ne prend pas encore en charge :
* pages externes
* intégration de calendrier
* rapports générés
* distribution par le biais de modèles de mise en page

Pour obtenir la liste complète des fonctionnalités qui ont été ajoutées aux tableaux de bord Canvas, voir [Tableaux de bord Canvas : activité de publication](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-release-activity.md)

## Accéder aux tableaux de bord de canevas

Une nouvelle option Tableaux de bord de canevas dans le panneau gauche de la page d’entrée des tableaux de bord existants peut être activée pour accéder aux tableaux de bord de canevas. Cette option de menu est désactivée par défaut et doit être activée pour y accéder. Voir les instructions ci-dessous pour plus d’informations sur l’activation de l’option de menu et la navigation vers celle-ci.

### Ajout de tableaux de bord de canevas au panneau de gauche Tableaux de bord

>[!IMPORTANT]
>
>Vous devez disposer au moins des droits d’affichage pour les rapports et les tableaux de bord afin de basculer l’élément Tableaux de bord du canevas dans le modèle de mise en page.

1. Commencez à travailler sur le modèle de mise en page dans lequel vous souhaitez activer les tableaux de bord de la zone de travail, comme décrit dans la section [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Cliquez sur le menu déroulant **Personnaliser ce que les utilisateurs voient**, puis cliquez sur **Tableaux de bord**.

1. Dans la liste **Panneau de gauche** qui s’affiche ci-dessous, cliquez sur l’icône ![](assets/delete-secondary-nav-item.png) en regard de **Tableaux de bord de canevas**. L’icône passera à ![](assets/add-secondary-nav-item.png) pour indiquer qu’elle est désormais visible dans le panneau de gauche Tableaux de bord .

1. Cliquez sur **Enregistrer** en bas de l’écran.

### Ouvrir les tableaux de bord de canevas

1. Assurez-vous d’avoir activé l’option Tableaux de bord de canevas dans votre modèle de mise en page. Voir **Ajout de tableaux de bord de canevas au menu Tableaux de bord** ci-dessus pour obtenir des instructions.

1. Cliquez sur l’icône du menu principal ![](assets/main-menu-icon.png), puis sur **Tableaux de bord**.

1. Dans le panneau de gauche, cliquez sur **Tableaux de bord de la zone de travail**.

## Utilisation des tableaux de bord de zone de travail

### Créer un tableau de bord de canevas

1. Ouvrez les tableaux de bord du canevas comme décrit dans la section **Open Canvas Dashboard** ci-dessus.

1. Cliquez sur **+ Nouveau tableau de bord**

1. Cliquez sur **Sans titre** dans le coin supérieur gauche pour saisir un nom pour le tableau de bord.

1. Cliquez sur **Terminé** dans le coin supérieur droit pour enregistrer votre nouveau tableau de bord ou commencez à ajouter des widgets comme décrit dans **Ajout d’un rapport à un tableau de bord de zone de travail** ci-dessous.

### Ajout d’un rapport à un tableau de bord Zone de travail

1. Ouvrez les tableaux de bord du canevas comme décrit dans la section **Open Canvas Dashboard** ci-dessus.

1. Cliquez sur le tableau de bord auquel vous souhaitez ajouter un rapport à partir de la liste des tableaux de bord.

1. Cliquez sur **Gérer les widgets** dans le coin supérieur droit, puis cliquez sur **Ajouter un widget**.

1. Pointez sur le type de widget de rapport à ajouter, puis cochez la case qui s’affiche.

1. Lorsque vous avez sélectionné tous les widgets à ajouter, cliquez sur **Ajouter** dans le coin supérieur droit.

1. Les widgets sélectionnés s’affichent dans le tableau de bord. Cliquez sur **Configuration** au centre d’un widget pour choisir le rapport qui s’affichera.

1. Commencez à saisir le nom du rapport que vous souhaitez afficher dans le champ **Rechercher le rapport** . Lorsque le rapport s’affiche dans la liste, cliquez sur l’icône **Liste du rapport** ou **Rapport de graphique** en regard de son nom pour afficher les informations de ce rapport dans le format de votre choix.

>[!WARNING]
> Bien que l’ajout de plusieurs widgets qui affichent des informations issues du même rapport soit actuellement possible, il est recommandé de n’afficher chaque rapport qu’une seule fois, car cela peut affecter les performances du tableau de bord.

### Modification d’un widget dans un tableau de bord de zone de travail

1. Ouvrez les tableaux de bord du canevas comme décrit dans la section **Open Canvas Dashboard** ci-dessus.

1. Cliquez sur le tableau de bord que vous souhaitez modifier dans la liste des tableaux de bord.

1. (Facultatif) Pour redimensionner un widget, faites glisser l’icône **Redimensionner** dans le coin inférieur gauche du widget jusqu’à la taille souhaitée.

1. (Facultatif) Pour repositionner un widget, faites glisser l’espace blanc bordant du widget jusqu’à la position relative souhaitée sur le tableau de bord.
