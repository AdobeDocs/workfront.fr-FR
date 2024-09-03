---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: scénario, performances
navigation-topic: get-started-with-workfront-fusion-2-0
title: Sécurisation des performances Adobe Workfront Fusion
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion en plus d’une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: ec5ed146456c2f75926820f5421bf4feee121399
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 94%

---

# Mécanismes de sécurisation des performances [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une licence [!DNL Adobe Workfront Fusion] en plus d’une [!DNL Adobe Workfront license].

L’automatisation du travail exige un traitement rapide, c’est pourquoi [!DNL Adobe Workfront Fusion] est conçu pour des performances élevées. Comme les scénarios de longue durée peuvent ralentir le rythme de votre travail, [!DNL Workfront Fusion] a été conçu avec des mécanismes de sécurisation permettant de préserver les performances, pour limiter le temps d’exécution, la taille des données et d’autres paramètres du scénario. Les équipes de conception de [!DNL Workfront Fusion] doivent connaître ces mécanismes de sécurisation et les intégrer dans leurs pratiques de conception.

## Navigateurs

* Workfront Fusion ne prend en charge que les navigateurs Chrome.

## Scénarios

* Le délai d’expiration par défaut pour l’exécution d’un scénario est de **40 minutes**. Lorsque l’exécution atteint ce délai d’expiration, [!DNL Workfront Fusion] interrompt l’exécution du scénario après le cycle ou l’opération suivant, selon le scénario. Cela force l’arrêt du scénario peu après l’atteinte de la limite de 40 minutes.
* La taille maximale d’un plan directeur de scénario est de **5 Mo**, mais nous recommandons de ne pas dépasser **3 Mo** pour la taille du scénario.

  Les modules d’application qui créent ou mettent à jour des données avec un grand nombre de champs peuvent générer des plans directeurs très volumineux.

   * Lors de l’utilisation de l’application [!DNL Workfront], veillez à sélectionner uniquement les champs nécessaires à vos cas d’utilisation de création ou de mise à jour.
   * Lors de l’utilisation d’autres applications, utilisez des modules API personnalisés pour interagir avec n’importe quel type d’enregistrement comportant un grand nombre de champs.

* Bien qu’il n’y ait pas de limite pour le nombre de modules dans un scénario, les scénarios comportant plus de 150 modules ont une incidence négative sur les performances de votre système [!DNL Workfront Fusion]. Pour cette raison, il est déconseillé de créer des scénarios comportant plus de 150 modules.

## Opérations

* Le délai d’expiration par défaut d’une opération est généralement de **40 secondes**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Fichiers

* La capacité totale de traitement des fichiers de Fusion est de **1 Go**. La limite est basée sur un coût total en mémoire. Chaque opération contribue à ce coût. Si un seul fichier de 400 Mo est téléchargé et chargé, le coût total de capacité du fichier sera de 800 Mo.

## Utilisation de la mémoire du serveur

* L’utilisation de la mémoire du serveur pour une seule exécution est limitée à **1 Go**.

  De nombreux facteurs, tels que les fichiers volumineux ou les modules complexes, peuvent affecter l’utilisation de la mémoire du serveur d’une manière difficile à prédire ou à contrôler. Pour cette raison, l’exécution de votre scénario peut dépasser la limite de mémoire de 1 Go, même si le scénario suit tous les autres mécanismes de sécurisation des performances. Le dépassement de la limite de mémoire entraîne l’échec de l’exécution.

## Webhooks

* La taille maximale par défaut d’un payload est de **5 Mo**.
* Les webhooks sont limités à **100 demandes par seconde**. Lorsque cette limite est atteinte, Workfront Fusion envoie un statut 429 ([!UICONTROL Trop de demandes]).
* [!DNL Workfront Fusion] stocke les payloads de webhook pendant 30 jours. L’accès à un payload de webhook plus de 30 jours après sa réception entraîne l’erreur « [!UICONTROL Échec de la lecture du fichier à partir de l’enregistrement.] »
* Les webhooks sont désactivés automatiquement si l’une des conditions suivantes s’applique :

   * Le webhook n’a été connecté à aucun scénario depuis plus de 5 jours.
   * Le webhook est utilisé uniquement dans les scénarios inactifs, qui sont inactifs depuis plus de 30 jours.

* Les webhooks désactivés sont supprimés et désinscrits automatiquement s’ils ne sont connectés à aucun scénario et s’ils sont restés désactivés pendant plus de 30 jours.

## Historique de l’exécution

* Les journaux d’historique d’exécution sont limités à une taille de **100 Mo**. Si l’historique d’exécution dépasse cette taille, seuls les 100 premiers Mo s’affichent.
* Si un scénario comporte plusieurs exécutions simultanées. seules 5 exécutions s’affichent dans la zone Exécutions de la page des détails du scénario. C’est le cas même lorsque plus de 5 exécutions sont en cours d’exécution.

## Exécutions incomplètes

* Les exécutions incomplètes sont limitées à une taille totale de 500 Mo. **** Si la limite de 500 Mo est atteinte, aucune autre exécution incomplète ne sera stockée.

## Reprises

* Lors de l’utilisation du module Break et de la spécification de la directive Réessayer, si un scénario échoue consécutivement 10 fois dans un délai de 2 minutes, le scénario est automatiquement désactivé.

