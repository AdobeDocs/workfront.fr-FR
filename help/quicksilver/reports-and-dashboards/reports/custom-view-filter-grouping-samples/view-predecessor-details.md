---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : détails du prédécesseur'
description: Cette vue de tâche affiche les détails des prédécesseurs des tâches à l’aide d’une vue Collection. Dans une vue de collection, vous pouvez afficher des informations sur les objets qui se trouvent dans une relation "un-à-plusieurs". Dans ce cas, chaque tâche (une) peut avoir plusieurs prédécesseurs (plusieurs). La vue affiche le nom des tâches, ainsi que les noms des prédécesseurs, les noms des projets des prédécesseurs, les dates d’achèvement prévues des prédécesseurs et les états des prédécesseurs.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 0187da94-4895-47b1-914f-284fed9e0fd0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 31%

---

# Vue : détails du projet antérieur

Cette vue de tâche affiche les détails des prédécesseurs des tâches à l’aide d’une vue Collection. Dans une vue de collection, vous pouvez afficher des informations sur les objets qui se trouvent dans une relation &quot;un-à-plusieurs&quot;. Dans ce cas, chaque tâche (une) peut avoir plusieurs prédécesseurs (plusieurs). La vue affiche le nom des tâches, ainsi que les noms des prédécesseurs, les noms des projets des prédécesseurs, les dates d’achèvement prévues des prédécesseurs et les états des prédécesseurs.

Pour plus d’informations sur le référencement des collections dans les rapports, voir [Référencer des collections dans un rapport](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

![prédécesseur_details_task_view.png](assets/predecessor-details-task-view-350x34.png)

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

## Afficher les détails du prédécesseur

1. Accédez à une liste de tâches.
1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, supprimez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode Texte, puis cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :
   <pre>column.0.displayname=<br>column.0.linkedname=direct<br>column.0.namekey=name<br>column.0.querysort=name<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.1.displayname=Predecessors Numbers &amp; Names<br>column.1.listseparer<br><br>column.1.listmethod=nested(prédécesseurs).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression=CONCAT({predecessor}){taskNumber},' - ',{predecessor}.{name})<br>column.1.valueformat=HTML<br>column.2.displayname=Predecessors Noms du projet<br>column.2.listsepariter=<br><br>column.2.listmethod=nested(prédécessors).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression=}.{predecessor}{project}.{name}<br>column.2.valueformat=HTML<br>column.3.displayname=Predecessors Dates d'achèvement<br>column.3.listsepariter=<br><br>column.3.listmethod=nested(prédécessors).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.value= 8}.{predecessor}{plannedCompletionDate}<br>column.3.valueformat=HTML<br>column.4.displayname=Predecessors Status<br>column.4.listsepariter=<br><br>column.4.listmethod=nested(prédécessors).lists<br>column.4.textmode=true<br>column.4.type=iterate<br>column.4.valueexpression={predecessor}}{status}<br>column.4.valueformat=HTML</pre>

1. Cliquez sur **Enregistrer la vue**.
