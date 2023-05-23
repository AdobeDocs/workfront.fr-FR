---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Affichage : société et groupe d’accueil attribués à l’utilisateur"
description: Cette vue affiche la Société et le groupe d’accueil du propriétaire Principal de la tâche. Il s’agit de valeurs qui ne sont pas disponibles dans l’interface standard, mais qui sont accessibles via le mode texte.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Afficher : société et groupe d’accueil de l’utilisateur affecté

Cette vue affiche la Société et le groupe d’accueil du propriétaire Principal de la tâche. Il s’agit de valeurs qui ne sont pas disponibles dans l’interface standard, mais qui sont accessibles via le mode texte.

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## Affichage de la société et du groupe d’accueil de l’utilisateur affecté

1. Accédez à une liste de tâches.
1. Dans la **Affichage** menu déroulant, sélectionnez **Nouvelle vue**.

1. Dans le **Aperçu des colonnes** , éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valuefield=ID<br> column.0.link.linkproperty.0.valueformat=int<br> column.0.link.lookup=link.view<br> column.0.link.valuefield=objCode<br> column.0.link.valueformat=val<br> column.0.linkedname=direct<br> column.0.listsort=string(name)<br> column.0.namekey=name.abbr<br> column.0.querysort=name<br> column.0.shortview=false<br> column.0.étich=100<br> column.0.valuefield=name<br> column.0.valueformat=HTML<br> column.0.width=150<br> column.1.descriptionkey=assignedto<br> column.1.link.linkproperty.0.name=ID<br> column.1.link.linkproperty.0.valuefield=assignedTo:ID<br> column.1.link.linkproperty.0.valueformat=int<br> column.1.link.lookup=link.view<br> column.1.link.valuefield=assignedTo:objCode<br> column.1.link.valueformat=val<br> column.1.linkedname=assignedTo<br> column.1.listsort=nested(assignedTo).string(name)<br> column.1.namekey=assignedto<br> column.1.querysort=assignedTo:name<br> column.1.shortview=false<br> column.1.étich=0<br> column.1.valuefield=assignedTo:name<br> column.1.valueformat=HTML<br> column.1.width=150<br> column.2.description=Affecté à la société<br> column.2.displayname=Assigned To Company<br> column.2.linkedname=assignedTo:company<br> column.2.listsort=nested(assignedTo:company).string(name)<br> column.2.namekey=assignedto<br> column.2.querysort=assignedTo:company:name<br> column.2.shortview=false<br> column.2.étich=0<br> column.2.valuefield=assignedTo:company:name<br> column.2.valueformat=HTML<br> column.2.width=150<br> column.3.description=Affecté au groupe d’accueil<br> column.3.displayname=Assigned To Home Group<br> column.3.linkedname=assignedTo:homeGroup<br> column.3.listsort=nested(assignedTo:homeGroup).string(name)<br> column.3.namekey=assignedto<br> column.3.querysort=assignedTo:homeGroup:name<br> column.3.shortview=false<br> column.3.étirement=0<br> column.3.valuefield=assignedTo:homeGroup:name<br> column.3.value.format=HTML<br> column.3.width=150</pre>

1. Cliquez sur **Enregistrer les modifications**.
