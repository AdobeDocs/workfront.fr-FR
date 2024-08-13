---
title: Présentation du type de licence lors de l’utilisation de la planification Adobe Workfront
description: Votre accès à Adobe Workfront Planning dépend de votre type de licence, en plus de vos autorisations sur les objets.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: f3641e2207563f3fc9d9ed059d889ab6c22f05b1
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 15%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning

{{planning-important-intro}}

Votre type de licence Adobe Workfront fonctionne conjointement avec vos autorisations Adobe Workfront Planning pour donner l’accès suivant :

* Affichage, contribution ou gestion des espaces de travail
* Affichage ou gestion des vues.

Pour plus d’informations sur les autorisations sur les objets Workfront Planning, consultez [Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## Relation entre les types de licences Workfront et les autorisations Workfront Planning

Le tableau ci-dessous décrit la relation entre le type de licence d’un utilisateur dans Adobe Workfront et le niveau d’autorisation que vous pouvez lui accorder aux objets de planification Adobe Workfront en fonction de cette licence.

L’attribution d’autorisations d’utilisateur à un espace de travail leur accorde également des autorisations pour les types d’enregistrement, les enregistrements et les champs.


| Type de licence Adobe Workfront* | Autorisations les plus élevées autorisées dans Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nouvelle : licence standard <br> ou <br>Actuelle : licence forfait | Les utilisateurs peuvent gérer les espaces de travail. Ils peuvent créer, modifier ou supprimer des espaces de travail, des types d’enregistrement, des enregistrements et des champs. <br> Les administrateurs système disposent des autorisations de gestion pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés. |
| Nouveau : léger, contributeur <br> ou <br>actuel : travail, demandeur, réviseur | Les utilisateurs peuvent afficher les espaces de travail partagés avec eux, ainsi que les types d’enregistrement, les enregistrements et les champs de ces espaces de travail. <br> Les utilisateurs ne peuvent pas créer, modifier ou supprimer des espaces de travail, des types d’enregistrement, des enregistrements ou des champs. |

*Pour plus d’informations, voir [Conditions d’accès dans la documentation de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Replace the table above with the following at GA:


| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|Standard                     | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| Light or Contributor  | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->

### Types de licence et autorisations d’espace de travail

Seuls les utilisateurs disposant d’une licence Standard (ou Plan) peuvent disposer de droits Contribute ou Gérer sur les espaces de travail. Les utilisateurs disposant de tous les autres types de licence peuvent disposer d’autorisations d’ affichage sur les espaces de travail partagés avec eux.

Les administrateurs système peuvent afficher tous les espaces de travail du système, même ceux qu’ils n’ont pas créés.

>[!INFO]
>
>**EXEMPLE :**
>
>Les demandeurs (ou collaborateurs, selon le nouveau modèle de licence) ne peuvent pas contribuer ou gérer les espaces de travail et leurs objets.
>
>La boîte de partage indique que les utilisateurs ne peuvent pas se voir accorder l’autorisation de contribuer ou de gérer un espace de travail lorsqu’ils détiennent une licence de niveau inférieur, car ces niveaux d’autorisation sont grisés.
>
>![](assets/permissions-grayed-out-for-requestor-user.png)


<!--Replace all the content in the section above with the following at Planning GA


Only users with a Standard license can have Contribute or Manage permissions to workspaces. Users with all other license types can have View permissions to workspaces shared with them. 

System administrators can view all workspaces in the system, even the ones they did not create. 

>[!INFO]
>
>**EXAMPLE:** 
>
>Contributors or Light-license users cannot contribute to or manage workspaces and their objects. 
>
>There is an indication in the sharing box that users cannot be granted permissions to contribute to or manage a workspace when they hold a lower-level license, as these permissions levels are dimmed. 
>
>![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)
-->


### Types de licence et autorisations d’affichage

Seuls les utilisateurs disposant d’une licence Standard (ou Plan) peuvent disposer des autorisations de gestion pour les vues. Les utilisateurs disposant de tous les autres types de licence peuvent disposer d’autorisations d’affichage pour les vues partagées avec eux.

>[!INFO]
>
>**EXEMPLE :**
>
>Les contributeurs (ou les demandeurs et les réviseurs) ne peuvent pas gérer les vues. Ils peuvent appliquer des filtres, des classements ou des regroupements temporaires aux vues auxquelles ils ont accès.
>
>La boîte de partage indique que les utilisateurs ne peuvent pas se voir accorder l’autorisation de gérer une vue lorsqu’ils détiennent une licence de niveau inférieur, car ces niveaux d’autorisation sont grisés.
>
>![](assets/permissions-grayed-out-for-reviewer-user-on-a-view.png)


<!--Replace all of the above in this section with the following at GA:

Only users with a Standard license can have Manage permissions to views. Users with all other license types can have View permissions to views shared with them. 

>[!INFO]
>
>**EXAMPLE:** 
>
>Contributors or Light-license users cannot manage views. They can apply temporary filters, sorts, or groupings to views they can access. 
>
>There is an indication in the sharing box that users cannot be granted permissions to manage a view when they hold a lower-level license, as these permissions levels are dimmed. 
>
>![](assets/permissions-grayed-out-for-light-user.png)-->
















<!--Replace all of the above with this:

The table below describes the relationship between the license type of a user in Adobe Workfront and the level of permissions you can grant to them to Adobe Workfront Planning objects based on that license. 

Granting a user permissions to a workspace also grants them permissions to record types, records, and fields. 

You must grant view permissions separately from workspace permissions. 


| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | <ul><li>Users can contribute to or manage workspaces and they can manage views. They can create, edit, or delete workspaces, record types, records, fields, and views.</li> <li> System administrators have Manage permissions to all workspaces, including the ones they did not create.</li> <li> System administrators can only access views they created.</li></ul>                                                                                                                     |
|New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | <ul><li>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</li> <li>Users can access views shared with them and apply temporary filters, sorts, or groupings, but they cannot modify the views. </li><li> Users cannot create, edit, or delete workspaces, record types, records, fields, or views.</li></ul>|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->