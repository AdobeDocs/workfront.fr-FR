---
content-type: reference
product-area: reporting;projects
keywords: calculate,agrégats,advanced,views
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Groupement : affiche le résultat de l''agrégation de plusieurs valeurs calculées dans un groupement'''
description: Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs dans la vue d'un rapport ou d'une liste. Chaque ligne affiche le calcul de chaque objet du rapport ou de la liste.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 23%

---

# Regroupement : afficher le résultat de l’agrégation de plusieurs valeurs calculées dans un regroupement

Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs dans la vue d&#39;un rapport ou d&#39;une liste. Chaque ligne affiche le calcul de chaque objet du rapport ou de la liste.

Par exemple, vous pouvez afficher la différence entre les Heures réelles et les Heures planifiées dans une troisième colonne appelée Équilibrage du travail pour chaque tâche dans un rapport de tâche. Pour plus d’informations sur les expressions de données calculées, voir [Présentation des expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Vous pouvez afficher la valeur agrégée de plusieurs éléments de vue calculée dans la même colonne d’un groupement en ajoutant un calcul à la ligne `aggregator` de la colonne contenant la valeur calculée. Par exemple, vous pouvez agréger (afficher la somme de) la somme des heures de l&#39;Équilibre du travail de toutes les tâches du groupement du rapport ou de la liste de la colonne Équilibre du travail. Cet article décrit la procédure à suivre.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demande de modification d’un groupement </p>
   <p>Prévoir la modification d’un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Editer l'accès aux Filtres, Vues, Groupements pour modifier un groupement</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher le résultat de l&#39;agrégation de plusieurs valeurs calculées dans un groupement

1. Accédez à un rapport de tâche, cliquez sur **Actions de rapport** > **Modifier**.
1. Dans l’onglet **Groupings**, cliquez sur **Ajouter un groupement**, puis commencez à saisir **Nom du projet** dans le champ **Regrouper votre rapport** > **Premier par**, puis sélectionnez-le lorsqu’il s’affiche dans la liste.

1. Dans l&#39;onglet **Columns(View)**, cliquez sur **Ajouter une colonne**, puis commencez à saisir **Heures planifiées** dans le champ **Afficher dans cette colonne**, puis sélectionnez-le lorsqu&#39;il s&#39;affiche dans la liste.

   >[!TIP]
   >
   >Commencez toujours à ajouter autant d’informations à l’aide de l’interface Standard avant de modifier les informations en mode texte. Ajoutez les champs les plus proches ou contenant le plus d&#39;informations que vous souhaitez obtenir pour le calcul que vous essayez d&#39;effectuer.

1. Dans le champ **Résumer cette colonne par** , sélectionnez **Somme**, puis cliquez sur **Terminé**.
1. Cliquez sur **Passer en mode Texte** dans la colonne que vous avez ajoutée.
1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Remplacez les lignes `valuefield ` et `aggregator.valuefield` par les lignes surlignées dans l’exemple de mode de texte suivant :

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
   >Pour obtenir la valeur agrégée dans le groupement afin d’afficher la différence agrégée entre les champs Heures planifiées et Heures réelles , saisissez la même équation dans la ligne `aggregator.valuefield`. La colonne `aggregator.displayformat` utilisée pour les heures planifiées convertit les minutes en heures. Comme le champ Heures planifiées a été utilisé comme espace réservé, cette ligne n’a pas besoin d’être ajustée.
   >
   >
   >La définition `minutesAsHoursString` de la ligne `aggregator.displayformat` signifie qu’il n’est pas nécessaire de diviser chaque champ par 60, comme cela a été fait sur `valueexpression` pour les résultats. Dans cet `aggregator.valuefield=workRequired` devient : `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Cliquez sur **Enregistrer+Fermer**.
