---
content-type: api
navigation-topic: general-api
title: Exigences de diffusion de l’abonnement à un événement
description: Exigences de diffusion de l’abonnement à un événement
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
TQID: https://experienceleague.adobe.com/rft0idTJddZkXvAcOymqXarAs1zTf77HttI6vuwCTlw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 275
ht-degree: 79%

---

# Exigences de diffusion de l’abonnement à un événement

Les messages d’abonnement aux événements sont des notifications qui peuvent être configurées pour avertir les utilisateurs et utilisatrices lorsque certains événements se produisent. Pour en savoir plus sur les abonnements aux événements, voir la section [Questions fréquentes - Abonnements aux événements](../../wf-api/general/event-subs-faq.md).

## Normes de diffusion des messages d’abonnement aux événements

Les points d’entrée des services qui utilisent les messages d’abonnement aux événements Adobe Workfront doivent répondre aux exigences de base suivantes, afin que les messages soient envoyés et reçus correctement :

* Le point d’entrée du service doit accepter les requêtes HTTP POST. La méthode HTTP POST est la méthode de requête utilisée dans toutes les diffusions de messages d’abonnement à des événements, y compris les messages de validation.

* Pour que le système de diffusion des abonnements aux événements reconnaisse que le message a bien été reçu, le point d’entrée doit renvoyer un statut HTTP de niveau 200 (par exemple, 200 OK ou 202) pour tous les messages entrants.

* Si aucun statut de niveau 200 n’est renvoyé, le système d’abonnement aux événements suppose que le message n’a pas été délivré correctement et commence à appliquer la politique de reprise appropriée. Pour en savoir plus sur la politique de reprise Workfront, voir la section [Reprises d’abonnement à un événement](../../wf-api/api/event-sub-retries.md).

* En plus de renvoyer un statut de niveau 200 comme statut de réponse, la réponse HTTP doit être reçue dans les cinq secondes suivant le début de la tentative de diffusion.Cette contrainte garantit que les processus métier ou les limitations d&#39;infrastructure des clients ne retardent pas la diffusion d&#39;autres messages en attente de diffusion.

* Si un processus métier à long terme se déclenche depuis un message d’abonnement à un événement, Workfront recommande que

   1. le point d’entrée enregistre les informations du message à la réception et réponde immédiatement avec un statut de niveau 200.
   1. Une fois qu’un point d’entrée a répondu à une demande de diffusion d’abonnement à un événement, les messages enregistrés peuvent être traités.

* Les objets ou messages d’abonnement à un événement ne peuvent pas dépasser 1 Mo.
