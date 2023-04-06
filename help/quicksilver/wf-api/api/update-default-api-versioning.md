---
content-type: api
navigation-topic: api-navigation-topic
title: Mise à jour des intégrations qui utilisent le contrôle de version des API par défaut
description: Mise à jour des intégrations qui utilisent le contrôle de version des API par défaut
author: Becky
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 2b9eacc9b2c8f499cdd1794a55879a56224051c8
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Mise à jour des intégrations qui utilisent le contrôle de version des API par défaut

Nous publions de nouvelles versions de l’API Adobe Workfront sur une base semestrielle. Chaque version est prise en charge pendant trois ans après sa publication, avec une année supplémentaire dans un état obsolète où la version est disponible mais pas prise en charge.

Les intégrations qui ne spécifient pas de version de l’API dans l’URI sont automatiquement acheminées vers Default. Si vous souhaitez que votre appel API utilise une version spécifique de l’API, vous devez spécifier cette version dans vos requêtes d’API Workfront.

>[!NOTE]
>
>Si votre entreprise utilise actuellement l’API par défaut, votre administrateur Workfront a reçu un message du centre d’annonces contenant des instructions supplémentaires sur l’API par défaut.

Pour en savoir plus sur la spécification d’une version dans vos requêtes d’API, voir [Spécification d’une version d’API dans vos intégrations](../../wf-api/api/specify-api-version-integrations.md).

## Remarques concernant l’utilisation de l’API par défaut

Tenez compte des points suivants lorsque vous utilisez l’API Workfront par défaut :

* La version par défaut de l’API est la version la plus récente. Tout appel API sans la version spécifiée utilise la version par défaut. Chaque fois que Workfront publie une nouvelle version de l’API, la version par défaut est mise à jour vers la dernière version. **Par conséquent, après la publication d’une nouvelle version de l’API Workfront, tous les appels d’API qui utilisent la version par défaut doivent être vérifiés pour s’assurer que la fonctionnalité est toujours prise en charge.**.
* Si votre entreprise utilise actuellement l’API par défaut obsolète, votre administrateur Workfront a reçu un message du centre d’annonces contenant des instructions supplémentaires sur l’API par défaut.

Pour consulter la version la plus récente de l’API, voir [Contrôle de version des API et planification de la prise en charge](../../wf-api/api/api-version-support-schedule.md).

## Mise à jour de vos intégrations vers les versions d’API prises en charge

Si vos demandes d’API Workfront ne spécifient pas de version, elles utilisent la valeur par défaut. Nous vous recommandons de spécifier une version prise en charge de l’API, de préférence vers la dernière API prise en charge.

Par exemple, la requête d’API Workfront suivante ne spécifie pas de version d’API :

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Lorsque cette requête est effectuée, vous recevez une réponse avec du texte codé JSON qui spécifie les données de votre instance Workfront. Comme aucune version d’API n’est spécifiée dans cet URI, l’appel est défini sur Par défaut.

Pour transformer une requête d’API par défaut en requête d’API versionnée, appelez simplement une version d’API prise en charge. Par exemple, l’URI suivant demande la version 15 :

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Lors de la mise à jour de vos requêtes d’API Workfront, vous pouvez spécifier n’importe quelle version prise en charge de notre API. Pour en savoir plus sur le référencement d’une API spécifique, voir [Spécification d’une version d’API dans vos intégrations](../../wf-api/api/specify-api-version-integrations.md).

Pour garantir une prise en charge maximale, vous devez appeler la dernière version. Vous trouverez une liste des API prises en charge dans [Contrôle de version des API et planification de la prise en charge](../../wf-api/api/api-version-support-schedule.md).

## Historique de la version par défaut de l’API

L’objectif d’origine de l’&quot;API par défaut&quot; était de la mapper à la dernière version de l’API Workfront. Les clients disposant d’intégrations de base appelées par défaut peuvent ainsi ne jamais avoir à mettre à jour leurs requêtes d’API.

En 2011, Workfront a publié la version 3.0 de l’API. La valeur par défaut a été automatiquement déplacée vers la version 3.0, ce qui a rompu de nombreuses intégrations client trop complexes pour utiliser la version 3.0 sans mise à jour. Par conséquent, Workfront a restauré cette modification et a laissé la version par défaut à la version 2.

Depuis 2011, Workfront a considérablement amélioré les fonctionnalités de l’API. C’est pourquoi nous avons abandonné les anciennes versions de notre API. En 2017, plutôt que de mettre à jour Default, nous avons entièrement supprimé le concept d&#39;une version par défaut. Cela a pour but d’encourager nos clients à utiliser des versions stables de nos API et de maintenir leurs intégrations sur un cycle de, au plus, trois ans.

Workfront rétablit désormais la version de l’API par défaut. L’API par défaut est définie sur la version la plus récente de l’API Workfront et est mise à jour vers la version la plus récente chaque fois qu’une nouvelle version est publiée.

