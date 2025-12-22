---
title: 23.3 Améliorations relatives à la méthode Agile
description: 23.3 Améliorations relatives à la méthode Agile
author: Lisa
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a47d2592-0f00-4bcd-bc8e-75f8e707a573
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1315'
ht-degree: 91%

---

# 23.3 Améliorations relatives à la méthode Agile

Cette page décrit toutes les améliorations apportées aux tableaux et à l’agile avec la version 23.3. Ces améliorations ont été mises à disposition dans l’environnement de production avec la version 23.3 les 20 et 21 juillet 2023.

Pour une liste de tous les changements disponibles à ce stade du cycle de publication de la version 23.3, voir [Vue d’ensemble de la version 23.3](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

Pour plus d’informations sur la manière de bénéficier des nouvelles fonctionnalités de panoramas avant la sortie de la version trimestrielle, consultez la page [Opt-in anticipé aux fonctionnalités de panorama pour Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

## La vue Agile d’un projet affiche un tableau Kanban

La vue agile d’un projet inclut désormais des fonctionnalités supplémentaires pour filtrer, regrouper et trier le travail dans un tableau Kanban. La nouvelle conception flexible de la vue comprend une fonction de recherche robuste et la possibilité d’ajouter de nouvelles tâches au projet directement à partir du tableau.

>[!NOTE]
>
>La vue Agile existe uniquement sur un projet, car il s’agit d’une vue alternative du projet et vous ne pouvez pas y accéder à partir d’autres zones de Workfront telles que le tableau de bord des tableaux.

Lorsque vous vous trouvez dans le tableau, vous pouvez choisir de passer à l’ancienne vue Agile.

Pour plus d’informations, voir [Gérer un projet dans la vue Agile](/help/quicksilver/manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

[Voir une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3421283/){target=_blank}

## Trier par colonnes du tableau

Nous avons ajouté la possibilité de trier les cartes dans les colonnes d’un tableau. Lorsque vous sélectionnez une option de tri, toutes les colonnes sont triées. Vous ne pouvez pas trier une seule colonne, et la colonne de liste d’attente ou de saisie n’est pas triée.

Vous pouvez trier, par ordre croissant ou décroissant, par nom de carte, date d’échéance, estimation, statut ou connexion (nom du projet). La connexion s’applique uniquement aux cartes connectées. Les autres options trient les cartes connectées et ad hoc dans la colonne.

L’option « ordre utilisateur » renvoie les cartes dans l’ordre dans lequel elles ont été définies manuellement, avant toute autre option de tri. Il s’agit du tri par défaut des colonnes.

Pour plus d’informations, voir [Filtrer et rechercher dans un tableau](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3420932/){target=_blank}

## Mode sombre désormais disponible sur les tableaux Adobe Workfront

Vous pouvez désormais afficher tous vos tableaux et flux de travail en mode sombre. Le nouveau paramètre est disponible via les préférences du tableau de bord des tableaux.

>[!NOTE]
>
>Si l’instance Workfront de votre organisation a été intégrée à Adobe Unified Experience, vous pouvez activer la mise en forme des thèmes sombres pour l’ensemble d’Adobe Experience Cloud via le menu de préférences (image de profil) et vous ne verrez pas d’option de mode sombre distincte pour les tableaux Workfront.

Pour plus d’informations, voir [Notifications par e-mail et préférences des tableaux](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

## Objectifs disponibles dans les itérations de flux de travail dans les tableaux Adobe Workfront

Nous avons ajouté la possibilité d’ajouter des objectifs à une itération, sans avoir à les répertorier sur une carte. Les objectifs sont ajoutés au format de liste de contrôle et peuvent être marqués comme étant terminés. La zone des mesures située en haut à droite de l’itération indique le nombre d’objectifs existants et le nombre d’objectifs terminés.

En outre, la colonne Itération suivante est désormais disponible sur les tableaux d’itération. Lorsque vous placez une carte dans cette colonne, elle est automatiquement reportée à l’itération suivante et ne retourne pas à la liste d’attente. Lors de l’itération suivante, la carte apparaît dans la colonne correspondant à son statut.

Pour plus d’informations, voir [Créer une itération dans un flux de travail](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

## Ajouter des commentaires aux cartes des tableaux

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Vous pouvez maintenant ajouter des commentaires aux cartes ad hoc et connectées sur les tableaux et identifier d’autres utilisateurs et utilisatrices dans les commentaires. Les commentaires sont disponibles dans les détails de la carte. La fonction de commentaire des tableaux utilise la nouvelle expérience de commentaire d’Adobe Workfront.

Pour plus d’informations, voir [Ajouter une carte ad hoc à un tableau](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) et [Utiliser des cartes connectées sur les tableaux](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Voir une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3420832/){target=_blank}

## Améliorations apportées au gestionnaire de balises des tableaux

L’interface du gestionnaire de balises a été améliorée, ce qui vous permet de créer de nouvelles balises rapidement et de les appliquer aux cartes. Vous pouvez également créer des balises pour les flux de travail.

Pour plus d’informations, voir [Ajouter des balises](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

## Filtres simples disponibles dans les colonnes de saisie du tableau

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Des filtres simplifiés ont été ajoutés à la configuration de la colonne de saisie afin que vous puissiez la définir plus rapidement. Les filtres disponibles sont des projets Workfront et des affectations par équipe, utilisateur ou utilisatrice. Vous pouvez passer aux filtres avancés si vous le souhaitez.

Pour plus d’informations, voir [Ajouter une colonne de saisie à un tableau](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

[Voir une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3419420/){target=_blank}

## Filtres simples ajoutés au modèle de tableau dynamique

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Les filtres du modèle de panorama dynamique ont été simplifiés pour vous permettre de créer un panorama plus rapidement. Les filtres disponibles sont des projets Workfront et des affectations par équipe, utilisateur ou utilisatrice. Vous pouvez passer aux filtres avancés si vous le souhaitez. Ces options de filtre se trouvent également dans le panneau Configurer des panoramas dynamiques.

Pour plus d’informations, voir [Créer ou modifier un panorama](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Modèle de panorama dynamique

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Un nouveau modèle, le panorama dynamique, est désormais disponible pour les panoramas autonomes. Ce modèle n’est pas disponible pour les panoramas à l’intérieur d’un flux de travail.

Le panorama dynamique vous permet de remplir automatiquement un panorama de cartes en fonction d’un projet Workfront. Grâce aux filtres, les cartes sont ajoutées aux colonnes en fonction de leur statut.

Pour plus d’informations, voir [Créer ou modifier un panorama](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3418600/){target=_blank}

## Migrer les cartes Kanban de l’équipe Agile vers les tableaux

Un nouveau bouton **Ajouter aux tableaux** sur les tableaux Kanban de l’équipe Agile vous permet d’ajouter toutes les cartes du tableau Kanban à un tableau Workfront. Vous pouvez choisir de créer un panorama Workfront ou d’ajouter les cartes à un panorama existant.

Le placement des cartes sur le panorama Workfront est basé sur des politiques de colonnes. (Par exemple, une politique peut déplacer toutes les cartes dont le statut est « En cours » vers une colonne spécifique.) S’il n’existe aucune stratégie ou si les cartes ne correspondent pas aux stratégies, les cartes sont placées dans la colonne la plus à gauche. Pour l’instant, les cartes de la colonne Liste d’attente du panorama hérité ne sont pas ajoutées au panorama Workfront.

Les cartes ne sont pas supprimées du tableau Kanban de l’équipe Agile et les modifications du statut des cartes sont synchronisées avec les deux tableaux. Vous pouvez conserver les deux tableaux actifs jusqu’à ce que vous soyez en mesure de passer aux panoramas Workfront.

Pour plus d’informations, voir [Migrer les cartes Kanban de l’équipe Agile vers les tableaux Workfront](/help/quicksilver/agile/use-boards-agile-planning-tools/migrate-kanban-cards-to-boards.md).

[Voir une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3420425/){target=_blank}

## Navigation de gauche ajoutée aux détails des cartes sur les panoramas

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront.

Comme de nouvelles options de champ ont été ajoutées aux cartes sur les panoramas Workfront, les détails des cartes sont désormais plus longs. Un nouveau panneau de navigation situé à gauche des détails de la carte vous permet de sélectionner une section et de passer automatiquement à ce groupe de champs.

En outre, vous pouvez maintenant ajouter des URL dans le champ Description ; elles deviennent des liens cliquables lors de l’enregistrement des détails de la carte. Ces mises à jour s’appliquent aux cartes ad hoc et connectées.

Pour plus d’informations, voir [Ajouter une carte ad hoc à un panorama](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md) et [Utiliser des cartes connectées sur les panoramas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

[Voir une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3418598/){target=_blank}

## Notifications par e-mail et préférences des panoramas

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans le cadre de l’activation anticipée des Panoramas Workfront. Étant donné que les notifications par e-mail ne sont généralement pas utilisées dans l’environnement de prévisualisation, cette fonctionnalité a été diffusée simultanément pour la prévisualisation et la production (pour les clientes et clients qui ont souscrit à l’activation des fonctionnalités de manière anticipée).

Les notifications par e-mail sont désormais disponibles pour les panoramas Adobe Workfront. Les notifications sont activées par défaut et vous pouvez sélectionner dans vos préférences les e-mails que vous souhaitez recevoir. Vous recevez un e-mail vous notifiant de votre ajout à un panorama et si une carte vous est attribuée.

Pour plus d’informations, voir [Notifications par e-mail et préférences des panoramas](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

[Voir une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3418597/){target=_blank}
