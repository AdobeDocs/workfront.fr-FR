---
content-type: api
navigation-topic: api-navigation-topic
title: Mise à jour des intégrations qui utilisent le contrôle de version des API par défaut
description: Mise à jour des intégrations qui utilisent le contrôle de version des API par défaut
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Mise à jour des intégrations qui utilisent le contrôle de version des API par défaut

Nous publions de nouvelles versions de l’API Adobe Workfront sur une base semestrielle. Chaque version est prise en charge pendant trois ans après sa publication, avec une année supplémentaire dans un état obsolète où la version est disponible mais pas prise en charge.

Les intégrations qui ne spécifient pas de version de l’API dans l’URI sont automatiquement acheminées vers Default, qui a été abandonné. Pour que vos intégrations Workfront soient valides, vous devez spécifier une version d’API prise en charge dans vos requêtes d’API Workfront.

Pour en savoir plus sur la spécification d’une version dans vos requêtes d’API, voir [Spécification d’une version d’API dans vos intégrations](../../wf-api/api/specify-api-version-integrations.md).

## Présentation de la version par défaut de l’API

L’objectif d’origine de l’&quot;API par défaut&quot; était de la mapper à la dernière version de l’API Workfront. Les clients disposant d’intégrations de base appelées par défaut peuvent ainsi ne jamais avoir à mettre à jour leurs requêtes d’API.

En 2011, Workfront a publié la version 3.0 de l’API. La valeur par défaut a été automatiquement déplacée vers la version 3.0, ce qui a rompu de nombreuses intégrations client trop complexes pour utiliser la version 3.0 sans mise à jour. Par conséquent, Workfront a restauré cette modification et a laissé la version par défaut à la version 2.

Malheureusement, cette rubrique n’a jamais été revisitée. À l’heure où nous prévoyons d’augmenter considérablement les fonctionnalités de l’API, nous sommes obligés de abandonner les anciennes versions de notre API, y compris Default. Plutôt que de mettre à jour Default, ce qui pourrait sans aucun doute interrompre davantage d’intégrations, nous supprimons entièrement le concept de version par défaut. Cela encourage nos clients à utiliser des versions stables de nos API et à maintenir leurs intégrations sur un cycle de trois ans au plus.

## Dépréciation de la valeur par défaut

Afin d’améliorer l’API Workfront, nous sommes en train de supprimer les anciennes versions d’API qui ont dépassé notre période de prise en charge de trois ans. L’une de ces versions est la version 2, à laquelle la valeur par défaut est mappée. Cette version a été publiée en 2010 et une grande partie de la logique prise en charge dans l’application Attask/Workfront à l’époque n’existe plus ou a considérablement changé.

Nous avons abandonné la valeur par défaut en juillet 2017 et nous ne désignerons plus une version spécifique de l’API comme version par défaut. À la place, toutes les demandes d’API Workfront doivent spécifier une version d’API spécifique.

>[!IMPORTANT]
>
> D’ici le 1er juillet 2018, toutes les intégrations Workfront qui utilisent la valeur par défaut doivent être mises à jour pour appeler une version d’API prise en charge spécifique. À compter de cette date, toutes les requêtes d’API Workfront utilisées par les intégrations qui ne spécifient pas de version échoueront.

Pour en savoir plus sur la cadence d’obsolescence de Workfront, voir [Contrôle de version des API et planification de la prise en charge](../../wf-api/api/api-version-support-schedule.md).

## Mise à jour de vos intégrations vers les versions d’API prises en charge

Si vos demandes d’API Workfront ne spécifient pas de version, elles utilisent la valeur par défaut. Vous devez mettre à jour vos requêtes d’API pour spécifier une version prise en charge de l’API, de préférence vers la dernière API prise en charge.

Par exemple, la requête d’API Workfront suivante ne spécifie pas de version d’API :

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Lorsque cette requête est effectuée, vous recevez une réponse avec du texte codé JSON qui spécifie les données de votre instance Workfront. Comme aucune version d’API n’est spécifiée dans cet URI, l’appel est défini sur Par défaut.

Pour transformer une requête d’API par défaut en requête d’API versionnée, appelez simplement une version d’API prise en charge. Par exemple, l’URI suivant demande la version 9 :

`https://davidwhite.my.workfront.com/attask/api/`**v9.0**`/project/metadata`

Lors de la mise à jour de vos requêtes d’API Workfront, vous pouvez spécifier n’importe quelle version prise en charge de notre API. Pour en savoir plus sur le référencement d’une API spécifique, voir [Spécification d’une version d’API dans vos intégrations](../../wf-api/api/specify-api-version-integrations.md).

Pour garantir une prise en charge maximale, vous devez appeler la dernière version (version 9). Vous trouverez une liste des API prises en charge dans [Contrôle de version des API et planification de la prise en charge](../../wf-api/api/api-version-support-schedule.md).

Il est impératif que vous mettiez à jour les intégrations que vous avez qui utilisent Default. Si vous disposez actuellement d’intégrations qui ne spécifient pas de version, vous pouvez recevoir une notification de votre représentant Workfront, de votre responsable de la réussite client, de votre représentant de l’assistance ou un message du centre d’annonces.

Dès que possible, veillez à ce que vos intégrations soient mises à jour afin d’appeler une version prise en charge de notre API.
