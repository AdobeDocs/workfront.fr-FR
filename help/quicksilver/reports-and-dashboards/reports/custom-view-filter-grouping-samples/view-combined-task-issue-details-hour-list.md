---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Affichage : détails combinés de la tâche et des problèmes dans une liste Heure'
description: Cette vue d’heure combine les colonnes Tâche et Nom du problème , ainsi que les heures planifiées de la tâche et du problème à l’aide de la balise sharecol . Une entrée d’heure ne pouvant appartenir qu’à une tâche ou à un problème, les deux objets ne peuvent pas apparaître simultanément dans la même colonne. Chaque ligne de la vue est renseignée avec les informations d’une tâche ou d’un problème.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 23%

---

# Vue : détails de tâche et de problème combinés dans une liste Heure

Cette vue d’heure combine les colonnes Tâche et Nom du problème , ainsi que les Heures planifiées de la tâche et de la publication à l’aide du

```
sharecol
```

balise . Une entrée d’heure ne pouvant appartenir qu’à une tâche ou à un problème, les deux objets ne peuvent pas apparaître simultanément dans la même colonne. Chaque ligne de la vue est renseignée avec les informations d’une tâche ou d’un problème.

Pour en savoir plus sur la variable

```
sharecol
```

Voir [Affichage : fusionner les informations de plusieurs colonnes dans une seule colonne partagée](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).\
![}custom_view_hours_with_task_and_issue_information.png{1](assets/custom-view-hours-with-350x48.png)

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

## Affichage des détails de tâche combinée et de problème dans une liste Heure

Pour appliquer cette vue :

1. Accédez à une liste d&#39;heures.
1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, supprimez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode Texte, puis cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :
   <pre>column.1.querysort=project:name<br>column.1.shortview=false<br>column.1.étich=0<br>column.1.valuefield=project:name<br>column.1.valueformat=HTML<br>column.1.width=100<br>column.2.description=Task ou issue<br>column.2.link.property.0 nom=ID<br>column.2.link.linkproperty.0.valuefield=task:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=task:objCode<br>column.2.link.value=val<br>column.2.linkedname=task<br>column.2.listsort=nested(task).string(name)<br>column.2.name=Task ou Issue<br>column.2.querysort=task:name<br>column.2.sharecol=true<br>column.2.shortview=false<br>column.2.2 ch=0<br>column.2.valuefield=task:name<br>column.2.valueformat=HTML<br>column.2.width=100<br>column.3.description=optask<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.property.0.valuefield=opTask:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=opTask:objCode<br>column.3.link.valueformat=val<br>column.3.linkedname optask<br>column.3.listsort=nested(opTask).string(name)<br>column.3.namekey=opTask<br>column.3.querysort=opTask:name<br>column.3.shortview=false<br>column.3.étich=0<br>column.3.value opTask:name<br>column.3.valueformat=HTML<br>column.3.width=1<br>column.4.valuefield=task:work<br>column.4.sharecol=true<br>column.4.linkedname=task<br>column.4.valueformat=doubleAsInt<br>column.4.namekey=view.relatedcolumn<br>column.4.querysort=task:work<br>column.4.textmode=true<br>column.4.namekeyargkey.0=task<br>column.4.namekeyargkey.1=work<br>column.4.displayname=schedu<br>column.5.displayname=ScheduEffort<br>column.5.viewalias=opTask:workrequired<br>column.5.linkedname=opTask<br>column.5.valuefield=opTask:workRequired<br>column.5.valueformat=composé<br>column.5.querysort=opTask:workwork<br>column.5.namekeyargkey.0=opTask<br>column.5.namekeyargkey.1=workrequired<br>column.5.namekey=view.relatedcolumn<br>column.5.textmode=true<br>column.6.descriptionkey=hours<br>column.6.linkedname=direct 60}column.6.listsort=doubleAsDouble(hours)<br>column.6.namekey=hours.abbr<br>column.6.querysort=hours<br>column.6.shortview=false<br>column.6.étich=0<br>column.6.valuefield=hours<br>column.6 .valueformat=doubleAsString<br>column.6.width=75<br>column.7.descriptionkey=entrydate<br>column.7.linkedname=direct<br>column.7.listsort=atDateAsAtDate(entryDate)<br>column.7.namekey=entrydate.abbentabb) r<br>column.7.querysort=entryDate<br>column.7.shortview=false<br>column.7.étich=0<br>column.7.valuefield=entryDate<br>column.7.valueformat=atDate<br>column.7.width=75<br>column.8.8 key=description<br>column.8.linkedname=direct<br>column.8.listsort=string(description)<br>column.8.namekey=description.abbr<br>column.8.querysort=description<br>column.8.shortview=false<br>column.8.étich=0<br>column.8.valuefield=description<br>column.8.valueformat=HTML<br>column.8.width=150<br></pre>

1. Cliquez sur **Enregistrer la vue**.
