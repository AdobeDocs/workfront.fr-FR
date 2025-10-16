---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Afficher : liste des utilisateurs du projet ayant des fonctions'
description: Vous pouvez appliquer cette vue dans une liste de projets ou un rapport pour afficher la liste des utilisateurs et utilisatrices associés au projet, ainsi qu’une liste des fonctions qu’ils assument dans le projet.
author: Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 77%

---

# Vue : liste des utilisateurs et utilisatrices de projet avec des fonctions

<!--Audited: 11/2024-->

Vous pouvez appliquer cette vue dans une liste de projets ou un rapport pour afficher la liste des utilisateurs et utilisatrices associés au projet, ainsi qu’une liste des fonctions qu’ils assument dans le projet.

Les informations de ce rapport se trouvent également dans la zone Personnes du projet.

>[!TIP]
>
>Si aucune fonction n’est répertoriée pour les utilisateurs et utilisatrices mais que vous savez qu’ils sont associés à des fonctions dans leur profil, cela peut signifier qu’ils sont affectés à des tâches et des problèmes, mais qu’ils ne sont pas associés à une fonction sur la tâche ou le problème. Cela peut aussi vouloir dire que les utilisateurs et utilisatrices répertoriés dans le rapport ne sont pas les personnes désignées des tâches et des problèmes, mais qu’ils assument d’autres rôles sur le projet (par exemple, personne propriétaire ou sponsor).

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou demande de modification d’une vue </p>
   <p>Standard ou Plan pour modifier un rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Modifier l’accès aux rapports, tableaux de bord et calendriers pour modifier un rapport</p> <p>Modifier l’accès aux filtres, affichages et groupes pour modifier un affichage</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer les autorisations d’un rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++


## Afficher une liste d’utilisateurs et utilisatrices de projet avec des fonctions

1. Accédez à une liste de projets.
1. Dans le menu déroulant **Affichage**, sélectionnez **Nouvel affichage**.
1. Dans la zone **Aperçu des colonnes**, éliminez toutes les colonnes à l’exception d’une seule.
1. Cliquez sur l’en-tête de la colonne restante, puis sur **Passer en mode Texte** > **Modifier le mode Texte**.
1. Supprimez le texte de la zone **Modifier le mode texte** et remplacez-le par le code suivant :

   ```
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=200
   column.1.displayname=Project Users
   column.1.listdelimiter=<br>
   column.1.listmethod=nested(projectUsers).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={user}.{name}
   column.1.valueformat=HTML
   column.2.displayname=Project Roles
   column.2.listdelimiter=<br>
   column.2.listmethod=nested(projectUserRoles).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={role}.{name}
   column.2.valueformat=HTML
   ```

1. Cliquez sur **Terminé** > **Enregistrer la vue**.
