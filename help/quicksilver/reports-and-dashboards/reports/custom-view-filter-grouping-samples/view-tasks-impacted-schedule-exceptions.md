---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : tâches affectées par les exceptions de planification'
description: Cette vue de tâche identifie les tâches qui devront être terminées en retard en raison des week-ends, de la désactivation de la fonction personnelle ou d’autres exceptions de planification.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Afficher : tâches affectées par les exceptions de planification

Cette vue de tâche identifie les tâches qui devront être terminées en retard en raison des week-ends, de la désactivation de la fonction personnelle ou d’autres exceptions de planification.

Cette vue affiche les éléments suivants :

* Durée des tâches
* Dates de début et de fin planifiées des tâches
* Durée des tâches en fonction du nombre de jours entre le début planifié et les dates d’achèvement planifiées des tâches (durée du calendrier)
* Numéro du jour dans le planning du projet lorsque la tâche commence (Date de début du calendrier).
* Durée de la semaine selon le nombre de jours en semaine entre le début planifié et les dates d’achèvement planifiées des tâches (durée de la semaine)
* Si la durée du jour de la semaine est supérieure à la durée des tâches, ce qui suggère qu’il existe des jours d’exception dans la durée des tâches, les tâches sont marquées comme une &quot;exception&quot;.\
   ![tasks_with_calendar_exceptions.png](assets/tasks-with-calendar-exceptions-350x51.png)

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

## Afficher les tâches affectées par les exceptions de planification

1. Accédez à une liste de tâches.
1. Dans la **Affichage** menu déroulant, sélectionnez **Nouvelle vue**.

1. Dans le **Aperçu des colonnes** , éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.étich=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.name=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.étich=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=composé<br>column.1.viewalias=duration<br>column.1.width=80<br>column.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(scheduledStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.querysort=scheduledStartDate<br>column.2.shortview=false<br>column.2.étich=0<br>column.2.valuefield=scheduledStartDate<br>column.2.valueformat=atDate<br>column.2.width=80<br>column.3.descriptionkey=plannedcompletiondate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(scheduledCompletionDate)<br>column.3.namekey=plannedcomplete.abbr<br>column.3.querysort=scheduledCompletionDate<br>column.3.shortview=false<br>column.3.étirement=0<br>column.3.valuefield=scheduledCompletionDate<br>column.3.valueformat=atDate<br>column.3.width=80<br>column.4.aggator.displayformat=int<br>column.4.aggator.function=SUM<br>column.4.aggator.namekey=id<br>column.4.aggator.valueexpression=DATEDIFF({scheduledCompletionDate},<br>{scheduledStartDate})+1<br>column.4.aggator.valueformat=intAsInt<br>column.4.descriptionkey=id<br>column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=Durée du calendrier<br>column.4.querysort=ID<br>column.4.shortview=false<br>column.4.étich=0<br>column.4.valueexpression=DATEDIFF({scheduledCompletionDate},{scheduledStartDate})+1<br>column.4.valueformat=int<br>column.4.width=80<br>column.5.aggator.displayformat=int<br>column.5.aggator.function=SUM<br>column.5.aggator.namekey=id<br>column.5.aggator.valueexpression=DATEDIFF({scheduledStartDate},{project}.<br>{scheduledStartDate})+0<br>column.5.aggator.valueformat=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=Date de début du calendrier<br>column.5.querysort=ID<br>column.5.shortview=false<br>column.5.étich=0<br>column.5.valueexpression=DATEDIFF({scheduledStartDate},{project}.{scheduledStartDate})+0<br>column.5.valueformat=int<br>column.5.width=80<br>column.6.aggator.displayformat=int<br>column.6.aggator.function=SUM<br>column.6.aggator.namekey=id<br>column.6.aggator.valueexpression=WEEKDAYDIFF({scheduledStartDate},<br>{scheduledCompletionDate})+0<br>column.6.aggator.valueformat=HTML<br>column.6.descriptionkey=id<br>column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=Week Day Duration<br>column.6.querysort=ID<br>column.6.shortview=false<br>column.6.étich=0<br>column.6.valueexpression=WEEKDAYDIFF({scheduledStartDate},{scheduledCompletionDate})+0<br>column.6.valueformat=int<br>column.6.width=80<br>column.7.aggator.displayformat=int<br>column.7.aggator.expression=IF((WEEKDAYDIFF({scheduledStartDate},{scheduledCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.aggator.function=SUM<br>column.7.aggator.namekey=id<br>column.7.aggator.valueformat=HTML<br>column.7.linkedname=direct<br>column.7.listsort=intAsInt(ID)<br>column.7.name=Schedule<br>column.7.querysort=ID<br>column.7.shortview=false<br>column.7.étich=0<br>column.7.valueexpression=IF((WEEKDAYDIFF({scheduledStartDate},{scheduledCompletionDate}))&gt;({duration}/480),"Exception",")<br>column.7.valueformat=HTML<br>column.7.width=80</pre>

1. Cliquez sur **Enregistrer la vue**.
