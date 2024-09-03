---
content-type: api
navigation-topic: api-navigation-topic
title: Mettre à jour les intégrations qui utilisent le contrôle de version par défaut de l’API
description: Mettre à jour les intégrations qui utilisent le contrôle de version par défaut de l’API
author: Becky
feature: Workfront API
role: Developer
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 100%

---

# Mettre à jour les intégrations qui utilisent le contrôle de version par défaut de l’API

Nous publions de nouvelles versions de l’API Adobe Workfront deux fois par an. Chaque version est prise en charge pendant trois ans après sa publication, avec une année supplémentaire sous l’état « obsolète », dans lequel la version est disponible mais n’est pas prise en charge.

Les intégrations qui ne spécifient pas de version de l’API dans l’URI sont automatiquement dirigées vers la version par défaut. Si vous souhaitez que votre appel API utilise une version spécifique de l’API, vous devez la spécifier dans vos demandes d’API Workfront.

>[!NOTE]
>
>Si votre organisation utilise actuellement l’API par défaut, votre administrateur ou administratrice Workfront a reçu un message du centre d’annonces contenant des instructions supplémentaires sur l’API par défaut.

Pour en savoir plus sur la spécification d’une version dans vos demandes d’API, voir la section [Spécifier une version d’API dans vos intégrations](../../wf-api/api/specify-api-version-integrations.md).

## Considérations relatives à l’utilisation de l’API par défaut

Tenez compte des éléments suivants lorsque vous travaillez avec l’API par défaut de Workfront :

* La version par défaut de l’API est la version la plus récente. Tout appel API sans la version spécifiée utilise la version par défaut. Chaque fois que Workfront publie une nouvelle version de l’API, la version par défaut est mise à jour vers la dernière version. **Par conséquent, après la publication d’une nouvelle version de l’API Workfront, tous les appels API qui utilisent la version par défaut doivent être vérifiés pour s’assurer que la fonctionnalité est toujours prise en charge**.
* Si votre organisation utilise actuellement l’API par défaut précédente, qui est obsolète, votre administrateur ou administratrice Workfront reçoit un message du centre d’annonces avec des instructions supplémentaires concernant l’API par défaut.

Pour consulter la version la plus récente de l’API, voir [Calendrier des versions de l’API et de la prise en charge](../../wf-api/api/api-version-support-schedule.md).

## Mise à jour de vos intégrations vers les versions d’API prises en charge

Si vos demandes d’API Workfront ne spécifient pas de version, elles utilisent la version par défaut. Nous vous recommandons de spécifier dans vos demandes API une version prise en charge de l’API, de préférence la dernière API prise en charge.

Par exemple, la demande API Workfront suivante ne spécifie pas de version d’API :

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Lorsque cette demande est faite, vous recevez une réponse avec un texte encodé JSON qui spécifie les données de votre instance Workfront. Aucune version de l’API n’étant spécifiée dans cette URI, l’appel passe à la version par défaut.

Pour transformer une demande API par défaut en une demande API versionnée, il suffit d’appeler une version d’API prise en charge. Par exemple, l’URI suivante demande la version 15 :

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Lorsque vous mettez à jour vos demandes API Workfront, vous pouvez spécifier n’importe quelle version prise en charge de notre API. Pour en savoir plus sur le référencement d’une API spécifique, voir la section [Spécifier une version d’API dans vos intégrations](../../wf-api/api/specify-api-version-integrations.md).

Pour bénéficier d’une fenêtre d’assistance maximale, il convient d’appeler la version la plus récente. Vous trouverez une liste des API prises en charge dans le [planning du contrôle des versions et de la prise en charge des API](../../wf-api/api/api-version-support-schedule.md).

## Historique de la version par défaut de l’API

L’intention initiale de « l’API par défaut », ou version par défaut, était de la faire correspondre à la dernière version de l’API Workfront. Cela permettrait aux clientes et clients ayant des intégrations de base qui ont appelé la version par défaut de ne jamais avoir à mettre à jour leurs demandes API.

En 2011, Workfront a publié la version 3.0 de l’API. La version par défaut est passée automatiquement à la version 3.0, ce qui a entraîné la rupture de nombreuses intégrations de clientes et clients qui étaient trop complexes pour utiliser la version 3.0 sans mise à jour. Par conséquent, Workfront a annulé cette modification et a laissé la version par défaut sur la version 2.

Depuis 2011, Workfront a considérablement augmenté les fonctionnalités de l’API. Pour cette raison, nous avons supprimé les anciennes versions de notre API. En 2017, plutôt que de mettre à jour la version par défaut, nous avons entièrement supprimé le concept de version par défaut. Ceci avait pour but d’encourager nos clientes et clients à utiliser des versions stables de nos API et à maintenir leurs intégrations sur un cycle de trois ans au maximum.

Workfront rétablit actuellement la version de l’API par défaut. L’API par défaut est définie sur la version la plus récente de l’API Workfront et sera mise à jour chaque fois qu’une nouvelle version sera publiée.

