---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Regroupement : tâches par Portfolio, programme et projet'
description: Utilisez ce regroupement de tâches pour classer les tâches par portfolio, programme, puis par projet auxquels elles sont liées.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fdad6a1-54b3-4d3e-8f21-4f2efc2dc27a
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 74%

---

# Regroupement : tâches par portfolio, programme et projet

<!--Audited: 10/2024-->

Utilisez ce regroupement de tâches pour classer les tâches par portfolio, programme, puis par projet auxquels elles sont liées.

![Regroupement de projets du programme Portfolio](assets/portfolio-program-project-grouping-for-tasks-350x120.png)

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

## Regrouper les tâches par portfolio, programme et projet

Pour appliquer ce regroupement :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.
1. Cliquez sur **Ajouter un regroupement**.

1. Cliquez sur **Passer en mode texte**.
1. Supprimez le texte de la zone **Regrouper par**.
1. Remplacez le texte par le code suivant :

   ```
   group.0.linkedname=project
   group.0.namekey=portfolio
   group.0.notime=false
   group.0.valuefield=project:portfolio:name
   group.0.valueformat=string
   group.1.linkedname=project
   group.1.namekey=program
   group.1.notime=false
   group.1.valuefield=project:program:name
   group.1.valueformat=string
   group.2.name=Project
   group.2.valuefield=project:name
   group.2.valueformat=HTML
   textmode=true
   ```

1. Cliquez sur **Terminé** > **Enregistrer le regroupement**.
1. (Facultatif) Mettez à jour le nom du regroupement, puis cliquez sur **Enregistrer le regroupement**.

