---
title: Autres améliorations au cours de la période de publication du 2e trimestre 2025
description: Autres améliorations au cours de la période de publication du deuxième trimestre de 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 30%

---

# Autres améliorations au cours de la période de publication du 2e trimestre 2025

Cette page décrit les améliorations apportées à l’environnement Aperçu de la version du deuxième trimestre 2025. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du deuxième trimestre 2025, consultez la section [Vue d’ensemble de la version du deuxième trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md).

## Effectuez la mise à niveau vers la nouvelle version d’abonnement aux événements avec les points d’entrée de mise à niveau de version

>[!NOTE]
>
>Production pour toute la clientèle : vendredi 6 mars 2025

Workfront dispose désormais de versions d’abonnements aux événements. La nouvelle version ne constitue pas une modification de l’API Workfront, mais plutôt une modification de la fonctionnalité d’abonnement aux événements.

La possibilité de mettre à niveau ou de rétrograder des abonnements aux événements garantit que, lorsque des modifications sont apportées à la structure des événements, les abonnements existants ne s’arrêtent pas. Cela permet de tester et de passer à la nouvelle version sans interruption de l’abonnement aux événements.

Pour plus d’informations sur les différences entre les deux versions, consultez l’article [Contrôle de version des abonnements aux événements](/help/quicksilver/wf-api/general/event-subs-versioning.md).

Pour plus d’informations sur les points d’entrée utilisés pour mettre à niveau ou rétrograder un abonnement à un événement entre différentes versions, consultez la section [Contrôle de version des abonnements à un événement](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) dans l’article API d’abonnement à un événement.

## Représenter les modifications utilisateur de Adobe Admin Console sous la forme « Système » dans le flux de mise à jour de Workfront

>[!NOTE]
>
>Version préliminaire : 23 janvier 2025 ; Production pour la version rapide : avec la version 25.2 (13 février 2025) ; Production pour la version trimestrielle : avec la version 25.4 (avril 2025)

Désormais, lorsque l’administrateur du Adobe Admin Console apporte une modification aux informations utilisateur d’un utilisateur Workfront, Workfront enregistre cette modification dans l’onglet Activité système de la zone Mises à jour de l’utilisateur comme appartenant au « Système ». Fait référence à l’administrateur Adobe Admin Console.

Avant cette mise à jour, les modifications utilisateur effectuées par l’administrateur de l’Admin Console étaient enregistrées comme effectuées par l’administrateur système Workfront principal.

Pour plus d’informations sur la gestion des utilisateurs dans Adobe Admin Console, voir [&#x200B; Gérer les utilisateurs dans Adobe Admin Console &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)
