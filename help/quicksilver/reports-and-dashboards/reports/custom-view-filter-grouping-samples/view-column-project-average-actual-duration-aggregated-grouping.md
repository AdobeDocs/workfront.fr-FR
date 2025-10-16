---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher et regrouper : affiche la durée réelle du projet agrégée par la moyenne dans un regroupement.'
description: Vous pouvez ajouter la colonne suivante dans un rapport sur les projets afin d’afficher la durée effective agrégée sous la forme d’une moyenne dans un regroupement.
author: Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 36%

---

# Afficher et regrouper : affiche la durée réelle du projet agrégée par la moyenne dans un regroupement.

<!--Audited: 11/2024-->

Vous pouvez ajouter la colonne suivante dans une vue de projet pour afficher la durée réelle agrégée en moyenne dans un regroupement.

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou demande de modification d’un filtre </p>
   <p>Standard ou Plan pour modifier un rapport</p>
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

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher la durée réelle du projet agrégée par la moyenne dans un regroupement

Pour ajouter cette colonne à une vue de projet, procédez comme suit :

1. Accédez à une liste de projets.
1. (Obligatoire) Pour afficher la valeur moyenne agrégée de la durée réelle du projet, vous devez ajouter un regroupement à votre liste de projets.\
   Pour plus d’informations sur la création de regroupements, consultez l’article [Présentation des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
1. Développez le menu déroulant **Affichage** et sélectionnez **Personnaliser l’affichage**.
1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Basculer en mode texte**, puis sur **Modifier le mode texte**.
1. Supprimez tout le texte de la zone **Modifier le mode texte** et remplacez-le par le code suivant :

   ```
   aggregator.displayformat=compound 
   aggregator.function=AVG 
   aggregator.namekey=view.relatedcolumn 
   aggregator.namekeyargkey=actualduration 
   aggregator.valuefield=actualDurationMinutes 
   aggregator.valueformat=val 
   displayname=Project Actual Duration 
   durationunitfield=durationUnit.value 
   linkedname=project 
   namekey=actualduration 
   namekeyargkey=actualduration 
   querysort=actualDurationMinutes 
   textmode=true 
   valuefield=actualDurationMinutes 
   valueformat=compound#M:D 
   viewalias=actualduration
   ```

1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.
1. (Facultatif) Mettez à jour le nom de la vue, puis cliquez sur **Enregistrer la vue**.
