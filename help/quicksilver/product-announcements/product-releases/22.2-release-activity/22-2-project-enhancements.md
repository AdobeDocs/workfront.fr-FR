---
title: 22.2&nbsp;améliorations du projet
description: 22.2&nbsp;améliorations du projet
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 43ea91db-d6f2-4218-9261-580a7e5b31d0
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 1%

---

# 2.2 Améliorations apportées au projet

Cette page décrit toutes les améliorations apportées aux projets avec la version 22.2 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semaine du 4 avril 2022. Pour obtenir la liste de toutes les modifications disponibles avec la version 22.2, voir [Présentation de la version 2.2.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Les panoramas Adobe Workfront sont désormais disponibles.

Les panoramas sont des outils flexibles qui permettent la collaboration des équipes en permettant d’accéder à un panorama partagé contenant des colonnes et des cartes.

Les panoramas vous permettent d’effectuer les opérations suivantes :

* Configuration rapide d’un tableau de tâches avec plusieurs colonnes
* Configurer des colonnes pour afficher un statut ou une catégorie
* Ajouter d’autres utilisateurs au panorama et les affecter aux cartes
* Ajout rapide de cartes et de listes de contrôle ouvertes

Notez que les cartes d’un panorama ne sont pas connectées aux objets et aux éléments de travail dans Adobe Workfront.

Un administrateur système doit activer les panoramas dans les modèles de mise en page pour que l’option soit disponible pour tous les utilisateurs du menu principal.

Pour plus d’informations, voir [Présentation des panoramas](../../../agile/boards-overview.md).

## Autres améliorations apportées aux panoramas Workfront

Les améliorations supplémentaires suivantes sont désormais disponibles pour les panoramas Workfront :

* Balisage des cartes sur les panoramas

  Vous pouvez désormais classer les cartes de votre panorama à l’aide de balises codées par couleur. Les balises vous permettent d’identifier rapidement les cartes. Vous pouvez même trier votre panorama en fonction des balises appliquées.

* Gestion des cartes sur les panoramas

  Nous avons ajouté les fonctionnalités suivantes pour vous aider à gérer les cartes sur votre panorama :

   * Copier une carte : créez une copie d’une carte existante sur votre panorama.
   * Déplacer une carte : déplacez rapidement les cartes vers le haut ou le bas d’un panorama avec les nouvelles options de menu Haut de colonne et Bas de colonne.

* Recherche dans les panoramas

  Nous avons ajouté une barre de recherche pour vous aider à rechercher toutes les cartes de votre panorama.

* Définition de la date d’échéance d’une carte dans les panoramas

  Vous pouvez maintenant définir une date d’échéance pour les cartes individuelles de votre panorama.

Pour plus d’informations, voir [Prise en main des panoramas dans Adobe Workfront](../../../agile/get-started-with-boards/get-started-with-boards.md).

## Option Annuler pour mettre à jour des publications

Il est désormais plus facile de repérer les erreurs lors de la publication d’une mise à jour. La finalisation d’un commentaire dans l’onglet Mise à jour d’un objet crée désormais une fenêtre contextuelle de 7 secondes qui vous permet d’annuler la publication et de revenir à la modification, avant l’horodatage du système ou l’envoi d’emails et de notifications in-app. Si vous ignorez la fenêtre contextuelle, quittez la page ou patientez 7 secondes pendant l’expiration de la fenêtre, la publication est effectuée normalement.

Pour plus d’informations, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Mise à jour de l’expérience lors de la copie et du déplacement de problèmes

Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Adobe Workfront, nous avons repensé l’interface pour la copie et le déplacement des problèmes. Cette option est actuellement disponible lors de la copie ou du déplacement d’un seul problème ou lors de la copie ou du déplacement de problèmes en masse à partir d’une liste ou d’un rapport.

Voici quelques-unes des améliorations apportées à cette nouvelle interface :

* Toutes les informations que vous devez mettre à jour avant le déplacement s’affichent sur une page continue.
* Workfront vérifie que vous avez accès au projet de destination immédiatement après avoir choisi le projet. Avant cette amélioration, Workfront vous avertissait que vous ne disposez pas d’un accès correct après avoir confirmé le déplacement, ce qui entraînait des étapes supplémentaires et empêchait le déplacement d’être autorisé.
* Possibilité de demander l’accès à un projet pour lequel vous souhaitez déplacer les problèmes sans quitter la zone Déplacer la tâche .
* Possibilité de supprimer des éléments (affectations, progression, documents, autorisations, mises à jour) d’un problème lorsque vous le déplacez vers un autre emplacement. Auparavant, cette fonctionnalité n’était disponible que pour les problèmes de copie.
* Possibilité de sélectionner une tâche de destination en plus de la sélection d’un projet de destination lors de la copie d’un problème.

Pour plus d’informations sur le déplacement ou la copie de problèmes, consultez les articles suivants :

* [Copie de problèmes](../../../manage-work/issues/manage-issues/copy-issues.md)
* [Déplacer les problèmes](../../../manage-work/issues/manage-issues/move-issues.md)

## Nouvelle expérience lors de la copie d’un projet

Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Adobe Workfront, nous avons repensé l’interface pour la copie de projets. Cette option est actuellement disponible lors de la copie d’un projet à partir de la page du projet ou lors de la copie d’un projet à partir d’une liste ou d’un rapport. Avant cette mise à jour, vous ne pouviez copier qu’un projet à partir de la page du projet.

Pour plus d’informations, voir [Copier un projet](../../../manage-work/projects/manage-projects/copy-project.md).

## Possibilité de gérer des projets à partir de listes et de rapports depuis un nouveau menu Plus

Nous avons ajouté un nouveau menu Plus dans les listes de projets et les rapports pour vous permettre d’effectuer les actions suivantes à partir de ces zones :

* Pour plusieurs projets à la fois :
* Recalculer chronologie
* Recalculer finances
* Recalculer les expressions personnalisées
* Pour un seul projet :
* Joindre modèle
* Exporter vers MS Project
* S&#39;abonner

Pour plus d’informations, voir les articles suivants :

* [Recalculer les calendriers du projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)
* [Recalculer les finances du projet](../../../manage-work/projects/project-finances/recalculate-project-finances.md)
* [Modifier les informations dans les champs de formulaire personnalisés](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)
* [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)
* [Exportation d’un projet vers un projet Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Abonnement aux éléments dans Adobe Workfront](../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Conserver les utilisateurs dans le tableau de bord, la liste ou le rapport après la conversion du problème en projet

Pour accroître l’efficacité et éliminer le nombre de clics, nous avons publié une amélioration lors de la conversion de problèmes en projets à partir d’une liste, d’un rapport ou d’un tableau de bord.

Les utilisateurs restent dans la liste, le rapport ou un tableau de bord après avoir converti un problème en projet au lieu d’être redirigés vers la page du projet. Une notification de réussite avec le lien vers le projet s’affiche une fois la conversion terminée, afin que vous puissiez facilement accéder au projet, si nécessaire.

Pour plus d’informations, voir [Convertir un problème en projet dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Les heures d’affectation ne seront plus supprimées lors de la modification des affectations.

>[!NOTE]
>
>Cette fonctionnalité était initialement prévue avec la version 22.2. Il sera publié en production le 21 avril 2022.

Pour garantir l’exactitude de vos données, nous avons apporté une modification afin de conserver les heures d’affectation et de conserver les heures planifiées de la tâche inchangées lors de la modification des affectations sur la tâche.

Les modifications suivantes ont été apportées aux tâches avec un type de durée simple :

* Les heures planifiées sont conservées lors de la suppression de tous les cessionnaires.
* Les affectations d’affectation individuelles sont conservées lors du remplacement des utilisateurs et des rôles.
* Les affectations d’affectation individuelles sont conservées sur le rôle lors de la suppression de l’utilisateur. (Supprimée de la version. Désormais, les heures planifiées seront définies sur 0 après la suppression de tous les cessionnaires.)

Pour plus d’informations sur les heures planifiées, voir [Présentation des heures planifiées](../../../manage-work/tasks/task-information/planned-hours.md).

## Partage de dossiers uniquement aux cinq premiers niveaux d’une hiérarchie de dossiers

>[!NOTE]
>
>Cette fonctionnalité est temporairement indisponible. Nous mettrons à jour cette note de mise à jour lorsque la fonctionnalité sera disponible en production.

Afin d’optimiser les performances pour les utilisateurs partageant des dossiers, nous limitons actuellement le partage aux cinq premiers niveaux d’une hiérarchie de dossiers sur un objet.

Chaque dossier au sixième niveau ou au-dessous hérite de ses configurations de partage à partir du dossier situé directement au-dessus.

Pour plus d’informations sur le partage de dossiers, voir [Partage d’un dossier de document](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

