---
title: Améliorations des requêtes (version 22.1)
description: Améliorations des requêtes (version 22.1)
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: be6da26d-1d80-4946-8222-cd164b2b633f
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 2%

---

# Améliorations des requêtes (version 22.1)

Cette page décrit toutes les améliorations apportées aux requêtes à l’aide de la version 22.1 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semaine du 17 janvier 2022.

Pour obtenir la liste de toutes les modifications disponibles avec la version 22.1, consultez la [présentation de la version 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Amélioration de l’interface pour les utilisateurs qui n’ont pas accès à la création de requêtes

Afin d’améliorer l’expérience des utilisateurs lorsqu’ils travaillent sur des requêtes, nous avons apporté une amélioration à l’interface qui indique à l’utilisateur connecté qu’il n’a pas accès à la création de requêtes. Avec cette amélioration, le bouton Nouvelle requête est grisé pour les utilisateurs n’ayant pas accès à la création de problèmes. Pointez sur le bouton grisé pour afficher une info-bulle qui explique que l’administrateur de Workfront a restreint l’accès de l’utilisateur actuel à la création de requêtes.

Avant cette amélioration, le bouton Nouvelle requête ne s’affichait pas dans la zone Demandes pour ces utilisateurs. La copie et l’envoi d’une demande en tant que nouvelle demande sont également restreints.

Pour plus d’informations sur la création de requêtes, voir [Création et envoi de requêtes Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Copier et soumettre les demandes

Pour optimiser votre processus d’envoi de requêtes, nous proposons une nouvelle fonctionnalité qui vous permet de copier une requête existante et de l’envoyer en tant que nouvelle requête. Cela s’avère utile lorsque vous soumettez fréquemment des requêtes similaires. Dans ce cas, vous pouvez réutiliser une requête existante, apporter quelques modifications, puis l’envoyer en tant que nouvelle requête.

Grâce à cette modification, les utilisateurs qui peuvent afficher les requêtes envoyées par d’autres utilisateurs peuvent également copier ces requêtes et les envoyer comme nouvelles. Vous pouvez empêcher cela de se produire en mettant à jour le paramètre suivant dans le projet de file d’attente des demandes : les personnes d’une même société hériteront des mêmes autorisations pour toutes les demandes.

>[!NOTE]
>
>Vous ne pouvez pas copier et soumettre à nouveau les problèmes qui ont été envoyés à une file d’attente de requêtes sans rubrique de file d’attente avant que cette fonctionnalité ne soit publiée.

Pour plus d’informations, voir [Copier et envoyer des requêtes](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Mise à jour de l’expérience du panneau Résumé dans la section Envoyé de la zone Demandes

>[!NOTE]
>
>Cette fonctionnalité a été temporairement supprimée de l’environnement Aperçu le 12 novembre 2021. Il sera ajouté à nouveau ultérieurement.

Pour améliorer la visibilité et l’interaction avec le panneau Résumé, nous avons ajouté un libellé à l’icône Ouvrir le résumé dans la section Envoyé de la zone Demandes . Le libellé est désormais dynamique et se met à jour selon que le panneau est ouvert ou fermé.

Lors de l’ouverture du panneau Résumé sans sélectionner au préalable une requête, une image plus conviviale s’affiche désormais pour indiquer clairement à l’utilisateur de sélectionner un élément avant d’ouvrir le panneau. Pour plus d’informations, voir [Localisation des requêtes envoyées](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

Avec cette modification, le panneau Résumé pour les tâches, les problèmes et les documents a également été mis à jour. Pour plus d’informations sur le panneau Résumé, voir [Aperçu du résumé](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).
