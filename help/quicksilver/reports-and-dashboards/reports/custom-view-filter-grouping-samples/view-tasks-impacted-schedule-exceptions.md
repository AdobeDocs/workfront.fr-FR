---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Vue : tâches affectées par les exceptions de planification'
description: Cette vue de tâche identifie les tâches qui devront être terminées en retard en raison des week-ends, de la désactivation de la fonction personnelle ou d’autres exceptions de planification.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 22%

---

# Vue : tâches affectées par des exceptions de planning

Cette vue de tâche identifie les tâches qui devront être terminées en retard en raison des week-ends, de la désactivation de la fonction personnelle ou d’autres exceptions de planification.

Cette vue affiche les éléments suivants :

* Durée des tâches
* Dates de début et de fin planifiées des tâches
* Durée des tâches en fonction du nombre de jours entre le début planifié et les dates d’achèvement planifiées des tâches (durée du calendrier)
* Numéro du jour dans le planning du projet au début de la tâche (Date de début du calendrier).
* Durée de la semaine selon le nombre de jours en semaine entre le début planifié et les dates d’achèvement planifiées des tâches (durée de la semaine)
* Si la durée du jour de la semaine est supérieure à la durée des tâches, ce qui suggère qu’il existe des jours d’exception dans la durée des tâches, les tâches sont marquées comme une &quot;exception&quot;.\
  ![tasks_with_calendar_exceptions.png](assets/tasks-with-calendar-exceptions-350x51.png)

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
   <td> <p>Demander la modification d’une vue </p>
   <p>Prévoir la modification d’un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier une vue</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher les tâches affectées par les exceptions de planification

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, supprimez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode de texte et cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br> 0.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.étich=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(duration)<br>column 1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.étich=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=composé<br>column.1.viewalias 5}column.1.width=80<br>column.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAtDate(scheduledStartDate)<br>column.2.namekey=plnedstartdate.abbr{3 0}column.2.querysort=scheduledStartDate<br>column.2.shortview=false<br>column.2.étich=0<br>column.2.valuefield=scheduledStartDate<br>column.2.valueformat=atDate<br>column.2.width=80<br>column.3.key=plnedcomplete-date<br>column.3.linkedname=direct<br>column.3.listsort=atDateAtDate(scheduledCompletionDate)<br>column.3.namekey=plannedcompletedate.abbr<br>column.3.querysort=scheduledCompletionDate<br>column.3.shortview=false<br>column.3.étich=0<br>column.3.valuefield=scheduledCompletionDate<br>column.3.valueformat=atDate<br>column.3.width=80<br>column.4.aggator.displayformat=int<br>column.4.aggator function=SUM<br>column.4.aggator.namekey=id<br>column.4.aggator.valueexpression=DATEDIFF({plannedCompletionDate},<br>{plannedStartDate})+1<br>column.4.aggator.value=intAsInt<br>column.4.descriptionkey=id{5 5}column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=Calendar Duration<br>column.4.querysort=ID<br>column.4.shortview=false<br>column.4.étich=0<br>column.4.value DATEDIFF({plannedCompletionDate},{plannedStartDate})+1<br>column.4.valueformat=int<br>column.4.width=80<br>column.5.aggator.displayformat=int<br>column.5.aggator.function=SUM<br>column.5.aggator.name=id{66 9}column.5.aggator.valueexpression=DATEDIFF({plannedStartDate},{project}.<br><br><br><br><br>{plannedStartDate})+0<br>column.5.aggator.valueformat=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=Calendar Date de début<br>column.5.querysort=8 column.5.shortview=false<br>column.5.étich=0<br>column.5.valueexpression=DATEDIFF({plannedStartDate},{project}).<br>{plannedStartDate})+0<br>column.5.valueformat=int<br>column.5.width=80<br>column.6.aggator.displayformat=int<br>column.6.aggator.function=SUM<br>column.6.aggator.namekey=id<br> column.6.aggueexpression=WEEKDAYDIFF({plannedStartDate},<br>{plannedCompletionDate})+0<br>column.6.aggator.valueformat=HTML<br>column.6.descriptionkey=id<br>column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=Week Day Duration{15.column 6.querysort=ID<br>column.6.shortview=false<br>column.6.étich=0<br>column.6.valueexpression=WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate})+0<br>column.6.valueformat=int<br>column.6.width=80<br>column.7.aggator.displayformat=int<br>column.7.aggator.expression=IF((WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.aggator.function=SUM<br>column.7.aggator .namekey=id<br>column.7.aggator.valueformat=HTML<br>column.7.linkedname=direct<br>column.7.listsort=intAsInt(ID)<br>column.7.name=Schedule<br>column.7.querysort=ID<br>column.7.shortview<br>column.7.étich=0<br>column.7.valueexpression=IF((WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.valueformat=HTML<br>column.7.width 0<br></pre>

1. Cliquez sur **Enregistrer la vue**.
