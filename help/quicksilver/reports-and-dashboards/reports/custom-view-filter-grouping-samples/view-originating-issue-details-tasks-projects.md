---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : détails du problème d’origine pour les tâches et les projets »'
description: Lorsqu’un problème est converti en tâche ou en projet, une relation d’objet résolvant est établie entre la tâche ou le projet et le problème. Cette vue affiche les champs du problème qui se termine automatiquement lorsque la tâche ou le projet se termine.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 100%

---

# Vue : détails du problème d’origine pour les tâches et les projets

Lorsqu’un problème est converti en tâche ou en projet, une relation d’objet résolvant est établie entre la tâche ou le projet et le problème. Cette vue affiche les champs suivants du problème qui se termine automatiquement lorsque la tâche ou le projet se termine :

* Nom
* Date d’entrée
* Date d&#39;achèvement prévue
* Date d&#39;achèvement effective
* Type de demande
* Nom du créateur ou de la créatrice
* Utilisateur ou utilisatrice « Affecté à »

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

Pour plus d’informations, voir également [Affichage : afficher les informations sur le problème d’origine dans les listes des tâches et des projets](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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

## Afficher les détails du problème d’origine pour les tâches et les projets

1. Accédez à une liste de tâches ou de projets.
1. Dans le menu déroulant **Vue**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Prévisualisation de la colonne**, éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis cliquez sur **Basculer en mode texte**.
1. Placez le pointeur de la souris sur la zone du mode texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte qui se trouve dans la zone **Mode texte** et remplacez-le par le code suivant :

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>column.0.textmode=false<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.descriptionkey=name<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.width=150<br>column.1.displayname=Resolvables (Issues)<br>column.1.listdelimiter=<br><br>column.1.listmethod=nested(resolvables).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={name}<br>column.1.valueformat=HTML<br>column.2.displayname=Resolvables Entry Date<br>column.2.listdelimiter=<br><br>column.2.listmethod=nested(resolvables).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={entryDate}<br>column.2.valueformat=HTML<br>column.3.displayname=Resolvables Due Date<br>column.3.listdelimiter=<br><br>column.3.listmethod=nested(resolvables).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Resolvables Actual Completion Date<br>column.4.listdelimiter=<br><br>column.4.listmethod=nested(resolvables).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={actualCompletionDate}<br>column.4.valueformat=HTML<br>column.5.displayname=Resolvables Request Type<br>column.5.listdelimiter=<br><br>column.5.listmethod=nested(resolvables).lists<br>column.5.textmode=true<br>column.5.type=iterate<br>column.5.valueexpression={opTaskType}<br>column.5.valueformat=HTML<br>column.6.displayname=Resolvables Originator<br>column.6.listdelimiter=<br><br>column.6.listmethod=nested(resolvables).lists<br>column.6.textmode=true<br>column.6.type=iterate<br>column.6.valueexpression={owner}.{name}<br>column.6.valueformat=HTML<br>column.7.descriptionkey=assignedto<br>column.7.linkedname=assignedTo<br>column.7.listsort=nested(assignedTo).string(name)<br>column.7.namekey=assignedto<br>column.7.querysort=assignedTo:name<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.textmode=true<br>column.7.valuefield=assignedTo:name<br>column.7.valueformat=HTML<br>column.7.width=150</code></pre>

1. Cliquez sur **Enregistrer la vue**.
