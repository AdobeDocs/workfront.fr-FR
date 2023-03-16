---
title: 23.2 Améliorations rapides
description: 23.2 Améliorations rapides
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 8a209bbe64b7b69b41cd9e4d2f603ff58491ba30
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 23.2 Améliorations rapides

Cette page décrit toutes les améliorations apportées à la version 23.2 de l’environnement Aperçu. Ces améliorations seront rendues disponibles dans l’environnement de production avec la version 23.2.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication 23.2, voir [Présentation de la version 23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

<!--

## Iteration functionality available in Adobe Workfront Boards

Several new features available in Workfront Boards make it possible to use agile Scrum functionality. These features include:

* Workstreams for grouping boards related to the same team, and collaborating on work
* A list of cards, or backlog of work, with the option to use sources to connect cards to Workfront tasks and issues
* Iteration planning and iteration process boards

Note that collections have been renamed to workstreams. Workstreams help you visualize data in different ways. You can display items on cards in a list, on a board, or on an iteration. Cards in a workstream can also be shared among multiple boards. You can easily facilitate workflows using cards and boards in a workstream.

For more information, see [Manage workstreams](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md), [Create an iteration](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md), and [Use the card list](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md). Second two articles will not be available in Main until I publish my branch.

## Add tasks and issues to Boards workstreams from lists and reports

You can now add existing tasks or issues to a workstream in Workfront Boards directly from a list or report view. Any items you add to the workstream are added to the card list as unplanned cards.

For more information, see [Add existing tasks or issues to a board](/help/quicksilver/agile/get-started-with-boards/add-card-from-list-to-board.md).

-->

## Journal des heures sur les cartes connectées sur un panorama

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement par le biais de l’accord préalable à la fonctionnalité des panoramas Workfront.

Vous pouvez désormais consigner les heures sur les cartes connectées, comme vous le feriez pour une tâche ou un problème. Pour consigner l’heure, vous devez disposer des autorisations appropriées pour la tâche ou le problème.

Par défaut, les champs de journalisation de l’heure ne s’affichent pas sur les cartes connectées. Vous devez activer **Heures** dans la zone Configurer sous Cartes.

Pour plus d’informations, voir [Utilisation de cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Personnalisation de l’affichage des champs sur une carte

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement par le biais de l’accord préalable à la fonctionnalité des panoramas Workfront.


La personnalisation est désormais disponible pour configurer les champs qui s’affichent sur une carte, à la fois dans le mode d’affichage complet lorsque la carte est ouverte et dans le mode Carte condensée du panorama. Lorsque vous désactivez un champ, il n’est affiché dans aucune des vues. Vous pouvez également activer un champ dans l’affichage complet et le masquer dans l’affichage condensé.

Pour plus d’informations, voir [Personnalisation des champs affichés sur une carte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3415710/){target=_blank}

## Définition de l’état par défaut des cartes déplacées dans une colonne de panorama

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement par le biais de l’accord préalable à la fonctionnalité des panoramas Workfront.

Vous pouvez désormais définir un état par défaut à appliquer aux cartes déplacées dans une colonne spécifique, en sélectionnant un état personnalisé et un état système dans les stratégies de colonne. Lorsque vous déplacez une carte dans la colonne, Workfront tente d’abord d’appliquer l’état personnalisé (par exemple, Commentaires en attente). Si l’état personnalisé n’est pas disponible pour cette carte, Workfront applique plutôt l’état du système (par exemple, En attente). En outre, si l’état de la tâche ou du problème connecté est modifié dans l’état personnalisé ou système défini dans la stratégie de colonne, la carte est automatiquement déplacée dans la colonne.

Auparavant, vous étiez invité à sélectionner l’état de chaque carte déplacée dans la colonne si plusieurs états étaient disponibles.

Pour plus d’informations, voir [Gestion des colonnes](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3415711/){target=_blank}

## Collections désormais disponibles dans les panoramas Adobe Workfront

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement par le biais de l’accord préalable à la fonctionnalité des panoramas Workfront.

Vous pouvez désormais créer des collections dans le tableau de bord des panoramas. Une collection est un groupe de conseils pour collaborer sur le travail. Une fois que vous avez nommé la collection, vous pouvez ajouter des panoramas à la collection à l’aide d’un ensemble de modèles offrant des paramètres prédéfinis tels que les noms de colonne. Vous pouvez également déplacer des panoramas autonomes dans une collection. Une fois qu’un panorama se trouve dans une collection, il peut être déplacé vers une autre collection, mais il ne peut pas devenir un panorama autonome.

L’ajout de membres à une collection fonctionne de la même manière que l’ajout de membres à un panorama. Une personne ou une équipe doit être membre de la collection avant de pouvoir être ajoutée en tant que membres à un panorama de la collection.

Pour plus d’informations, voir [Gestion des collections](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3415609/){target=_blank}

## Champ d’estimation sur les cartes connectées correspond au champ Points d’article sur les objets Workfront

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement par le biais de l’accord préalable à la fonctionnalité des panoramas Workfront.

Le champ Estimation des cartes connectées dans les panoramas Workfront est désormais associé au champ Points d’article pour l’objet Workfront associé.

Le nouveau champ Points d’article est un champ de forme libre modifiable que vous pouvez ajouter à une vue dans une liste ou un rapport pour des tâches ou des problèmes. Il n’est pas lié aux heures planifiées ou aux affectations d’équipe.

Auparavant, l’estimation de la carte était une entrée manuelle qui n’était associée à aucun champ d’une tâche ou d’un problème.

En outre, le champ Estimation sur les cartes ad hoc et connectées n’a plus de limite de caractères. Auparavant, le nombre maximum de caractères était de 99.

Pour plus d’informations, voir [Utilisation de cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Carte d’aperçu dans la colonne d’entrée

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement par le biais de l’accord préalable à la fonctionnalité des panoramas Workfront.

Vous pouvez maintenant cliquer sur une carte connectée dans la colonne d’entrée pour afficher une version en lecture seule de son contenu. Vous ne pouvez pas modifier le contenu de la carte tant que celle-ci n’a pas été déplacée de la colonne d’entrée vers une autre colonne du panorama.
