---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : afficher les majuscules pour le nom des tâches parents'
description: Vous pouvez ajouter cette colonne à une vue de tâche pour afficher le nom des tâches parent en majuscules.
author: Courtney
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/WYEh0h4BI8XzeV1TLSOix9-fgg33etfitS7U4rczXgo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 244
ht-degree: 69%

---

# Vue : afficher le nom des tâches parent en majuscules

<!--Audited: 10/2024-->

Vous pouvez ajouter cette colonne à une vue de tâche pour afficher le nom des tâches parent en majuscules.

![Colonne avec tâche parent en majuscules](assets/column-task-with-all-caps-parent-350x112.png)

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

## Afficher le nom des tâches parent en majuscules

Pour créer cette colonne dans une vue de tâche :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, sélectionnez une vue, puis cliquez sur l&#39;icône **Modifier** ![Icône Modifier](assets/edit-icon.png).
Ou\
   Dans le menu déroulant **Vue**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu de la colonne**, cliquez sur l’en-tête de la colonne qui affiche le nom de la tâche dans la liste.
1. Cliquez sur **Basculer en mode texte** puis sur **Modifier le mode texte**.
1. Supprimez le texte qui se trouve dans la zone **Mode texte** et remplacez-le par le code suivant :

   ```
   linkedname=direct
   namekey=name
   querysort=name
   styledef.case.0.comparison.icon=false
   styledef.case.0.comparison.leftmethod=numberOfChildren
   styledef.case.0.comparison.lefttext=numberOfChildren
   styledef.case.0.comparison.operator=gt
   styledef.case.0.comparison.operatortype=int
   styledef.case.0.comparison.righttext=0
   styledef.case.0.comparison.trueproperty.0.name=fontstyle
   styledef.case.0.comparison.trueproperty.0.value=bold
   valueexpression=IF({numberOfChildren}>"0",UPPER({name}),{name})
   valueformat=HTML
   ```

1. Cliquez sur **Terminé**, puis cliquez sur **Enregistrer l’affichage**.
