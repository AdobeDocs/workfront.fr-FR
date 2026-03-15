---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher et regrouper : afficher la durée réelle du projet agrégée par la moyenne dans un regroupement'
description: Vous pouvez ajouter la colonne suivante dans un rapport sur les projets afin d’afficher la durée effective agrégée sous la forme d’une moyenne dans un regroupement.
author: Courtney
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 42%

---

# Vue et regroupement : affichage de la durée effective du projet agrégée par la moyenne dans un regroupement

<!--Audited: 11/2024-->

Vous pouvez ajouter la colonne suivante dans une vue de projet pour afficher la durée réelle agrégée en tant que moyenne dans un regroupement.

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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
   Pour plus d&#39;informations sur la création de groupes, consultez l&#39;article [Présentation des groupes dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
1. Développez le menu déroulant **Affichage** et sélectionnez **Personnaliser l&#39;affichage**.
1. Cliquez sur **Ajouter une colonne**.
1. Cliquez sur **Passer en mode Texte**, puis cliquez sur **Modifier le mode Texte**.
1. Supprimez tout le texte dans la zone **Modifier le mode texte** et remplacez-le par le code suivant :

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
