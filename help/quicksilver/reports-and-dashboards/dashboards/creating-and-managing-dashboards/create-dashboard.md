---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Créer un tableau de bord
description: Vous pouvez créer des tableaux de bord pour accéder rapidement aux informations dans Adobe Workfront. Les rapports, les calendriers et les pages externes peuvent être ajoutés aux tableaux de bord que vous pouvez partager avec d’autres utilisateurs pour une collaboration optimale.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 8%

---

# Créer un tableau de bord

<!--Audited: 01/2024-->

Vous pouvez créer des tableaux de bord pour accéder rapidement aux informations dans Adobe Workfront. Les rapports, les calendriers et les pages externes peuvent être ajoutés aux tableaux de bord que vous pouvez partager avec d’autres utilisateurs pour une collaboration optimale.

Pour en savoir plus sur les tableaux de bord, voir [Prise en main des tableaux de bord](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Forfait Adobe Workfront</strong></p> </td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Licence Adobe Workfront*</strong></p> </td> 
   <td> <p>Actuel : formule </p>
   Ou
   <p>Nouveau : Standard </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Paramétrages du niveau d'accès</strong> </td> 
   <td> <p>Modification de l’accès aux rapports, aux tableaux de bord et aux calendriers</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Autorisations d’objet</strong> </p> </td> 
   <td> <p>Vous obtiendrez les autorisations Gérer pour les tableaux de bord que vous créez.</p> </td> 
  </tr> 
 </tbody> 
</table>

* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront. Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Vous devez créer l’un des objets suivants avant de pouvoir les ajouter à un tableau de bord :

* **Rapports**: pour plus d’informations sur la création de rapports, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Calendriers**: pour plus d’informations sur la création de calendriers, voir [Présentation des rapports sur les calendriers](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

Vous pouvez ajouter des pages externes existantes à un tableau de bord ou en créer une à partir du nouveau tableau de bord. Pour plus d’informations sur la création de pages externes, voir [Incorporation d’une page web externe dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Créer un tableau de bord

{{step1-to-dashboards}}

1. Cliquez sur **Nouveau tableau de bord**.\
   La boîte de dialogue Nouveau tableau de bord s’affiche.

1. Indiquez les informations suivantes :

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nom</strong></td>
      <td><p>Il s’agit du nom de votre tableau de bord.</p><p>Si vous ne spécifiez aucun nom, le nom du premier rapport du tableau de bord devient, par défaut, celui du tableau de bord.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Description (facultatif)</strong></td>
      <td>Cette section décrit votre tableau de bord.</td>
     </tr>
    </tbody>
   </table>

1. Sélectionnez une mise en page en cliquant sur le bouton radio qui lui correspond dans la partie supérieure de la **Sélectionner Mise en page/Ajouter des rapports/Ajouter des calendriers** . Il s’agit de la disposition dans laquelle les rapports, les calendriers ou les pages externes s’afficheront sur le tableau de bord.

   La mise en page à une seule colonne est la mise en page par défaut.

   Pour plus d’informations sur la disposition des rapports dans les tableaux de bord, voir [Comprendre comment les rapports s’affichent sur un tableau de bord](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. Recherchez des rapports, des calendriers ou des pages externes dans le **Effectuez une recherche par nom ou par type ...** puis faites-les glisser vers le volet de mise en page lorsqu’elles apparaissent dans la liste.

   >[!NOTE]
   >
   >Lors de la recherche d’un élément, la recherche renvoie l’un des 2 000 rapports créés le plus récemment. Les noms de rapports contenant des caractères Unicode ne sont pas renvoyés dans les résultats de recherche. Il est recommandé d’éviter d’inclure des caractères Unicode lors de l’attribution d’un nom aux objets dans Workfront en saisissant des noms plutôt que de copier et coller des noms à partir d’une autre source.

   ![Recherche de rapports](assets/qs-new-dashboard-ui-0722.png)

1. (Facultatif) Cliquez sur **Ajouter une page externe** pour ajouter une nouvelle page externe au tableau de bord.

   Pour plus d’informations sur la création de pages externes et leur incorporation dans les tableaux de bord, voir [Incorporation d’une page web externe dans un tableau de bord](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Cliquez sur **Enregistrer + Fermer**.

   Un horodatage s’affiche dans le coin supérieur droit du tableau de bord. L’horodatage inclut la date, l’heure et le fuseau horaire de la dernière actualisation du tableau de bord.
