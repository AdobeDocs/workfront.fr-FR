---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : tâche avec écart Toutes les dates »'
description: Cette vue de tâche est similaire à la vue « Toutes les dates » fournie avec votre compte Adobe Workfront. Cette vue spécifique comprend les colonnes d’écart calculant la différence en jours entre les dates.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 20df7cd8-113e-4c0d-b3f5-1def7db968a5
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 100%

---

# Vue : tâche avec écart Toutes les dates

Cette vue de tâche est similaire à la vue « Toutes les dates » fournie avec votre compte Adobe Workfront. Cette vue spécifique comprend les colonnes *Écart* calculant la différence en jours entre les dates suivantes :

* Dates de début prévue et prévisionnelle
* Dates de début prévue et effective
* Dates d’achèvement prévue et prévisionnelle
* Dates d’achèvement prévue et effective

Cette vue illustre un exemple de colonnes calculées, où vous pouvez prendre les valeurs de deux colonnes différentes et les combiner par un calcul pour obtenir une troisième valeur. Dans ce cas, vous soustrayez la date 1 de la date 2.

Pour plus d’informations sur l’utilisation des calculs dans une vue, consultez la section [Vue d’ensemble des utilisations courantes du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md) dans [Vue d’ensemble des utilisations courantes du mode texte](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).

![Screen_Shot_2017-04-24_at_11.35.33_AM.png](assets/screen-shot-2017-04-24-at-11.35.33-am-350x95.png)

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

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre équipe d’administration Workfront.

## Afficher les tâches avec l’écart « Toutes les dates »

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Affichage**, sélectionnez **Nouvel affichage**.

1. Dans la zone **Prévisualisation de la colonne**, éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis cliquez sur **Basculer en mode texte**.
1. Placez le pointeur de la souris sur la zone du mode texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Mode texte** et remplacez-le par le code suivant :
   <pre>column.1.descriptionkey=name<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=direct<br>column.1.listsort=string(name)<br>column.1.namekey=name.abbr<br>column.1.querysort=name<br>column.1.shortview=false<br>column.1.stretch=95<br>column.1.styledef.case.0.comparison.attribute=css<br>column.1.styledef.case.0.comparison.isrowcase=true<br>column.1.styledef.case.0.comparison.leftmethod=intAsInt(numberOfChildren)<br>column.1.styledef.case.0.comparison.lefttext=numberOfChildren<br>column.1.styledef.case.0.comparison.operator=gt<br>column.1.styledef.case.0.comparison.operatortype=int<br>column.1.styledef.case.0.comparison.righttext=0<br>column.1.styledef.case.0.comparison.trueproperty.0.name=fontstyle<br>column.1.styledef.case.0.comparison.trueproperty.0.value=bold<br>column.1.styledef.case.0.comparison.truetext=<br>column.1.styledef.case.0.comparison.usefield=false<br>column.1.valuefield=name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(plannedStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.querysort=plannedStartDate<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=plannedStartDate<br>column.2.valueformat=atDate<br>column.2.width=75<br>column.3.descriptionkey=projectedstartdate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(projectedStartDate)<br>column.3.namekey=projectedstartdate.abbr<br>column.3.querysort=projectedStartDate<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=projectedStartDate<br>column.3.valueformat=atDate<br>column.3.width=75<br>column.4.descriptionkey=plannedstartdate<br>column.4.displayname=Projected Start Variance<br>column.4.linkedname=direct<br>column.4.listsort=atDateAsAtDate(plannedStartDate)<br>column.4.namekey=plannedstartdate.abbr<br>column.4.querysort=plannedStartDate<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.styledef.case.0.comparison.attribute=css<br>column.4.styledef.case.0.comparison.isrowcase=false<br>column.4.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedStartDate)<br>column.4.styledef.case.0.comparison.lefttext=plannedStartDate<br>column.4.styledef.case.0.comparison.operator=notnull<br>column.4.styledef.case.0.comparison.operatortype=date<br>column.4.styledef.case.0.comparison.righttext=<br>column.4.styledef.case.0.comparison.trueproperty.0.name=bgcolor<br>column.4.styledef.case.0.comparison.trueproperty.0.value=E1E1E1<br>column.4.styledef.case.0.comparison.truetext=<br>column.4.styledef.case.0.comparison.usefield=false<br>column.4.valueexpression=ROUND(DATEDIFF({projectedStartDate},{plannedStartDate}))<br>column.4.valueformat=HTML<br>column.4.width=75<br>column.5.descriptionkey=plannedstartdate<br>column.5.linkedname=direct<br>column.5.listsort=atDateAsAtDate(plannedStartDate)<br>column.5.namekey=plannedstartdate.abbr<br>column.5.querysort=plannedStartDate<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valuefield=plannedStartDate<br>column.5.valueformat=atDate<br>column.5.width=75<br>column.6.descriptionkey=actualstartdate<br>column.6.linkedname=direct<br>column.6.listsort=atDateAsAtDate(actualStartDate)<br>column.6.namekey=actualstartdate.abbr<br>column.6.querysort=actualStartDate<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valuefield=actualStartDate<br>column.6.valueformat=atDate<br>column.6.width=75<br>column.7.descriptionkey=plannedstartdate<br>column.7.displayname=Actual Start Variance<br>column.7.linkedname=direct<br>column.7.listsort=atDateAsAtDate(plannedStartDate)<br>column.7.namekey=plannedstartdate.abbr<br>column.7.querysort=plannedStartDate<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.styledef.case.0.comparison.attribute=css<br>column.7.styledef.case.0.comparison.isrowcase=false<br>column.7.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedStartDate)<br>column.7.styledef.case.0.comparison.lefttext=plannedStartDate<br>column.7.styledef.case.0.comparison.operator=notnull<br>column.7.styledef.case.0.comparison.operatortype=date<br>column.7.styledef.case.0.comparison.righttext=<br>column.7.styledef.case.0.comparison.trueproperty.0.name=bgcolor<br>column.7.styledef.case.0.comparison.trueproperty.0.value=E1E1E1<br>column.7.styledef.case.0.comparison.truetext=<br>column.7.styledef.case.0.comparison.usefield=false<br>column.7.valueexpression=ROUND(DATEDIFF({actualStartDate},{plannedStartDate}))<br>column.7.valueformat=HTML<br>column.7.width=75<br>column.8.descriptionkey=plannedcompletiondate<br>column.8.linkedname=direct<br>column.8.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.8.namekey=plannedcompletiondate.abbr<br>column.8.querysort=plannedCompletionDate<br>column.8.shortview=false<br>column.8.stretch=0<br>column.8.valuefield=plannedCompletionDate<br>column.8.valueformat=atDate<br>column.8.width=75<br>column.9.descriptionkey=projectedcompletiondate<br>column.9.linkedname=direct<br>column.9.listsort=atDateAsAtDate(projectedCompletionDate)<br>column.9.namekey=projectedcompletiondate.abbr<br>column.9.querysort=projectedCompletionDate<br>column.9.shortview=false<br>column.9.stretch=0<br>column.9.valuefield=projectedCompletionDate<br>column.9.valueformat=atDate<br>column.9.width=75<br>column.10.descriptionkey=plannedcompletiondate<br>column.10.displayname=Projected Completion Variance<br>column.10.linkedname=direct<br>column.10.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.10.namekey=plannedcompletiondate.abbr<br>column.10.querysort=plannedCompletionDate<br>column.10.shortview=false<br>column.10.stretch=0<br>column.10.styledef.case.0.comparison.attribute=css<br>column.10.styledef.case.0.comparison.isrowcase=false<br>column.10.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedCompletionDate)<br>column.10.styledef.case.0.comparison.lefttext=plannedCompletionDate<br>column.10.styledef.case.0.comparison.operator=notnull<br>column.10.styledef.case.0.comparison.operatortype=date<br>column.10.styledef.case.0.comparison.righttext=<br>column.10.styledef.case.0.comparison.trueproperty.0.name=bgcolor<br>column.10.styledef.case.0.comparison.trueproperty.0.value=E1E1E1<br>column.10.styledef.case.0.comparison.truetext=<br>column.10.styledef.case.0.comparison.usefield=false<br>column.10.valueexpression=ROUND(DATEDIFF({projectedCompletionDate},{plannedCompletionDate}))<br>column.10.valueformat=HTML<br>column.10.width=75<br>column.11.descriptionkey=plannedcompletiondate<br>column.11.linkedname=direct<br>column.11.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.11.namekey=plannedcompletiondate.abbr<br>column.11.querysort=plannedCompletionDate<br>column.11.shortview=false<br>column.11.stretch=0<br>column.11.valuefield=plannedCompletionDate<br>column.11.valueformat=atDate<br>column.11.width=75<br>column.12.descriptionkey=actualcompletiondate<br>column.12.linkedname=direct<br>column.12.listsort=atDateAsAtDate(actualCompletionDate)<br>column.12.namekey=actualcompletiondate.abbr<br>column.12.querysort=actualCompletionDate<br>column.12.shortview=false<br>column.12.stretch=0<br>column.12.valuefield=actualCompletionDate<br>column.12.valueformat=atDate<br>column.12.width=75<br>column.13.descriptionkey=plannedcompletiondate<br>column.13.displayname=Actual Completion Variance<br>column.13.linkedname=direct<br>column.13.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.13.namekey=plannedcompletiondate.abbr<br>column.13.querysort=plannedCompletionDate<br>column.13.shortview=false<br>column.13.stretch=0<br>column.13.styledef.case.0.comparison.attribute=css<br>column.13.styledef.case.0.comparison.isrowcase=false<br>column.13.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedCompletionDate)<br>column.13.styledef.case.0.comparison.lefttext=plannedCompletionDate<br>column.13.styledef.case.0.comparison.operator=notnull<br>column.13.styledef.case.0.comparison.operatortype=date<br>column.13.styledef.case.0.comparison.righttext=<br>column.13.styledef.case.0.comparison.trueproperty.0.name=bgcolor<br>column.13.styledef.case.0.comparison.trueproperty.0.value=E1E1E1<br>column.13.styledef.case.0.comparison.truetext=<br>column.13.styledef.case.0.comparison.usefield=false<br>column.13.valueexpression=ROUND(DATEDIFF({actualCompletionDate},{plannedCompletionDate}))<br>column.13.valueformat=HTML<br>column.13.width=75<br>row.0.styledef.applyallcases=true<br>row.0.styledef.case.0.comparison.attribute=css<br>row.0.styledef.case.0.comparison.isrowcase=true<br>row.0.styledef.case.0.comparison.leftmethod=intAsInt(numberOfChildren)<br>row.0.styledef.case.0.comparison.lefttext=numberOfChildren<br>row.0.styledef.case.0.comparison.operator=gt<br>row.0.styledef.case.0.comparison.operatortype=int<br>row.0.styledef.case.0.comparison.righttext=0<br>row.0.styledef.case.0.comparison.trueproperty.0.name=fontstyle<br>row.0.styledef.case.0.comparison.trueproperty.0.value=bold<br>row.0.styledef.case.0.comparison.truetext=<br>row.0.styledef.case.0.comparison.usefield=false</pre>

1. Cliquez sur **Enregistrer l’affichage**.
