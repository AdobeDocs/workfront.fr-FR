---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Vue d’ensemble des regroupements dans Adobe Workfront
description: Vous pouvez ajouter des regroupements pour gérer la disposition des informations dans vos rapports et listes.
author: Nolan
feature: Reports and Dashboards
exl-id: d050372e-c4a0-4c49-b220-5b35334ab8d0
source-git-commit: 69dec186cdb8a6d29853703edb41073282cdd447
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 85%

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

Par défaut, les regroupements sont mis en surbrillance grise dans votre rapport ou liste. Les résultats du rapport ou de la liste sont répertoriés sous leur regroupement individuel, sans mise en surbrillance.

![Exemple de regroupements](assets/grouping-example-blue.png)

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
>Les exceptions suivantes s&#39;appliquent aux objets parents (par exemple, les tâches parents) lorsque vous agrégez des valeurs pour les champs suivants dans des >regroupements :
>
>* Tous les champs de nombre, de devise et de date, à l’exception des heures réelles, agrégent les valeurs uniquement pour les tâches enfants et les tâches autonomes. Elles n&#39;agrègent pas les valeurs des tâches parents ou des parents de parents. L&#39;agrégation des champs de nombre, de devise et de date d&#39;une liste qui inclut uniquement des tâches parents n&#39;affiche pas de valeur agrégée dans la barre de regroupement.
>
>* Les heures réelles agrégent les valeurs des tâches parents principales et autonomes ; elles n&#39;agrégent pas les valeurs des tâches enfants ou des parents des tâches parents. <!--Examples of Actual hours include Planned/Actual Labor Cost, Planned/Actual Expense Cost, Planned/Actual Cost, and Planned Hours.-->
>
>* Les champs de données personnalisées de valeurs numériques et de devise regroupent toutes les tâches : parents, enfants, parents de parents et tâches autonomes.


### Trier par regroupement {#sort-by-a-grouping}

Les regroupements ne peuvent pas être triés. En revanche, les vues peuvent être triées. Pour trier une liste par la valeur capturée dans le regroupement, vous devez inclure la même valeur dans l’une des colonnes de la vue et appliquer le tri dans la vue. Ainsi, la liste trie indirectement la valeur du regroupement (elle trie par la valeur de la vue qui est également capturée dans le regroupement). Pour plus d’informations sur la création de vues et le tri par valeurs dans les vues, consultez la section [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Supprimer un regroupement {#remove-a-grouping}

Le mode de suppression d’un regroupement varie selon que vous l’avez initialement créé ou que le regroupement a été partagé avec vous. Vous ne pouvez pas supprimer un regroupement par défaut.

* **Si vous avez créé le regroupement et que vous le supprimez**, le regroupement est supprimé du système Workfront. Le regroupement n’est plus disponible pour les personnes avec lesquelles vous l’avez partagé.
* **Si le regroupement a été partagé avec vous et que vous le supprimez**, le regroupement est supprimé uniquement pour vous. La personne qui l’a créé à l’origine et toutes les autres personnes avec lesquelles il a été partagé ont toujours accès au regroupement.

Pour plus d’informations sur la suppression d’un regroupement, consultez l’article [Supprimer des filtres, des vues et des regroupements](../../../reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).


<!--Original note

The following exceptions apply for parent objects (for example, parent tasks) when you are aggregating values for the following fields in groupings:
All the number and currency fields except Actual Hours (for example, Planned/ Actual Labor Cost, Planned/ Actual Expense Cost, Planned/ Actual Cost, Planned Hours) aggregate only the values for the children tasks, and standalone tasks. They do not aggregate the values for the parent tasks or parents of parents.
Actual Hours aggregate the values for the main parent and the standalone tasks; they do not aggregate the numbers for the parents of parent tasks or the children tasks.
Custom data fields for number and currency values aggregate all tasks: parents, children, parents of parents, and standalone tasks.

-->