---
title: Présentation Du Type De Licence Lors De L’Utilisation D’Adobe Workfront Planning
description: Votre accès à Adobe Workfront Planning dépend de votre type de licence et de vos autorisations d'objets. Tous les utilisateurs de l’organisation n’ont pas le même accès et les mêmes autorisations pour utiliser Adobe Workfront Planning. Cet article décrit les niveaux d’accès que les utilisateurs peuvent avoir à Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: cf3b5d3f8e3a8a1922da757a41b4c5e0ee84e6fd
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 10%

---


# Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de manière générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Votre type de licence Adobe Workfront fonctionne de concert avec vos autorisations Adobe Workfront Planning pour donner les accès suivants :

* Affichage, contribution ou gestion des espaces de travail
* Afficher ou gérer des vues.

Pour plus d’informations sur les autorisations sur les objets Workfront Planning, consultez [Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Pour plus d’informations sur l’accès à Workfront Planning, consultez la présentation de l’accès à Adobe Planning [](/help/quicksilver/planning/access/access-overview.md).

## Relation entre les types de licences Workfront et les autorisations Workfront Planning

Le tableau ci-dessous décrit la relation entre le type de licence d’un utilisateur dans Adobe Workfront et le niveau des autorisations que vous pouvez lui accorder sur les objets Adobe Workfront Planning en fonction de cette licence.

L’octroi des autorisations d’un utilisateur à un espace de travail lui accorde également des autorisations sur les types d’enregistrements, les enregistrements et les champs.

Pour pouvoir accéder aux vues et les gérer, vous devez accorder aux utilisateurs des autorisations distinctes aux vues, en plus de celles dont ils disposent pour les espaces de travail.

| Type de licence Adobe Workfront* | Autorisations les plus élevées autorisées dans Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standard | <p>Les utilisateurs peuvent gérer les espaces de travail et les vues. Ils peuvent créer, modifier ou supprimer des espaces de travail, des types d’enregistrements, des enregistrements, des champs et des vues.</p> <br> <p>Les administrateurs système disposent des autorisations de niveau Gérer pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p> |
| Léger ou contributeur | <p>Les utilisateurs peuvent afficher les espaces de travail partagés avec eux, ainsi que les types d’enregistrements, les enregistrements et les champs de ces espaces de travail.</p> <br> <p>Les utilisateurs peuvent afficher les vues partagées avec eux, mais ils ne peuvent pas créer les leurs. </p><br> <p>Les utilisateurs ne peuvent pas créer, modifier ni supprimer des espaces de travail, des types d’enregistrements, des enregistrements ou des champs.</p> |

*Workfront Planning n’est pas disponible pour les licences Workfront héritées.
Pour plus d’informations, voir [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


<!--OLD 

| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

### Types de licences et autorisations d’espace de travail

Seuls les utilisateurs disposant d’une licence Standard peuvent disposer d’autorisations Contribute ou Gérer sur les espaces de travail. Les utilisateurs disposant de tous les autres types de licence peuvent disposer d’autorisations d’affichage des espaces de travail partagés avec eux.

Les administrateurs système peuvent afficher tous les espaces de travail du système, même ceux qu’ils n’ont pas créés.

>[!INFO]
>
>**EXEMPLE**
>
>Les contributeurs ou les utilisateurs sous licence light ne peuvent pas contribuer aux espaces de travail et à leurs objets ni les gérer.
>
>Le champ Partage indique que les utilisateurs ne peuvent pas être autorisés à contribuer à ou gérer un espace de travail s’ils disposent d’une licence de niveau inférieur, car ces niveaux d’autorisation sont grisés.
>
><span class="preview">![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)</span>


### Types de licence et autorisations d’affichage

Seuls les utilisateurs disposant d’une licence Standard peuvent disposer d’autorisations de niveau Gérer pour les vues. Les utilisateurs disposant de tous les autres types de licence peuvent disposer d&#39;autorisations d&#39;affichage des vues partagées avec eux.

>[!INFO]
>
>**EXEMPLE**
>
>Les contributeurs ou les utilisateurs de licence light ne peuvent pas gérer les vues. Ils peuvent appliquer des filtres, des tris ou des regroupements temporaires aux vues auxquelles ils ont accès.
>
>Le champ Partage indique que les utilisateurs ne peuvent pas se voir accorder d’autorisations pour gérer une vue s’ils disposent d’une licence de niveau inférieur, car ces niveaux d’autorisations sont grisés.
>
><span class="preview">![](assets/permissions-grayed-out-for-light-user.png)</span>
