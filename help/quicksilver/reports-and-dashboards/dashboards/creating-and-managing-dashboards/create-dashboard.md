---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Créer un tableau de bord
description: Vous pouvez créer des tableaux de bord pour accéder rapidement aux informations dans Adobe Workfront. Des rapports, des calendriers et des pages externes peuvent être ajoutés aux tableaux de bord que vous pouvez partager avec d’autres personnes pour une collaboration optimale.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 507cb64eb21c2798cdafe184794c0d9ed7ebc0c6
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 84%

---

# Créer un tableau de bord

<!--Audited: 01/2025-->

Vous pouvez créer des tableaux de bord pour accéder rapidement aux informations dans Adobe Workfront. Vous pouvez ajouter jusqu’à 25 rapports, calendriers et pages externes aux tableaux de bord afin de les partager avec d’autres personnes pour une collaboration optimale.

Pour en savoir plus sur les tableaux de bord, voir [Commencer avec les tableaux de bord](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux rapports, aux tableaux de bord et aux calendriers</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Vous obtiendrez les autorisations de gestion pour les tableaux de bord que vous créez.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Vous devez créer l’un des objets suivants avant de pouvoir l’ajouter à un tableau de bord :

* **Rapports** : pour plus d’informations sur la création de rapports, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendriers** : pour plus d’informations sur la création de calendriers, voir [Vue d’ensemble des rapports sur les calendriers](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

Vous pouvez ajouter des pages externes existantes à un tableau de bord ou en créer une à partir du nouveau tableau de bord. Pour plus d’informations sur la création de pages externes, voir [Incorporer une page web externe dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Créer un tableau de bord

{{step1-to-dashboards}}

1. Cliquez sur **Nouveau tableau de bord**.\
   La boîte de dialogue Nouveau tableau de bord s’affiche.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nom</strong></td>
      <td><p>Il s’agit du nom de votre tableau de bord. Nous vous recommandons d’utiliser uniquement des caractères UTF-8 pour éviter des problèmes de compatibilité.</p><p>Si vous ne spécifiez aucun nom, le nom du premier rapport du tableau de bord devient, par défaut, celui du tableau de bord.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Description (facultative)</strong></td>
      <td>Il s’agit d’une description de votre tableau de bord.</td>
     </tr>
    </tbody>
   </table>

1. Sélectionnez une disposition en cliquant sur le bouton radio qui lui correspond dans la partie supérieure de la section **Sélectionner une disposition/Ajouter des rapports/Ajouter des calendriers**. Il s’agit de la disposition dans laquelle les rapports, les calendriers ou les pages externes s’afficheront sur le tableau de bord.

   La disposition à une seule colonne est la disposition par défaut.

   Pour plus d’informations sur la structure des rapports dans les tableaux de bord, voir [Comprendre comment les rapports s’affichent sur un tableau de bord](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. Dans la section **Rapports et calendriers disponibles**, commencez à saisir le nom d’un rapport, d’un calendrier ou d’une page externe dans la barre de recherche, puis faites glisser et déposez le rapport, le calendrier ou la page externe dans le volet de disposition à droite.

   >[!NOTE]
   >
   >Lors de la recherche d’un élément, la recherche renvoie l’un des 2 000 rapports créés le plus récemment. Les noms de rapports contenant des caractères Unicode ne sont pas renvoyés dans les résultats de recherche. Une bonne pratique est d’éviter d’inclure des caractères Unicode lors de l’attribution d’un nom aux objets dans Workfront en saisissant des noms plutôt que de copier et coller des noms à partir d’une autre source.

   ![Rechercher des rapports](assets/unshimmed-dashboard-ui.png)

1. (Facultatif) Cliquez sur **Ajouter une page externe** pour ajouter une nouvelle page externe au tableau de bord.

   Pour plus d’informations sur la création de pages externes et leur incorporation dans les tableaux de bord, voir [Incorporer une page web externe dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Cliquez sur **Enregistrer + Fermer**.

   Une date et une heure s’affichent dans le coin supérieur droit du tableau de bord. La date et l’heure incluent la date, l’heure et le fuseau horaire de la dernière actualisation du tableau de bord.
