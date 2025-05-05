---
content-type: release-notes
keywords: notes,trimestrielle,mise à jour
navigation-topic: product-releases
title: 21.1 Autres améliorations
description: Cette page décrit toutes les autres améliorations apportées par la version 21.1 à l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 99%

---

# 21.1 Autres améliorations

Cette page décrit toutes les autres améliorations apportées par la version 21.1 à l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.

Pour obtenir une liste de tous les changements disponibles avec la version 21.1, voir [Vue d’ensemble de la version 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Mises à jour des exigences en matière d’échec d’abonnement à un événement

Nous mettons à jour les exigences de désactivation progressive des échecs d’abonnement à un événement. Outre les exigences existantes, les abonnements à des événements seront désormais progressivement désactivés s’ils n’atteignent pas une diffusion réussie avant 2 000 tentatives. L’objectif est de renforcer la règle actuelle des 70 % d’échec, qui peut conduire à des quantités excessives d’échecs dans certains cas.

En outre, nous avons ajouté des exigences de désactivation irréversible à compter de février 2021.

Pour plus d’informations sur les nouvelles exigences de désactivation progressive et de désactivation irréversible, voir la section [Questions fréquentes - Abonnements à un événement](../../../wf-api/general/event-subs-faq.md).

## Nouveaux champs d’équipe disponibles pour la synthèse quotidienne

Nous avons ajouté des champs d’approbation et d’affectation d’équipe à l’e-mail Synthèse quotidienne des actions nécessaires.

Pour plus d’informations, voir la section [Notifications : action nécessaire](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## Remplacer l’option d’e-mail POP dans les files d’attente des demandes

Nous remplaçons l’option d’e-mail POP pour les files d’attente des demandes par un nouveau système géré par Workfront. Vous pourrez toujours envoyer des demandes par e-mail, mais vous devrez plutôt configurer une nouvelle adresse e-mail gérée par Adobe Workfront dans la zone File d’attente des demandes.

Ces modifications peuvent être testées dans l’environnement de prévisualisation.

La fonctionnalité E-mail est automatiquement désactivée dans tous les environnements de prévisualisation. Pour activer l’e-mail à des fins de test, voir la section [Activer la diffusion des e-mails à partir de l’environnement de sandbox de prévisualisation](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Pour plus d’informations, voir la section [Autoriser les utilisateurs et utilisatrices à envoyer un problème par e-mail dans un projet de file d’attente des demandes](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Pour plus d’informations sur les raisons pour lesquelles procéder à cette modification, voir la section [Nouveau système géré par Adobe Workfront pour remplacer un e-mail POP pour les files d’attente des demandes avec la version 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Cette fonctionnalité est désormais incluse dans le parcours de formation [Gestion des files d’attente dans la nouvelle expérience Workfront](https://experienceleague.adobe.com/fr/docs/workfront-learn/tutorials-workfront/home) sur Workfront One.

## Limiter la modification des heures sur les feuilles de temps

Pour mieux contrôler les feuilles de temps et la modification des heures, nous avons ajouté un paramètre qui permet de réserver la modification des heures aux personnes propriétaires de feuilles de temps et aux équipes d’administration système.

Auparavant, les personnes dont l’option Feuilles de temps et heures était activée dans leur niveau d’accès pouvaient modifier les heures sur n’importe quelle feuille de temps.

Pour plus d’informations, voir la section [Configurer les préférences des feuilles de temps et des heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Amélioration des filtres et des vues dans la zone Feuilles de temps

Nous avons apporté les améliorations suivantes lorsque vous ajoutez un projet, une tâche ou un problème à une feuille de temps :

* Filtres : nous avons ajouté des filtres pour les projets et les problèmes. Cliquez sur Autres options pour afficher ces filtres. Auparavant, seules les tâches possédaient un filtrage.
* Vues : nous avons ajouté des options d’affichage et de regroupement à la page Rechercher.

Pour plus d’informations, voir la section [Consigner le temps](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Masquer la zone des heures supplémentaires dans les feuilles de temps

Vous pouvez désormais masquer la zone des heures supplémentaires afin d’atténuer la confusion des utilisateurs et utilisatrices si vous n’effectuez pas le suivi des heures supplémentaires dans Workfront. Vous pouvez masquer la zone des heures supplémentaires pour une feuille de temps à usage unique ou dans le profil de feuille de temps :

* Feuille de temps à usage unique : lorsque vous choisissez de masquer la zone des heures supplémentaires dans une feuille de temps individuelle, celle-ci n’est masquée que pour cette feuille de temps. Pour plus d’informations, voir la section [Créer une feuille de temps à usage unique](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Profil de feuille de temps : lorsque vous choisissez de masquer la zone des heures supplémentaires dans le profil de la feuille de temps, toutes les feuilles de temps créées ensuite pour la ou les personnes affectées à ce profil ne tiendront pas compte de la zone des heures supplémentaires. Pour plus d’informations, voir la section [Créer, modifier et affecter des profils de feuille de temps](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Auparavant, vous ne pouviez pas masquer la zone des heures supplémentaires sur les feuilles de temps.

## Développer ou réduire des éléments dans le chemin de navigation

Pour faciliter l’affichage du chemin de navigation complet, nous avons ajouté des fonctionnalités de développement et de réduction.

Désormais, tous les éléments tronqués sont regroupés avant le projet, avec le mot « autre(s) ». Par exemple, « 3 autres » indique qu’il existe 3 objets qui ne s’affichent pas.

Auparavant, vous deviez cliquer sur les trois points pour afficher les objets tronqués dans un menu déroulant.

Pour afficher tous les éléments du chemin de navigation, cliquez sur « autre(s) » au début du chemin de navigation pour développer les éléments. Une fois développé, vous pouvez cliquer sur « Moins » pour réduire à nouveau les éléments.

## Nouvel aspect de la navigation dans le chemin de navigation

Pour aider les utilisateurs et utilisatrices à mieux identifier leur emplacement dans Workfront et à naviguer plus facilement entre les objets, nous avons apporté les améliorations suivantes à la navigation par chemin de navigation :

* Chaque élément du chemin de navigation comprend désormais un libellé d’objet.
* La page active est désormais incluse dans le chemin de navigation et apparaît en italique.
* La navigation au clavier et la navigation dans les lecteurs d’écran sont désormais disponibles pour les chemins de navigation.
* Autres modifications mineures de style

