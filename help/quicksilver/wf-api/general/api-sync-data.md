---
content-type: api
keywords: API,data,sync,journal,entry,object
navigation-topic: general-api
title: Utilisation de l’API pour synchroniser les données des programmes et services
description: Utilisation de l’API pour synchroniser les données des programmes et services
author: Becky
feature: Workfront API
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---


# Utilisation de l’API pour synchroniser les données pour les programmes et services

Il s’agit de méthodes courantes permettant d’utiliser l’API pour synchroniser les données des programmes et services.

## Mises à jour en temps quasi réel

Adobe Workfront utilise &quot;Abonnements à un événement&quot; (également appelés webhooks) pour envoyer en temps quasi réel des mises à jour sur les objets et actions pris en charge, via l’API, aux points de terminaison souhaités. Vous pouvez vous attendre à recevoir une mise à jour concernant les nouveaux objets et actions dans les 5 secondes qui suivent, mais les mises à jour se produisent en moyenne en environ 1 seconde. Pour plus d’informations sur les types d’objets pris en charge, les types d’actions pris en charge, des détails techniques et des exemples de configuration des abonnements à un événement, voir [API d’abonnement à un événement](../../wf-api/general/event-subs-api.md) et [Exigences de diffusion de l’abonnement à un événement](../../wf-api/general/setup-event-sub-endpoint.md).

## Mises à jour par lots

Les mises à jour par lots permettent de configurer votre système pour des mises à jour en effectuant des requêtes périodiques sur les serveurs Workfront. Il existe de nombreuses façons de le faire, mais le processus consiste généralement à demander à votre service d’adresser une requête aux serveurs API de Workfront et de rechercher les objets qui ont été créés ou modifiés depuis le dernier appel de requête. Pour plus d’informations sur les appels de requêtes potentiels et les paramètres utiles, voir [Comportement des GET](../../wf-api/general/api-basics.md#get-behavior) de la section [Principes de base des API](../../wf-api/general/api-basics.md) article.

À mesure que vous configurez votre service pour les mises à jour par lots, voici quelques points importants à garder à l’esprit :

### Dates d’entrée

Les dates d’entrée sont stockées selon la mise en forme ISO 8601. Cette norme inclut des informations sur la date, l’heure et le fuseau horaire.

**Exemple :** Format de date ISO 8601

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

La date de création d’un objet et la date de dernière modification de l’objet sont respectivement stockées sous les forme &quot;entryDate&quot; et &quot;lastUpdateDate&quot;. Pour des informations détaillées sur les objets Workfront, leurs champs associés et leurs noms de champ, reportez-vous à la section [Explorateur d’API](../../wf-api/general/api-explorer.md). Notez que la entryDate d’un objet Workfront donné ne change pas, car la lastUpdatedDate change chaque fois que l’objet est modifié.

**Exemple :** Requête de GET pour un objet de problème, à l’aide de la méthode **lastUpdateDate** champ . Cette requête renvoie tous les problèmes mis à jour depuis cette date spécifiée.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Objet d’entrée du journal

Si vous souhaitez obtenir des modifications concernant un champ spécifique d’un objet, vous pouvez interroger l’objet &quot;Entrée du journal&quot;. L’objet Entrée du journal Workfront peut être configuré pour consigner des informations sur des champs d’objet spécifiques chaque fois que ces champs sont modifiés. Voir [Configuration des mises à jour du système](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) pour plus d’informations.

Lorsqu’un champ est configuré pour être consigné dans le cadre de l’objet Journal Entry , une entrée de journal correspondante est créée chaque fois que ce champ est modifié. Vous pouvez ensuite interroger l’objet Entrée de journal à l’aide d’un appel API semblable à ce qui suit :

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>&quot;entryDate&quot; est utilisé pour examiner une entrée de journal d’une modification, au lieu de regarder l’objet modifié lui-même.
