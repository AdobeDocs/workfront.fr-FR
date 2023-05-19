---
content-type: reference
product-area: reporting;projects
keywords: calculate,agrégats,advanced,views
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Groupement : afficher le résultat de l''agrégation de plusieurs valeurs calculées dans un groupement"'
description: Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs dans la vue d'un rapport ou d'une liste. Chaque ligne affiche le calcul de chaque objet du rapport ou de la liste.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Regroupement : afficher le résultat de l&#39;agrégation de plusieurs valeurs calculées dans un groupement ;

Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs dans la vue d&#39;un rapport ou d&#39;une liste. Chaque ligne affiche le calcul de chaque objet du rapport ou de la liste.

Par exemple, vous pouvez afficher la différence entre les Heures réelles et les Heures planifiées dans une troisième colonne appelée Équilibrage du travail pour chaque tâche dans un rapport de tâche. Pour plus d’informations sur les expressions de données calculées, voir [Expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

Vous pouvez afficher la valeur agrégée de plusieurs éléments de vue calculée dans la même colonne d’un groupement en ajoutant un calcul au `aggregator` ligne de la colonne contenant la valeur calculée. Par exemple, vous pouvez agréger (afficher la somme de) la somme des heures de l&#39;Équilibre du travail de toutes les tâches du groupement du rapport ou de la liste de la colonne Équilibre du travail. Cet article décrit comment procéder.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers</p> <p>Modifier l’accès aux filtres, vues et groupes</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Afficher le résultat de l&#39;agrégation de plusieurs valeurs calculées dans un groupement

1. Accédez à un rapport de tâche, puis cliquez sur **Actions de rapport** > **Modifier**.
1. Dans le **Groupements** , cliquez sur **Ajouter un groupement**, puis commencez à taper **Nom du projet** dans le **Regrouper votre rapport** > **First by** puis sélectionnez-la lorsqu’elle s’affiche dans la liste.

1. Dans le **Colonnes (vue)** , cliquez sur **Ajouter une colonne**, puis commencez à taper **Heures planifiées** dans le **Afficher dans cette colonne** puis sélectionnez-la lorsqu’elle s’affiche dans la liste.

   >[!TIP]
   >
   >Commencez toujours à ajouter autant d’informations à l’aide de l’interface Standard avant de modifier les informations en mode texte. Ajoutez les champs les plus proches ou contenant le plus d&#39;informations que vous souhaitez obtenir pour le calcul que vous essayez d&#39;effectuer.

1. Dans le **Résumer cette colonne par** champ, sélectionnez **Somme**, puis cliquez sur **Terminé**.
1. Cliquez sur **Passer en mode Texte** dans la colonne que vous avez ajoutée.
1. Pointez sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Remplacez la variable `valuefield ` et le `aggregator.valuefield` lignes avec les lignes surlignées dans l’exemple de mode texte suivant :

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
   >Pour obtenir la valeur agrégée dans le groupement afin d’afficher la différence agrégée entre les champs Heures planifiées et Heures réelles , saisissez la même équation dans la variable `aggregator.valuefield` ligne. Le `aggregator.displayformat` utilisé pour la colonne Heures planifiées convertit les minutes en heures. Comme le champ Heures planifiées a été utilisé comme espace réservé, cette ligne n’a pas besoin d’être ajustée.
   >
   >
   >Le `minutesAsHoursString` définition de la variable `aggregator.displayformat` ligne signifie qu’il n’est pas nécessaire de diviser chaque champ par 60, comme c’est le cas sur la ligne `valueexpression` pour les résultats. Dans ce `aggregator.valuefield=workRequired` devient : `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. Cliquez sur **Enregistrer + Fermer**.
