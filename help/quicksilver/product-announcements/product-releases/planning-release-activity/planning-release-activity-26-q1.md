---
content-type: release-notes
title: Activité de la version du premier trimestre 2026 pour Adobe Workfront Planning
description: Il s’agit de l’activité de publication du produit Planification d’Adobe Workfront pour le premier trimestre 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: a58e7da96c43dd308a213c6d7ef74d5085a2e1ba
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 2%

---

# Activité de la version du premier trimestre 2026 pour Adobe Workfront Planning

Cet article décrit les nouvelles fonctionnalités de Workfront Planning de la version du premier trimestre 2026.

<!--keep the sentence below for all future quarterly release pages-->

Pour obtenir la liste de toutes les fonctionnalités publiées pour Adobe Workfront Planning, voir [Activité de version d’Adobe Workfront Planning : index des articles](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Partage de vues dans la page Projets - Enregistrements connectés

>[!NOTE]
>
>Aperçu : 18 décembre 2025
>Version rapide de production : 14 janvier 2026\
>Production pour tous : 15 janvier 2026

Pour vous assurer plus facilement de voir les informations dont vous avez besoin, nous avons ajouté la possibilité de partager des vues sur la page Enregistrements connectés aux projets . Vous pouvez désormais partager des vues avec d’autres utilisateurs, équipes ou groupes.

Pour plus d’informations sur les vues de requête, notamment le partage, consultez [Création et gestion de vues dans la zone des Requêtes](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md).

## Le caractère générique de l’utilisateur actuel est désormais disponible dans les filtres d’affichage de connexion du projet

>[!NOTE]
>
>Aperçu : 18 décembre 2025
>Version rapide de production : 14 janvier 2026\
>Production pour tous : 15 janvier 2026

Pour faciliter le filtrage des connexions de projet qui vous concernent, nous avons créé un caractère générique d&#39;utilisateur actuel. Désormais, lors du filtrage, vous pouvez sélectionner « Moi (utilisateur connecté) ». Le filtre s’applique alors à l’utilisateur qui consulte la liste des demandes.

Cela peut s’avérer pratique lors de l’ajout d’un filtre à une vue que plusieurs utilisateurs utiliseront. Chaque utilisateur verra les résultats des filtres qui s’appliquent à lui.

Le caractère générique est disponible dans les champs où la valeur est un utilisateur.

Pour plus d&#39;informations sur la configuration des vues de connexion au projet, y compris les filtres, voir [Ajouter une page Enregistrements connectés à un enregistrement](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

<!--

## Create record type hierarchies in workspaces

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production all: January 15, 2026 

You can now define flexible but structured hierarchies between record or object types.  

Hierarchies are connections between record types. You can have up to 4 record and object types connected in one hierarchy, and you can have multiple hierarchies in one workspace. The first record type in the hierarchy is a parent, and all the other record or object types are its children objects.  

You can use hierarchies to organize work in a way that reflects how your teams actually plan, operate, and deliver and to visualize how strategy flows into execution. 

Consider the following when building hierarchies: 

* You can have multiple hierarchies in a workspace 
* You can connect only Planning record types from one workspace and Workfront projects in a hierarchy.  
* A record type or a project can only have one parent in the same workspace. 
* A record type can be the parent in multiple hierarchies 
* Connectable record types cannot be used in hierarchies in other workspaces than their own. 
* Global record types can be used in hierarchies only in the workspaces that they were created in or have been added to.  

When you create hierarchies between record types, they generate breadcrumbs for records that belong to those record types. 

For more information, see [Hierarchy and breadcrumb overview](help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

<!--

## New unified breadcrumbs added to records' pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

We have added breadcrumbs to a record's page to reflect its spot in a hierarchy. After you create hierarchies, you can see a record's breadcrumb at the top of its page, indicating what other parent or children objects are connected to it. Hierarchies are consistent across Workfront and Planning.  

For example, you can view a project's Planning hierarchy when it's connected to Planning record types in its Planning breadcrumb, and its Workfront hierarchy when it's connected to Workfront object types, like Portfolios or Programs, in Workfront.  

For information, see [Hierarchy and breadcrumb overview](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

-->

## Améliorations de la page principale de Workspace

>[!NOTE]
>
>Aperçu : 18 décembre 2025
>Production rapide : 14 janvier 2026
>Production pour tous : 15 janvier 2026

Les améliorations suivantes ont été apportées à la page principale Espaces de travail dans la planification Workfront :

* Un défilement plus rapide et plus dynamique. Cela est particulièrement visible si votre organisation dispose d’un grand nombre d’espaces de travail et pour les administrateurs et administratrices système.

* Nous avons ajouté une zone de recherche qui vous permet désormais de rechercher un espace de travail spécifique par nom.

* L’onglet **Autres espaces de travail** a été renommé **Tous les espaces de travail** et comprend tous les espaces de travail que vous êtes autorisé à afficher, y compris ceux que vous avez créés.

Pour plus d’informations, voir [Modifier les espaces de travail](/help/quicksilver/planning/architecture/edit-workspaces.md).

<!--

## Improvements to connected records pages

>[!NOTE]
>
>Preview: December 18, 2025 
>Production fast: January 14, 2026 
>Production for all: January 15, 2026 

To give you more flexibility when working with connected records pages, we have enhanced the functionality of views in this area of Workfront Planning. The following are improvements in the connected records pages of a record that are coming with this release:

* You can now add a timeline and a calendar view to a record's connected records page.
* You can now share views from a connected records page. The views shared from these pages are visible system-wide by all users you share them with in any other area of Workfront Planning. All views shared in any other areas of Planning are also visible in the connected records page for the same users they are shared with.
* We have added a restriction to only allow one connected records page per each record or object type. Prior to this enhancement, you could add multiple pages for the same record or object type. Now, you can use multiple views for the same record type in one connected records page.
* We have added a **New row** link at the bottom of a table view and a **Connect records** button in the upper-right area of the connected records page. Prior to this enhancement, the **New row** link and the **Connect records** button existed only on a project connected page. 

For information, see [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

-->

## Ajout par défaut du champ Connexion de marque aux produits et aux personnes dans l’espace de travail GenStudio

>[!NOTE]
>
>Aperçu : 11 décembre 2025
>Version rapide de production : 11 décembre 2025
>Production pour tous : 11 décembre 2025

Le champ de connexion avec la marque GenStudio for Performance Marketing est désormais ajouté par défaut aux types d’enregistrements Produits et Personnes dans l’espace de travail GenStudio de Workfront Planning.

Votre organisation doit disposer de Workfront Planning et d’Adobe GenStudio for Performance Marketing.

Avant cette amélioration, vous ne pouviez ajouter manuellement le champ Connexion à Brand qu’à n’importe quel type d’enregistrement, y compris les produits et les personnes. Vous pouvez toujours connecter manuellement le type d’enregistrement Brand GenStudio à d’autres types d’enregistrements dans Workfront Planning.

Pour plus d’informations, voir [Prise en main de l’intégration d’Adobe Workfront Planning et d’Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).

## Restreindre la suppression des autorisations des utilisateurs de GenStudio for Performance Marketing de Planning

>[!NOTE]
>
>Aperçu : 11 décembre 2025
>Version rapide de production : 11 décembre 2025
>Production pour tous : 11 décembre 2025

Nous avons ajouté un mécanisme de sécurisation qui vous empêche de supprimer les autorisations des utilisateurs de GenStudio for Performance Marketing des objets Workfront Planning. Grâce à cette amélioration, vous ne pouvez plus supprimer les utilisateurs de GenStudio de l’espace de travail GenStudio dans Planning. Vous ne pouvez pas non plus désactiver les autorisations héritées pour les types d’enregistrements dans l’espace de travail GenStudio, si ces autorisations incluent les utilisateurs de GenStudio. Avant cette amélioration, lorsque vous supprimiez ces utilisateurs de l’espace de travail GenStudio dans Planning, ils perdaient également les autorisations pour les types d’enregistrements dans GenStudio.

Votre organisation doit disposer de Workfront Planning et d’Adobe GenStudio for Performance Marketing.

Pour plus d’informations, voir [Prise en main de l’intégration d’Adobe Workfront Planning et d’Adobe GenStudio for Performance Marketing](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md).


## Suppression du partage public de vues sur un type d’enregistrement global dans un espace de travail secondaire


>[!NOTE]
>
>Aperçu : 3 décembre 2025
>Version rapide de production : 4 décembre 2025
>Production pour tous : 15 janvier 2026


Nous avons supprimé l&#39;onglet Partage public lors du partage d&#39;une vue pour un enregistrement global dans un espace de travail secondaire. Vous ne pouvez pas partager publiquement une vue à partir d’un type d’enregistrement global ajouté à un autre espace de travail à partir d’un type d’enregistrement global existant. Vous pouvez partager publiquement une vue de type enregistrement global à partir de son espace de travail d’origine.

Pour plus d’informations, voir [Partager des vues](/help/quicksilver/planning/access/share-views.md).


## Connecter des marques GenStudio for Performance Marketing à des types d’enregistrements Workfront Planning

>[!NOTE]
>
>Aperçu : 13 novembre 2025
>Version rapide de production : 13 novembre 2025
>Production pour tous : 13 novembre 2025

Vous pouvez désormais connecter les types d’enregistrements Workfront Planning aux marques à partir d’Adobe GenStudio for Performance Marketing. Votre organisation doit disposer de Workfront Planning et d’Adobe GenStudio for Performance Marketing.

Pour plus d’informations, voir [Connecter les types d’enregistrements](/help/quicksilver/planning/architecture/connect-record-types.md).


## Nouvelle zone de recherche de champs dans les icônes Filtres, Champs et Couleurs de ligne dans les vues Planning

>[!NOTE]
>
>Aperçu : 6 novembre 2025
>Version rapide de production : 11 décembre 2025
>Production pour tous : 15 janvier 2026

Vous pouvez désormais rechercher un champ spécifique lors de la création d’un élément de vue dans une vue de type enregistrement. Nous avons ajouté des zones de recherche lorsque vous créez un filtre, un tri, un regroupement ou lorsque vous configurez vos champs ou les couleurs des lignes. Avant cette amélioration, il vous suffisait de faire défiler la liste des champs disponibles.

Cette amélioration est disponible dans toutes les vues de type d’enregistrement.

Pour plus d’informations, consultez la section [Gérer la vue en tableau](/help/quicksilver/planning/views/manage-the-table-view.md).


## Types d’enregistrements globaux et possibilité de les ajouter en tant que types d’enregistrements existants à d’autres espaces de travail

>[!NOTE]
>
>Aperçu : 16 octobre 2025
>Version rapide de production : 13 novembre 2025
>Production pour tous : 15 janvier 2026

Lors de l’implémentation de Workfront Planning pour une organisation multi-équipes avec des workflows communs, vous devrez peut-être définir une structure et des métadonnées cohérentes pour les types d’enregistrements clés (tels que les campagnes ou les éléments livrables) qui peuvent être ajoutés aux espaces de travail de chaque équipe pour capturer et gérer leur travail.

En outre, vous aurez peut-être besoin du travail de chaque équipe pour atteindre un niveau central.

Dans un tel workflow, vous pouvez vous assurer que les équipes capturent leur travail de manière cohérente tout en déverrouillant la visibilité entre les équipes, sans avoir à ajouter tous les membres de l’organisation à chaque espace de travail. Pour ce faire, vous pouvez utiliser des types d’enregistrements globaux.

Vous pouvez désormais désigner un type d’enregistrement comme global et l’utiliser sur plusieurs espaces de travail. Les utilisateurs peuvent utiliser la même structure de champs et les mêmes connexions que celles déjà configurées dans un espace de travail central.

Pour plus d’informations, consultez les articles suivants :

* [Présentation du type d’enregistrement de l’espace de travail](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md)

* [Configurer les fonctionnalités inter-espaces de travail du type d’enregistrement](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)

* [Ajouter des types d’enregistrements existants depuis un autre espace de travail](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md)

## Nouvelle limite pour les champs de connexion d’un type d’enregistrement

>[!NOTE]
>
>Aperçu : 16 octobre 2025
>Version rapide de production : 13 novembre 2025
>Production pour tous : 15 janvier 2026

Nous avons introduit une limite de 30 champs de connexion pour chaque type d’enregistrement.

REMARQUE : si votre organisation compte actuellement plus de 30 champs de connexion pour un type d’enregistrement, vous pouvez conserver les champs supplémentaires qui dépassent la limite de 30. Cependant, vous ne pouvez pas ajouter d’autres champs de connexion aux types d’enregistrements qui dépassent la limite. À l’avenir, la nouvelle limite de 30 champs de connexion sera appliquée.

Pour plus d’informations, voir [Présentation des types d’enregistrements connectés](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Définir des valeurs conviviales pour les choix de champs de type sélectionné

>[!NOTE]
>
>Aperçu : 16 octobre 2025
>Version rapide de production : 13 novembre 2025
>Production pour tous : 15 janvier 2026

Lors de l’ajout de choix de champs à un champ à sélection unique ou multiple, Workfront attribue désormais des valeurs conviviales uniques à chaque choix. Avant cette amélioration, Workfront générait un identifiant alphanumérique difficile à comprendre et à utiliser dans les appels d’API et d’autres intégrations.

Tenez compte des points suivants grâce à cette amélioration :

* Les nouvelles valeurs seront ajoutées aux nouveaux choix de champ. Les choix de champs existants conserveront leurs identifiants alphanumériques.

* Les valeurs de choix sont uniques pour un champ, mais peuvent être répétées entre différents champs.

* Renommer un choix ne met pas à jour sa valeur d’origine.

* Les valeurs de choix s’affichent en minuscules et sont séparées par des traits de soulignement dans le cas de choix comportant plusieurs mots. Si vous utilisez un libellé déjà utilisé comme autre nom de choix pour le même champ, Workfront ajoute un numéro séquentiel à la valeur.

Pour plus d’informations, consultez [Créer des champs](/help/quicksilver/planning/fields/create-fields.md).






