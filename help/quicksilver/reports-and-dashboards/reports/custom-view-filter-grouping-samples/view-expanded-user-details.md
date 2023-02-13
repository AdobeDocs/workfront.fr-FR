---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Affichage : détails utilisateur étendus'
description: Cette vue Utilisateur affiche des informations sur vos utilisateurs. Outre leur nom, leur niveau d’accès et leur société, il affiche également la liste de leurs groupes, équipes et rôles de tâche.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a978b43-4718-43fb-80b8-844b35e09d06
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Afficher : détails utilisateur étendus

Cette vue Utilisateur affiche des informations sur vos utilisateurs. Outre leur nom, leur niveau d’accès et leur société, il affiche également la liste de leurs groupes, équipes et rôles de tâche.

![expand_user_view.png](assets/expanded-user-view-350x75.png)

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

## Affichage des détails utilisateur étendus

Pour appliquer cette vue :

1. Accédez à une liste d’utilisateurs.
1. Dans la **Affichage** menu déroulant, sélectionnez **Nouvelle vue**.

1. Dans le **Aperçu des colonnes** , éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode de texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la **Mode texte** et remplacez-le par le code suivant :

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: extra tag here that adds extra spaces in Preview)
   </MadCap:conditionalText>
   -->

   <pre>column.0.descriptionkey=name <br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.étich=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=acclevel<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.value=accessLevel:ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=accessLevel:objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=accessLevel<br>column.1.listsort=string(displayName)<br>column.1.namekey=accessible level<br>column.1.querysort=name<br>column.1.shortview=false<br>column.1.étich=0<br>column.1.valuefield=accessLevel:displayName<br>column.1.valueformat=HTML<br>column.1.viewalias=accessLevel:displayName<br>column.1.width=100<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.value=val(objCode)<br>column.2.listsepariter=<br>column.2.listmethod=nested(userGroups).lists<br>column.2.namekey=group.plural<br>column.2.étirement=50<br>column.2.type=iterate<br>column.2.valuefield=group:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.displayname=Teams<br>column.3.listsepariter=<br>column.3.listmethod=nested(équipes).lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.value.expression={name}<br>column.3.value.format=HTML<br>column.4.link.linkproperty.0.name=ID<br>column.4.link.linkproperty.0.valuefield=ID<br>column.4.link.linkproperty.0.valueformat=int<br>column.4.link.lookup=link.view<br>column.4.link.value=val(objCode)<br>column.4.listsepariter=<br>column.4.listmethod=nested(userRoles).lists<br>column.4.namekey=jobrole.plural<br>column.4.étich=50<br>column.4.type=iterate<br>column.4.valuefield=role:name<br>column.4.valueformat=HTML<br>column.4.width=150<br>column.5.descriptionkey=company<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valuefield=company:ID<br>column.5.link.linkproperty.0.valueformat=int<br>column.5.link.lookup=link.view<br>column.5.link.valuefield=company:objCode<br>column.5.link.valueformat=val<br>column.5.linkedname=company<br>column.5.listsort=nested(company).string(name)<br>column.5.namekey=company<br>column.5.querysort=company:name<br>column.5.shortview=false<br>column.5.étich=0<br>column.5.valuefield=company:name<br>column.5.valueformat=HTML<br>column.5.width=150</pre>

1. Cliquez sur **Enregistrer la vue**.
