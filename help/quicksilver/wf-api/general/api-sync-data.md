---
content-type: api
keywords: API,données,synchronisation,journal,entrée,objet
navigation-topic: general-api
title: Utiliser l’API pour synchroniser les données des programmes et services
description: Utiliser l’API pour synchroniser les données des programmes et services
author: Becky
feature: Workfront API
role: Developer
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 100%

---


# Utiliser l’API pour synchroniser les données des programmes et services

Il s’agit de méthodes courantes permettant d’utiliser l’API pour synchroniser les données des programmes et services.

## Mises à jour en temps quasi réel

Adobe Workfront utilise des « abonnements aux événements » (également appelés « webhooks ») pour envoyer des mises à jour en temps quasi réel sur les objets et les actions pris en charge, via l’API, au(x) point(s) d’entrée souhaité(s). Le délai de mise à jour des nouveaux objets et actions est de 5 secondes, mais en moyenne, les mises à jour sont effectuées en 1 seconde environ. Pour plus d’informations sur les types d’objets et d’actions pris en charge, les détails techniques et les exemples de mise en place d’abonnements aux événements, consultez les sections [API d’abonnement aux événements](../../wf-api/general/event-subs-api.md) et [Exigences de diffusion de l’abonnement aux événements](../../wf-api/general/setup-event-sub-endpoint.md).

## Mises à jour par lots

Les mises à jour par lots vous permettent de configurer votre système pour effectuer des mises à jour en envoyant périodiquement des requêtes aux serveurs Workfront. Il existe diverses méthodes pour y parvenir, mais en général, le processus implique de demander à votre service d’envoyer une requête aux serveurs API de Workfront et de rechercher les objets créés ou modifiés depuis le dernier appel de requête. Pour plus d’informations sur les appels de requêtes potentiels et les paramètres utiles, consultez la section [Comportement des GET](../../wf-api/general/api-basics.md#get-behavior) dans l’article [Principes de base des API](../../wf-api/general/api-basics.md).

À mesure que vous configurez votre service pour les mises à jour par lots, voici quelques points importants à garder à l’esprit :

### Dates d’entrée

Les dates d’entrée sont stockées en utilisant le formatage ISO 8601. Cette norme inclut des informations sur la date, l’heure et le fuseau horaire.

**Exemple :** format de date ISO 8601

<!-- [Copy](javascript:void(0);) -->
 
<pre><code>2020-05-18T17:00:00:000-0600</code></pre> 

La date de création d’un objet est enregistrée sous la forme « entryDate », tandis que la date de dernière modification de l’objet est enregistrée sous la forme « lastUpdateDate ». Pour obtenir des informations détaillées sur les objets Workfront, les champs qui leur sont affectés et les noms des champs, veuillez consulter la section [Explorateur d’API](../../wf-api/general/api-explorer.md). Remarquez que la entryDate d’un objet Workfront donné ne change pas, alors que la lastUpdatedDate change chaque fois que l’objet est modifié.

**Exemple :** requête GET pour un objet problème, utilisant le champ **lastUpdateDate**. Cette requête renvoie tous les problèmes mis à jour depuis cette date spécifiée.

<!-- [Copy](javascript:void(0);) -->
 

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Objet « Entrée du journal »

Pour obtenir des modifications concernant un champ spécifique d’un objet, vous pouvez consulter l’objet « Entrée du journal ». L’objet « Entrée du journal Workfront » peut être configuré pour consigner des informations sur des champs d’objet spécifiques chaque fois que ces champs sont modifiés. Pour plus d’informations, consultez la section [Configurer les mises à jour du système](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Lorsqu’un champ est configuré pour être enregistré en tant qu’objet « Entrée du journal », une entrée du journal correspondante est créée chaque fois que ce champ est modifié. Vous pouvez ensuite interroger l’objet « Entrée du journal » à l’aide d’un appel API comme suit :

<!-- [Copy](javascript:void(0);) -->

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>« entryDate » est utilisé pour consulter l’entrée du journal d’une modification, plutôt que l’objet modifié lui-même.
