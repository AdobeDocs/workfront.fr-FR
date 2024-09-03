---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : projet avec toutes les personnes et tous les rôles de l’équipe de projet »'
description: Cette vue du projet présente une liste de personnes et de fonctions affectées à l’équipe de projet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 84a1e065-992e-4aa5-81ba-e699ac704837
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 100%

---

# Vue : projet avec toutes les personnes et tous les rôles de l’équipe de projet

Cette vue du projet présente une liste de personnes et de fonctions affectées à l’équipe de projet.

>[!NOTE]
>
>Si la fonction figure sur la même ligne qu’une personne, cela ne signifie pas que la personne remplit ce rôle dans le projet, ni que ce rôle lui a été affecté dans son profil.

![project_custom_view_with_all_users_and_roles_on_the_project_.png](assets/project-custom-view-350x52.png)

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Demander la modification d’un affichage </p>
   <p>Prévoir de modifier un rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si votre niveau d’accès est soumis à des restrictions supplémentaires. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

## Afficher un projet avec toutes les personnes et tous les rôles de l’équipe de projet

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Affichage**, sélectionnez **Nouvel affichage**.

1. Dans la zone **Prévisualisation de la colonne**, éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis cliquez sur **Basculer en mode texte**.
1. Placez le pointeur de la souris sur la zone du mode texte, puis cliquez sur **Cliquer pour modifier le texte**.
1. Supprimez le texte qui se trouve dans la zone **Mode texte** et remplacez-le par le code suivant :
   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=60<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Team Users<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=userID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.page=/userView.cmd<br>column.1.listdelimiter=<br>column.1.listmethod=nested(projectUsers).lists<br>column.1.namekey=user.plural<br>column.1.stretch=30<br>column.1.type=iterate<br>column.1.valuefield=user:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=Team Roles<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.page=/roleView.cmd<br>column.2.listdelimiter=<br>column.2.listmethod=nested(roles).lists<br>column.2.namekey=jobrole.plural<br>column.2.stretch=10<br>column.2.type=iterate<br>column.2.valuefield=name<br>column.2.valueformat=HTML<br>column.2.width=150.stretch=0</pre>

1. Cliquez sur **Enregistrer la vue**.
