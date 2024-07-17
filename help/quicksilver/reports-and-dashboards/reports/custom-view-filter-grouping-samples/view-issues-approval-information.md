---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : problèmes avec les informations de validation'
description: La vue de problème suivante affiche le processus d’approbation, l’étape, les noms des approbateurs et l’état du problème avant l’approbation. Certains de ces champs ne sont pas accessibles par le biais du créateur d’interface standard.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 29%

---

# Vue : problèmes avec informations d’approbation

La vue de problème suivante affiche le processus d’approbation, l’étape, les noms des approbateurs et l’état du problème avant l’approbation. Certains de ces champs ne sont pas accessibles par le biais du créateur d’interface standard.

![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

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

## Afficher les problèmes avec les informations d’approbation

1. Accédez à une liste de problèmes.
1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, supprimez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode Texte, puis cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :
   <pre style="font-style: normal;">column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br> 0.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.étich=40<br>column 0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=220<br>column.1.description=assignedto<br>column.1.linkedname=assignedTo<br>column.1.listsort=nested(assignedTo).string(name){1) 8}column.1.name=assignedto<br>column.1.querysort=assignedTo:name<br>column.1.shortview=true<br>column.1.étich=0<br>column.1.valuefield=assignedTo:name<br>column.1.valueformat=HTML<br>column 1.1.width=150<br>column.2.descriptionkey=role<br>column.2.linkedname=role<br>column.2.listsort=nested(role).string(name)<br>column.2.name=role<br>column.2.querysort=role:name<br>column.2 shortview=false<br>column.2.étich=25<br>column.2.valuefield=role:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=Approval Process Name<br>column.3.linkedname=direct<br> column.3.listsort=string(name)<br>column.3.name=Approval Process Name<br>column.3.querysort=name<br>column.3.shortview=false<br>column.3.étich=35<br>column.3.valuefield=approvalProcess:name<br>column.3.value HTML<br>column.3.width=220<br>column.4.description=Approval Step Name<br>column.4.linkedname=direct<br>column.4.listsort=string(name)<br>column.4.name=Approval Step Name<br>column.4.querysort=name<br>column.4 shortview=false<br>column.4.étich=0<br>column.4.valuefield=currentApprovalStep:name<br>column.4.valueformat=HTML<br>column.4.width=220<br>column.5.description=Previous Status<br>column.5.linkedname=direct<br>column.5.listsort=string(name)<br>column.5.name=Previous Status<br>column.5.querysort=name<br>column.5.shortview=false<br>column.5.étich=0<br>column.5.valuefield=previousStatus<br>column.5.valueformat=HTML{6 4}column.5.width=220<br>column.6.linkedname=direct<br>column.6.listsort=HTML(approversString)<br>column.6.namekey=approver.plural.abbr<br>column.6.querysort=approversString<br> column.6.view=false<br>column.6.étich=0<br>column.6.valuefield=approversString<br>column.6.valueformat=HTML<br>column.6.viewalias=approver.plural<br>column.6.width=200<br><br><br></pre>

1. Cliquez sur **Enregistrer la vue**.
