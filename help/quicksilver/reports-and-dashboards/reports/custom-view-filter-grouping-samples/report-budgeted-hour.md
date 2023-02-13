---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Rapport : Heure budgétée'''
description: 'Rapport : Heure budgétée'''
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# Rapport : Heure budgétée

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

Lorsque vous souhaitez partager des informations sur l’heure budgétée avec d’autres utilisateurs qui n’ont pas accès au planificateur de ressources, vous pouvez le faire en créant un rapport sur l’heure planifiée. Vous pouvez ensuite partager le rapport avec eux.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>Les heures budgétisées sont mises à jour toutes les heures dans la base de données Adobe Workfront. L’actualisation du rapport n’actualise pas nécessairement les informations horaires qu’il contient. Vous pouvez afficher le délai écoulé depuis la dernière mise à jour dans le coin supérieur droit de chaque rapport Heure budgétaire . L&#39;actualisation du rapport actualise les informations qu&#39;il contient uniquement lorsqu&#39;il y a eu plus d&#39;une heure depuis la dernière mise à jour.
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Création d’un rapport Heure planifiée

1. Cliquez sur le bouton **Menu Principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit, puis cliquez sur **Rapports**.

1. Cliquez sur **Nouveau Rapport > Heure budgétée**.

   La vue par défaut est appliquée au rapport.

1. (Facultatif) Pour faciliter la lecture du rapport, cliquez sur le bouton **Heures budgétées** colonne, puis **Passer en mode Texte**, puis modifiez la variable

   ```
   valuefield
   ```

   line vers

   ```
   valueexpreesion
   ```

   et saisissez l’expression d’arrondi.

   Cela arrondit le nombre d’heures budgétisées à un certain nombre de décimales que vous spécifiez.

   Pour plus d’informations sur la manière d’arrondir un nombre dans Workfront, reportez-vous à l’article . [Expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. (Facultatif) Cliquez sur **Ajouter une colonne** pour ajouter des colonnes supplémentaires.
1. (Facultatif) Pour faciliter la lecture du rapport, il est recommandé d&#39;y ajouter un groupement. Nous proposons le regroupement suivant :

   Cliquez sur le bouton **Groupements** , puis effectuez une ou plusieurs des opérations suivantes :

   1. Cliquez sur **Ajouter un groupement** et commencez à saisir &quot;Nom du projet&quot;, puis sélectionnez-le lorsqu’il apparaît dans la liste.
   1. Cliquez sur **Ajouter un groupement** et commencez à saisir &quot;Nom du rôle de la tâche&quot;, puis sélectionnez-le lorsqu’il apparaît dans la liste.
   1. Cliquez sur **Ajouter un groupement** et commencez à taper **Date d’affectation**, sélectionnez-le lorsqu’il apparaît dans la liste, puis sélectionnez la période de regroupement à partir du **Regrouper les dates par** champ .

1. (Facultatif) Cliquez sur **Filtres** pour ajouter des filtres au rapport.
1. (Facultatif) Cliquez sur **Graphique** pour ajouter un graphique au rapport.
1. Cliquez sur **Enregistrer + Fermer**.

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
   <td role="rowheader">Utilisateur</td> 
   <td>Il s’agit du nom de l’utilisateur associé à l’Heure budgétée.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Alloc. Date</td> 
   <td> <p>Il s’agit de la date d’attribution. Il s’agit du premier jour de la semaine (un dimanche) pour lequel vous avez budgété les heures.</p> <p>Conseil :  <p>Si une semaine s’étend sur deux mois, elle génère deux lignes dans le rapport : un correspondant au premier jour de la semaine (le dimanche de la semaine qui se trouve pendant le premier mois), et un second correspondant au premier jour du deuxième mois (et qui peut être n’importe quel jour de la semaine).</p> <p>Si, par exemple, vous allouez 8 heures à un utilisateur pour la semaine du 30 juin (dimanche) au 6 juillet (samedi), les deux lignes indiquent une date d’attribution du 30 juin et du 1er juillet.</p> </p> </td> 
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
