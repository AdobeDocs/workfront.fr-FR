---
title: Présentation du type de licence lors de l’utilisation de la planification Adobe Workfront
description: Votre accès à Adobe Workfront Planning dépend de votre type de licence, en plus de vos autorisations d’accès aux objets. Tous les utilisateurs de l’organisation ne disposent pas des mêmes droits d’accès et autorisations pour utiliser Adobe Workfront Planning. Cet article décrit les niveaux d’accès que les utilisateurs peuvent avoir à Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 9%

---


# Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning

{{planning-important-intro}}

Votre type de licence Adobe Workfront fonctionne conjointement avec vos autorisations Adobe Workfront Planning pour donner l’accès suivant :

* Affichage, contribution ou gestion des espaces de travail
* Affichage ou gestion des vues.

Pour plus d’informations sur les autorisations sur les objets Workfront Planning, consultez [Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Pour plus d’informations sur l’accès à Workfront Planning, consultez la [présentation de l’accès à Adobe Planning](/help/quicksilver/planning/access/access-overview.md).

## Relation entre les types de licences Workfront et les autorisations Workfront Planning

Le tableau ci-dessous décrit la relation entre le type de licence d’un utilisateur dans Adobe Workfront et le niveau d’autorisation que vous pouvez lui accorder aux objets de planification Adobe Workfront en fonction de cette licence.

L’attribution d’autorisations d’utilisateur à un espace de travail leur accorde également des autorisations pour les types d’enregistrement, les enregistrements et les champs.

Vous devez accorder aux utilisateurs des autorisations distinctes pour les vues, en plus de celles dont ils disposent pour les espaces de travail, afin qu’ils puissent accéder aux vues et les gérer.

| Type de licence Adobe Workfront* | Autorisations les plus élevées autorisées dans Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standard | <p>Les utilisateurs peuvent gérer les espaces de travail et les vues. Ils peuvent créer, modifier ou supprimer des espaces de travail, des types d’enregistrement, des enregistrements, des champs et des vues.</p> <br> <p>Les administrateurs système disposent des autorisations de gestion pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p> |
| Clair ou contributeur | <p>Les utilisateurs peuvent afficher les espaces de travail partagés avec eux, ainsi que les types d’enregistrement, les enregistrements et les champs de ces espaces de travail.</p> <br> <p>Les utilisateurs peuvent afficher les vues partagées avec eux, mais ils ne peuvent pas créer les leurs. </p><br> <p>Les utilisateurs ne peuvent pas créer, modifier ou supprimer des espaces de travail, des types d’enregistrement, des enregistrements ou des champs.</p> |

*Workfront Planning n’est pas disponible pour les licences Workfront héritées.
Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


<!--OLD 

| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

### Types de licence et autorisations d’espace de travail

Seuls les utilisateurs disposant d’une licence Standard peuvent disposer de droits Contribute ou Gérer sur les espaces de travail. Les utilisateurs disposant de tous les autres types de licence peuvent disposer d’autorisations d’ affichage sur les espaces de travail partagés avec eux.

Les administrateurs système peuvent afficher tous les espaces de travail du système, même ceux qu’ils n’ont pas créés.

>[!INFO]
>
>**EXEMPLE**
>
>Les contributeurs ou les utilisateurs de licence légère ne peuvent pas contribuer aux espaces de travail et à leurs objets ni les gérer.
>
>La boîte de partage indique que les utilisateurs ne peuvent pas se voir accorder l’autorisation de contribuer ou de gérer un espace de travail lorsqu’ils détiennent une licence de niveau inférieur, car ces niveaux d’autorisation sont grisés.
>
>![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Types de licence et autorisations d’affichage

Seuls les utilisateurs disposant d’une licence Standard peuvent disposer des autorisations de gestion pour les vues. Les utilisateurs disposant de tous les autres types de licence peuvent disposer d’autorisations d’affichage pour les vues partagées avec eux.

>[!INFO]
>
>**EXEMPLE**
>
>Les contributeurs ou les utilisateurs de licence légère ne peuvent pas gérer les vues. Ils peuvent appliquer des filtres, des classements ou des regroupements temporaires aux vues auxquelles ils ont accès.
>
>La boîte de partage indique que les utilisateurs ne peuvent pas se voir accorder l’autorisation de gérer une vue lorsqu’ils détiennent une licence de niveau inférieur, car ces niveaux d’autorisation sont grisés.
>
>![](assets/permissions-grayed-out-for-light-user.png)
