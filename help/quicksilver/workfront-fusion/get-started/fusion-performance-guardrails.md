---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: scénario,performances
navigation-topic: get-started-with-workfront-fusion-2-0
title: Mécanismes de sécurisation des performances d’Adobe Workfront Fusion
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion et une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: ec5ed146456c2f75926820f5421bf4feee121399
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 94%

---

# Barrières de sécurité des performances de [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une licence [!DNL Adobe Workfront Fusion] et une licence [!DNL Adobe Workfront license].

L’automatisation du travail exige un traitement rapide, c’est pourquoi  est conçu pour des performances élevées. [!DNL Adobe Workfront Fusion] Comme les scénarios de longue durée peuvent ralentir le rythme de votre travail,  a été conçu avec des barrières de sécurité permettant de préserver les performances, pour limiter le temps d’exécution, la taille des données et d’autres paramètres du scénario. [!DNL Workfront Fusion] Les équipes de conception de scénarios [!DNL Workfront Fusion] doivent connaître ces barrières de sécurité et les intégrer dans leurs pratiques de conception.

## Navigateurs

* Workfront Fusion ne prend en charge que les navigateurs Chrome.

## Scénarios

* Le délai d’exécution par défaut du scénario est le suivant : 40 minutes. **** Une fois ce délai dépassé,  interrompt l’exécution du scénario après le cycle ou l’opération suivant, selon le scénario. [!DNL Workfront Fusion] Cette action entraîne l’arrêt du scénario peu après l’atteinte de la limite de 40 minutes.
* La taille maximale d’un plan directeur de scénario est de **5 Mo**, mais nous recommandons de conserver la taille du scénario sous **3 Mo**.

  Les modules d’application qui créent ou mettent à jour des données avec un grand nombre de champs peuvent entraîner des plans directeurs très volumineux.

   * Lors de l’utilisation de l’application [!DNL Workfront], veillez à sélectionner uniquement les champs nécessaires à vos cas d’utilisation de création ou de mise à jour.
   * Lors de l’utilisation d’autres applications, utilisez des modules API personnalisés pour interagir avec n’importe quel type d’enregistrement comportant un grand nombre de champs.

* Bien qu’il n’y ait pas de limite pour le nombre de modules dans un scénario, les scénarios comportant plus de 150 modules entraînent une baisse des performances de votre système . [!DNL Workfront Fusion] Pour cette raison, il est déconseillé de créer des scénarios comportant plus de 150 modules.

## Opérations

* Le délai d’expiration de l’opération par défaut est généralement de **40 secondes**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Fichiers

* La capacité totale de traitement des fichiers de Fusion est la suivante : 1 Go. **** La limite est basée sur un coût total de mémoire. Chaque opération contribue à ce coût. Si un seul fichier de 400 Mo est téléchargé et chargé, le coût total de capacité du fichier sera de 800 Mo.

## Utilisation de la mémoire serveur

* L’utilisation de la mémoire serveur pour une seule exécution est limitée à **1 Go**.

  De nombreux facteurs, tels que les fichiers volumineux ou les modules complexes, ont un impact sur l’utilisation de la mémoire serveur d’une manière difficile à prédire ou à contrôler. Pour cette raison, l’exécution de votre scénario peut dépasser la limite de mémoire de 1 Go, même si le scénario respecte toutes les autres barrières de sécurisation des performances. Le dépassement de la limite de mémoire entraîne l’échec de l’exécution.

## Webhooks

* La taille maximale par défaut d’une payload est de **5 Mo**.
* Les webhooks sont limités à 100 requêtes par seconde. **** Lorsque cette limite est atteinte, Workfront Fusion envoie un statut 429 ([!UICONTROL Trop de requêtes]).
* [!DNL Workfront Fusion] stocke les payloads de webhook pendant 30 jours. L’accès à une payload de webhook plus de 30 jours après sa réception entraîne l’erreur « [!UICONTROL Échec de la lecture du fichier à partir du stockage.] ».
* Les webhooks sont désactivés automatiquement si l’une des conditions suivantes s’applique :

   * Le webhook n’est connecté à aucun scénario depuis plus de 5 jours.
   * Le webhook est utilisé uniquement dans les scénarios inactifs (inactifs depuis plus de 30 jours).

* Les webhooks désactivés sont supprimés et désinscrits automatiquement s’ils ne sont connectés à aucun scénario et s’ils sont restés désactivés pendant plus de 30 jours.

## Historique de l’exécution

* Les journaux d’historique d’exécution sont limités à une taille de 100 Mo. **** Si l’historique d’exécution dépasse cette taille, seuls les 100 premiers Mo s’affichent.
* Si un scénario comporte plusieurs exécutions simultanées. seules 5 exécutions s’affichent dans la zone Exécutions de la page des détails du scénario. C’est le cas même lorsque plus de 5 exécutions sont en cours d’exécution.

## Exécutions incomplètes

* Les exécutions incomplètes sont limitées à une taille totale de 500 Mo. **** Si la limite de 500 Mo est atteinte, aucune autre exécution incomplète ne sera stockée.

## Reprises

* Lors de l’utilisation du module Break et de la spécification de la directive Réessayer, si un scénario échoue consécutivement 10 fois dans un délai de 2 minutes, le scénario est automatiquement désactivé.

