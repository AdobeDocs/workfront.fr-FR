---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Regroupement : organise les résultats de la liste selon une valeur calculée commune à tous les objets du regroupement.'
description: Vous pouvez afficher vos tâches groupées par « Pourcentage d’achèvement » dans des fourchettes de 0 à 25, 26 à 50, 51 à 75, 75 à 99 et 100. Pour ce faire, vous pouvez créer un regroupement en mode texte.
author: Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 81%

---

# Regroupement : organise les résultats de la liste en fonction d’une valeur calculée commune à tous les objets du regroupement.

<!--Audited: 10/2024-->

Vous pouvez afficher vos tâches groupées par « Pourcentage d’achèvement » dans des fourchettes de 0 à 25, 26 à 50, 51 à 75, 75 à 99 et 100. Pour ce faire, vous pouvez créer un regroupement en mode texte.

![Regroupement par valeur calculée](assets/grouping-calculated-value-column-to-all-objects.png)

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

## Organiser les résultats d’une liste en fonction d’une valeur calculée commune à tous les objets du regroupement

Pour appliquer ce regroupement à une liste de tâches :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Regroupement**, sélectionnez **Nouveau regroupement**.

1. Cliquez sur **Basculer en mode texte**.
1. Dans l’espace disponible, ajoutez le code suivant :

   ```
   textmode=true
   group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({percentComplete}>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))
   group.0.linkedname=direct
   group.0.valueformat=doubleAsString
   group.0.namekey=percentComplete
   ```

1. Cliquez sur **Terminé**, puis sur **Enregistrer le regroupement**.
1. (Facultatif) Mettez à jour le nom du regroupement, puis cliquez sur **Enregistrer le regroupement**.
