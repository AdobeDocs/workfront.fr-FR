---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Rapport : Heure budgétée"
description: "Rapport : Heure budgétée"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 16%

---

# Rapport : heure budgétée

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

Lorsque vous souhaitez partager des informations sur l’heure budgétée avec d’autres utilisateurs qui n’ont pas accès au planificateur de ressources, vous pouvez le faire en créant un rapport sur l’heure budgétée. Vous pouvez ensuite partager le rapport avec eux.

>[!IMPORTANT]
>
>Les heures budgétisées sont normalement mises à jour toutes les heures (rarement, il peut s’écouler un maximum de trois heures) dans la base de données Adobe Workfront. L’actualisation du rapport n’actualise pas nécessairement les informations horaires qu’il contient. Vous pouvez afficher le délai écoulé depuis la dernière mise à jour dans le coin supérieur droit de chaque rapport Heure budgétaire . L&#39;actualisation du rapport actualise les informations qu&#39;il contient uniquement lorsqu&#39;il y a eu plus d&#39;une heure depuis la dernière mise à jour.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Création d’un rapport Heure planifiée

1. Cliquez sur le **menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis sur **Rapports**.

1. Cliquez sur **Nouveau rapport > Heure budgétée**.

   La vue par défaut est appliquée au rapport.

1. (Facultatif) Pour faciliter la lecture du rapport, cliquez sur la colonne **Heures budgétaires**, puis **Basculer vers le mode Texte**, puis modifiez la variable

   ```
   valuefield
   ```

   line vers

   ```
   valueexpreesion
   ```

   et saisissez l’expression d’arrondi.

   Cela arrondit le nombre d’heures budgétisées à un certain nombre de décimales que vous spécifiez.

   Pour plus d’informations sur la manière d’arrondir un nombre dans Workfront, consultez l’article [Présentation des expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Facultatif) Cliquez sur **Ajouter une colonne** pour ajouter des colonnes supplémentaires.
1. (Facultatif) Pour faciliter la lecture du rapport, il est recommandé d&#39;y ajouter un groupement. Nous proposons le regroupement suivant :

   Cliquez sur l’onglet **Groupings** , puis effectuez une ou plusieurs des opérations suivantes :

   1. Cliquez sur **Ajouter un groupement** et commencez à saisir &quot;Nom du projet&quot;, puis sélectionnez-le lorsqu’il apparaît dans la liste.
   1. Cliquez sur **Ajouter un groupement** et commencez à saisir &quot;Nom du rôle de la tâche&quot;, puis sélectionnez-le lorsqu’il apparaît dans la liste.
   1. Cliquez sur **Ajouter un regroupement** et commencez à saisir **Date d’affectation**, sélectionnez-la lorsqu’elle apparaît dans la liste, puis sélectionnez la période par laquelle vous souhaitez regrouper dans le champ **Dates de groupe par**.

1. (Facultatif) Cliquez sur **Filtres** pour ajouter des filtres au rapport.
1. (Facultatif) Cliquez sur **Graphique** pour ajouter un graphique au rapport.
1. Cliquez sur **Enregistrer + Fermer**.

## Révision du rapport Heure budgétisée

Par défaut, les informations suivantes sont disponibles dans le rapport Heure budgétée :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Projet </td> 
   <td>Il s’agit du nom du projet associé à l’Heure budgétaire.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Rôle de tâche</p> </td> 
   <td>Il s’agit du nom du rôle de tâche associé à l’Heure budgétaire. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">l’utilisateur ou de l’utilisatrice</td> 
   <td>Il s’agit du nom de l’utilisateur associé à l’Heure budgétée.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Date alloc.</td> 
   <td> <p>Il s’agit de la date d’attribution. Il s’agit du premier jour de la semaine (un dimanche) pour lequel vous avez budgété les heures.</p> <p>Conseil :  <p>Si une semaine s’étend sur deux mois, elle génère deux lignes dans le rapport : l’une correspondant au premier jour de la semaine (le dimanche de la semaine qui se trouve pendant le premier mois), l’autre correspondant au premier jour du deuxième mois (et qui peut être n’importe quel jour de la semaine).</p> <p>Si, par exemple, vous allouez 8 heures à un utilisateur pour la semaine du 30 juin (dimanche) au 6 juillet (samedi), les deux lignes indiquent une date d’attribution du 30 juin et du 1er juillet.</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Hrs budgétées</td> 
   <td>Il s’agit des heures budgétées allouées à l’utilisateur dans le planificateur de ressources.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pln. Hrs budgétées</td> 
   <td>Il s’agit des heures budgétées allouées au rôle de tâche ou au projet dans le planificateur de ressources.</td> 
  </tr> 
 </tbody> 
</table>
