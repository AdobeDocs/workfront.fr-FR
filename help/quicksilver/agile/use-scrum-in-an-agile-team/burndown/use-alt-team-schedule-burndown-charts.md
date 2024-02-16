---
product-area: agile-and-teams
navigation-topic: burndown
title: Utilisation d’un autre planning d’équipe pour les graphiques de ventilation
description: Planifications définies dans [!DNL Adobe Workfront] affectent le graphique de la charge en excluant les jours de congé (week-ends et jours fériés) de la charge.
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Utilisation d’un autre planning d’équipe pour les graphiques de ventilation

Planifications définies dans [!DNL Adobe Workfront] affectent le graphique de la charge en excluant les jours de congé (week-ends et jours fériés) de la charge.

Par défaut, le graphique de ventilation utilise le planning par défaut. Outre la planification par défaut, les équipes agiles peuvent choisir d’utiliser une autre planification afin d’incorporer des jours non ouvrés spécifiques à l’équipe. Ce planning alternatif est ensuite repris dans le graphique de répartition de toute itération affectée à l’équipe. La planification alternative affecte uniquement le graphique de ventilation. (Pour plus d’informations sur la planification par défaut, ainsi que sur la manière dont la variable [!DNL Workfront] L’administrateur peut créer une planification spécifique à l’équipe. Voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

Le graphique de charge ne prend pas en compte les jours partiels. Si, par exemple, votre équipe travaille 4 heures par vendredi, elle est représentée sous la forme d’une journée complète dans le graphique de ventilation.

Pour plus d’informations sur l’utilisation du graphique de ventilation, voir [Présentation du graphique en décharge agile](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Work] ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan ou le type de licence dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Utilisation d’un autre planning d’équipe pour les graphiques de ventilation

1. Assurez-vous que la variable [!DNL Workfront] L’administrateur a déjà créé la planification alternative, comme décrit dans la section [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Équipes]**.

1. (Facultatif) Cliquez sur le **[!UICONTROL Equipe de commutation]** icon ![Icône Changer l’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le bouton **[!UICONTROL Plus]** , puis sélectionnez **[!UICONTROL Modifier]**.

1. Dans le **[!UICONTROL Agile]** , dans la section **[!UICONTROL Planification]** , sélectionnez le nouveau planning dans le menu déroulant.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
