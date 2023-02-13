---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Activité Publication de fusion Workfront : Semaine du 7 novembre 2022"'
description: Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion au cours de la semaine du 7 novembre 2022.
author: Luke
feature: Product Announcements, Workfront Fusion
hidefromtoc: true
exl-id: 802db851-39bb-4f40-8a66-ecb8c8b3ced6
source-git-commit: 9aaba3062bc5d1166c37821a6a3216f7f1d965b1
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Activité Publication de fusion Workfront : Semaine du 7 novembre 2022

**Optimisation de la file d’attente de webhook**

La file d’attente de webhook de Fusion a été optimisée avec cette version. Le service qui accepte les webhooks est désormais distinct de la file d’attente et des autres processus. Ce changement permet à Fusion de traiter les files d’attente webhook à un rythme plus rapide et plus cohérent.

Au cours de la mise en oeuvre de cette modification, nous avons pu mieux comprendre le temps de traitement des logs attendu pour les événements webhook en file d’attente. La page de la visionneuse webhook de Fusion ne devrait pas dépasser 1 minute.

Pour afficher les événements webhook actuellement en file d’attente, accédez à Webhooks, dans le volet de navigation de gauche. Les icônes de camion comportant un nombre dans le numérateur indiquent les événements de file d’attente pour ce webhook. Cliquez sur l’icône de camion pour afficher les événements placés dans la file d’attente.

![](assets/fusion-webhook-queue-1866x567.png)


**Les webhooks inutilisés seront désormais désactivés ou supprimés.**

Nous avons apporté quelques modifications à la façon dont Workfront Fusion gère les webhooks inutilisés. Désormais, les webhooks sont désactivés automatiquement si l’une des conditions suivantes s’applique :

* Le webhook n’est connecté à aucun scénario depuis plus de 5 jours.
* Le webhook est utilisé uniquement dans les scénarios inactifs, qui sont inactifs depuis plus de 30 jours.

Les webhooks désactivés sont supprimés et désenregistrés automatiquement s’ils ne sont connectés à aucun scénario et sont désactivés depuis plus de 30 jours.
