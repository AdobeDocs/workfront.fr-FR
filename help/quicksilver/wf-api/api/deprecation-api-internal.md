---
content-type: api
navigation-topic: api-navigation-topic
title: Obsolescence d’API-Internal
description: Obsolescence d’API-Internal
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
source-git-commit: acc7414a9c6eef838147aee675603b6cc2566fb9
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 100%

---

# Obsolescence d’API-Internal

API-Internal est une version de l’API Adobe Workfront qui n’est pas prise en charge en raison de sa conception et de son objectif. Bien qu’elle contienne les mises à jour les plus récentes de l’API Workfront, elle est susceptible d’être modifiée sans préavis et doit donc être utilisée avec prudence dans les intégrations de production. Workfront recommande fortement de mettre à jour toutes les intégrations d’API-Internal avec une API versionnée.

Pour en savoir plus sur les versions prises en charge de l’API Workfront, voir [Planning de la prise en charge et du contrôle de version de l’API](../../wf-api/api/api-version-support-schedule.md).

**Utiliser l’API-Unsupported**

Si vos intégrations nécessitent une fonctionnalité qui n’est pas disponible dans une API versionnée, Workfront recommande d’utiliser API-Unsupported. Comme pour API-Internal, API-Unsupported n’est pas prise en charge. API-Unsupported comprend également les modifications les plus récentes apportées à l’API Workfront et est susceptible d’être modifiée sans préavis. Workfront vous encourage à utiliser API-Unsupported dans votre environnement de test où vous pouvez explorer de nouvelles fonctionnalités et vous assurer que l’API est exempte de bugs.

**Déterminer la version de l’API que vous utilisez.**

Vous pouvez déterminer la version de l’API que vos intégrations utilisent en vous servant de REST pour construire un URI qui envoie un appel via HTTPS à Workfront et renvoie ensuite une réponse JSON.

L’exemple suivant montre un URI qui appelle API-Internal :

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

L’exemple suivant montre un URI qui appelle API-Unsupported :

```
https://<domainname>.my.workfront.com/attask/api-unsupported/proj/4c70...
```

>[!NOTE]
>
>Les appels d’API-Unsupported omettent la section `/api` de l’URL.

L’exemple suivant montre un URI qui appelle la version 15.0 de l’API :

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
