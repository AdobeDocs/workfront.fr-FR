---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : afficher les informations sur le programme et le Portfolio dans une vue de tâche'
description: Cette vue de tâche affiche le programme et le Portfolio associés au projet de la tâche. Ces informations ne sont pas disponibles dans le créateur de rapports lors de la création d’un affichage de tâche. Ces informations sont disponibles uniquement en mode texte.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Afficher : afficher les informations sur le programme et le Portfolio dans une vue de tâche ;

Cette vue de tâche affiche le programme et le Portfolio associés au projet de la tâche. Ces informations ne sont pas disponibles dans le créateur de rapports lors de la création d’un affichage de tâche. Ces informations sont disponibles uniquement en mode texte.

La vue fournit également des liens vers le projet, le programme et le Portfolio à partir d’une liste de tâches.

![](assets/view--program-and-portfolio-350x116.png)

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

## Affichage des informations sur le programme et le Portfolio dans une vue de tâche

Pour appliquer cette vue à une liste de tâches :

1. Accédez à une liste de tâches.
1. Dans la **Affichage** menu déroulant, sélectionnez **Nouvelle vue**.

1. Dans le **Aperçu des colonnes** , éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.étich=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=project<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=project:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=project:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=project<br>column.1.listsort=nested(project).string(name)<br>column.1.namekey=project<br>column.1.querysort=project:name<br>column.1.shortview=false<br>column.1.étich=0<br>column.1.valuefield=project:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=program<br>column.2.displayname=Program<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=project:program:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=project:program:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=project<br>column.2.listsort=nested(project:program).string(name)<br>column.2.namekey=project<br>column.2.querysort=project:program:name<br>column.2.shortview=false<br>column.2.étich=0<br>column.2.valuefield=project:program:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.descriptionkey=portfolio<br>column.3.displayname=Portfolio<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=project:portfolio:ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=project:portfolio:objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=project<br>column.3.listsort=nested(project:portfolio).string(name)<br>column.3.namekey=project<br>column.3.querysort=project:portfolio:name<br>column.3.shortview=false<br>column.3.étirement=0<br>column.3.valuefield=project:portfolio:name<br>column.3.value.format=HTML<br>column.3.width=150 </pre>

1. Cliquez sur **Enregistrer la vue**.
