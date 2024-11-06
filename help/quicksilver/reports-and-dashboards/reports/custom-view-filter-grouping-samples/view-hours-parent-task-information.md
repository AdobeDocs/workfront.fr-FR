---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Affichage : heures avec les informations sur la tâche parente"
description: Cette vue des heures affiche le nom de la tâche pour laquelle les heures ont été enregistrées, ainsi que le nom de la tâche parent.
author: Nolan
feature: Reports and Dashboards
exl-id: c24555fc-3bae-451b-8a44-28a8158199d1
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 80%

---

# Vue : heures avec les informations sur la tâche parent

<!--Audited: 11/2024-->

Cette vue des heures affiche le nom de la tâche pour laquelle les heures ont été enregistrées, ainsi que le nom de la tâche parent.

![custom_hour_view_with_task_and_parent_task_info.png](assets/custom-hour-view-with-task-and-parent-task-info-350x55.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Nouveau :<ul><li>Contributeur à la modification d’une vue</li><li>Standard pour modifier un rapport</li></ul></p><p>Ou</p>Actuel :<ul><li>Demander la modification d’un affichage</li><li>Prévoir de modifier un rapport</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher les heures avec les informations sur la tâche parent

1. Accédez à une liste d’heures.
1. Dans le menu déroulant **Affichage**, sélectionnez **Nouvel affichage**.

1. Dans la zone **Aperçu des colonnes**, supprimez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis cliquez sur **Basculer en mode texte**.
1. Cliquez sur **Modifier le mode Texte**.
1. Supprimez le texte que vous trouvez dans la zone **Edit Text Mode** et remplacez-le par le code suivant :



   ```
   column.0.aggregator.displayformat=doubleAsString
   column.0.aggregator.function=SUM
   column.0.aggregator.namekey=hours
   column.0.aggregator.valuefield=hours
   column.0.aggregator.valueformat=doubleAsDouble
   column.0.descriptionkey=hours
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=doubleAsDouble(hours)
   column.0.namekey=hours.abbr
   column.0.querysort=hours
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=hours
   column.0.valueformat=doubleAsString
   column.0.width=150
   column.1.descriptionkey=task
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=task:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=task:objCode
   column.1.link.valueformat=val
   column.1.linkedname=task
   column.1.listsort=nested(task).string(name)
   column.1.namekey=task
   column.1.querysort=task:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=task:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.description=Parent Task Name
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=task:parent:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=task:objCode
   column.2.link.valueformat=val
   column.2.linkedname=task
   column.2.listsort=nested(task:parent).string(name)
   column.2.name=Parent Task Name
   column.2.querysort=task:parent:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=task:parent:name
   column.2.valueformat=HTML
   column.2.width=150
   ```

1. Cliquez sur **Terminé**, puis sur **Enregistrer la vue**.

