---
title: 23.1 Améliorations Agile
description: 23.1 Améliorations Agile
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bd041a5-a6e3-4fe3-ae23-45980701e904
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 98%

---

# 23.1 Améliorations Agile

Cette page décrit toutes les améliorations apportées à la version 23.1 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 16 janvier 2023.

Pour consulter la liste de tous les changements disponibles avec la version 23.1, voir [Vue d’ensemble de la version 23.1](/help/quicksilver/product-announcements/product-releases/23.1-release-activity/23-1-release-overview.md).

## Planification Scrum pour les panoramas Workfront

Les nouvelles fonctionnalités de planification Scrum des tableaux Adobe Workfront offrent des options flexibles pour gérer vos processus Agile. Grâce à ces outils, vous pouvez effectuer les opérations suivantes :

* Suivre le travail dans les itérations ou les sprints
* Utiliser la vitesse pour guider les engagements de l’équipe
* Suivre l’avancement et le taux d’achèvement

Les fonctionnalités de planification Scrum seront une « suite rapide » de la version 23.1.

## Les dates d’échéance des cartes correspondent à la date d’achèvement prévue sur l’objet Workfront

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Les dates d’échéance sur les cartes connectées dans les panoramas Workfront correspondent désormais à la date d’achèvement prévue sur l’objet Workfront associé. Si vous mettez à jour la date d’échéance sur une carte, la date d’achèvement prévue est mise à jour sur la tâche ou le problème. La modification de la date d’achèvement prévue modifie également la date d’échéance sur la carte. Auparavant, la date d’échéance de la carte était une entrée manuelle et ne correspondait à aucune date pour une tâche ou un problème.

Le mappage des dates s’applique également aux éléments de liste de contrôle connectés qui sont synchronisés avec les sous-tâches.

La date d’échéance sur les cartes connectées et sur les cartes ad hoc inclut désormais également un champ d’heure.

Pour plus d’informations, voir [Utiliser des cartes connectées sur des panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3411952/){target=_blank}

## Les éléments de liste de contrôle du panorama et les sous-tâches Workfront sont désormais liés.

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Lorsque vous ajoutez une carte connectée à un panorama pour une tâche Workfront, toutes les sous-tâches sont importées en tant qu’éléments de liste de contrôle sur la carte. En outre, lorsque vous créez un élément de liste de contrôle sur une carte connectée, une sous-tâche est ajoutée à la tâche Workfront. Les éléments de liste de contrôle en cas de problème ne sont connectés à aucun objet Workfront.

Auparavant, les éléments de liste de contrôle et les sous-tâches n’étaient pas liés. Si vous souhaitez inclure une sous-tâche dans le panorama, vous pouvez l’importer en tant que carte connectée distincte ou ajouter manuellement un élément de liste de contrôle à une carte.

Pour plus d’informations, voir [Utiliser des cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) et [Gérer les éléments de liste de contrôle sur des cartes](/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3411951/){target=_blank}

## Compteur de carte dans les colonnes du panorama

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Un nouveau paramètre de configuration est disponible, qui permet d’activer un compteur de cartes pour toutes les colonnes d’un panorama. Si vous utilisez la limite de travaux en cours sur une colonne, aucun compteur de cartes distinct n’est ajouté.

Pour plus d’informations, voir [Gérer des colonnes de panorama](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).

## Rechercher et trier dans le tableau de bord des panoramas

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Vous pouvez désormais trier le tableau de bord des panoramas par nom ou date, puis rechercher un panorama spécifique dans la liste.

Pour plus d’informations, voir [Utiliser le tableau de bord des panoramas](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md).

## Statut affiché sur la carte

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Si un statut est attribué à une carte d’un panorama, il s’affiche désormais sur la carte, de sorte que vous n’ayez pas à l’ouvrir pour afficher le statut. Cette amélioration s’applique aux cartes ad hoc et connectées.

Pour plus d’informations, voir [Utiliser des cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md) et [Ajouter une carte ad hoc à un panorama](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

![Statut sur la carte](/help/quicksilver/product-announcements/product-releases/assets/boards-connected-card-details-110922.png)

## Les cartes pouvant faire l’objet d’un lien sont désormais disponible sur les panoramas.

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Vous pouvez désormais envoyer un lien vers une carte spécifique à une autre personne utilisant le panorama. La personne doit avoir accès au panorama avant de pouvoir ouvrir le lien.

Lorsque vous ouvrez une carte sur un panorama, l’URL du navigateur se présente comme suit :

```
https://<Workfront-URL>/boards/<board-id>/card/<card-id>. 
```

Vous pouvez copier l’URL complète et l’envoyer à une autre personne. Elle accédera directement à la carte ouverte en cliquant sur le lien.

Auparavant, les liens étaient disponibles pour les panoramas, mais pas pour les cartes spécifiques.

Pour plus d’informations sur les cartes, voir [Ajouter une carte ad hoc à un panorama](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) et [Utiliser des cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Filtrer par connexion sur les panoramas

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

La liste des filtres sur un panorama inclut désormais l’option permettant de filtrer par connexion, ce qui vous présente toutes les cartes connectées pour un projet spécifique. Vous pouvez également filtrer par cartes non connectées.

Pour plus d’informations, voir [Filtrer et rechercher dans un panorama](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3412381/){target=_blank}

## Archiver des cartes d’un panorama selon un planning

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Vous pouvez configurer un panorama afin que les cartes soient archivées ou « tombent » du panorama selon un planning précis. Des options sont disponibles pour définir des cartes dans une colonne particulière afin de les archiver dans un certain nombre de jours ou de semaines. Par exemple, vous pouvez définir le détachement afin que les cartes d’une colonne Terminé soient archivées après avoir été placées dans la colonne pendant deux semaines.

Si vous souhaitez réafficher les cartes après leur détachement du panorama, vous pouvez définir le filtre du panorama pour afficher les cartes archivées.

Pour plus d’informations, voir [Configurer le détachement des cartes](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3412323/){target=_blank}
