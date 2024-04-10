---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: scénario,performance
navigation-topic: get-started-with-workfront-fusion-2-0
title: Mécanismes de sécurisation des performances d’Adobe Workfront Fusion
description: Adobe Workfront Fusion requiert une licence Adobe Workfront Fusion en plus d’une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 370743780e5be419eb6a8c432619e5d76acfbfce
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion] mécanismes de sécurisation des performances

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiert un [!DNL Adobe Workfront Fusion] en plus d&#39;une licence [!DNL Adobe Workfront license].

L&#39;automatisation du travail nécessite un traitement rapide, donc [!DNL Adobe Workfront Fusion] est conçu pour offrir des performances élevées. Comme les scénarios de longue durée peuvent ralentir le rythme de votre travail, nous avons conçu [!DNL Workfront Fusion] avec des mécanismes de sécurisation de préservation des performances qui limitent le temps d’exécution, la taille des données et d’autres paramètres de scénario. [!DNL Workfront Fusion] les concepteurs doivent être conscients de ces mécanismes de sécurisation et les intégrer dans leurs pratiques de conception.

## Navigateurs

Workfront Fusion ne prend en charge que les navigateurs basés sur Chrome.

## Scénarios

* Le délai d’exécution par défaut du scénario est **40 minutes**. Lorsque l&#39;exécution atteint ce délai, [!DNL Workfront Fusion] interrompt l’exécution du scénario après le cycle ou l’opération suivant, selon le scénario. Cela force l’arrêt du scénario peu après l’atteinte de la limite de 40 minutes
* La taille maximale d’un plan directeur de scénario est de **5 MO**, mais nous vous recommandons de conserver la taille du scénario sous **3 MO**.

  Les modules d’application qui créent ou mettent à jour des données avec un grand nombre de champs peuvent entraîner des plans directeurs très volumineux.

   * Lors de l’utilisation du [!DNL Workfront] , veillez à ne sélectionner que les champs nécessaires pour vos cas d’utilisation de création ou de mise à jour.
   * Lorsque vous utilisez d’autres applications, utilisez des modules d’API personnalisés pour interagir avec tout type d’enregistrement qui comporte un grand nombre de champs.

* Bien qu’il n’y ait pas de limite au nombre de modules dans un scénario, les scénarios comportant plus de 150 modules ont une incidence négative sur les performances de votre [!DNL Workfront Fusion] système. Pour cette raison, il est déconseillé de créer des scénarios avec plus de 150 modules.

## Opérations

* Le délai d’expiration de l’opération par défaut est généralement de . **40 secondes**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Fichiers

* La capacité totale de traitement des fichiers par Fusion est de . **1 GO**. La limite est basée sur le coût total de la mémoire. Chaque entreprise contribue à ce coût. Si un seul fichier de 400 Mo est téléchargé, le coût total de la capacité du fichier est de 800 Mo.

## Utilisation de la mémoire du serveur

* L’utilisation de la mémoire du serveur pour une seule exécution est limitée à **1 GO**.

  De nombreux facteurs, tels que des fichiers volumineux ou des modules complexes, peuvent affecter l’utilisation de la mémoire du serveur d’une manière difficile à prévoir ou à contrôler. Pour cette raison, l’exécution de votre scénario peut dépasser la limite de mémoire de 1 Go, même si le scénario suit tous les autres mécanismes de sécurisation des performances. Le dépassement de la limite de mémoire entraîne l’échec de l’exécution.

## Webhooks

* La taille maximale par défaut d’une payload est de . **5 MO**.
* Les Webhooks sont limités à **100 requêtes par seconde**. Lorsque cette limite est atteinte, Workfront Fusion envoie un message 429 ([!UICONTROL Trop de requêtes]Statut de ).
* [!DNL Workfront Fusion] stocke les payloads webhook pendant 30 jours. L’accès à une payload webhook plus de 30 jours après sa réception entraîne l’erreur «[!UICONTROL Impossible de lire le fichier depuis le stockage.]«
* Les Webhooks sont désactivés automatiquement si l’une des conditions suivantes s’applique :

   * Le webhook n’a été connecté à aucun scénario depuis plus de 5 jours
   * Le webhook est utilisé uniquement dans les scénarios inactifs, qui sont inactifs depuis plus de 30 jours.

* Les webhooks désactivés sont automatiquement supprimés et désenregistrés s’ils ne sont connectés à aucun scénario et ont un statut désactivé depuis plus de 30 jours.

## Historique de l’exécution

* Les journaux de l’historique d’exécution sont limités à une taille de **100 MO**. Si l’historique d’exécution dépasse cette taille, seuls les 100 premiers Mo sont affichés.

## Reprises

Lors de l’utilisation du module Break et de la spécification de la directive Retry, si un scénario échoue 10 fois de manière consécutive au cours d’une période de 2 minutes, le scénario est automatiquement désactivé.
