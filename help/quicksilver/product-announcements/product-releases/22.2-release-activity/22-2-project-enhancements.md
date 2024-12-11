---
title: 2.2 Améliorations du projet
description: 2.2 Améliorations du projet
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 43ea91db-d6f2-4218-9261-580a7e5b31d0
source-git-commit: 8425f8be7d30d36986ac1c062603e680c69902c6
workflow-type: tm+mt
source-wordcount: '1093'
ht-degree: 100%

---

# 2.2 Améliorations du projet

Cette page décrit toutes les améliorations apportées aux projets par la version 22.2 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semaine du 4 avril 2022. Pour obtenir la liste de toutes les modifications disponibles avec la version 22.2, voir [Présentation de la version 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Les panoramas Adobe Workfront sont désormais disponibles !

Les panoramas sont des outils flexibles qui permettent la collaboration en équipe en donnant accès à un panorama partagé contenant des colonnes et des cartes.

Les panoramas vous permettent d’effectuer les opérations suivantes :

* Créer rapidement un panorama des tâches avec plusieurs colonnes
* Configurer des colonnes pour afficher un statut ou une catégorie
* Ajouter d’autres personnes au tableau et leur assigner des cartes
* Ajouter rapidement des cartes ouvertes et des listes de contrôle

Notez que les cartes d’un panorama ne sont pas connectées aux objets et aux éléments de travail dans Adobe Workfront.

Un administrateur ou une administratrice système doit activer les cartes dans les modèles de mise en page pour que l’option soit disponible pour tout le monde dans le menu principal.

Pour plus d’informations, voir [Vue d’ensemble de projets](../../../agile/boards-overview.md).

## Améliorations supplémentaires apportées aux Panoramas Workfront

Les améliorations suivantes sont désormais disponibles pour les Panoramas Workfront :

* Taguer des cartes sur les panoramas

  Vous pouvez désormais classer les cartes de votre panorama par catégories grâce à des balises de couleur. Les balises permettent d’identifier rapidement les cartes. Vous pouvez même trier votre panorama en fonction des balises appliquées.

* Gérer des cartes sur les panoramas

  Nous avons ajouté les fonctionnalités suivantes pour vous aider à gérer les cartes sur votre panorama :

   * Copier une carte : créez une copie d’une carte existante sur votre panorama.
   * Déplacer une carte : déplacez rapidement les cartes vers le haut ou le bas d’un panorama grâce aux nouvelles options de menu Haut de la colonne et Bas de la colonne.

* Rechercher dans les panoramas

  Nous avons ajouté une barre de recherche pour vous aider à rechercher toutes les cartes de votre panorama.

* Fixer une date d’échéance pour une carte dans les panoramas

  Vous pouvez désormais fixer une date d’échéance pour chaque carte de votre panorama.

Pour plus d’informations, voir [Commencer avec les panoramas dans Adobe Workfront](../../../agile/get-started-with-boards/get-started-with-boards.md).

## Option d’annulation pour les messages de mise à jour

Il est désormais plus facile de repérer les erreurs lors de la publication d’une mise à jour. La finalisation d’un commentaire dans l’onglet Mise à jour d’un objet crée désormais une fenêtre contextuelle de 7 secondes qui vous permet d’annuler le message et de revenir à l’édition, avant que le système ne l’horodate ou n’envoie des e-mails ou des notifications dans l’application. Si vous ignorez la fenêtre pop-up, quittez la page ou attendez 7 secondes pour que la fenêtre se ferme. La publication sera publiée normalement.

Pour plus d’informations, voir [Mettre à jour le travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Mise à jour de l’expérience lors de la copie et du déplacement de problèmes

Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Adobe Workfront, nous avons redessiné l’interface pour la copie et le déplacement des problèmes. Cette fonction est actuellement disponible lors de la copie ou du déplacement d’un seul problème ou lors de la copie ou du déplacement en masse de problèmes à partir d’une liste ou d’un rapport.

Voici quelques-unes des améliorations apportées à cette nouvelle interface :

* Toutes les informations que vous devez mettre à jour avant le déplacement s’affichent sur une page continue.
* Workfront vérifie que vous avez accès au projet de destination immédiatement après avoir choisi le projet. Avant cette amélioration, Workfront vous avertissait que vous ne disposiez pas d’un accès correct après avoir confirmé le déplacement, ce qui entraînait des étapes supplémentaires et empêchait le déplacement d’être autorisé.
* Possibilité de demander l’accès à un projet pour lequel vous souhaitez déplacer les problèmes sans quitter la boîte Déplacer une tâche.
* Possibilité de supprimer des éléments (affectations, progression, documents, autorisations, mises à jour) d’un problème lorsque vous le déplacez vers un autre emplacement. Cette fonctionnalité n’était auparavant disponible que pour la copie de problèmes.
* Possibilité de sélectionner une tâche de destination en plus de la sélection d’un projet de destination lors de la copie d’un problème.

Pour plus d’informations sur le déplacement ou la copie de problèmes, voir les articles suivants :

* [Copier des problèmes](../../../manage-work/issues/manage-issues/copy-issues.md)
* [Déplacer les problèmes](../../../manage-work/issues/manage-issues/move-issues.md)

## Nouvelle expérience lors de la copie d’un projet

Afin d’harmoniser votre utilisation de Workfront avec la nouvelle expérience Adobe Workfront, nous avons repensé l’interface de copie de projets. Cette fonction est actuellement disponible lors de la copie d’un projet à partir de la page du projet ou lors de la copie d’un projet à partir d’une liste ou d’un rapport. Avant cette mise à jour, vous ne pouviez copier un projet qu’à partir de la page du projet.

Pour plus d’informations, voir la section [Copier un projet](../../../manage-work/projects/manage-projects/copy-project.md).

## Possibilité de gérer des projets à partir de listes et de rapports à partir d’un nouveau menu Plus

Nous avons ajouté un nouveau menu Plus dans les listes de projets et les rapports pour vous permettre d’effectuer les actions suivantes à partir de ces zones :

* Pour plusieurs projets à la fois :
* Recalculer chronologie
* Recalculer finances
* Recalculer les expressions personnalisées
* Pour un seul projet :
* Joindre modèle
* Exporter vers MS Project
* S&#39;abonner

Pour plus d’informations, consultez les articles suivants :

* [Recalculer les chronologies du projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md)
* [Recalculer le financement du projet](../../../manage-work/projects/project-finances/recalculate-project-finances.md)
* [Modifier les informations dans les champs des formulaires personnalisés](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md)
* [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)
* [Exporter un projet vers Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [S’abonner aux éléments dans Adobe Workfront](../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Maintenir les personnes sur le tableau de bord, la liste ou le rapport après avoir converti le problème en projet

Afin d’accroître l’efficacité et d’éliminer le nombre de clics, nous avons apporté une amélioration à la conversion de problèmes en projets à partir d’une liste, d’un rapport ou d’un tableau de bord.

Les utilisateurs et utilisatrices restent sur la liste, le rapport ou le tableau de bord après avoir converti un problème en projet au lieu d’être redirigés vers la page du projet. Une fois la conversion terminée, une notification de réussite s’affiche avec le lien vers le projet, pour vous permettre de naviguer facilement vers le projet, si nécessaire.

Pour plus d’informations, voir la section [Convertir un problème en projet dans Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md).

## Les heures d’affectation ne seront plus supprimées lors de la modification des affectations.

>[!NOTE]
>
>Cette fonctionnalité était initialement prévue pour la version 22.2. La mise en production aura lieu le 21 avril 2022.

Pour garantir l’exactitude de vos données, nous avons apporté une modification afin de préserver les heures d’attribution et de maintenir inchangé le nombre d’heures prévues pour la tâche lorsque des changements sont apportés aux affectations de la tâche.

Les changements suivants ont été apportés aux tâches avec un type de durée simple :

* Le nombre d’heures prévues est conservé lors de la suppression de toutes les personnes cessionnaires.
* Les attributions d’affectations individuelles sont conservées lors du remplacement des utilisateurs et utilisatrices et des rôles.
* Les attributions d’affectations individuelles sont conservées sur le rôle lors de la suppression de l’utilisateur ou de l’utilisatrice. (Retiré de la version. Désormais, le nombre d’heures prévues sera défini sur 0 après la suppression de toutes les personnes cessionnaires).

Pour plus d’informations sur les heures prévues, voir la section [Vue d’ensemble des heures prévues](../../../manage-work/tasks/task-information/planned-hours.md).

## Partager des dossiers uniquement dans les cinq premiers niveaux d’une hiérarchie de dossiers

>[!NOTE]
>
>Cette fonctionnalité est temporairement indisponible. Nous mettrons à jour cette note de version lorsque la fonctionnalité sera disponible en production.

Pour garantir les meilleures performances aux utilisateurs et utilisatrices qui partagent des dossiers, nous limitons actuellement le partage aux cinq premiers niveaux d’une hiérarchie de dossiers sur un objet.

Chaque dossier du sixième niveau ou d’un niveau inférieur hérite ses configurations de partage du dossier qui lui est directement supérieur.

Pour plus d’informations sur le partage de dossiers, voir la section [Partager un dossier de documents](../../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

