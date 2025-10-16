---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Regroupement : Répartition en pourcentage du projet 2'
description: 'Dans ce regroupement de projets personnalisé, vous pouvez afficher les projets regroupés selon une plage de valeurs de pourcentage terminé. Les répartitions affichent une valeur de pourcentage d’achèvement de 10 incréments de point de pourcentage : 0 à 10 %, 11 à 20 %, 21 à 30 %, etc.'
author: Nolan
feature: Reports and Dashboards
exl-id: 7845fd66-8304-4154-8630-e72482cd753f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 71%

---

# Regroupement : répartition en pourcentage des projets (2)

<!--Audited: 10/2024-->

Dans ce regroupement de projets personnalisé, vous pouvez afficher les projets regroupés selon une plage de valeurs de pourcentage terminé. Les répartitions affichent une valeur de pourcentage d’achèvement de 10 incréments de point de pourcentage : 0 à 10 %, 11 à 20 %, 21 à 30 %, etc.

Le regroupement suivant classe les projets par valeur de pourcentage terminé dans l’un de ces regroupements :

* 0%
* 1-10 %
* 11-20 %
* 21-30 %
* 31-40 %
* 41-50 %
* 51-60 %
* 61-70 %
* 71-80 %
* 81-90 %
* 91-99 %
* 100%

![percent_complete_breakdown_for_projects_in_10__increments.png](assets/percent-complete-breakdown-350x94.png)

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

## Regrouper par répartition des projets en pourcentage

Pour appliquer ce regroupement :

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.

1. Cliquez sur **Basculer en mode texte**.
1. Supprimez le texte de la zone et collez le code suivant dans l’espace disponible :

   ```
   group.0.linkedname=direct
   group.0.name=Percent Breakdown
   group.0.notime=false
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=11,"1-10 %",IF({percentComplete}<=21,"11-20 %",IF({percentComplete}<=31,"21-30 %",IF({percentComplete}<41,"31-40 %",IF({percentComplete}<51,"41-50 %",IF({percentComplete}<61,"51-60 %",IF({percentComplete}<71,"61-70 %",IF({percentComplete}<81,"71-80 %",IF({percentComplete}<91,"81-90 %",IF({percentComplete}<100,"91-99 %","100 %")))))))))))
   textmode=true
   ```

1. Cliquez sur **Terminé** > **Enregistrer le regroupement**.
1. (Facultatif) Mettez à jour le nom du regroupement, puis cliquez sur **Enregistrer le regroupement**.
