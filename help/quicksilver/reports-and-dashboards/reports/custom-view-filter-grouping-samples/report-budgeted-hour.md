---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Rapport : heures budgétées »'
description: '« Rapport : heures budgétées »'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 100%

---

# Rapport : heure budgétée

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

Lorsque vous souhaitez partager des informations sur les heures budgétées avec d’autres personnes qui n’ont pas accès au planificateur de ressources, vous pouvez le faire en créant un rapport sur les heures budgétées. Vous pouvez ensuite partager le rapport avec elles.

>[!IMPORTANT]
>
>Les heures budgétées sont normalement mises à jour toutes les heures (rarement, il peut s’écouler un maximum de trois heures) dans la base de données Adobe Workfront. L’actualisation du rapport n’actualise pas nécessairement les informations horaires qu’il contient. Vous pouvez afficher le délai écoulé depuis la dernière mise à jour dans le coin supérieur droit de chaque rapport Heures budgétées. L’actualisation du rapport actualise les informations qu’il contient uniquement lorsqu’il s’est écoulé plus d’une heure depuis la dernière mise à jour.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès en modification aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Créer un rapport Heures budgétées

1. Cliquez sur le **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **Rapports**.

1. Cliquez sur **Nouveau Rapport > Heures budgétées**.

   La vue par défaut est appliquée au rapport.

1. (Facultatif) Pour faciliter la lecture du rapport, cliquez sur la colonne **Heures budgétées**, puis **Vasculer en mode Texte**, puis modifiez la ligne

   ```
   valuefield
   ```

   en

   ```
   valueexpreesion
   ```

   et saisissez l’expression d’arrondi.

   Cela arrondit le nombre d’heures budgétées à un certain nombre de décimales que vous spécifiez.

   Pour plus d’informations sur la manière d’arrondir un nombre dans Workfront, voir l’article [Vue d’ensemble des expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Facultatif) Cliquez sur **Ajouter une colonne** pour ajouter des colonnes supplémentaires.
1. (Facultatif) Pour faciliter la lecture du rapport, il est recommandé d’y ajouter un regroupement. Nous proposons le regroupement suivant :

   Cliquez sur l’onglet **Regroupements**, puis effectuez une ou plusieurs des opérations suivantes :

   1. Cliquez sur **Ajouter un regroupement** et commencez à saisir le « Nom du projet », puis sélectionnez-le lorsqu’il apparaît dans la liste.
   1. Cliquez sur **Ajouter un regroupement** et commencez à saisir le « Nom de la fonction », puis sélectionnez-le lorsqu’il apparaît dans la liste.
   1. Cliquez sur **Ajouter un regroupement** et commencez à saisir la **Date d’attribution** ; sélectionnez-la lorsqu’elle apparaît dans la liste, puis sélectionnez la période de regroupement à partir du champ **Regrouper les dates par**.

1. (Facultatif) Cliquez sur **Filtres** pour ajouter des filtres au rapport.
1. (Facultatif) Cliquez sur **Graphique** pour ajouter un graphique au rapport.
1. Cliquez sur **Enregistrer et fermer**.

## Examiner le rapport Heures budgétées

Par défaut, les informations suivantes sont disponibles dans le rapport Heures budgétées :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Projet </td> 
   <td>Il s’agit du nom du projet associé aux Heures budgétées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Fonction</p> </td> 
   <td>Il s’agit du nom de la fonction associée aux Heures budgétées. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">l’utilisateur ou de l’utilisatrice</td> 
   <td>Il s’agit du nom de la personne associée aux Heures budgétées.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Date alloc.</td> 
   <td> <p>Il s’agit de la date d’attribution. Il s’agit du premier jour de la semaine (un dimanche) pour lequel vous avez budgété les heures.</p> <p>Conseil :  <p>Si une semaine s’étend sur deux mois, elle génère deux lignes dans le rapport : l’une correspondant au premier jour de la semaine (le dimanche de la semaine qui se trouve pendant le premier mois), l’autre correspondant au premier jour du deuxième mois (et qui peut être n’importe quel jour de la semaine).</p> <p>Si, par exemple, vous allouez 8 heures à une personne pour la semaine du 30 juin (dimanche) au 6 juillet (samedi), les deux lignes indiquent une date d’attribution du 30 juin et du 1er juillet.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hrs budgétées</td> 
   <td>Il s’agit des heures budgétées allouées à la personne dans le planificateur de ressources.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hrs Hrs budgétées</td> 
   <td>Il s’agit des heures budgétées allouées à la fonction ou au projet dans le planificateur de ressources.</td> 
  </tr> 
 </tbody> 
</table>
