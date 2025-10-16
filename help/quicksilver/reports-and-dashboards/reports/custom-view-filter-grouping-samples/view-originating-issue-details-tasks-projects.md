---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : Détails de l''événement d''origine pour les tâches et les projets'
description: Lorsqu’un problème est converti en tâche ou en projet, une relation d’objet résolvant est établie entre la tâche ou le projet et le problème. Cette vue affiche les champs du problème qui se termine automatiquement lorsque la tâche ou le projet se termine.
author: Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 66%

---

# Vue : détails du problème d’origine pour les tâches et les projets

<!--Audited: 11/2024-->

Lorsqu’un problème est converti en tâche ou en projet, une relation d’objet résolvant est établie entre la tâche ou le projet et le problème. Cette vue affiche les champs suivants de l’événement qui se termine automatiquement à la fin de la tâche ou du projet :

* Nom
* Date d’entrée
* Date d&#39;achèvement prévue
* Date d&#39;achèvement effective
* Type de demande
* Nom du créateur ou de la créatrice
* Utilisateur ou utilisatrice « Affecté à »

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

Pour plus d&#39;informations, voir également [Afficher : afficher les informations sur l&#39;événement d&#39;origine dans les listes de tâches ou de projets](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou demande de modification d’une vue </p>
   <p>Standard ou Plan pour modifier un rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Afficher les détails du problème d’origine pour les tâches et les projets

1. Accédez à une liste de tâches ou de projets.
1. Dans le menu déroulant **Vue**, sélectionnez **Nouvelle vue**.
1. Dans la zone **Prévisualisation de la colonne**, éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante et cliquez sur **Basculer en mode texte**, puis sur **Modifier le mode texte**.
1. Supprimez le texte de la zone **Modifier le mode texte** et remplacez-le par le code suivant :

   ```
   column.0.textmode=false
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.descriptionkey=name
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.width=150
   column.1.displayname=Resolvables (Issues)
   column.1.listdelimiter=
   column.1.listmethod=nested(resolvables).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={name}
   column.1.valueformat=HTML
   column.2.displayname=Resolvables Entry Date
   column.2.listdelimiter=
   column.2.listmethod=nested(resolvables).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={entryDate}
   column.2.valueformat=HTML
   column.3.displayname=Resolvables Due Date
   column.3.listdelimiter=
   column.3.listmethod=nested(resolvables).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={plannedCompletionDate}
   column.3.valueformat=HTML
   column.4.displayname=Resolvables Actual Completion Date
   column.4.listdelimiter=
   column.4.listmethod=nested(resolvables).lists
   column.4.textmode=true
   column.4.type=iterate
   column.4.valueexpression={actualCompletionDate}
   column.4.valueformat=HTML
   column.5.displayname=Resolvables Request Type
   column.5.listdelimiter=
   column.5.listmethod=nested(resolvables).lists
   column.5.textmode=true
   column.5.type=iterate
   column.5.valueexpression={opTaskType}
   column.5.valueformat=HTML
   column.6.displayname=Resolvables Originator
   column.6.listdelimiter=
   column.6.listmethod=nested(resolvables).lists
   column.6.textmode=true
   column.6.type=iterate
   column.6.valueexpression={owner}.{name}
   column.6.valueformat=HTML
   column.7.descriptionkey=assignedto
   column.7.linkedname=assignedTo
   column.7.listsort=nested(assignedTo).string(name)
   column.7.namekey=assignedto
   column.7.querysort=assignedTo:name
   column.7.shortview=false
   column.7.stretch=0
   column.7.textmode=true
   column.7.valuefield=assignedTo:name
   column.7.valueformat=HTML
   column.7.width=150
   ```

1. Cliquez sur **Terminé** > **Enregistrer la vue**.
