---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Affichage : Heures planifiées par rapport aux Heures réelles par affectation dans un affichage de tâche'
description: Cette vue affiche le nombre total d’heures planifiées d’une tâche, le nombre d’heures planifiées allouées à chaque personne désignée, le nombre total d’heures réelles et le nombre d’heures réelles consignées par chaque personne désignée.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f249ff57-50c7-4aa9-a563-cb7f5562b96a
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 49%

---

# Vue : nombre d’heures prévues et heures effectives par affectation dans une vue de tâche

Cette vue affiche le nombre total d’heures planifiées d’une tâche, le nombre d’heures planifiées allouées à chaque personne désignée, le nombre total d’heures réelles et le nombre d’heures réelles consignées par chaque personne désignée.

![multi_assignment_budget_vs_real_for_tasks.png](assets/multi-assignment-budget-vs-actual-for-tasks-350x66.png)

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

## Afficher les heures planifiées par rapport aux heures réelles par affectation dans une vue de tâche

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, supprimez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode Texte, puis cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :

   ```
   column.0.descriptionkey=name<br>column.0.isInlineEditable=false<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=workrequired<br>column.1.isInlineEditable=false<br>column.1.linkedname=direct<br>column.1.listsort=doubleAsDouble(workRequired)<br>column.1.namekey=workrequired.abbr<br>column.1.querysort=workRequired<br>column.1.section=0<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=workFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=workrequired<br>column.1.width=100<br>column.2.listdelimiter=<br>column.2.listmethod=nested(assignments).lists<br>column.2.name=Wrk Assignment(s)<br>column.2.stretch=0<br>column.2.type=iterate<br>column.2.valueexpression=CONCAT(right(CONCAT('~~~',{assignmentPercent}),3),'% (', {workRequired}/60 ,' Hours) - ',{assignedTo}.{name})<br>column.2.valueformat=HTML<br>column.2.width=300<br>column.3.descriptionkey=actualworkrequired<br>column.3.isInlineEditable=false<br>column.3.linkedname=direct<br>column.3.listsort=intAsInt(actualWorkRequired)<br>column.3.namekey=actualworkrequired.abbr<br>column.3.querysort=actualWork<br>column.3.section=0<br>column.3.shortview=false<br>column.3.stretch=100<br>column.3.valuefield=actualWorkFieldLong<br>column.3.valueformat=compound<br>column.3.viewalias=actualworkrequired<br>column.3.width=100<br>column.4.listdelimiter=<br>column.4.listmethod=nested(hours).lists<br>column.4.name=Actual Hours<br>column.4.stretch=0<br>column.4.type=iterate<br>column.4.valueexpression=CONCAT('(', {hours} ,' Hours) - ',{owner}.{name})<br>column.4.valueformat=HTML<br>column.4.width=300
   ```

1. Cliquez sur **Enregistrer la vue**.
