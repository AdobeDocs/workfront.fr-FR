---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Présentation des regroupements dans Adobe Workfront
description: Vous pouvez ajouter des regroupements pour gérer la disposition des informations dans vos rapports et listes.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Présentation des regroupements dans Adobe Workfront

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This article was supposed to be replaced by "Groupings overview", but decided to keep this here because this is linked in too many places. "Create groupings" and "Edit existing groupings" have been added also (with videos) to replace portions of the old content here.) </p>
-->

Vous pouvez ajouter des regroupements pour gérer la disposition des informations dans vos rapports et listes.

Vous pouvez ajouter des regroupements aux rapports comme suit :

* Vous pouvez créer des groupements en modifiant les groupements existants.

   Pour plus d’informations sur la personnalisation d’un groupement existant, voir [Modifier les groupements existants](../../../reports-and-dashboards/reports/reporting-elements/edit-existing-groupings.md).

* Vous pouvez créer des regroupements à partir de zéro.

   Pour plus d’informations sur la création d’un groupement, voir [Création de groupes dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Par défaut, les regroupements s’affichent en surbrillance grise ou bleue dans votre rapport ou liste. Les résultats du rapport ou de la liste sont répertoriés sous leur groupement individuel, sans mise en surbrillance.

Vous pouvez ajouter jusqu’à trois groupes à un rapport. Vous pouvez organiser vos informations avec jusqu&#39;à quatre regroupements en créant un rapport de matrice. Pour plus d’informations sur les rapports de matrice, voir [Créer un rapport de matrice](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

Dans un rapport de groupement standard, le premier groupement est de couleur plus foncée, les deuxième et troisième groupements sont plus clairs. Vous ne pouvez pas personnaliser la couleur de surbrillance de votre groupement ni la police de son nom. Le nombre entre parenthèses après le nom du groupement représente le nombre de résultats sous ce groupement. Si votre rapport s’étend sur plusieurs pages, veillez à afficher *Tous* le résultat dans le rapport ou la liste pour obtenir un comptage précis des résultats sous chaque groupement.

![Exemple de groupement](assets/grouping-example-blue.png)

Tenez compte des points suivants lorsque vous travaillez avec des regroupements :

* Vous pouvez personnaliser les informations dans les regroupements existants. Tous les utilisateurs qui peuvent afficher les regroupements peuvent également voir vos modifications.
* L’administrateur Workfront doit vous accorder l’accès aux options Modifier les filtres, les vues et les groupes pour créer des groupes.

   Pour plus d’informations sur l’octroi de l’accès aux filtres, aux vues et aux groupes, voir [Accorder l’accès aux filtres, aux vues et aux regroupements](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).

* Le niveau d’autorisation d’un groupement détermine la manière dont il est enregistré. Si vous avez créé le groupement à l’origine, vous pouvez enregistrer les modifications, sinon vous êtes invité à enregistrer une version du groupement. Si vous apportez des modifications à un groupe que vous avez partagé avec d’autres, cela les impacte également.
* Vous pouvez personnaliser un regroupement qui a été partagé avec vous uniquement si l’utilisateur qui l’a partagé vous a accordé l’accès Gérer . Pour plus d’informations sur le partage d’un groupement, voir [Partage d’un filtre, d’une vue ou d’un regroupement](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* Vous ne pouvez pas modifier un groupement intégré.
* Vous ne pouvez pas les regrouper par des champs personnalisés à sélection multiple (par exemple, des cases à cocher) ou par des champs pouvant avoir plusieurs valeurs (par exemple, Gestionnaire de ressources).

## Informations supplémentaires sur les regroupements

Vous pouvez gérer les informations d&#39;un rapport de manière plus détaillée lors de l&#39;utilisation des Regroupements en agrégeant les valeurs de chaque colonne de la ligne Groupement et en triant vos informations par champ de votre Regroupement. Vous pouvez également supprimer un groupement lorsqu&#39;il n&#39;est plus nécessaire.

* [Agrégat des valeurs en regroupements](#aggregate-values-in-groupings)
* [Tri par groupement](#sort-by-a-grouping)
* [Suppression d’un groupe](#remove-a-grouping)

### Agrégat des valeurs en regroupements {#aggregate-values-in-groupings}

Vous pouvez agréger dans votre ligne de groupement les données affichées dans votre rapport, en synthétisant les valeurs de chaque colonne du rapport. Pour plus d’informations sur le résumé des données de colonne dans un groupement, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

>[!NOTE]
>
>Les exceptions suivantes s’appliquent aux objets parents (par exemple, les tâches parents) lorsque vous agrègez des valeurs pour les champs suivants en regroupements :
>
>* Tous les champs de nombre et de devise, à l’exception des heures réelles (par exemple, le coût du travail planifié/réel, le coût des dépenses planifiées/réelles, le coût planifié/réel, les heures planifiées), ne regroupent que les valeurs des tâches enfants et des tâches autonomes. Ils n’agrégent pas les valeurs des tâches parents ou des parents des parents.
>* Les heures réelles combinent les valeurs du parent principal et des tâches autonomes ; ils n’agrégent pas les chiffres des parents des tâches parents ou des tâches enfants.
>* Les champs de données personnalisés pour les valeurs numériques et monétaires regroupent toutes les tâches : parents, enfants, parents et tâches autonomes.


### Tri par groupement {#sort-by-a-grouping}

Les groupes ne peuvent pas être triés. Les vues peuvent être triées. Pour trier une liste par la valeur capturée dans le groupement, vous devez inclure la même valeur dans l&#39;une des colonnes de la vue et appliquer le tri dans la vue. Ainsi, la liste trie indirectement la valeur du groupement (elle trie par la valeur de la vue qui est également capturée dans le groupement). Pour plus d’informations sur la création de vues et le tri par valeurs dans les vues, voir [Présentation des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Suppression d’un groupe {#remove-a-grouping}

La manière dont vous supprimez un groupement varie selon que vous l’avez initialement créé ou que le regroupement a été partagé avec vous. Vous ne pouvez pas supprimer un regroupement par défaut.

* **Si vous avez créé le groupement et que vous le supprimez**, le regroupement est supprimé du système Workfront. Le regroupement n’est plus disponible pour les utilisateurs avec lesquels vous l’avez partagé.
* **Si le regroupement a été partagé avec vous et que vous le supprimez**, le regroupement est supprimé uniquement pour vous. L’utilisateur qui l’a créée à l’origine et tous les autres utilisateurs avec lesquels elle a été partagée ont toujours accès au regroupement.

Pour plus d’informations sur la suppression d’un regroupement, reportez-vous à l’article [Suppression des filtres, des vues et des regroupements](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
