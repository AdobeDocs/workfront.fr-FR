---
content-type: reference
product-area: reporting;projects
keywords: calculé, agrégats, avancé, vues
navigation-topic: custom-view-filter-and-grouping-samples
title: "Regroupement : affiche le résultat de l’agrégation de plusieurs valeurs calculées dans un groupement"
description: Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs dans la vue d’un rapport ou d’une liste. Chaque ligne affiche le calcul pour chaque objet du rapport ou de la liste.
author: Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 83%

---

# Regroupement : afficher le résultat de l’agrégation de plusieurs valeurs calculées dans un regroupement.

<!--Audited: 10/2024-->

Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs dans la vue d’un rapport ou d’une liste. Chaque ligne affiche le calcul pour chaque objet du rapport ou de la liste.

Par exemple, vous pouvez afficher la différence entre les heures effectives et les heures prévues dans une troisième colonne appelée Proportion de travail pour chaque tâche dans un rapport de tâches. Pour plus d’informations sur les expressions de données calculées, consultez [Vue d’ensemble des expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Vous pouvez afficher la valeur agrégée de plusieurs éléments d’affichage calculés dans la même colonne d’un regroupement en ajoutant un calcul à la ligne `aggregator` de la colonne qui contient la valeur calculée. Par exemple, vous pouvez agréger (afficher la somme) le nombre d’heures de la proportion de travail de toutes les tâches dans le regroupement du rapport ou la liste de la colonne Proportion de travail. Cet article décrit comment réaliser cette opération.

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

## Afficher le résultat de l’agrégation de plusieurs valeurs calculées dans un regroupement

1. Accédez à un rapport de tâches, cliquez sur **Actions de rapport** > **Modifier**.
1. Dans l&#39;onglet **Groupings**, cliquez sur **Ajouter un groupement**, puis commencez à saisir **Nom du projet** dans le champ **Grouper par**, puis sélectionnez **Projet > Nom** lorsqu&#39;il s&#39;affiche dans la liste.

1. Dans l’onglet **Colonnes (Affichage)**, cliquez sur **Ajouter une colonne**, puis saisissez le **Nombre d’heures prévues** dans le champ **Afficher dans cette colonne**, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

   >[!TIP]
   >
   >Commencez toujours par ajouter autant d’informations que possible à l’aide de l’interface standard avant de modifier les informations en mode texte. Ajoutez les champs qui se rapprochent le plus du calcul que vous essayez d’effectuer ou qui contiennent le plus d’informations sur celui-ci.

1. Dans le champ **Résumer cette colonne par** , sélectionnez **Somme**.
1. Cliquez sur **Passer en mode Texte** dans la colonne que vous avez ajoutée, puis cliquez sur **Modifier le mode Texte**.
1. Remplacez le texte de la zone par l’exemple de mode de texte suivant :

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >Pour que la valeur agrégée dans le regroupement affiche la différence agrégée entre les champs Nombre d’heures prévues et Heures effectives, saisissez la même équation dans la ligne `aggregator.valuefield`. L’élément `aggregator.displayformat` utilisé pour la colonne Nombre d’heures prévues convertit les minutes en heures. Étant donné que le champ Nombre d’heures prévues était utilisé comme espace de substitution, cette ligne n’a pas besoin d’être modifiée.
   >
   >
   >La définition `minutesAsHoursString` de la ligne `aggregator.displayformat` signifie qu’il n’est pas nécessaire de diviser chaque champ par 60 pour les résultats comme c’est le cas pour `valueexpression`. Ainsi, `aggregator.valuefield=workRequired` devient : `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.
1. Cliquez sur **Terminé**.
1. Cliquez sur **Enregistrer et fermer**.
