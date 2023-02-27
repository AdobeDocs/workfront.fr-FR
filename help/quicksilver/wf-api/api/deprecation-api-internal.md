---
content-type: api
navigation-topic: api-navigation-topic
title: Abandon de l’API interne
description: Abandon de l’API interne
author: Becky
feature: Workfront API
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Abandon de l’API interne

API-Interne est une version de l’API Adobe Workfront qui n’est pas prise en charge en raison de sa conception et de son objectif. Bien qu’il contienne les mises à jour les plus récentes de l’API Workfront, il peut être modifié sans préavis et doit donc être utilisé avec précaution dans les intégrations de production. Workfront recommande vivement de mettre à jour toutes les intégrations internes à l’API vers une API versionnée.

Pour en savoir plus sur les versions prises en charge de l’API Workfront, voir [Contrôle de version des API et planification de la prise en charge](../../wf-api/api/api-version-support-schedule.md).

**Utilisation d’API non prise en charge**

Si vos intégrations nécessitent des fonctionnalités qui ne sont pas disponibles dans une API versionnée, Workfront recommande d’utiliser l’API non prise en charge. Tout comme API-Interne, API-Non pris en charge n’est pas pris en charge. L’API non prise en charge inclut également les modifications les plus récentes apportées à l’API Workfront et peut être modifiée sans préavis. Workfront vous encourage à utiliser API non pris en charge dans votre environnement de test afin que vous puissiez explorer de nouvelles fonctionnalités et vous assurer que l’API est exempte de bogues.

**Détermination de la version d’API que vous utilisez**

Vous pouvez déterminer la version de l’API utilisée par vos intégrations à l’aide de REST pour construire un URI qui envoie un appel via HTTPS à Workfront, puis renvoie une réponse JSON.

L’exemple suivant illustre un URI qui appelle API-Internal :

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

L’exemple suivant illustre un URI qui appelle API-Unsupported :

```
https://<domainname>.my.workfront.com/attask/api/api-unsupported/proj/4c70...
```

L’exemple suivant illustre un URI qui appelle la version 15.0 de l’API :

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
