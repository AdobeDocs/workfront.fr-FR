---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Afficher : afficher le nom des tâches parentes en tant que toutes les majuscules"
description: Vous pouvez ajouter cette colonne à une vue de tâche pour afficher le nom des tâches parent en majuscules.
author: Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: a7cdee912e5047f1c8ef224aff6a41eaa3633df6
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 74%

---

# Vue : afficher le nom des tâches parent en majuscules

<!--Audited: 10/2024-->

Vous pouvez ajouter cette colonne à une vue de tâche pour afficher le nom des tâches parent en majuscules.

![](assets/column-task-with-all-caps-parent-350x112.png)

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

## Afficher le nom des tâches parent en majuscules

Pour créer cette colonne dans une vue de tâche :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Affichage**, sélectionnez une vue, puis cliquez sur l&#39;icône **Modifier** ![](assets/edit-icon.png).
Ou\
   Dans le menu déroulant **Vue**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, cliquez sur l’en-tête de la colonne qui indique le nom de la tâche dans la liste.
1. Cliquez sur **Passer en mode Texte**, puis sur **Modifier le mode Texte**.
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
