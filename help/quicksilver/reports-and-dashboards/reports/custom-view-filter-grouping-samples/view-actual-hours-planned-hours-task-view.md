---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Affichage : heures effectives par rapport au nombre d’heures prévues dans la même colonne d’un affichage de tâche »'
description: Dans cet affichage de tâche, le nombre effectif d’heures enregistrées sur une tâche est affiché au-dessus des heures prévues pour chaque tâche.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 100%

---

# Affichage : heures effectives par rapport au nombre d’heures prévues dans la même colonne d’un affichage de tâche

Dans cet affichage de tâche, le nombre effectif d’heures enregistrées sur une tâche est affiché au-dessus des heures prévues pour chaque tâche.

![real_vs_scheduled_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

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

## Afficher les heures effectives par rapport aux heures prévues dans un affichage de tâche

Pour appliquer cet affichage :

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Affichage**, sélectionnez **Nouvel affichage**.

1. Dans la zone **Prévisualisation de la colonne**, éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis cliquez sur **Basculer en mode texte**.
1. Placez le pointeur de la souris sur la zone du mode texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte qui se trouve dans la zone **Mode texte** et remplacez-le par le code suivant :
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=assignments<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=assignments<br>column.1.valuefield=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=Actual/ Planned Hours<br>column.2.linkedname=direct<br>column.2.namekey=actualworkrequired<br>column.2.querysort=actualWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=actualWorkRequired<br>column.2.valueformat=compound<br>column.2.viewalias=actualworkrequired<br>column.3.aggregator.function=SUM<br>column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})<br>column.3.aggregator.valueformat=compound<br>column.3.displayname=Hours Variance<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB({actualWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. Cliquez sur **Enregistrer l’affichage**.
