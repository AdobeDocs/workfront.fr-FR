---
title: Autres améliorations au cours de la période de publication du 2e trimestre 2025
description: Autres améliorations au cours de la période de publication du deuxième trimestre 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 214f0e67-1da4-4abd-b942-09889e8bd92b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 30%

---

# Autres améliorations au cours de la période de publication du 2e trimestre 2025

Cette page décrit les améliorations apportées à l’environnement Aperçu avec la version du deuxième trimestre 2025. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du deuxième trimestre 2025, consultez la section [Vue d’ensemble de la version du deuxième trimestre 2025](/help/quicksilver/product-announcements/product-releases/25-q2-release-activity/25-q2-release-overview.md).

## Mise à niveau vers la nouvelle version de l’abonnement aux événements avec les points de terminaison de mise à niveau de version

>[!NOTE]
>
>Production pour toute la clientèle : vendredi 6 mars 2025

Workfront dispose désormais de versions des abonnements aux événements. La nouvelle version ne constitue pas une modification de l’API Workfront, mais plutôt une modification de la fonctionnalité d’abonnement aux événements.

La possibilité de mettre à niveau ou de rétrograder des abonnements aux événements garantit que, lorsque des modifications sont apportées à la structure des événements, les abonnements existants ne s’arrêtent pas. Cela permet de tester et de passer à la nouvelle version sans interruption de l’abonnement aux événements.

Pour plus d&#39;informations sur les différences entre les deux versions, consultez l&#39;article [Versions d&#39;abonnement aux événements](/help/quicksilver/wf-api/general/event-subs-versioning.md).

Pour plus d&#39;informations sur les points de terminaison utilisés pour mettre à niveau ou rétrograder un abonnement à un événement entre les versions, consultez la section [Contrôle de version d&#39;un abonnement à un événement](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning) dans l&#39;article API d&#39;abonnement à un événement.

## Représenter les modifications de l’utilisateur Adobe Admin Console comme « Système » dans le flux de mise à jour de Workfront

>[!NOTE]
>
>Version d’aperçu : 23 janvier 2025 ; production pour la version rapide : avec la version 25.2 (13 février 2025) ; production pour la version trimestrielle : avec la version 25.4 (avril 2025)

Désormais, lorsque l’administrateur de Adobe Admin Console modifie les informations utilisateur d’un utilisateur Workfront, Workfront enregistre cette modification dans l’onglet Activité système de la zone Mises à jour de l’utilisateur comme appartenant au « Système ». Il s’agit de l’administrateur Adobe Admin Console.

Avant cette mise à jour, les modifications d’utilisateur effectuées par l’administrateur du Admin Console étaient enregistrées comme effectuées par l’administrateur système principal de Workfront.

Pour plus d&#39;informations sur la gestion des utilisateurs dans Adobe Admin Console, voir [Gérer les utilisateurs dans Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)
