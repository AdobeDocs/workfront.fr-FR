---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '« Vue : liste des utilisateurs et utilisatrices du projet avec des fonctions »'
description: Vous pouvez appliquer cette vue dans une liste de projets ou un rapport pour afficher la liste des utilisateurs et utilisatrices associés au projet, ainsi qu’une liste des fonctions qu’ils assument dans le projet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 100%

---

# Vue : liste des utilisateurs et utilisatrices de projet avec des fonctions

Vous pouvez appliquer cette vue dans une liste de projets ou un rapport pour afficher la liste des utilisateurs et utilisatrices associés au projet, ainsi qu’une liste des fonctions qu’ils assument dans le projet.

Les informations de ce rapport se trouvent également dans la zone Personnes du projet.

>[!TIP]
>
>Si aucune fonction n’est répertoriée pour les utilisateurs et utilisatrices mais que vous savez qu’ils sont associés à des fonctions dans leur profil, cela peut signifier qu’ils sont affectés à des tâches et des problèmes, mais qu’ils ne sont pas associés à une fonction sur la tâche ou le problème. Cela peut aussi vouloir dire que les utilisateurs et utilisatrices répertoriés dans le rapport ne sont pas les personnes désignées des tâches et des problèmes, mais qu’ils assument d’autres rôles sur le projet (par exemple, personne propriétaire ou sponsor).

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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

## Afficher une liste d’utilisateurs et utilisatrices de projet avec des fonctions

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Vue**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu de la colonne**, éliminez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis cliquez sur **Basculer en mode texte**.
1. Placez la souris sur la zone Mode texte, puis cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Mode texte** et remplacez-le par le code suivant :
   <pre>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.displayname=Project Users<br>column.1.listdelimiter=&lt;br&gt;<br>column.1.listmethod=nested(projectUsers).lists<br>column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={user}.{name}<br>column.1.valueformat=HTML<br>column.2.displayname=Project Roles<br>column.2.listdelimiter=&lt;br&gt;<br>column.2.listmethod=nested(projectUserRoles).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.valueexpression={role}.{name}<br>column.2.valueformat=HTML</pre>

1. Cliquez sur **Enregistrer la vue**.
