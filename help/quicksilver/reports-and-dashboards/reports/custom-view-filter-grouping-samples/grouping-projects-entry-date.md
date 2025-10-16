---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Regroupement : Projets par date de saisie'
description: Dans ce regroupement personnalisé de projets, vous pouvez afficher les projets regroupés par leurs valeurs Date d’entrée.
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 77%

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

## Regrouper les projets par date d’entrée

Pour appliquer ce regroupement :

1. Accédez à un rapport de projet existant ou créez un nouveau rapport de projet.\
   Pour plus d’informations sur la création d’un rapport, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Cliquez sur **Actions du rapport** > **Modifier**.
1. Dans l’onglet **Regroupement**, cliquez sur **Ajouter un regroupement**.
1. Cliquez sur **Basculer en mode texte**.
1. Supprimez le texte de la zone **Regrouper par**.
1. Remplacez le texte par le code suivant :


   ```
   group.0.linkedname=direct
   group.0.name=Project Entry
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))
   group.0.valueformat=atDateAsMonthString
   textmode=true
   ```

1. Cliquez sur **Terminé** > **Enregistrer le regroupement**.
1. (Facultatif) Mettez à jour le nom du regroupement, puis cliquez sur **Enregistrer le regroupement**.
