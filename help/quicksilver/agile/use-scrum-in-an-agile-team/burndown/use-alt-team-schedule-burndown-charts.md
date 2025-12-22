---
product-area: agile-and-teams
navigation-topic: burndown
title: Utiliser un calendrier d'équipe alternatif pour les graphiques d'avancement
description: Les plannings définis dans  [!DNL Adobe Workfront]  affectent le graphique d’avancement en excluant les jours de congé (week-ends et jours fériés) de l’avancement.
author: Jenny
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 86%

---

# Utiliser un autre planning d’équipe pour les graphiques d’avancement

Les plannings définis dans [!DNL Adobe Workfront] affectent le graphique d’avancement en excluant les jours de congé (week-ends et jours fériés) de l’avancement.

Par défaut, le graphique d’avancement utilise le planning par défaut. En plus du planning par défaut, les équipes Agile peuvent choisir d&#39;utiliser également un planning alternatif afin d&#39;incorporer des jours non ouvrés spécifiques à l&#39;équipe. Ce planning alternatif est ensuite repris dans le graphique d’avancement de toute itération affectée à l’équipe. Le planning alternatif affecte uniquement le graphique d’avancement. (Pour plus d’informations sur le planning par défaut, ainsi que sur la manière dont l’administrateur ou administratrice [!DNL Workfront] peut créer un planning spécifique à l’équipe, voir [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

Le graphique d’avancement ne prend pas en compte les jours partiels. Si, par exemple, votre équipe travaille 4 heures chaque vendredi, ceci est représenté sous la forme d’une journée complète dans le graphique d’avancement.

Pour plus d’informations sur l’utilisation du graphique d’avancement, voir [Vue d’ensemble du graphique d’avancement agile](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Travail ou supérieur</p> </td> 
  </tr>
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utiliser un autre planning d’équipe pour les graphiques d’avancement

1. Assurez-vous que l’administrateur ou administratrice [!DNL Workfront] a déjà créé le planning alternatif, comme décrit dans la section [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

{{step1-to-team}}

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe Agile à gérer.
1. Cliquez sur le menu **[!UICONTROL Plus]**, puis sélectionnez **[!UICONTROL Modifier]**.

1. Dans la section **[!UICONTROL Agile]**, dans la zone **[!UICONTROL Planning]**, sélectionnez le nouveau planning dans le menu déroulant.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
