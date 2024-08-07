---
content-type: release-notes
keywords: notes,trimestriel,mise à jour
navigation-topic: product-releases
title: Autres améliorations (version 21.1)
description: Cette page décrit toutes les autres améliorations apportées à la version 21.1 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 2%

---

# Autres améliorations (version 21.1)

Cette page décrit toutes les autres améliorations apportées à la version 21.1 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.

Pour obtenir la liste de toutes les modifications disponibles avec la version 21.1, consultez la [présentation de la version 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Mises à jour des exigences en matière d’échec d’abonnement à un événement

Nous mettons à jour les exigences de désactivation progressive des échecs d’abonnement à un événement. Outre les exigences existantes, les abonnements à des événements seront désormais désactivés en douceur s’ils ne parviennent pas à obtenir une diffusion réussie dans les 2000 tentatives. Il s’agit de renforcer la règle actuelle de 70 % d’échec, qui peut conduire à des quantités excessives de défaillances, sous certaines conditions.

En outre, nous ajouterons des exigences de désactivation irréversible à compter de février 2021.

Pour plus d’informations sur les nouvelles exigences de désactivation progressive et de désactivation progressive, voir [FAQ - Abonnements à des événements](../../../wf-api/general/event-subs-faq.md).

## Nouveaux champs d’équipe disponibles pour le Daily Digest

Nous avons ajouté les champs d’approbation et d’affectation de l’équipe au courrier électronique Action Needed Daily Digest.

Pour plus d’informations, voir [Notifications : action requise](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## Remplacement de l’option de courrier électronique POP dans les files d’attente de requête

Nous remplaçons l’option de messagerie POP pour les files d’attente de demandes par un nouveau système géré par Workfront. Vous pourrez toujours envoyer des demandes par courrier électronique, mais vous devrez plutôt configurer une nouvelle adresse électronique gérée par Adobe Workfront dans la zone File d’attente des demandes .

Ces modifications peuvent être testées dans l’aperçu.

La fonctionnalité Email est automatiquement désactivée dans tous les environnements de prévisualisation. Pour activer les emails à des fins de test, voir [Activation de la diffusion des emails à partir de l’environnement de prévisualisation Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Pour plus d’informations, voir [Autoriser les utilisateurs à envoyer par courrier électronique un problème dans un projet de file d’attente des demandes](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Pour plus d’informations sur les raisons de cette modification, voir [Nouveau système géré Adobe Workfront pour remplacer les courriers électroniques POP des files d’attente de requête par 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Cette fonctionnalité est désormais incluse dans la [gestion de la file d’attente dans le nouveau chemin d’apprentissage de l’expérience Workfront](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) sur Workfront One.

## Limitation de la modification des heures sur les feuilles de temps

Pour mieux contrôler les feuilles de temps et la modification des heures, nous avons ajouté un paramètre qui vous permet de limiter la modification des heures aux propriétaires de feuilles de temps et aux administrateurs système.

Auparavant, les utilisateurs dont l’option Fiches horaires et heures était activée dans leur niveau d’accès pouvaient modifier les heures sur n’importe quelle feuille de temps.

Pour plus d’informations, consultez [Configurer les préférences de feuilles de temps et d’heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Amélioration des filtres et des vues dans la zone Fiches horaires

Nous avons ajouté les améliorations suivantes lorsque vous ajoutez un projet, une tâche ou un problème à une feuille de calcul :

* Filtres : nous avons ajouté des filtres pour les projets et les problèmes. Cliquez sur Autres options pour afficher ces filtres. Auparavant, seules les tâches étaient filtrées.
* Vues : nous avons ajouté des options d’affichage et de regroupement à la page Rechercher.

Pour plus d’informations, consultez [Consigner des heures](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Masquer la zone des heures supplémentaires dans les feuilles de calcul

Vous pouvez désormais masquer la zone des heures supplémentaires afin de faciliter la confusion des utilisateurs si vous ne effectuez pas le suivi des heures supplémentaires dans Workfront. Vous pouvez masquer la zone des heures supplémentaires pour une feuille de temps à usage unique ou dans le profil de la feuille de temps :

* Frise chronologique à usage unique : lorsque vous choisissez de masquer la zone des heures supplémentaires dans une feuille de temps individuelle, elle est masquée uniquement pour cette feuille de temps. Pour plus d’informations, voir [Création d’une feuille de temps à usage unique](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Profil de la feuille de temps : lorsque vous choisissez de masquer la zone des heures supplémentaires dans le profil de la feuille de temps, toutes les futures feuilles de temps créées pour le ou les utilisateurs affectés à ce profil ne verront pas la zone des heures supplémentaires. Pour plus d’informations, voir [Créer, modifier et affecter des profils de feuille de temps](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Auparavant, vous ne pouviez pas masquer la zone des heures supplémentaires sur les feuilles de temps.

## Développer ou réduire les éléments dans la navigation du chemin de navigation

Pour faciliter l’affichage du chemin de navigation complet, nous avons ajouté des fonctionnalités de développement et de réduction.

Désormais, tous les éléments tronqués sont regroupés avant le projet avec le texte &quot;plus&quot;. Par exemple, &quot;3 autres&quot; indique qu’il existe 3 objets qui ne s’affichent pas.

Auparavant, vous deviez cliquer sur les points de suspension pour afficher les objets tronqués dans un menu déroulant.

Pour afficher tous les éléments du chemin de navigation, cliquez sur &quot;plus&quot; au début du chemin de navigation pour développer les éléments. Une fois développé, vous pouvez cliquer sur &quot;Inférieur&quot; pour réduire à nouveau les éléments.

## Nouvelle apparence de la navigation dans le chemin de navigation

Pour aider les utilisateurs à mieux identifier leur emplacement dans Workfront et à naviguer plus facilement entre les objets, nous avons apporté les améliorations suivantes à la navigation par chemin de navigation :

* Chaque élément du chemin de navigation comprend désormais un libellé d’objet.
* La page active est désormais incluse dans le chemin de navigation et est en italique.
* La navigation au clavier et la navigation dans les lecteurs d’écran sont désormais disponibles pour les chemins de navigation.
* Autres modifications mineures de style

