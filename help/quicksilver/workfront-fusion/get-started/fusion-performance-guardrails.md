---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: scénario, performances
navigation-topic: get-started-with-workfront-fusion-2-0
title: Protections des performances d’Adobe Workfront Fusion
description: Adobe Workfront Fusion nécessite une licence Adobe Workfront Fusion en plus d’une licence Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 00ef33666bebe434739056cb38c3dff24285d682
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion] barrières de sécurité des performances

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] nécessite une [!DNL Adobe Workfront Fusion] en plus d’une [!DNL Adobe Workfront license].

L&#39;automatisation du travail nécessite un traitement rapide. [!DNL Adobe Workfront Fusion] est conçu pour des performances élevées. Puisque les scénarios à long terme peuvent ralentir le rythme de votre travail, nous avons conçu [!DNL Workfront Fusion] grâce à des barrières de sécurité conservant les performances qui limitent le temps d’exécution, la taille des données et d’autres paramètres de scénario. [!DNL Workfront Fusion] les concepteurs doivent être conscients de ces barrières de sécurité et les intégrer dans leurs pratiques de conception.

## Navigateurs

Wokfront Fusion ne prend en charge que les navigateurs Chrome.

## Scénarios

* Le délai d’exécution par défaut du scénario est le suivant : **40 minutes**. Lorsque l’exécution atteint ce délai d’expiration, [!DNL Workfront Fusion] interrompt l’exécution du scénario après le cycle ou l’opération suivant, selon le scénario. Cela force l’arrêt du scénario peu après l’atteinte de la limite de 40 minutes.
* La taille maximale d’un plan directeur de scénario est **5 Mo**, mais nous recommandons de conserver la taille du scénario sous **3 Mo**.

  Les modules d’application qui créent ou mettent à jour des données avec un grand nombre de champs peuvent entraîner des plans directeurs très volumineux.

   * Lors de l’utilisation de la variable [!DNL Workfront] , veillez à sélectionner uniquement les champs nécessaires à vos cas d’utilisation de création ou de mise à jour.
   * Lors de l’utilisation d’autres applications, utilisez des modules API personnalisés pour interagir avec n’importe quel type d’enregistrement comportant un grand nombre de champs.

* Bien qu’il n’y ait pas de limite pour le nombre de modules dans un scénario, les scénarios comportant plus de 150 modules ont une incidence négative sur les performances de votre [!DNL Workfront Fusion] système. Pour cette raison, il est déconseillé de créer des scénarios comportant plus de 150 modules.

## Opérations

* Le délai d’expiration de l’opération par défaut est généralement **40 secondes**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Fichiers

* La capacité totale de traitement des fichiers de Fusion est la suivante : **1 Go**. La limite est basée sur un coût total de mémoire. Chaque opération contribue à ce coût. Si un seul fichier de 400 Mo est téléchargé et téléchargé, le coût total de capacité du fichier sera de 800 Mo.

## Utilisation de la mémoire du serveur

* L’utilisation de la mémoire serveur pour une seule exécution est limitée à **1 Go**.

  De nombreux facteurs, tels que les fichiers volumineux ou les modules complexes, peuvent affecter l’utilisation de la mémoire du serveur d’une manière difficile à prédire ou à contrôler. Pour cette raison, l’exécution de votre scénario peut dépasser la limite de mémoire de 1 Go, même si le scénario suit toutes les autres barrières de performance. Le dépassement de la limite de mémoire entraîne l’échec de l’exécution.

## Webhooks

* La taille maximale par défaut d’une payload est : **5 Mo**.
* Les webhooks sont limités à **100 demandes par seconde**. Lorsque cette limite est atteinte, Workfront Fusion envoie un 429 ([!UICONTROL Trop de requêtes]).
* [!DNL Workfront Fusion] stocke les charges utiles webhook pendant 30 jours. L’accès à une payload webhook plus de 30 jours après sa réception entraîne l’erreur &quot;[!UICONTROL Échec de la lecture du fichier à partir du stockage.]&quot;
* Les webhooks sont désactivés automatiquement si l’une des conditions suivantes s’applique :

   * Le webhook n’est connecté à aucun scénario depuis plus de 5 jours.
   * Le webhook est utilisé uniquement dans les scénarios inactifs, qui sont inactifs depuis plus de 30 jours.

* Les webhooks désactivés sont supprimés et désenregistrés automatiquement s’ils ne sont connectés à aucun scénario et sont à l’état désactivé depuis plus de 30 jours.

## Historique de l’exécution

* Les logs d&#39;historique d&#39;exécution sont limités à une taille de **100 Mo**. Si l’historique d’exécution dépasse cette taille, seuls les 100 premiers Mo s’affichent.

## Reprises

Lors de l’utilisation du module Break et de la spécification de la directive Retry (Réessayer), si un scénario échoue consécutivement 10 fois dans un délai de 2 minutes, le scénario est automatiquement désactivé.

