---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Affichage : Heures réelles par rapport aux heures planifiées dans la même colonne d’un affichage de tâche"
description: Dans cette vue de tâche, le nombre réel d’heures enregistrées sur une tâche s’affiche au-delà des heures prévues pour chaque tâche.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Afficher : Heures réelles par rapport aux heures planifiées dans la même colonne d’un affichage de tâche

Dans cette vue de tâche, le nombre réel d’heures enregistrées sur une tâche s’affiche au-delà des heures prévues pour chaque tâche.

![real_vs_scheduled_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

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
   <td> <p>Demande de modification d’une vue </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modification de l’accès aux rapports, tableaux de bord et calendriers pour la modification d’un rapport</p> <p>Modifier l’accès aux filtres, vues et groupes pour modifier une vue</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gestion des autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Afficher les heures réelles par rapport aux heures planifiées dans un affichage de tâche

Pour appliquer cette vue :

1. Accédez à une liste de tâches.
1. Dans la **Affichage** menu déroulant, sélectionnez **Nouvelle vue**.

1. Dans le **Aperçu des colonnes** , éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.étich=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.viewalias=assignments<br>column.1.displayname=<br>column.1.linkedname=direct<br>column.1.namekey=assignments<br>column.1.valuefield=assignmentsListString<br>column.1.valueformat=HTML<br>column.1.tile.name=component.assignmentslist<br>column.2.displayname=Realtime/ Heures planifiées<br>column.2.linkedname=direct<br>column.2.namekey=actualworkrequired<br>column.2.querysort=realWork<br>column.2.textmode=true<br>column.2.valueexpression=CONCAT({realWorkRequired}/60,' / ',{workRequired}/60)<br>column.2.valuefield=realWorkRequired<br>column.2.valueformat=composé<br>column.2.viewalias=actualworkrequired<br>column.3.aggator.function=SUM<br>column.3.aggator.valueexpression=SUB({realWork}, {workRequired})<br>column.3.aggator.valueformat=composé<br>column.3.displayname=Hours Variance<br>column.3.linkedname=direct<br>column.3.textmode=true<br>column.3.valueexpression=SUB({realWork}, {workRequired})/60<br>column.3.valueformat=customNumberAsString</pre>

1. Cliquez sur **Enregistrer la vue**.
