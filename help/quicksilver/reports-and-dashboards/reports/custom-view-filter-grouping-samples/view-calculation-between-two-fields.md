---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : afficher le résultat d’un calcul entre deux champs d’une colonne »'
description: Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 100%

---

# Vue : afficher le résultat d’un calcul entre deux champs d’une colonne

Vous pouvez utiliser le mode texte dans une colonne pour afficher un calcul entre deux champs.

Par exemple, si vous souhaitez connaître le nombre de jours de la semaine écoulés entre deux dates, vous pouvez utiliser la syntaxe du mode texte et les expressions de données pour calculer cette différence.\
Par exemple, vous pouvez calculer la différence de jours de la semaine entre la date d’achèvement prévue et la date d’achèvement effective d’une tâche et afficher le résultat dans une colonne.

Vous pouvez utiliser deux autres dates dans ce calcul (date de début effective, d’achèvement effective, de début prévisionnelle, d’achèvement prévisionnelle, etc.).\
Pour plus d’informations sur les expressions de données calculées, consultez [Vue d’ensemble des expressions de données calculées](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demander la modification d’un affichage </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher le résultat d’un calcul entre deux champs d’une colonne

Pour ajouter cette colonne à une vue de tâche, procédez comme suit :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Vue**, cliquez sur **Nouvelle vue**.

1. Cliquez sur **Ajouter une colonne**, puis sur **Passer en mode texte**.

1. Pointez sur la zone de mode texte, puis cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte qui se trouve dans la zone **Mode texte** et remplacez-le par le code suivant :
   <pre>displayname=Week Day Difference<br>textmode=true<br>valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})<br>valueformat=HTML</pre>

1. (Facultatif) Pour agréger les valeurs affichées dans la vue d’un regroupement, procédez comme décrit dans [Regroupement : afficher le résultat de l’agrégation de plusieurs valeurs calculées dans un regroupement](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Cliquez sur **Enregistrer**, puis sur **Enregistrer la vue**.
