---
title: Présentation Du Type De Licence Lors De L’Utilisation D’Adobe Workfront Planning
description: Votre accès à Adobe Workfront Planning dépend de votre type de licence et de vos autorisations d'objets. Tous les utilisateurs de l’organisation n’ont pas le même accès et les mêmes autorisations pour utiliser Adobe Workfront Planning. Cet article décrit les niveaux d’accès que les utilisateurs peuvent avoir à Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 5404cec0cb02d363154a3696b63aaedaafc82688
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 6%

---


# Vue d’ensemble du type de licence lors de l’utilisation d’Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Votre type de licence Adobe Workfront fonctionne de concert avec vos autorisations Adobe Workfront Planning pour donner les accès suivants :

* Afficher, contribuer ou gérer des espaces de travail ou des types d’enregistrements
* Afficher ou gérer des vues. <!--<span class="preview">and records</span>-->

Pour plus d’informations sur les autorisations sur les objets Workfront Planning, consultez [Vue d’ensemble du partage d’autorisations dans Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Pour plus d’informations sur l’accès à Workfront Planning, consultez [Présentation de l’accès à Adobe Planning](/help/quicksilver/planning/access/access-overview.md).

## Relation entre les types de licences Workfront et les autorisations Workfront Planning

Le tableau ci-dessous décrit la relation entre le type de licence d’un utilisateur dans Adobe Workfront et le niveau des autorisations que vous pouvez lui accorder sur les objets Adobe Workfront Planning en fonction de cette licence.

L’octroi des autorisations d’un utilisateur à un espace de travail lui accorde également des autorisations sur les types d’enregistrements, les enregistrements et les champs.

Pour pouvoir accéder aux vues et les gérer, vous devez accorder aux utilisateurs des autorisations distinctes aux vues, en plus de celles dont ils disposent pour les espaces de travail.

Tenez compte des points suivants lorsque vous utilisez des autorisations de type enregistrement :

* Les utilisateurs héritent automatiquement des autorisations de type d’enregistrement des espaces de travail.
* Lorsque l’utilisateur dispose d’autorisations de niveau Gérer sur un espace de travail, il ne peut pas avoir un accès moindre à un type d’enregistrement.
* Les utilisateurs ne peuvent pas disposer d’autorisations plus importantes pour un type d’enregistrement que pour l’espace de travail auquel appartient le type d’enregistrement.
* La suppression des autorisations des utilisateurs sur un type d’enregistrement ne supprime pas leur accès en lecture seule à tous les types d’enregistrements dans l’espace de travail, car cela ne supprime pas leurs autorisations sur l’espace de travail.

| Type de licence Adobe Workfront | Autorisations les plus élevées autorisées dans Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standard | <p>Les utilisateurs peuvent gérer les espaces de travail, les types d’enregistrements, les <!--<span class="preview">records</span>--> et les vues. Ils peuvent créer, modifier ou supprimer des espaces de travail, des types d’enregistrements, des enregistrements, des champs et des vues.</p><br><p>Les administrateurs système disposent des autorisations de niveau Gérer pour tous les espaces de travail, y compris ceux qu’ils n’ont pas créés.</p> |
| Léger ou contributeur | <p>Les utilisateurs peuvent afficher les espaces de travail partagés avec eux, ainsi que les types d’enregistrements, les enregistrements et les champs de ces espaces de travail.</p> <br> <p>Les utilisateurs peuvent afficher les vues partagées avec eux, mais ils ne peuvent pas créer les leurs. </p><br> <p>Les utilisateurs ne peuvent pas créer, modifier ni supprimer des espaces de travail, des types d’enregistrements, des enregistrements ou des champs.</p> |

<!--Old: 
*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->


### Types de licence et autorisations des espaces de travail et des types d’enregistrement

Seuls les utilisateurs disposant d’une licence Standard peuvent disposer d’autorisations de niveau Contribution ou Gérer sur les espaces de travail et les types d’enregistrements. Les autorisations Contribuer et Gérer des espaces de travail et des types d’enregistrements sont également transférées vers des enregistrements et des champs.

Les administrateurs système peuvent afficher tous les espaces de travail du système, y compris ceux qu’ils n’ont pas créés.

Les utilisateurs disposant de tous les autres types de licence peuvent disposer d’autorisations en lecture seule sur les espaces de travail et les types d’enregistrements partagés avec eux, ainsi que sur leurs enregistrements et champs.


>[!INFO]
>
>**EXEMPLE**
>
>Les contributeurs ou les utilisateurs sous licence light ne peuvent pas contribuer aux espaces de travail et à leurs objets ni les gérer.
>
>Le champ Partage indique que les utilisateurs ne peuvent pas être autorisés à contribuer à ou gérer un espace de travail s’ils disposent d’une licence de niveau inférieur, car ces niveaux d’autorisation sont grisés.
>
>![Autorisations grisées pour l’utilisateur contributeur sur l’espace de travail](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Types de licences et autorisations des vues

Seuls les utilisateurs disposant d’une licence Standard peuvent disposer d’autorisations de niveau Gérer pour les vues.

Les administrateurs système ne peuvent pas accéder aux vues qu&#39;ils n&#39;ont pas créées. Ils doivent être partagés avec eux.

Les utilisateurs disposant de tous les autres types de licence peuvent disposer d&#39;autorisations d&#39;affichage des vues partagées avec eux.

>[!INFO]
>
>**EXEMPLE**
>
>Les contributeurs ou les utilisateurs de licence light ne peuvent pas gérer les vues. Ils peuvent appliquer des filtres, des tris ou des regroupements temporaires aux vues auxquelles ils ont accès.
>
>Le champ Partage indique que les utilisateurs ne peuvent pas se voir accorder d’autorisations pour gérer une vue s’ils disposent d’une licence de niveau inférieur, car ces niveaux d’autorisations sont grisés.
>
>![Autorisations grisées pour un utilisateur léger sur le partage d’affichage](assets/permissions-grayed-out-for-light-user.png)
