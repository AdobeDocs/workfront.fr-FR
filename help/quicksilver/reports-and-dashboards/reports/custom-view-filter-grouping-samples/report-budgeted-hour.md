---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Rapport : heure budgétée'
description: 'Rapport : heure budgétée'
author: Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 73%

---

# Rapport : heure budgétée

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

Lorsque vous souhaitez partager des informations sur les heures budgétées avec d’autres personnes qui n’ont pas accès au planificateur de ressources, vous pouvez le faire en créant un rapport sur les heures budgétées. Vous pouvez ensuite partager le rapport avec elles.

>[!IMPORTANT]
>
>Les heures budgétées sont normalement mises à jour toutes les heures (rarement, il peut s’écouler un maximum de trois heures) dans la base de données Adobe Workfront. L’actualisation du rapport n’actualise pas nécessairement les informations horaires qu’il contient. Vous pouvez afficher le délai écoulé depuis la dernière mise à jour dans le coin supérieur droit de chaque rapport Heures budgétées. L’actualisation du rapport actualise les informations qu’il contient uniquement lorsqu’il s’est écoulé plus d’une heure depuis la dernière mise à jour.
>
>![Avertissement de synchronisation de l&#39;heure du rapport des heures budgétées](assets/budgeted-hour-report-time-sync-warning-350x74.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> 
    <p>Nouveau :</p>
   <ul><li><p>Contributeur pour modifier un filtre </p></li>
   <li><p>Standard pour modifier un rapport</p></li> </ul>

<p>Actuel :</p>
   <ul><li><p>Demande de modification d’un filtre </p></li>
   <li><p>Prévoir de modifier un rapport</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, aux vues et aux regroupements pour modifier un filtre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer un rapport Heures budgétées

1. Cliquez sur l&#39;icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit, ou sur l&#39;icône **Menu principal** ![lignes du menu principal](assets/lines-main-menu.png) dans le coin supérieur gauche, le cas échéant, puis cliquez sur **Rapports**.

1. Cliquez sur **Nouveau rapport** > **Plus** > **Heure budgétée**.

   La vue par défaut est appliquée au rapport.

1. (Facultatif) Pour faciliter la lecture du rapport, cliquez sur le bouton **. Heures** colonne, puis **Passer en mode texte**, puis cliquez sur **Modifier le mode texte**.
1. Remplacez la ligne `valuefield` par `valueexpreesion` et saisissez l’expression d’arrondi.

   Cela arrondit le nombre d’heures budgétées à un certain nombre de décimales que vous spécifiez.

   Pour plus d’informations sur la manière d’arrondir un nombre dans Workfront, voir l’article [Vue d’ensemble des expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. Cliquez sur **Terminé**.
1. (Facultatif) Cliquez sur **Ajouter une colonne** pour ajouter des colonnes supplémentaires.
1. (Facultatif) Pour faciliter la lecture du rapport, il est recommandé d’y ajouter un regroupement. Nous proposons le regroupement suivant :

   Cliquez sur l’onglet **Regroupements**, puis effectuez une ou plusieurs des opérations suivantes :

   * Cliquez sur **Ajouter un regroupement** et commencez à saisir « Nom du projet », puis sélectionnez-le lorsqu’il apparaît dans la liste.
   * Cliquez sur **Ajouter un regroupement** et commencez à saisir « Nom de la fonction », puis sélectionnez-la lorsqu’elle apparaît dans la liste.
   * Cliquez sur **Ajouter un regroupement** et commencez à saisir « Date d’affectation », sélectionnez-la lorsqu’elle apparaît dans la liste, puis sélectionnez la période selon laquelle vous souhaitez regrouper dans le champ **Regrouper les dates par**.

1. (Facultatif) Cliquez sur **Filtres** pour ajouter des filtres au rapport.
1. (Facultatif) Cliquez sur **Graphique** pour ajouter un graphique au rapport.
1. Cliquez sur **Enregistrer + Fermer**.

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
