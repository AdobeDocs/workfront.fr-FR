---
title: 22.4 Améliorations apportées aux projets
description: 22.4 Améliorations apportées aux projets
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# 22.4 Améliorations apportées aux projets

Cette page décrit toutes les améliorations apportées aux projets avec la version 22.4 de l’environnement Aperçu. Ces améliorations seront disponibles la semaine du 3 octobre 2022.

Pour obtenir la liste de toutes les modifications disponibles avec la version 22.4, voir [Présentation de la version 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Les détails du prédécesseur sont désormais disponibles.

Pour afficher les détails des prédécesseurs d’une tâche, vous pouvez maintenant passer la souris sur le numéro du prédécesseur dans la colonne Prédécesseurs . La zone Détails affiche la tâche et le projet prédécesseur référencés, les dates de début et de fin prévues pour la tâche précédente et le nombre de prédécesseurs et de successeurs de la tâche précédente. Vous pouvez développer les détails du projet pour afficher plus d’informations sur le projet. Des informations supplémentaires sont incluses pour les prédécesseurs sur plusieurs projets.

Pour plus d’informations, voir [Créer une relation de prédécesseur sur la liste des tâches](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Affecter plusieurs équipes à une tâche ou à un problème

Pour vous offrir une plus grande flexibilité dans la gestion des tâches et des problèmes, nous avons permis d’affecter plusieurs équipes à une tâche ou à un problème. Auparavant, une seule équipe pouvait être affectée à une tâche ou à un problème.

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible dans l’équilibreur de charge de travail de la zone Équipes.

Pour plus d’informations, voir [Affecter des tâches](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) et [Attribuer des problèmes](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Sélection intelligente d’utilisateurs pour les rôles de projet dans les zones Modifier et Détails

Nous avons amélioré l’affichage des utilisateurs lorsque vous les ajoutez aux champs de projet suivants à partir de la boîte de dialogue Modifier et de la section Détails du projet :

* Propriétaire du projet

* Sponsor du projet

* Gestionnaire des ressources

Désormais, lorsque vous ajoutez un utilisateur à l’un de ces champs dans les zones Modifier ou Détails, en plus de son nom et de son avatar, son Rôle de Principal et son email s’affichent également. Cela permet de distinguer plusieurs utilisateurs portant des noms similaires ou identiques.

Pour plus d’informations, voir [Modifier des projets](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

REMARQUE : D’autres champs utilisateur pour les projets, les tâches et les problèmes seront mis à jour avec cette fonctionnalité dans les prochaines versions.

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Les champs de date calculée sont toujours enregistrés en fonction du temps universel coordonné (UTC).

Désormais, vous pouvez être certain que toutes les fonctions de date dans les champs calculés fonctionnent de manière cohérente et produisent le même résultat pour tout le monde, indépendamment de la manière dont une expression de données personnalisée est mise à jour ou de l’endroit où les utilisateurs collaborent sur l’objet dans le monde entier.

Tous les calculs sont désormais calculés et enregistrés selon une norme (temps universel coordonné), et non selon les configurations de fuseau horaire définies pour l’instance de votre entreprise et votre profil utilisateur individuel. Cependant, les calculs sont affichés dans un formulaire personnalisé en fonction des fuseaux horaires individuels définis dans le navigateur de chaque utilisateur.

Auparavant, les paramètres d’heure dans les calculs étaient source de confusion lorsqu’ils variaient selon les situations suivantes :

* Si quelqu’un recalcule une expression de champ calculée à l’aide de &quot;Mettre à jour les calculs précédents&quot; sur le créateur de formulaires, les résultats de la fonction de date sont déterminés par le fuseau horaire UTC de votre entreprise.

* Si un utilisateur a modifié l’objet et que l’expression du champ calculé était recalculée, les résultats de la fonction de date étaient déterminés par le fuseau horaire local de l’utilisateur. Dans ce scénario, le champ Date calculée entraîne également le calcul en fonction du UTC.

Pour plus d’informations, voir [Utilisation des fuseaux horaires](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Améliorations des formulaires personnalisés : Adobe XD et Filtre rapide

Sur la base de vos commentaires, nous avons introduit les améliorations suivantes afin d’améliorer votre expérience de gestion des formulaires personnalisés :

* Ajoutez un fichier Adobe XD pour rendre un formulaire personnalisé plus visuel et informatif. Lorsque le formulaire est joint à un objet, les utilisateurs qui l’utilisent peuvent afficher et interagir avec le fichier XD depuis le formulaire.

  Pour plus d’informations, voir [Ajout ou modification d’une image ou d’un autre widget de ressource dans un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Utilisez le filtre rapide pour localiser facilement des éléments dans la liste de champs et de formulaires personnalisés modernisés. Profitez également d’une apparence améliorée lors de la gestion de vos formulaires et champs.

  Pour plus d’informations sur le filtre rapide, voir [Appliquer le filtre rapide à une liste](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Version bêta publique : nouvelle expérience de filtrage pour les projets, les tâches et les problèmes

Le filtrage dans les listes de projets, de tâches et de problèmes a été repensé afin de vous aider à créer et partager rapidement des filtres. Les fonctionnalités incluent :

* Interface intuitive de &quot;créateur bêta&quot; pour créer un nouveau filtre

* La possibilité de marquer un filtre comme favori

* Empilement des filtres (application de plusieurs filtres enregistrés)

* Duplication de filtres

* Partage de filtres

* Suppression des filtres partagés avec vous


La nouvelle expérience de filtrage est également disponible dans les listes de feuilles de temps et dans le planificateur de scénario.

Le mode Texte reste disponible pour l’édition avancée de filtres, et les administrateurs système peuvent toujours attribuer des filtres par défaut à tous les utilisateurs par le biais des modèles de mise en page.

### Où cela sera-t-il disponible ?

* Listes des projets/tâches/problèmes

* Planificateur de scénarios

* Feuilles de temps


### Nous voulons vos commentaires !

Avec cette version bêta publique, les utilisateurs ont la possibilité d’envoyer leurs commentaires directement à l’équipe qui travaille sur l’expérience de filtrage en cliquant sur le bouton de commentaire. Nous sommes impatients d’avoir de vos nouvelles et de celles de vos utilisateurs sur la nouvelle expérience de filtrage en version bêta publique. Si votre équipe souhaite rencontrer directement un produit afin de fournir des commentaires supplémentaires, n’hésitez pas à programmer une réunion ici : https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### Quelle sera la suite ?

* Nouvelle expérience de groupes et de vues (également appelée Colonnes)

  Nous allons commencer à travailler sur la nouvelle expérience pour les regroupements et les vues (également appelées colonnes) afin qu’elle soit cohérente avec la nouvelle expérience des filtres et qu’elle présente certaines des mêmes fonctionnalités que la nouvelle expérience des filtres.

* Mise en oeuvre de nouveaux filtres dans d’autres zones d’Adobe Workfront

  Nous collaborerons avec des équipes du produit pour mettre en oeuvre la nouvelle expérience de filtrage dans d’autres zones de Workfront.


Nous voulons vous offrir une valeur itérative, de sorte que nous continuerons à vous offrir à mesure que les nouvelles expériences et d’autres domaines seront prêts. Restez à l&#39;écoute pour des mises à jour plus excitantes.

Pour plus d’informations, voir [Présentation des filtres](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) et [Création ou modification de filtres dans Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412391/)
