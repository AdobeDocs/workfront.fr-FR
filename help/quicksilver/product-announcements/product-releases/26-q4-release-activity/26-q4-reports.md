---
title: Améliorations des rapports pour le quatrième trimestre 2026
description: Améliorations des rapports pour le quatrième trimestre 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: 3599b27bb1b838ebe7d0a2648e6c67333da83dc8
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 5%
---
# Améliorations des rapports pour le quatrième trimestre 2026

Cette page décrit les améliorations apportées aux rapports avec la version du quatrième trimestre 2026 dans l’environnement Aperçu. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication du quatrième trimestre 2026, voir [présentation de la version du quatrième trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Tableaux de bord de la zone de travail désormais disponibles sur Google Cloud Platform et Microsoft Azure

>[!NOTE]
>
>Aperçu : S.O.
>Version rapide de production : 14 octobre 2026
>Production pour tous : 15 octobre 2026

Les instances Workfront sur Google Cloud Platform (GCP) et Azure peuvent désormais activer la version Beta ouverte des tableaux de bord de la zone de travail. Pour plus d’informations, voir [ Utilisation des tableaux de bord de la zone de travail ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Enregistrer une liste privée Snowflake pour Workfront Data Connect

>[!NOTE]
>
>Aperçu : S.O.
>Version rapide de production : 14 octobre 2026
>Production pour tous : 15 octobre 2026

Vous pouvez désormais partager vos données Workfront Data Connect directement avec le compte Snowflake de votre organisation en enregistrant une liste privée. Cette méthode de connexion utilise la fonctionnalité de liste privée de Snowflake pour partager des données en toute sécurité entre les organisations sans les exposer publiquement. Elle fonctionne également entre les régions et les plateformes d’hébergement.

Une liste privée est utile lorsque vous souhaitez joindre vos données Workfront à d’autres données de votre entrepôt de données d’entreprise. Comme les données résident sur votre propre compte Snowflake, vous pouvez les interroger avec le reste de vos données.

Pour plus d’informations, voir [Enregistrement d’une liste privée pour Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/register-a-private-listing.md).

## Outils de MCP de création de rapports désormais disponibles pour les tableaux de bord de zone de travail

>[!NOTE]
>
>Aperçu : 1er octobre 2026
>Version rapide de production : 14 octobre 2026
>Production pour tous : 15 octobre 2026

Pour faciliter l’utilisation des tableaux de bord de la zone de travail, nous avons ajouté des outils au MCP Workfront. Vous pouvez désormais créer et gérer des tableaux de bord de zone de travail par le biais du chat. En outre, le tableau de bord et les widgets sont créés pour vous à l’aide de vos données Workfront. Cela fonctionne à partir de clients MCP comme Claude et Cursor.

Par exemple, vous pouvez effectuer les opérations suivantes :

* Créez des rapports en demandant des informations. Décrivez un tableau de bord ou un graphique en langage naturel au lieu de le créer manuellement.
* Modifier sur place. Demandez à de renommer un widget, de modifier un filtre, de permuter un type de graphique ou de redimensionner, et les modifications s’appliqueront au tableau de bord dynamique.
* Réutilisez ce que vous avez. Dupliquez un tableau de bord ou un widget existant comme point de départ au lieu de reconstruire à partir de zéro.

### Fonctionnalités prises en charge

**Tableaux de bord**

* Créer un tableau de bord
* Répertoriez vos tableaux de bord (les vôtres, partagés avec vous, tous ou favoris) et effectuez une recherche par titre
* Ouverture ou affichage de la structure d’un tableau de bord
* Mettre à jour le titre, la description, la devise, les filtres et les invites
* Dupliquer un tableau de bord (avec ou sans ses widgets, invites et filtres)
* Supprimer un tableau de bord

**Widgets**

* KPI : un seul nombre agrégé (somme, moyenne, nombre, min, max, etc.)
* Graphique : à barres, à colonnes, en courbes et à secteurs ; prend en charge les graphiques simples, à séries multiples et empilés
* Tableau — tableaux à plusieurs colonnes avec regroupement des lignes
* Affichage de la configuration d’un widget et mise à jour, copie, redimensionnement ou repositionnement, ou suppression de celui-ci

**Options de reporting**

* Filtrer les données avec des conditions et des groupes ET/OU
* Regrouper et agréger par n’importe quel champ
* Accéder aux enregistrements sous-jacents à partir d’un KPI ou d’un graphique
* Libellés de colonne personnalisés, format des nombres, des dates et des devises, et style de cellule conditionnel
* Invites et filtres au niveau du tableau de bord

Pour plus d’informations, voir [ Utilisation des tableaux de bord de la zone de travail ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Copier ou déplacer des widgets entre les tableaux de bord de la zone de travail

>[!NOTE]
>
>Aperçu : 1er octobre 2026
>Version rapide de production : 14 octobre 2026
>Production pour tous : 15 octobre 2026

Vous pouvez désormais copier un widget dans le même tableau de bord, dans un autre tableau de bord auquel vous avez un accès en modification ou dans un nouveau tableau de bord. Vous pouvez également déplacer un widget vers un autre tableau de bord auquel vous avez un accès en modification ou vers un nouveau tableau de bord.

Lorsque vous copiez un widget, une boîte de dialogue s’ouvre désormais dans laquelle vous sélectionnez le tableau de bord de destination et si vous souhaitez copier ou déplacer le widget. Auparavant, le Report Builder s’ouvrait immédiatement.

## Filtrer les relations de collection dans les tableaux de bord de la zone de travail

>[!NOTE]
>
>Aperçu : 1er octobre 2026
>Version rapide de production : 14 octobre 2026
>Production pour tous : 15 octobre 2026

Lorsque vous créez un filtre dans un tableau de bord Zone de travail, vous pouvez désormais filtrer les relations de collection, qui sont des champs liés à un groupe d’enregistrements associés plutôt qu’à un seul enregistrement. Par exemple, vous pouvez filtrer par statut des tâches appartenant à un projet pour afficher la liste des projets dont le statut des tâches est défini sur « Nouveau ».

Auparavant, le filtrage sur les relations de collection nécessitait le mode texte.

Pour plus d’informations, voir [Référence de filtre de rapport pour les tableaux de bord de la zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md).

## Copie de tableaux de bord dans les tableaux de bord de la zone de travail

>[!NOTE]
>
>Aperçu : 3 septembre 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Vous pouvez désormais copier un tableau de bord de zone de travail à l’aide de la nouvelle action **Copier le tableau de bord**. Cette action est disponible pour tout utilisateur dont le niveau d’accès accorde des droits de modification ou de création sur les tableaux de bord, même s’il ne dispose que d’un accès en lecture seule au tableau de bord spécifique en cours de copie. Les utilisateurs ne disposant pas de droits de modification ou de création sur les tableaux de bord ne voient pas cette action.

Lorsque vous copiez un tableau de bord, vous pouvez le renommer, mettre à jour sa description et sa devise, et choisir les widgets, les filtres de tableau de bord et les invites à transférer vers la copie.

L’exécution en tant que configurations utilisateur sur les widgets n’est conservée que si vous êtes l’utilisateur désigné ou un administrateur système. Les préférences de partage ne sont pas copiées dans le nouveau tableau de bord et un message de confirmation contenant un lien vers le nouveau tableau de bord s’affiche une fois la copie terminée.

Auparavant, il n’existait aucun moyen de copier un tableau de bord ; les utilisateurs devaient reconstruire les tableaux de bord en partant de zéro pour créer des variations spécifiques à l’audience.

## Champ Type d’approbation dans les tableaux de bord de la zone de travail

>[!NOTE]
>
>Production pour tous : 28 août 2026
>[!BADGE Hors planning]{type=Neutral}

L&#39;entité Approbation comprend désormais un champ **Type d&#39;approbation**, qui permet aux utilisateurs de distinguer les approbations d&#39;épreuves, les approbations de version de documents, les approbations d&#39;admission et d&#39;autres types d&#39;approbation.

## Mise à jour de la terminologie d’approbation dans les tableaux de bord de la zone de travail

>[!NOTE]
>
>Production pour tous : 28 août 2026
>[!BADGE Hors planning]{type=Neutral}

Les noms de champ suivants utilisés dans les tableaux de bord de la zone de travail pour les approbations de document et de travail ont été renommés par souci de clarté :

| Nom précédent | Nouveau nom |
| --- | --- |
| Approbation du document | Approbation |
| Étape d’approbation du document | Étape d’approbation |
| Personne participant à l’étape d’approbation du document | Participant ou participante à l’étape d’approbation |
| Processus d’approbation | Processus d’approbation du travail |
| Étape d’approbation | Étape d’approbation du travail |
| Statut de l&#39;approbateur | Statut de l’approbateur ou approbatrice du travail |
| Approbation en attente | Approbation de travail en attente |

Cette modification n’a aucune incidence sur le fonctionnement des rapports actuels.

## Rapports de tableau croisé dynamique dans les tableaux de bord de la zone de travail

>[!NOTE]
>
>Aperçu : 27 août 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Le nouveau type de rapport de tableau croisé dynamique des tableaux de bord de la zone de travail agrège les données avec des déploiements complets et précis. Vous pouvez créer des mesures telles que les nombres, les sommes et les moyennes directement sur votre tableau de bord, puis accéder aux enregistrements sous-jacents derrière un total.

Pour plus d&#39;informations, voir [Créer un rapport de tableau croisé dynamique dans un tableau de bord Zone de travail](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md).

## Application de dates de fin aux rapports planifiés

>[!NOTE]
>
>Aperçu : 13 août 2026
>Mise à jour rapide de la production : 17 septembre 2026
>Production pour tous : 15 octobre 2026

Les rapports planifiés requièrent désormais une date de fin pour empêcher une diffusion indéfinie. Les plannings dont la date de fin est dépassée sont automatiquement désactivés.

Les plannings existants ont été mis à jour avec des dates de fin pour améliorer la fiabilité et réduire l’utilisation inutile du système. Workfront offre également une visibilité accrue et des avertissements pour vous aider à gérer les cycles de vie des planifications de rapports à l’approche de leur date de fin.

Pour plus d’informations, voir [Planification de la diffusion automatique des rapports](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Les champs de référence natifs sont disponibles pour les listes et les rapports

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Vous pouvez désormais ajouter des champs de référence natifs aux listes et aux rapports dans Workfront.

Un champ de référence natif est un champ personnalisé. Lorsque le champ se trouve sur un formulaire personnalisé joint à un objet, le champ est renseigné à partir des données d’objet. Par exemple, si le champ fait référence au champ Description et s’il figure sur un formulaire personnalisé joint à un projet, il extrait la description du projet. (Le champ peut afficher « S.O. » si aucune donnée n’est disponible.)

Pour plus d’informations sur la création de champs de référence natifs, y compris la liste des champs natifs pris en charge, voir [Créer un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
Pour plus d’informations sur l’ajout de champs aux rapports, voir [Créer un rapport personnalisé](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Ordre cohérent des valeurs de champ à sélection multiple dans les listes et rapports hérités

>[!NOTE]
>
>Aperçu : 30 juillet 2026
>Version rapide de production : 13 août 2026
>Production pour tous : 15 octobre 2026

Les options sélectionnées pour les champs personnalisés à sélection multiple s’affichent désormais dans un ordre cohérent et prévisible sur les listes et rapports hérités. L’ordre des champs est déterminé par la manière dont les champs sont organisés dans le formulaire personnalisé.

![L’ordre des champs de formulaire personnalisé correspond à l’ordre des valeurs sélectionnées dans une liste ou un rapport](assets/new-field-order-multi-select.png)

Auparavant, les options sélectionnées s’affichaient dans l’ordre dans lequel vous les aviez choisies ou dans un ordre incohérent, ce qui rendait les lignes plus difficiles à analyser et à comparer.

Remarque : le nouveau tri ne s’applique pas si le champ utilise le mode texte.
