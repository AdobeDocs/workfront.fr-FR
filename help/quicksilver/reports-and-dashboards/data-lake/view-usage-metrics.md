---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Affichage des mesures d’utilisation de Workfront Data Connect
description: Grâce à l’onglet Mesures de Workfront Data Connect , vous pouvez afficher les mesures d’utilisation de votre organisation en fonction des heures de calcul mensuelles utilisées et du nombre de requêtes effectuées.
author: Nolan
feature: Reports and Dashboards
exl-id: 29185bd1-e058-4b42-a508-53406fb9ddd2
source-git-commit: 7764e512a3fb30a89e6645a4d8544a5fcffee231
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 9%

---

# Affichage des mesures d’utilisation des [!DNL Workfront Data Connect]

À l’aide de l’onglet [!DNL Workfront Data Connect] [!UICONTROL Mesures], vous pouvez afficher les mesures d’utilisation de votre organisation en fonction des heures de calcul utilisées et du nombre de requêtes effectuées. Les entreprises disposent d’un nombre limité d’heures de calcul mensuelles disponibles en fonction de leur type de licence et de leurs achats de module complémentaire Data Connect. L’onglet [!UICONTROL Mesures] affiche des informations sur les heures de calcul mensuelles disponibles par rapport à ce qui a été utilisé.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Affichage des mesures d’utilisation et des heures de calcul disponibles

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur [!UICONTROL **Configuration**].

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Système**] > [!UICONTROL **Accès aux données**].

1. Cliquez sur l’onglet [!UICONTROL **Mesures**]. Vos mesures d’utilisation s’affichent dans le graphique **Calculer l’utilisation**, tandis que le nombre de requêtes exécutées s’affiche dans le graphique **Nombre de requêtes**.

   ![Mesures d’utilisation de Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. (Facultatif) Vous pouvez utiliser le menu déroulant [!UICONTROL **Sélectionner une vue**] pour modifier la période des informations incluses dans les deux graphiques.

1. (Facultatif) Vous pouvez utiliser les cases à cocher situées au-dessus du graphique **Calculer l’utilisation** pour afficher ou masquer :
   * [!UICONTROL **Heures de calcul quotidiennes**] - Nombre d’heures de calcul utilisées quotidiennement par votre entreprise.
   * [!UICONTROL **Heures de calcul cumulées mensuelles**] - Nombre total d’heures de calcul utilisées par votre entreprise au cours d’un mois. Se réinitialise à zéro tous les mois.
   * [!UICONTROL **Allocation mensuelle d’heures de calcul**] - Nombre d’heures de calcul disponibles pour votre entreprise en fonction des achats de licence et/ou de module complémentaire.
