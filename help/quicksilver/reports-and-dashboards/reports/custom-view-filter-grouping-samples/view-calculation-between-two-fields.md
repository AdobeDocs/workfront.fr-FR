---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : afficher le résultat d’un calcul entre deux champs d’une colonne »'
description: Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: ecce7484423419823effa2cb41da892ba3fb207c
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 91%

---

# Vue : afficher le résultat d’un calcul entre deux champs d’une colonne

<!--Audited: 11/2024-->

Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs.

Par exemple, si vous souhaitez connaître le nombre de jours de la semaine écoulés entre deux dates, vous pouvez utiliser la syntaxe du mode texte et les expressions de données pour calculer cette différence.\
Par exemple, vous pouvez calculer la différence de jours de la semaine entre la date d’achèvement prévue et la date d’achèvement effective d’une tâche et afficher le résultat dans une colonne.

Vous pouvez utiliser deux autres dates dans ce calcul (date de début effective, d’achèvement effective, de début prévisionnelle, d’achèvement prévisionnelle, etc.).\
Pour plus d’informations sur les expressions de données calculées, consultez [Vue d’ensemble des expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

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


## Afficher le résultat d’un calcul entre deux champs d’une colonne

Pour ajouter cette colonne à une vue de tâche, procédez comme suit :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**, puis **Basculer vers le mode Texte** > **Modifier le mode Texte**.
1. Supprimez le texte qui se trouve dans la zone **Mode texte** et remplacez-le par le code suivant :

   ```
   displayname=Week Day Difference
   textmode=true
   valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})
   valueformat=HTML
   ```

1. (Facultatif) Pour agréger les valeurs affichées dans la vue d’un regroupement, procédez comme décrit dans [Regroupement : afficher le résultat de l’agrégation de plusieurs valeurs calculées dans un regroupement](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.
