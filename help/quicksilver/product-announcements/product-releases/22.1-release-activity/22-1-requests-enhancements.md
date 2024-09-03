---
title: 2.2.1 Améliorations des demandes
description: 2.2.1 Améliorations des demandes
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 100%

---

# 2.2.1 Améliorations des demandes

Cette page décrit toutes les améliorations des demandes apportées à l’environnement de prévisualisation avec la version 22.4. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

Semaine du 17 janvier 2022.

Pour consulter la liste de tous les changements disponibles avec la version 22.1, voir [Vue d’ensemble de la version 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Amélioration apportée à l’interface pour les utilisateurs et utilisatrices qui n’ont pas accès à la création de demandes.

Pour améliorer l’expérience des utilisateurs et utilisatrices lors de l’utilisation de demandes, nous avons apporté une amélioration à l’interface qui indique à la personne connectée qu’elle n’a pas accès à la création de demandes. Grâce à cette amélioration, le bouton Nouvelle demande est désormais grisé pour les personnes qui n’ont pas accès à la création de problèmes. Une infobulle s’affiche lors du survol du bouton grisé, indiquant que l’administration de Workfront a restreint l’accès à la création de demandes pour cette personne.

Avant cette amélioration, le bouton Nouvelle demande ne s’affichait pas dans la zone Demandes pour ces personnes. La copie et la soumission d’une demande en tant que nouvelle demande sont également impossibles.

Pour plus d’informations sur la création de demandes, voir [Créer et soumettre des demandes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Copier et soumettre les demandes

Pour optimiser votre processus de soumission des demandes, nous avons introduit une nouvelle fonctionnalité qui vous permet de copier une demande existante et de la soumettre en tant que nouvelle demande. Cette fonctionnalité est utile lorsque vous soumettez fréquemment des demandes similaires. En effet, il vous suffit de réutiliser une demande existante, d’y apporter quelques modifications, puis de la soumettre en tant que nouvelle demande.

Avec cette nouvelle fonctionnalité, les personnes qui peuvent consulter les demandes que d’autres ont soumises peuvent également copier ces demandes et les soumettre en tant que nouvelles demandes. Pour empêcher ce comportement, mettez à jour le paramètre suivant dans le projet de file d’attente des demandes : Les personnes appartenant à la même entreprise hériteront d’autorisations identiques pour toutes les demandes.

>[!NOTE]
>
>Vous ne pouvez pas copier et soumettre à nouveau des questions qui ont été soumises à une file d’attente des demandes sans rubrique de file d’attente avant que cette fonctionnalité ne soit disponible.

Pour plus d’informations, voir [Copier et soumettre des demandes](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Mise à jour de l’expérience du panneau Résumé dans la section Envoyées de la zone Demandes

>[!NOTE]
>
>Cette fonctionnalité a été temporairement supprimée de l’environnement de prévisualisation le 12 novembre 2021. Elle sera ajoutée à nouveau ultérieurement.

Pour améliorer la visibilité et l’interaction avec le panneau Résumé, nous avons ajouté un libellé à l’icône Ouvrir le résumé dans la section Envoyées de la zone Demandes. Le libellé est désormais dynamique et reflète l’ouverture ou la fermeture du panneau.

Lorsque le panneau Résumé est ouvert sans sélection préalable d’une demande, une image plus conviviale s’affiche désormais pour indiquer clairement à la personne qu’elle doit sélectionner un élément avant d’ouvrir le panneau. Pour plus d’informations, voir [Localiser les demandes envoyées](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Grâce à cette modification, le panneau Résumé pour les tâches, les problèmes et les documents a également été mis à jour. Pour plus d’informations sur le panneau Résumé, voir [Vue d’ensemble du résumé](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
