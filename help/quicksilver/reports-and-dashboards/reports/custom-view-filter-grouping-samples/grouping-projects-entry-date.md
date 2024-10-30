---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Groupement : projets par date d’entrée"
description: Dans ce regroupement personnalisé de projets, vous pouvez afficher les projets regroupés par leurs valeurs Date d’entrée.
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: a6874c3a2dfda02b8a25f78056767d8c59c888e9
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 80%

---

# Regroupement : projets par date d’entrée

<!--Audited: 10/2024-->

Dans ce regroupement personnalisé de projets, vous pouvez afficher les projets regroupés par leurs valeurs Date d’entrée.

Chaque regroupement affiche les projets avec une date d’entrée :

* des 30 derniers jours ;
* entre 30 et 60 jours ;
* supérieure ou égale à 60 jours.

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
   <ul><li><p>Contributeur à la modification d’un filtre </p></li>
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

*Pour plus d’informations, voir [Exigences d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Regrouper les projets par date d’entrée

Pour appliquer ce regroupement :

1. Accédez à un rapport de projet existant ou créez un nouveau rapport de projet.\
   Pour plus d’informations sur la création d’un rapport, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Cliquez sur **Actions de rapport** > **Modifier**.
1. Dans l’onglet **Regroupement**, cliquez sur **Ajouter un regroupement**.
1. Cliquez sur **Basculer en mode texte**.
1. Supprimez le texte dans la zone **Group by**.
1. Remplacez le texte par le code suivant :


   ```
   group.0.linkedname=direct
   group.0.name=Project Entry
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))
   group.0.valueformat=atDateAsMonthString
   textmode=true
   ```

1. Cliquez sur **Done** > **Save Grouping**.
1. (Facultatif) Mettez à jour le nom du groupement, puis cliquez sur **Enregistrer le groupement**.
