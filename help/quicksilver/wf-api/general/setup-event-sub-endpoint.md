---
content-type: api
navigation-topic: general-api
title: Exigences en matière de diffusion d’abonnements aux événements
description: Exigences en matière de diffusion d’abonnements aux événements
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 4%

---


# Exigences en matière de diffusion d’abonnements aux événements

Les messages d’abonnement aux événements sont des notifications qui peuvent être configurées pour avertir les utilisateurs lorsque certains événements se produisent. Pour en savoir plus sur les abonnements à des événements, voir [FAQ - Abonnements à des événements](../../wf-api/general/event-subs-faq.md).

## Normes de diffusion des messages d’abonnement à un événement

Les points de terminaison de service qui utilisent les messages d’abonnement aux événements Adobe Workfront doivent répondre aux exigences de base suivantes, afin de garantir que les messages seront envoyés et reçus correctement :

* Le point de terminaison de service doit accepter les requêtes de POST HTTP. Le POST HTTP est la méthode de requête utilisée dans toutes les diffusions de messages d’abonnement d’événement, y compris les messages de validation.

* Pour que le système de diffusion d’abonnement à l’événement reconnaisse que le message a bien été reçu, le point de terminaison doit renvoyer un état HTTP de 200 niveaux (par exemple, 200 OK ou 202) pour tous les messages entrants.

* Si aucun statut de niveau 200 n’est renvoyé, le système d’abonnement à l’événement suppose que le message n’a pas été délivré correctement et commence à appliquer la stratégie de reprise appropriée. Pour en savoir plus sur la stratégie de nouvelle tentative Workfront, voir [Reprises d’abonnement à un événement](../../wf-api/api/event-sub-retries.md).

* Outre le renvoi d’un état de réponse de 200 niveaux, la réponse HTTP doit être reçue dans les cinq secondes suivant le début de la tentative de diffusion. Cette contrainte permet aux clients d’exécuter des processus métier ou des limitations d’infrastructure de ne pas retarder la diffusion d’autres messages en attente de diffusion.

* Si un processus d’entreprise à long terme déclenche un message d’abonnement à un événement, Workfront recommande  that

   1. le point de terminaison enregistre les informations du message à la réception et répond immédiatement avec un état de 200 niveaux.
   1. Une fois qu’un point de terminaison a répondu à une demande de diffusion d’abonnement à un événement, les messages enregistrés peuvent être traités.
