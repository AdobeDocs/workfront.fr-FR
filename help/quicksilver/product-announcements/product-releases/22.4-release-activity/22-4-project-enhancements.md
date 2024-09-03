---
title: Améliorations apportées aux projets (version 22.4)
description: Améliorations apportées aux projets (version 22.4)
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 100%

---

# Améliorations apportées aux projets (version 22.4)

Cette page décrit toutes les améliorations apportées aux projets avec la version 22.4 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans la semaine du 3 octobre 2022.

Pour obtenir la liste de toutes les modifications disponibles avec la version 22.4, voir [Vue d’ensemble de la version 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Les détails des tâches antérieures sont désormais disponibles.

Pour afficher les détails des tâches antérieures d’une tâche, vous pouvez maintenant passer la souris sur le numéro de la tâche antérieure dans la colonne Tâches antérieures. La zone Détails affiche la tâche antérieure et le projet référencés, les dates de début et de fin prévues pour la tâche antérieure et le nombre de tâches antérieures et ultérieures de la tâche antérieure. Vous pouvez développer les détails du projet pour afficher plus d’informations sur le projet. Des informations supplémentaires sont incluses pour les projets transversaux antérieurs.

Pour plus d’informations, voir [Créer une relation de tâche antérieure sur la liste des tâches](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Affecter plusieurs équipes à une tâche ou à un problème

Pour vous offrir une plus grande flexibilité dans la gestion des tâches et des problèmes, nous avons permis d’affecter plusieurs équipes à une tâche ou à un problème. Auparavant, une seule équipe pouvait être affectée à une tâche ou à un problème.

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible dans l’équilibreur de charge de travail de la zone Équipes.

Pour plus d’informations, voir [Affecter des tâches](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) et [Affecter des problèmes](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Sélection intelligente de personnes pour les rôles de projet dans les zones Modifier et Détails

Nous avons amélioré l’affichage des personnes lorsque vous les ajoutez aux champs de projet suivants à partir de la boîte de dialogue Modifier et de la section Détails du projet :

* Propriétaire du projet

* Sponsor du projet

* Gestionnaire des ressources

Désormais, lorsque vous ajoutez une personne à l’un de ces champs dans les zones Modifier ou Détails, son rôle principal et son e-mail s’affichent en plus de son nom et de son avatar. Cela permet de distinguer plusieurs utilisateurs portant des noms similaires ou identiques.

Pour plus d’informations, voir [Modifier des projets](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

NOTE : d’autres champs utilisateur pour les projets, les tâches et les problèmes seront mis à jour avec cette fonctionnalité dans les prochaines versions.

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Les champs calculés de date sont toujours enregistrés en fonction du temps universel coordonné (UTC).

Désormais, vous savez que toutes les fonctions de date dans les champs calculés fonctionnent de manière cohérente et produisent le même résultat pour tout le monde, indépendamment de la manière dont une expression de données personnalisées est mise à jour ou de l’endroit où les personnes collaborent sur l’objet dans le monde entier.

Tous les calculs sont désormais calculés et enregistrés selon une norme, le temps universel coordonné (UTC), et non selon les configurations de fuseau horaire définies pour l’instance de votre entreprise et votre profil utilisateur individuel. Cependant, les calculs sont affichés dans un formulaire personnalisé en fonction des fuseaux horaires individuels définis dans le navigateur de chaque personne.

Auparavant, les paramètres d’heure dans les calculs étaient source de confusion lorsqu’ils variaient selon les situations suivantes :

* Si quelqu’un recalculait une expression de champ calculée à l’aide de « Mettre à jour les calculs précédents » sur le créateur de formulaires, les résultats de la fonction de date étaient déterminés par le fuseau horaire UTC de votre entreprise.

* Si quelqu’un modifiait l’objet et que l’expression du champ calculé était recalculée, les résultats de la fonction de date étaient déterminés par le fuseau horaire local de la personne. Dans ce scénario, le champ Date calculée entraîne également le calcul en fonction du UTC.

Pour plus d’informations, voir [Utiliser des fuseaux horaires](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Améliorations apportées aux formulaires personnalisés : Adobe XD et Filtre rapide

Sur la base de vos commentaires, nous avons introduit les améliorations suivantes afin d’améliorer votre expérience de gestion des formulaires personnalisés :

* Ajoutez un fichier Adobe XD pour rendre un formulaire personnalisé plus visuel et informatif. Lorsque le formulaire est joint à un objet, les personnes qui l’utilisent peuvent afficher et interagir avec le fichier XD depuis le formulaire.


* Utilisez le filtre rapide pour localiser facilement des éléments dans la liste de champs et de formulaires personnalisés modernisés. Profitez également d’un aspect amélioré lors de la gestion de vos formulaires et champs.

  Pour plus d’informations sur le filtre rapide, voir [Appliquer le filtre rapide à une liste](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Version bêta publique : nouvelle expérience de filtrage pour les projets, les tâches et les problèmes

Le filtrage dans les listes de projets, de tâches et de problèmes a été repensé afin de vous aider à créer et partager rapidement des filtres. Les fonctionnalités incluent :

* Une interface intuitive de « création bêta » pour créer un filtre

* La possibilité de marquer un filtre comme favori

* Empiler des filtres (appliquer plusieurs filtres enregistrés)

* Dupliquer des filtres

* Partager des filtres

* Supprimer des filtres partagés avec vous


La nouvelle expérience de filtrage est également disponible dans les listes de feuilles de temps et dans le planificateur de scénarios.

Le mode Texte reste disponible pour l’édition avancée de filtres, et les administrateurs et administratrices système peuvent toujours attribuer des filtres par défaut à toutes les personnes par le biais des modèles de disposition.

### Où cela sera-t-il disponible ?

* Listes des projets/tâches/problèmes

* Planificateur de scénarios

* Feuilles de temps


### Nous voulons connaitre votre avis.

Avec cette version bêta publique, les personnes ont la possibilité d’envoyer leurs commentaires directement à l’équipe qui travaille sur l’expérience de filtrage en cliquant sur le bouton de commentaire. Il nous tarde d’avoir de vos nouvelles et de celles de vos utilisateurs et utilisatrices sur la nouvelle expérience de filtrage en version bêta publique. Si votre équipe souhaite découvrir directement un produit afin de fournir des commentaires supplémentaires, n’hésitez pas à programmer une réunion ici : https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### Quelle est la suite ?

* Nouvelle expérience de regroupements et de vues (également appelée Colonnes)

  Nous allons commencer à travailler sur la nouvelle expérience pour les regroupements et les vues (également appelées colonnes) afin qu’elle soit cohérente avec la nouvelle expérience des filtres et qu’elle présente certaines des mêmes fonctionnalités que la nouvelle expérience des filtres.

* Implémenter de nouveaux filtres dans d’autres zones d’Adobe Workfront

  Nous collaborerons avec des équipes du produit pour implémenter la nouvelle expérience de filtrage dans d’autres zones de Workfront.


Nous voulons améliorer votre expérience de manière itérative, de sorte que nous continuerons à vous satisfaire à mesure que les nouvelles expériences et d’autres domaines seront prêts. Restez à l’écoute pour davantage de mises à jour excitantes.

Pour plus d’informations, voir [Vue d’ensemble des filtres](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) et [Créer ou modifier des filtres dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412391/)
