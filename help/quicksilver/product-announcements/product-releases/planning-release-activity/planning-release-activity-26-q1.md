---
content-type: release-notes
title: Activité de la version du premier trimestre 2026 pour Adobe Workfront Planning
description: Il s’agit de l’activité de publication du produit Planification d’Adobe Workfront pour le premier trimestre 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: bbb0399787938033886807d0372e9958ce2fcc00
workflow-type: tm+mt
source-wordcount: '2003'
ht-degree: 1%

---

# Activité de la version du premier trimestre 2026 pour Adobe Workfront Planning

Cet article décrit les nouvelles fonctionnalités de Workfront Planning de la version du premier trimestre 2026.

<!--keep the sentence below for all future quarterly release pages-->

Pour obtenir la liste de toutes les fonctionnalités publiées pour Adobe Workfront Planning, voir [Activité de version d’Adobe Workfront Planning : index des articles](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


## Les types d’enregistrements globaux peuvent être partagés depuis l’espace de travail secondaire

>[!NOTE]
>
>Aperçu : 15 janvier 2026
>Version rapide de production : 15 janvier 2026
>Production pour tous : 15 janvier 2026
>[!BADGE Hors programme ]{type=Neutral}

Vous pouvez désormais partager les types d’enregistrements globaux que vous avez ajoutés à un espace de travail secondaire à partir de cet espace de travail. Les utilisateurs recevront également les mêmes autorisations pour tous les enregistrements de l’espace de travail secondaire que vous partagez.

>[!NOTE]
>
>Les utilisateurs peuvent disposer d’autorisations différentes pour le même type d’enregistrement global dans l’espace de travail principal ou tout autre espace de travail secondaire où le type d’enregistrement a été ajouté. Les autorisations de type Workspace et enregistrement sont transférées vers les enregistrements.

Avant cette modification, vous ne pouviez partager le type d’enregistrement global qu’à partir de son espace de travail principal d’origine.

Pour plus d’informations, voir [Présentation du type d’enregistrement de l’espace de travail croisé](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


## Les enregistrements ajoutés à un type d’enregistrement global dans un espace de travail secondaire ne sont pas visibles à partir des autres espaces de travail secondaires

>[!NOTE]
>
>Aperçu : 15 janvier 2026
>Version rapide de production : 15 janvier 2026
>Production pour tous : 15 janvier 2026
>[!BADGE Hors programme ]{type=Neutral}

Les enregistrements ajoutés à un type d&#39;enregistrement global dans un espace de travail secondaire sont visibles uniquement à partir de cet espace de travail ou de l&#39;espace de travail principal d&#39;origine du type d&#39;enregistrement. Avant cette mise à jour, les enregistrements ajoutés à un espace de travail secondaire étaient également visibles à partir d’autres espaces de travail secondaires que vous pouviez avoir l’autorisation d’afficher.

Pour plus d’informations, voir [Présentation du type d’enregistrement de l’espace de travail croisé](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

## Créer des hiérarchies de type d’enregistrement dans les espaces de travail

>[!NOTE]
>
>Aperçu : 23 décembre 2025
>Version rapide de production : 14 janvier 2026
>Production pour tous : 15 janvier 2026

Vous pouvez désormais définir des hiérarchies flexibles mais structurées entre les types d’enregistrement ou d’objet.

Les hiérarchies sont des connexions entre les types d’enregistrements. Vous pouvez avoir jusqu&#39;à 4 types d&#39;enregistrements et d&#39;objets connectés dans une hiérarchie, et jusqu&#39;à 5 hiérarchies dans un espace de travail. Le premier type d&#39;enregistrement dans la hiérarchie est le premier parent.

Vous pouvez utiliser des hiérarchies pour organiser le travail et visualiser le flux de la stratégie vers l’exécution.

Tenez compte des points suivants lors de la création de hiérarchies :

* Vous pouvez connecter uniquement des types d’enregistrements Planning à partir d’un espace de travail et de projets Workfront dans une hiérarchie.
* Un type d’enregistrement ou un projet ne peut avoir qu’un seul parent dans le même espace de travail.
* Un type d’enregistrement peut être le parent dans plusieurs hiérarchies.
* Les types d&#39;enregistrements connectables ne peuvent pas être utilisés dans les hiérarchies des espaces de travail autres que les leurs.
* Les types d’enregistrements globaux ne peuvent être utilisés dans les hiérarchies que dans les espaces de travail dans lesquels ils ont été créés ou auxquels ils ont été ajoutés.

Pour plus d’informations, voir [ Présentation de la hiérarchie et du chemin de navigation ](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Nouveaux chemins de navigation unifiés ajoutés aux pages des enregistrements

>[!NOTE]
>
>Aperçu : 23 décembre 2025
>Version rapide de production : 14 janvier 2026
>Production pour tous : 15 janvier 2026

Lorsque vous créez des hiérarchies entre les types d&#39;enregistrements, elles génèrent des chemins de navigation pour les enregistrements appartenant à ces types d&#39;enregistrements.

Les chemins de navigation des enregistrements reflètent leur place dans une hiérarchie. Après avoir créé des hiérarchies, vous pouvez voir le chemin de navigation d&#39;un enregistrement en haut de sa page, indiquant quels autres objets parents ou enfants y sont connectés. Les hiérarchies sont cohérentes dans Workfront et Planning.

Par exemple, vous pouvez afficher la hiérarchie Planning d&#39;un projet lorsqu&#39;il est connecté à des types d&#39;enregistrements Planning dans son chemin de navigation Planning, et sa hiérarchie Workfront lorsqu&#39;il est connecté à des types d&#39;objets Workfront, tels que Portfolios ou Programmes, dans Workfront.

Pour plus d’informations, voir [ Présentation de la hiérarchie et du chemin de navigation ](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).


## Améliorations apportées aux pages d’enregistrements connectés

>[!NOTE]
>
>Aperçu : 19 décembre 2025
>Production rapide : 14 janvier 2026
>Production pour tous : 15 janvier 2026

Pour plus de flexibilité lors de l’utilisation de pages d’enregistrements connectées, nous avons amélioré la fonctionnalité des vues dans cette zone de la planification Workfront. Les améliorations suivantes ont été apportées aux pages d’enregistrements connectés d’un enregistrement :

* Vous pouvez désormais ajouter une chronologie et une vue Calendrier à la page d’enregistrements connectés d’un enregistrement.
* Vous pouvez désormais partager toutes les vues à partir d’une page d’enregistrements connectée. Les vues partagées à partir de ces pages sont visibles dans tout le système par tous les utilisateurs avec lesquels vous les partagez dans toute autre zone de Workfront Planning. Toutes les vues partagées dans d&#39;autres zones de Planning sont également visibles dans la page des enregistrements connectés pour les mêmes utilisateurs avec lesquels elles sont partagées.
* Nous avons ajouté une restriction pour n&#39;autoriser qu&#39;une seule page d&#39;enregistrements connectés par type d&#39;enregistrement ou d&#39;objet. Avant cette amélioration, vous pouviez ajouter plusieurs pages pour le même type d’enregistrement ou d’objet. Désormais, vous pouvez utiliser plusieurs vues pour le même type d’enregistrement dans une page d’enregistrements connectée.
* Nous avons ajouté un lien **Nouvelle ligne** au bas d’un tableau et un bouton **Connecter les enregistrements** dans la zone supérieure droite de la page des enregistrements connectés. Avant cette amélioration, le lien **Nouvelle ligne** et le bouton **Connecter des enregistrements** n’existaient que sur une page connectée au projet.

Pour plus d’informations, voir [Ajouter une page Enregistrements connectés à un enregistrement](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

## Partage de vues dans la page Projets - Enregistrements connectés

>[!NOTE]
>
>Aperçu : 18 décembre 2025
>Version rapide de production : 14 janvier 2026\
>Production pour tous : 15 janvier 2026

Pour vous assurer plus facilement de voir les informations dont vous avez besoin, nous avons ajouté la possibilité de partager des vues sur la page Enregistrements connectés aux projets . Vous pouvez désormais partager des vues avec d’autres utilisateurs, équipes ou groupes.

Pour plus d’informations, voir [Ajouter une page Enregistrements connectés à un enregistrement](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

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


## Ajout par défaut du champ Connexion de marque aux produits et aux personnes dans l’espace de travail GenStudio

>[!NOTE]
>
>Aperçu : 11 décembre 2025
>Version rapide de production : 11 décembre 2025
>Production pour tous : 11 décembre 2025
>[!BADGE Hors programme ]{type=Neutral}

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
>[!BADGE Hors programme ]{type=Neutral}

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






