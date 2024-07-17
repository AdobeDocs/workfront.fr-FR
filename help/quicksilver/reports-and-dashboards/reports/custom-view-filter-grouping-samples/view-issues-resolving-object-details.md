---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Affichage : problèmes liés à la résolution des détails de l’objet'
description: Cette vue affiche le nom et le pourcentage de l’objet de résolution du problème, ce qui permet à l’auteur du problème d’avoir un aperçu de l’avancement du problème, même sans accès à la tâche ou au projet de résolution.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 24%

---

# Vue : problèmes avec détails de l’objet de résolution

Cette vue affiche le nom et le pourcentage de l’objet de résolution du problème, ce qui permet à l’auteur du problème d’avoir un aperçu de l’avancement du problème, même sans accès à la tâche ou au projet de résolution.

Cette vue utilise la variable

```
sharecol=true
```

pour combiner plusieurs champs sous le même en-tête de colonne. Pour plus d’informations sur la variable

```
sharecol
```

Voir [Affichage : fusionner les informations de plusieurs colonnes dans une seule colonne partagée](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

![issue_custom_view_with_resolve_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

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

## Affichage des problèmes liés à la résolution des détails de l’objet

1. Accédez à une liste de problèmes.
1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, supprimez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode Texte, puis cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :<pre>column.0.querysort=name</pre><pre>column.0.étich=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=sourceobject<br>column.1.linkedname=direct<br>column.1.listsort=nested(referenceObject).HTML(name) 6}column.1.namekey=sourceobject.abbr<br>column.1.shortview=false<br>column.1.étich=0<br>column.1.valuefield=referenceObject:name<br>column.1.valueformat=HTML<br>column.1.viewalias=source<br>column.1.width=10<br>column.2.descriptionkey=assignedto<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=assignedTo:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup view<br>column.2.link.valuefield=assignedTo:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=assignedTo<br>column.2.listsort=nested(assignedTo).string(name)<br>column.2.namekey=assignedto{2 3}column.2.querysort=assignedTo:name<br>column.2.shortview=false<br>column.2.étich=25<br>column.2.valuefield=assignedTo:name<br>column.2.value=HTML<br>column.2.width=150<br>column 3.descriptionkey=entrydate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsDate(entryDate)<br>column.3.namekey=entrydate.abbr<br>column.3.querysort=entryDate<br>column.3.shortview<br>column.3.étich=0<br>column.3.valuefield=entryDate<br>column.3.valueformat=atDate<br>column.3.width=150<br>column.4.description=40}column.4.linkedname=direct<br>column.4.listlist sort=string(description)<br>column.4.namekey=description.abbr<br>column.4.querysort=description<br>column.4.shortview=false<br>column.4.étich=75<br>column.4.valuefield=description<br>column.4.valueformat=HTML<br>column.4.width=150<br>column.5.descriptionkey=status<br>column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum<br>column.5.linkedname=direct<br>column.5.listsort=string(status)<br>column.5.namekey status.abbr<br>column.5.querysort=status<br>column.5.shortview=false<br>column.5.étich=0<br>column.5.type=enum<br>column.5.valuefield=status<br>column.5.valueformat=val<br>column.5.width=15 0<br>column.6.displayname=Resolving Object Name<br>column.6.linkedname=resolveTask<br>column.6.namekey=view.relatedcolumn<br>column.6.namekeyargkey.0=resolveTask<br>column.6.namekeyargkey.1=name<br>column 6.querysort=resolveTask:name<br>column.6.sharecol=true<br>column.6.textmode=true<br>column.6.valuefield=resolveTask:name<br>column.6.valueformat=HTML<br>column.7.displayname=<br>column.7.linkedname=OpTask<br>column.7.namekey=view.relatedcolumn<br>column.7.namekeyargkey.0=resolveOpTask<br>column.7.namekeyargkey.1=name<br>column.7.querysort=resolveOpTask:name<br> column.sharecol=true 78}column.7.textmode=true<br>column.7.valuefield=resolveOpTask:name<br>column.7.valueformat=HTML<br>column.8.displayname=<br>column.8.linkedname=resolveProject<br>column.8.namekey=view.relatedcolumn{8 4}column.8.namekeyargkey.0=resolveProject<br>column.8.namekeyargkey.1=name<br>column.8.querysort=resolveProject:name<br>column.8.textmode=true<br>column.8.valuefield=resolveProject:name<br>column.8.value<br>column.9.displayname=Resolving Object Percent Complete<br>column.9.textmode=true<br>column.9.value expression=IF(ISBLANK({resolveTask}).<br><br><br><br><br>{ID}),{resolveProject}.{percentComplete},IF(ISBLANK({resolveProject}).{ID}),{resolveTask}.{percentComplete},&#39;&#39;)<br>column.9.valueformat=doubleAsPercentRounded</pre>

1. Cliquez sur **Enregistrer la vue**.
