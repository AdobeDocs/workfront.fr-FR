---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : Détails du prédécesseur'
description: Cette vue de tâche affiche les détails des prédécesseurs des tâches à l’aide d’une vue de collection. Dans une vue de collection, vous pouvez afficher des informations sur les objets qui se trouvent dans une relation "un-à-plusieurs". Dans ce cas, chaque tâche (une) peut avoir plusieurs prédécesseurs (plusieurs). La vue affiche le nom des tâches, ainsi que les noms des prédécesseurs, les noms des projets des prédécesseurs, les dates d’achèvement prévues des prédécesseurs et les états des prédécesseurs.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Afficher : Détails du prédécesseur

Cette vue de tâche affiche les détails des prédécesseurs des tâches à l’aide d’une vue de collection. Dans une vue de collection, vous pouvez afficher des informations sur les objets qui se trouvent dans une relation &quot;un-à-plusieurs&quot;. Dans ce cas, chaque tâche (une) peut avoir plusieurs prédécesseurs (plusieurs). La vue affiche le nom des tâches, ainsi que les noms des prédécesseurs, les noms des projets des prédécesseurs, les dates d’achèvement prévues des prédécesseurs et les états des prédécesseurs.

Pour plus d’informations sur le référencement des collections dans les rapports, voir [Collections de référence dans un rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![prédécesseur_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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

## Afficher les détails du prédécesseur

1. Accédez à une liste de tâches.
1. Dans la **Affichage** menu déroulant, sélectionnez **Nouvelle vue**.

1. Dans le **Aperçu des colonnes** , éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=Predecessors Numbers &amp; Names<br>column.1.listsepariter=<br><br>column.1.listmethod=nested(prédécesseurs).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({prédécesseur}).{taskNumber},' - ',{prédécesseur}.{name})<br>column.1.valueformat=HTML<br>column.2.displayname=Predecessors Project Names<br>column.2.listsepariter=<br><br>column.2.listmethod=nested(prédécesseurs).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.value expression={prédécesseur}.{projet}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=Predecessors Compledate<br>column.3.listsepariter=<br><br>column.3.listmethod=nested(prédécesseurs).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.value expression={prédécesseur}.{scheduledCompletionDate}<br>column.3.value.format=HTML<br>column.4.displayname=Predecessors Status<br>column.4.listsepariter=<br><br>column.4.listmethod=nested(prédécesseurs).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.value expression={prédécesseur}.{status}<br>column.4.valueformat=HTML</pre>

1. Cliquez sur **Enregistrer la vue**.
