---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Vue d’ensemble des regroupements dans Adobe Workfront
description: Vous pouvez ajouter des regroupements pour gérer la disposition des informations dans vos rapports et listes.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 98%

---

# Vue d’ensemble des regroupements dans Adobe Workfront

<!-- Audited: 11/2024 -->

<!--(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.)-->

Vous pouvez ajouter des regroupements pour gérer la disposition des informations dans vos rapports et listes.

Vous pouvez ajouter des regroupements aux rapports comme suit :

* Vous pouvez créer des regroupements en modifiant les regroupements existants.

  Pour plus d’informations sur la personnalisation d’un regroupement existant, consultez la section [Modifier les regroupements existants](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* Vous pouvez créer des regroupements à partir de zéro.

  Pour plus d’informations sur la création d’un regroupement, consultez la section [Créer des regroupements dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Par défaut, les regroupements s’affichent en surbrillance grise dans votre rapport ou liste. Les résultats du rapport ou de la liste sont répertoriés sous leur regroupement individuel, sans mise en surbrillance.

![Exemple de groupement](assets/grouping-example-blue.png)

Vous pouvez ajouter jusqu’à trois regroupements à un rapport. Vous pouvez organiser vos informations avec jusqu’à quatre regroupements en créant un rapport de matrice. Pour plus d’informations sur les rapports de matrice, consultez la section [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

Le nombre entre parenthèses après le nom du regroupement représente le nombre de résultats sous ce regroupement. Si votre rapport s’étend sur plusieurs pages, veillez à afficher *Tous* les résultats dans le rapport ou la liste pour obtenir un nombre précis de résultats sous chaque regroupement.

Tenez compte des points suivants lorsque vous utilisez des regroupements :

* Vous pouvez personnaliser les informations dans les regroupements existants. Tous les utilisateurs et utilisatrices qui peuvent afficher les regroupements peuvent également voir vos modifications.
* L’administration de Workfront doit vous accorder l’accès aux options Modifier les filtres, les vues et les regroupements pour créer des regroupements.

  Pour plus d’informations sur l’octroi de l’accès aux filtres, aux vues et aux regroupements, consultez la section [Accorder l’accès aux filtres, vues et regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Le niveau d’autorisation d’un regroupement détermine son mode d’enregistrement. Si vous êtes le créateur ou la créatrice du regroupement, vous pouvez enregistrer les modifications, sinon, vous devez enregistrer une version du regroupement. Si vous apportez des modifications à un regroupement que vous avez partagé avec d’autres personnes, ces modifications seront également répercutées pour ces personnes.
* Vous pouvez personnaliser un regroupement qui a été partagé avec vous uniquement si la personne qui l’a partagé vous a accordé un accès en gestion. Pour plus d’informations sur le partage d’un regroupement, consultez la section [Partager un filtre, une vue ou un regroupement](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* Vous ne pouvez pas modifier un regroupement en ligne.
* Vous ne pouvez pas regrouper des champs personnalisés à sélection multiple (par exemple, des cases à cocher) ou des champs pouvant avoir plusieurs valeurs (par exemple, le gestionnaire de ressources).

## Informations supplémentaires sur les regroupements

Pour obtenir des informations plus précises dans les rapports à l’aide des regroupements, agrégez les valeurs de chaque colonne de la ligne Regroupement, puis triez vos informations selon le champ de votre regroupement. Vous pouvez également supprimer un regroupement lorsqu’il n’est plus nécessaire.

* [Agréger des valeurs dans des regroupements](#aggregate-values-in-groupings)
* [Trier par regroupement](#sort-by-a-grouping)
* [Supprimer un regroupement](#remove-a-grouping)

### Agréger des valeurs dans des regroupements {#aggregate-values-in-groupings}

Vous pouvez agréger dans votre ligne de regroupement les données affichées dans votre rapport, en synthétisant les valeurs de chaque colonne du rapport. Pour plus d’informations sur le résumé des données de colonne dans un regroupement, consultez la section [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>Les exceptions suivantes s’appliquent aux objets parent (par exemple, les tâches parent) lorsque vous agrégez des valeurs pour les champs suivants en regroupements :
>
>* Tous les champs de nombre et de devise, à l’exception des heures effectives (par exemple, le coût prévu/réel de main-d’œuvre, le coût réel/prévu des dépenses, le coût prévu/réel, le nombre d’heures prévues), n’agrègent que les valeurs des tâches enfant et des tâches autonomes. Ils n’agrègent pas les valeurs des tâches parent ou des parents des parents.
>* Les heures effectives agrègent les valeurs principales des tâches parent et des tâches autonomes. Elles n’agrègent pas les nombres pour les parents des tâches parent ou des tâches enfant.
>* Les champs de données personnalisées de valeurs numériques et de devise regroupent toutes les tâches : parents, enfants, parents de parents et tâches autonomes.

### Trier par regroupement {#sort-by-a-grouping}

Les regroupements ne peuvent pas être triés. En revanche, les vues peuvent être triées. Pour trier une liste par la valeur capturée dans le regroupement, vous devez inclure la même valeur dans l’une des colonnes de la vue et appliquer le tri dans la vue. Ainsi, la liste trie indirectement la valeur du regroupement (elle trie par la valeur de la vue qui est également capturée dans le regroupement). Pour plus d’informations sur la création de vues et le tri par valeurs dans les vues, consultez la section [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Supprimer un regroupement {#remove-a-grouping}

Le mode de suppression d’un regroupement varie selon que vous l’avez initialement créé ou que le regroupement a été partagé avec vous. Vous ne pouvez pas supprimer un regroupement par défaut.

* **Si vous avez créé le regroupement et que vous le supprimez**, le regroupement est supprimé du système Workfront. Le regroupement n’est plus disponible pour les personnes avec lesquelles vous l’avez partagé.
* **Si le regroupement a été partagé avec vous et que vous le supprimez**, le regroupement est supprimé uniquement pour vous. La personne qui l’a créé à l’origine et toutes les autres personnes avec lesquelles il a été partagé ont toujours accès au regroupement.

Pour plus d’informations sur la suppression d’un regroupement, consultez l’article [Supprimer des filtres, des vues et des regroupements](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
