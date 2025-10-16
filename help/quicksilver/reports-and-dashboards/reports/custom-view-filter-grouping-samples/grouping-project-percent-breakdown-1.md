---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Regroupement : Répartition en pourcentage du projet 1'
description: Dans ce regroupement de projets personnalisé, vous pouvez afficher les projets regroupés selon une plage de valeurs de pourcentage terminé.
author: Nolan
feature: Reports and Dashboards
exl-id: 7cdc8e56-3486-4e78-b494-b2ba9389c1f7
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 75%

---

# Regroupement : répartition en pourcentage du projet 1

<!--Audited: 10/2024-->

Dans ce regroupement de projets personnalisé, vous pouvez afficher les projets regroupés selon une plage de valeurs de pourcentage terminé. Les répartitions affichent une valeur de pourcentage d’achèvement de 25 points de pourcentage par incréments : 0 à 25 %, 26 à 50 %, 51 à 75 %, etc.

Le regroupement suivant classe les projets par valeur de pourcentage terminé dans l’un de ces regroupements :

* 0%
* 1 % à 25 %
* 26 % à 50 %
* 51 % à 75 %
* 76 % à 99 %
* 100%

![percent_complete_breakdown_custom_project_grouping_25__increments.png](assets/percent-complete-breakdown-custom-350x56.png)

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
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=26,"0-25 %",IF({percentComplete}<=51,"26-50 %",IF({percentComplete}<=76,"51-75 %",IF({percentComplete}<100,"76-99 %","100 %")))))
   group.0.valueformat=string
   ```

1. Cliquez sur **Terminé** > **Enregistrer le regroupement**.
1. (Facultatif) Mettez à jour le nom du regroupement, puis cliquez sur **Enregistrer le regroupement**.
