---
content-type: api
navigation-topic: api-navigation-topic
title: Reprises pour les abonnements aux événements
description: Reprises pour les abonnements aux événements
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 63%

---

# Reprises pour les abonnements aux événements

Lors de l’implémentation d’un système de diffusion de messages, quelques avertissements doivent être pris en compte afin de garantir la stabilité, la cohérence et une bonne expérience client. L’un des inconvénients d’un système de diffusion des messages est de s’assurer que les messages arrivent à destination avec succès et de savoir quoi faire lorsqu’ils ne sont pas reçus.

Certaines intégrations peuvent accepter un échec de diffusion, puis abandonner le message et passer au suivant.  Dans d’autres intégrations, l’échec de diffusion d’un message ne peut pas être ignoré. Par exemple, une intégration financière peut tenter de diffuser un message, mais recevoir à la place un code de statut HTTP 404, indiquant que le serveur n’a pas trouvé le point d’entrée sur lequel le message devait être diffusé. Dans de tels cas, un message manquant pourrait signifier qu’une personne ne sera pas payée pour ses heures ou qu’une entreprise dépassera le budget des ressources sous contrat.

## Stratégie Adobe Workfront pour les reprises d’abonnement aux événements

Dans la mesure où les clientes et clients tirent parti de la plateforme Workfront comme une composante essentielle de leur travail intellectuel quotidien, la structure d’abonnement à un événement Workfront fournit un mécanisme permettant d’assurer la diffusion de chaque message dans la mesure du possible.

Les messages sortants déclenchés par un événement et qui ne parviennent pas à être diffusés aux points d’entrée clients sont renvoyés jusqu’à ce que la diffusion soit réussie pendant une période maximale de 48 heures. Pendant ce temps, les reprises se produisent à une fréquence progressivement accrue jusqu’à ce que la diffusion soit réussie ou jusqu’à ce que 11 tentatives aient été effectuées.

La formule pour ces nouvelles tentatives est la suivante :

`((2^attempt) - 1) * 84800ms`

La première reprise a lieu après 1,5 min, la seconde à près de 5 min et la 11e à environ 48 heures.

Les clientes et clients doivent s’assurer que tous les points d’entrée qui consomment des messages sortants provenant des abonnements à Workfront Event sont configurés pour renvoyer un message de réponse de 200 niveaux à Workfront en cas de diffusion réussie.

## Règles d&#39;abonnement désactivées et gelées

* Une URL d’abonnement est **désactivée** si son taux d’échec est supérieur à 70 % avec plus de 100 tentatives OU si elle présente 2 000 échecs consécutifs
* Une URL d’abonnement est **figée** si elle a plus de 2 000 échecs consécutifs et que le dernier succès remonte à plus de 72 heures OU si elle a 50 000 échecs consécutifs dans n’importe quelle période.
* Une URL d’abonnement **désactivée** continuera à tenter d’être diffusée toutes les 10 minutes et sera réactivée avec une diffusion réussie.
* Une URL d’abonnement **figée** ne tentera jamais d’être diffusée à moins qu’elle ne soit activée manuellement en effectuant une requête API.




<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![Event sub retries](assets/event-subscription-circuit-breaker-retries-350x234.png)

The following explanations correspond with the steps depicted in the flowchart:

1. Message fails to be delivered. 
1. Message delivery failure information is logged.

   All failed attempts to deliver a message are logged so that debugging may be performed to determine the root cause of a given failure or series of failures. 

1. URL failures incremented. 
1. Message attempt count is incremented. 
1. Calculate the delay until this message's delivery will be attempted again. 
1. Message is placed onto the message retry queue.

   As shown in the preceding flowchart, the message queue used for processing message delivery retries is a separate queue from the one that processes the initial delivery attempt for each message. This allows the near real-time flow of messages to continue unimpeded by the failure of any subset of messages. 

1. URL circuit status is evaluated. One of the following occurs:

   * If the circuit is open and not allowing deliveries at this time, restart the process at step 5.
   * If the circuit is half-open, this implies that our circuit is currently open, but enough time has passed to allow testing of the URL to see if the problem with delivering to it has been resolved.
   * If the message delivery attempt limits have been reached (48 hours of retrying) then the message is dropped

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1 

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1.
   -->
