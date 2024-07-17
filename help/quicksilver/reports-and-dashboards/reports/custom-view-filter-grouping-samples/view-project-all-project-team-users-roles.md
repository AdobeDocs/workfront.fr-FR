---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : projet avec tous les utilisateurs et rôles de l’équipe de projet'
description: Cette vue de projet affiche la liste des utilisateurs et des rôles de tâche affectés à l’équipe de projet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 84a1e065-992e-4aa5-81ba-e699ac704837
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 36%

---

# Vue : projet avec tous les utilisateurs et utilisatrices et rôles de l’équipe du projet

Cette vue de projet affiche la liste des utilisateurs et des rôles de tâche affectés à l’équipe de projet.

>[!NOTE]
>
>Si le rôle de tâche est répertorié sur la même ligne qu’un utilisateur, cela n’implique pas que l’utilisateur remplit ce rôle sur le projet, ni qu’il se voit attribuer ce rôle dans son profil.

![project_custom_view_with_all_users_and_rôles_on_the_project_.png](assets/project-custom-view-350x52.png)

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

## Affichage d’un projet avec tous les utilisateurs et rôles de l’équipe de projet

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, supprimez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode Texte, puis cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :
   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=5}column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.étich=60<br>column.0.valuefield=name<br> column 0.valueformat=HTML<br>column.0.width=150<br>column.1.description=Team Users<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=userID<br>column.1.link.linkproperty.0.value int<br>column.1.link.page=/userView.cmd<br>column.1.listsepariter=<br>column.1.listmethod=nested(projectUsers).lists<br>column.1.namekey=user.plural<br>column.1.étich=30<br>column.1.type=iterate<br>column.1.valuefield=user:name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=Team Roles<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=3 0}column.2.link.linkproperty.0.valueformat=int<br>column.2.link.page=/roleView.cmd<br>column.2.listsepariter=<br>column.2.listmethod=nested(rôles).lists<br>column.2.namekey=jobrole.plural<br>column.2.étich=10<br>column.2.type=iterate<br>column.2.valuefield=name<br>column.2.valueformat=HTML<br>column.2.width=150.étich=0<br><br></pre>

1. Cliquez sur **Enregistrer la vue**.
