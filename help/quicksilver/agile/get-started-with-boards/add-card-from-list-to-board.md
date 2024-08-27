---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Ajout de tâches ou de problèmes existants à un panorama Workfront
description: Vous pouvez ajouter n’importe quelle tâche ou problème à un panorama dans Adobe Workfront à partir d’une vue de liste ou de rapport.
author: Lisa
feature: Agile
exl-id: 5e6fd681-8068-4091-9f42-0364b17e0465
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 13%

---

# Ajout de tâches ou de problèmes existants à un panorama [!DNL Workfront]

>[!IMPORTANT]
>
>Les flux de travail ne sont disponibles que pour un groupe spécifique de clientes et de clients.

Vous pouvez ajouter n’importe quelle tâche ou problème à un panorama ou à un workflow dans [!DNL Adobe Workfront] à partir d’une vue de liste ou de rapport, ou à partir des détails de l’objet.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>
   <td> <p>N’importe quelle</p> </td>
  </tr>
  <tr>
   <td role="rowheader">[!DNL Adobe Workfront] licence</td>
   <td>
   <p>Nouvelle : [!UICONTROL Standard]</p> 
   <p>ou</p>
   <p>Actuelle : [!UICONTROL Work] ou licence supérieure</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Autorisations d’objet</td>
   <td>Autorisations [!UICONTROL View] ou supérieures pour la tâche ou le problème </td>
  </tr>
 </tbody>
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ajout de tâches ou de problèmes existants à un panorama ou à un workflow à partir d’une liste

{{step1-click-main-menu}}

1. Choisissez l’une des options suivantes : **[!UICONTROL Projets]**, **[!UICONTROL Rapports]** ou **[!UICONTROL Tableaux de bord]**.
1. Accédez au projet, au rapport ou au tableau de bord qui contient la tâche ou le problème que vous souhaitez ajouter au panorama ou au workflow.
1. Sélectionnez une ou plusieurs tâches ou problèmes.

   Si vous sélectionnez une sous-tâche, elle sera également ajoutée en tant que carte sur le panorama.

1. Cliquez sur [!UICONTROL **Plus**] > [!UICONTROL **Ajouter aux panoramas**] ou [!UICONTROL **Ajouter aux flux de travail**].
1. Dans la boîte de dialogue [!UICONTROL Ajouter à] , sélectionnez le panorama ou le processus auquel ajouter les éléments.

   Pour un panorama, seuls les panoramas autonomes sont disponibles, et non les panoramas qui font partie de flux de travail.

1. Cliquez sur [!UICONTROL **Ajouter**].

   Pour un panorama : la tâche ou le problème est ajouté au panorama sous la forme d’une carte. Si des stratégies de colonne sont appliquées à l’état du panorama, la carte est ajoutée dans la colonne correspondant à son état. Sinon, elle apparaît dans la première colonne à gauche, sans compter la colonne d’ingestion.

   Pour plus d’informations sur les stratégies de colonnes, voir [Gestion des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

   Pour un flux de travail : la tâche ou le problème est ajouté à la liste des cartes du flux de travail en tant que carte non planifiée.

## Ajout de tâches ou de problèmes existants à un panorama ou à un workflow à partir des détails de l’objet

{{step1-click-main-menu}}

1. Cliquez sur [!UICONTROL **Projets**], puis sur le nom d’un projet pour l’ouvrir.
1. Cliquez sur [!UICONTROL **Tâches**] ou [!UICONTROL **Problèmes**] dans le panneau de gauche.
1. Cliquez sur la tâche, la sous-tâche ou le problème à ajouter à un panorama ou à un workflow.
1. Cliquez sur le menu **[!UICONTROL Plus]** en regard du nom de l’objet et sélectionnez [!UICONTROL **Ajouter aux panoramas**] ou [!UICONTROL **Ajouter aux flux de travail**].
1. Dans la boîte de dialogue [!UICONTROL Ajouter à] , sélectionnez le panorama ou le processus auquel ajouter les éléments.

   Pour un panorama, seuls les panoramas autonomes sont disponibles, et non les panoramas qui font partie de flux de travail.

1. Cliquez sur [!UICONTROL **Ajouter**].

   Pour un panorama : la tâche ou le problème est ajouté au panorama sous la forme d’une carte. Si des stratégies de colonne sont appliquées à l’état du panorama, la carte est ajoutée dans la colonne correspondant à son état. Sinon, elle apparaît dans la première colonne à gauche, sans compter la colonne d’ingestion.

   Pour plus d’informations sur les stratégies de colonnes, voir [Gestion des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

   Pour un flux de travail : la tâche ou le problème est ajouté à la liste des cartes du flux de travail en tant que carte non planifiée.

## Afficher les panoramas associés à une tâche ou à un problème dans une liste

1. Accédez au projet, au rapport ou au tableau de bord qui contient la tâche ou le problème pour lequel vous souhaitez afficher les informations des panoramas.
1. Sélectionnez une vue qui comprend la colonne Panoramas ou créez une vue avec la colonne Panoramas .
Pour plus d’informations sur les vues, voir [Créer ou modifier des vues dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).
1. Cliquez sur [!UICONTROL **Afficher**] dans la colonne pour afficher la liste des panoramas sur lesquels se trouve la tâche ou le problème.

   ![Afficher les panoramas dans la colonne](assets/show-boards-in-column.png)

1. Cliquez sur le nom d’un panorama pour ouvrir la tâche ou le problème connecté au panorama.

   ![Sélectionner un panorama](assets/select-board-in-column.png)
