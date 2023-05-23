---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : heures avec les informations de tâche parente'
description: Cette vue d’heure affiche le nom de la tâche où les heures ont été enregistrées, ainsi que le nom de la tâche parente.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c24555fc-3bae-451b-8a44-28a8158199d1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# Afficher : heures avec les informations de tâche parente

Cette vue d’heure affiche le nom de la tâche où les heures ont été enregistrées, ainsi que le nom de la tâche parente.

![custom_hour_view_with_task_and_parent_task_info.png](assets/custom-hour-view-with-task-and-parent-task-info-350x55.png)

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

## Afficher les heures avec les informations sur la tâche parente

1. Accédez à une liste d&#39;heures.
1. Dans la **Affichage** menu déroulant, sélectionnez **Nouvelle vue**.

1. Dans le **Aperçu des colonnes** , éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :
   <pre>column.0.aggator.displayformat=doubleAsString<br>column.0.aggator.function=SUM<br>column.0.aggator.namekey=hours<br>column.0.aggator.valuefield=hours<br>column.0.aggator.valueformat=doubleAsDouble<br>column.0.descriptionkey=hours<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=doubleAsDouble(hours)<br>column.0.namekey=hours.abbr<br>column.0.querysort=hours<br>column.0.shortview=false<br>column.0.étich=100<br>column.0.valuefield=hours<br>column.0.valueformat=doubleAsString<br>column.0.width=150<br>column.1.descriptionkey=task<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=task:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=task:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=task<br>column.1.listsort=nested(task).string(name)<br>column.1.namekey=task<br>column.1.querysort=task:name<br>column.1.shortview=false<br>column.1.étich=0<br>column.1.valuefield=task:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=Parent Task Name<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=task:parent:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=task:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=task<br>column.2.listsort=nested(task:parent).string(name)<br>column.2.name=Parent Task Name<br>column.2.querysort=task:parent:name<br>column.2.shortview=false<br>column.2.étich=0<br>column.2.valuefield=task:parent:name<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. Cliquez sur **Enregistrer la vue**.
