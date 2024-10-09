---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Affichage des mesures d’utilisation de la connexion aux données Workfront
description: L’onglet Mesures de connexion aux données de Workfront vous permet d’afficher les mesures d’utilisation de votre entreprise en fonction des heures de calcul mensuelles utilisées et du nombre de requêtes effectuées.
author: Nolan
feature: Reports and Dashboards
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 14%

---

# Affichage des mesures d’utilisation [!DNL Workfront Data Connect]

À l’aide de l’onglet [!DNL Workfront Data Connect] [!UICONTROL Mesures] , vous pouvez afficher les mesures d’utilisation de votre entreprise en fonction des heures de calcul utilisées et du nombre de requêtes effectuées. Les entreprises disposent d’un nombre limité d’heures de calcul mensuelles disponibles en fonction de leur type de licence et de leurs achats de modules complémentaires Data Connect. L’onglet [!UICONTROL Mesures] affiche des informations sur les heures de calcul mensuelles disponibles par rapport à ce qui a été utilisé.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td><p>Inclus dans les plans suivants :</p>
    <ul>
        <li>Final</li> 
    </ul>    
   <p>Peuvent être achetées sous la forme d’un module complémentaire pour les forfaits suivants :</p> 
    <ul>
        <li>Sélectionner</li> 
        <li>Principal</li>
    </ul> 
    <p>Workfront Data Connect n’est pas disponible pour les plans Workfront hérités.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Affichage des mesures d’utilisation et des heures de calcul disponibles

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, ou (le cas échéant), cliquez sur l’icône **[!UICONTROL Menu principal]** ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) dans le coin supérieur gauche, puis cliquez sur [!UICONTROL **Configuration**].

1. Dans le panneau de gauche, cliquez sur [!UICONTROL **Système**] > [!UICONTROL **Accès aux données**].

1. Cliquez sur l’onglet [!UICONTROL **Mesures**] . Vos mesures d’utilisation s’affichent dans le graphique **Compute Usage**, tandis que le nombre de requêtes effectuées s’affiche dans le graphique **Query Count**.

   ![ Mesures d’utilisation de la connexion aux données ](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. (Facultatif) Vous pouvez utiliser le menu déroulant [!UICONTROL **Sélectionner une vue**] pour modifier la période des informations incluses dans les deux graphiques.

1. (Facultatif) Vous pouvez utiliser les cases à cocher situées au-dessus du graphique **Compute Usage** pour afficher ou masquer :
   * [!UICONTROL **Heures de calcul quotidiennes**] : nombre d’heures de calcul quotidiennes utilisées par votre organisation.
   * [!UICONTROL **Heures de calcul cumulées mensuelles**] : nombre total d’heures de calcul utilisées par votre organisation au cours d’un mois. Il se réinitialise à zéro tous les mois.
   * [!UICONTROL **Heure de calcul mensuelle**] : nombre d’heures de calcul disponibles pour votre organisation en fonction des achats de licences et/ou de modules complémentaires.
