---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : détails de la tâche antérieure'
description: Cette vue de tâche affiche les détails des tâches antérieures à l’aide d’une vue de collection. Dans une vue de collection, vous pouvez afficher des informations sur les objets qui se trouvent dans une relation « un-à-multiple ». Dans ce cas, chaque tâche (un) peut avoir plusieurs tâches antérieures (multiple). La vue affiche les noms des tâches, des tâches antérieures et des projets des tâches antérieures, ainsi que les dates d’achèvement prévues et les statuts des tâches antérieures.
author: Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 80%

---

# Vue : détails de la tâche antérieure

<!--Audited: 11/2024-->

Cette vue de tâche affiche les détails des tâches antérieures à l’aide d’une vue de collection. Dans une vue de collection, vous pouvez afficher des informations sur les objets qui se trouvent dans une relation « un-à-multiple ». Dans ce cas, chaque tâche (un) peut avoir plusieurs tâches antérieures (multiple). La vue affiche les noms des tâches, des tâches antérieures et des projets des tâches antérieures, ainsi que les dates d’achèvement prévues et les statuts des tâches antérieures.

Pour plus d’informations sur le référencement des collections dans les rapports, voir [Référencer des collections dans un rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![predecessor_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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

## Afficher les détails de la tâche antérieure

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Affichage**, sélectionnez **Nouvel affichage**.

1. Dans la zone **Prévisualisation de la colonne**, éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte** > **Modifier le mode Texte**.
1. Supprimez le texte de la zone **Modifier le mode texte** et remplacez-le par le code suivant :

   ```
   column.0.displayname=
   column.0.linkedname=direct
   column.0.namekey=name
   column.0.querysort=name
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.1.displayname=Predecessors Numbers & Names
   column.1.listdelimiter=
   column.1.listmethod=nested(predecessors).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression=CONCAT({predecessor}.{taskNumber},' - ',{predecessor}.{name})
   column.1.valueformat=HTML
   column.2.displayname=Predecessors Project Names
   column.2.listdelimiter=
   column.2.listmethod=nested(predecessors).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={predecessor}.{project}.{name}
   column.2.valueformat=HTML
   column.3.displayname=Predecessors Completion Dates
   column.3.listdelimiter=
   column.3.listmethod=nested(predecessors).lists
   column.3.textmode=true
   column.3.type=iterate
   column.3.valueexpression={predecessor}.{plannedCompletionDate}
   column.3.valueformat=HTML
   column.4.displayname=Predecessors Status
   column.4.listdelimiter=
   column.4.listmethod=nested(predecessors).lists
   column.4.textmode=true
   column.4.type=iterate
   column.4.valueexpression={predecessor}.{status}
   column.4.valueformat=HTML
   ```

1. Cliquez sur **Terminé** > **Enregistrer la vue**.
