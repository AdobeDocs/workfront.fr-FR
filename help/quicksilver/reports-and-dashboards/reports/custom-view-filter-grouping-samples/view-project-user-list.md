---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Affichage : liste des utilisateurs de projet avec des rôles de tâche"
description: Vous pouvez appliquer cette vue dans une liste de projets ou un rapport pour afficher la liste des utilisateurs associés au projet, ainsi qu’une liste des rôles de tâche qu’ils effectuent dans le projet.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 30%

---

# Vue : liste des utilisateurs et utilisatrices du projet avec les fonctions

Vous pouvez appliquer cette vue dans une liste de projets ou un rapport pour afficher la liste des utilisateurs associés au projet, ainsi qu’une liste des rôles de tâche qu’ils effectuent dans le projet.

Les informations de ce rapport se trouvent également dans la zone Personnes du projet.

>[!TIP]
>
>Si aucun rôle de tâche n’est répertorié pour les utilisateurs mais que vous savez qu’ils sont associés à des rôles de travail dans leur profil utilisateur, cela peut signifier qu’ils sont affectés à des tâches et des problèmes, mais qu’ils ne sont pas associés à un rôle de tâche sur la tâche ou le problème, ou que les utilisateurs répertoriés dans le rapport ne sont pas les personnes désignées sur des tâches et des problèmes, mais remplissent d’autres rôles sur le projet (par exemple, Propriétaire ou Sponsor.)

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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

## Affichage d’une liste d’utilisateurs de projet avec des rôles de tâche

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Afficher**, sélectionnez **Nouvelle vue**.

1. Dans la zone **Aperçu des colonnes**, supprimez toutes les colonnes sauf une.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte**.
1. Placez le pointeur de la souris sur la zone de mode Texte, puis cliquez sur **Cliquez pour modifier le texte**.
1. Supprimez le texte que vous trouvez dans la zone **Text Mode** et remplacez-le par le code suivant :
   <pre>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.section=0<br>column.0.shortview=false<br>column.0.étich=10 0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=200<br>column.1.displayname=Project Users<br>column.1.listsepariter=&lt;br&gt;<br>column.1.listmethod=nested(projectUsers).lists 3}column.1.textmode=true<br>column.1.type=iterate<br>column.1.valueexpression={user}.<br>{name}<br>column.1.valueformat=HTML<br>column.2.displayname=Project Roles<br>column.2.listsepariter=&lt;br&gt;<br>column.2.listmethod=nested(projectUserRoles).lists<br>column.2.textmode=true<br>column.2.type=iterate<br>column.2.2.2 ueexpression={role}.{name}<br>column.2.valueformat=HTML</pre>

1. Cliquez sur **Enregistrer la vue**.
