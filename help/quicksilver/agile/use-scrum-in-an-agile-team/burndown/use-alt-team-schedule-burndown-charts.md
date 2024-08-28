---
product-area: agile-and-teams
navigation-topic: burndown
title: Utilisation d’une autre planification d’équipe pour les graphiques de Burndown
description: Les plannings définis dans  [!DNL Adobe Workfront] affectent le graphique de la charge en excluant les jours de congé (week-ends et jours fériés) de la charge.
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 27%

---

# Utiliser un autre planning d’équipe pour les graphiques d’avancement.

Les planifications définies dans [!DNL Adobe Workfront] affectent le graphique de charge en excluant les jours de congé (week-ends et jours fériés) de la charge.

Par défaut, le graphique de ventilation utilise le planning par défaut. Outre la planification par défaut, les équipes agiles peuvent choisir d’utiliser une autre planification afin d’incorporer des jours non ouvrés spécifiques à l’équipe. Ce planning alternatif est ensuite repris dans le graphique de répartition de toute itération affectée à l’équipe. La planification alternative affecte uniquement le graphique de ventilation. (Pour plus d’informations sur la planification par défaut, ainsi que sur la façon dont l’administrateur [!DNL Workfront] peut créer une planification spécifique à l’équipe, voir [Création d’une planification](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

Le graphique de charge ne prend pas en compte les jours partiels. Si, par exemple, votre équipe travaille 4 heures par vendredi, elle est représentée sous la forme d’une journée complète dans le graphique de ventilation.

Pour plus d’informations sur l’utilisation du graphique de ventilation, consultez la [présentation du graphique de ventilation agile](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td> <p>Nouvelle : [!UICONTROL Standard]</p> 
   ou
   <p>Actuelle : [!UICONTROL Work] ou licence supérieure</p> </td> 
  </tr>
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Utiliser un autre planning d’équipe pour les graphiques d’avancement.

1. Assurez-vous que l&#39;administrateur [!DNL Workfront] a déjà créé la planification alternative, comme décrit dans la section [Créer une planification](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

{{step1-to-team}}

1. (Facultatif) Cliquez sur l’icône **[!UICONTROL Changer d’équipe]** ![Icône Changer d’équipe](assets/switch-team-icon.png), puis sélectionnez une nouvelle équipe Scrum dans le menu déroulant ou recherchez une équipe dans la barre de recherche.

1. Sélectionnez l’équipe agile à gérer.
1. Cliquez sur le menu **[!UICONTROL Plus]**, puis sélectionnez **[!UICONTROL Modifier]**.

1. Dans la section **[!UICONTROL Agile]** , dans la zone **[!UICONTROL Planning]** , sélectionnez la nouvelle planification dans le menu déroulant.

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.
