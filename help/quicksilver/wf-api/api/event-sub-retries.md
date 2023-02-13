---
content-type: api
navigation-topic: api-navigation-topic
title: Reprises d’abonnement à un événement
description: Reprises d’abonnement à un événement
author: John
feature: Workfront API
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 606d19b8a83b833aba6d6b15231a8683aa2cee40
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Reprises d’abonnement à un événement

Lors de la mise en oeuvre d’un système de diffusion de messages, quelques avertissements doivent être pris en compte afin de garantir la stabilité, la cohérence et une bonne expérience utilisateur. Un des défauts d&#39;un système de diffusion des messages est de s&#39;assurer que les messages arrivent à destination avec succès et de savoir quoi faire lorsque les messages ne parviennent pas.

Certaines intégrations peuvent accepter l’échec de la diffusion, puis abandonner le message et passer au message suivant.  Dans d’autres intégrations, l’échec de diffusion d’un message ne peut pas être ignoré. Par exemple, une intégration financière peut tenter de diffuser un message, mais reçoit à la place un code d’état HTTP 404, qui indique que le serveur n’a pas trouvé le point de terminaison auquel le message devait être diffusé. Dans de tels cas, un message manquant pourrait signifier qu&#39;une personne n&#39;est pas payée pour son temps ou qu&#39;une organisation dépasse le budget des ressources sous contrat.

## Stratégie Adobe Workfront pour les reprises d’abonnement aux événements

Dans la mesure où les clients tirent parti de la plateforme Workfront comme élément essentiel de leur travail quotidien de connaissances, la structure d’abonnement à un événement Workfront fournit un mécanisme permettant de s’assurer que la diffusion de chaque message est tentée dans toute la mesure du possible.

Les messages sortants déclenchés par un événement et qui ne parviennent pas à être diffusés aux points de terminaison clients sont renvoyés jusqu’à ce que la diffusion soit réussie pendant une période maximale de 48 heures. Pendant ce temps, les reprises se produisent à une fréquence réduite de manière incrémentielle jusqu&#39;à ce que la diffusion soit réussie ou jusqu&#39;à ce que 48 heures se soient écoulées.

Les clients doivent s’assurer que tous les points de terminaison qui consomment des messages sortants à partir des abonnements à Workfront Event sont configurés pour renvoyer un message de réponse de 200 niveaux à Workfront en cas de diffusion réussie.

## Gestion des messages sortants déclenchés par un événement ayant échoué

L’organigramme suivant présente la stratégie de réactivation des diffusions de messages avec les abonnements à des événements Workfront :

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

Les explications suivantes correspondent aux étapes décrites dans l’organigramme :

1. La diffusion du message échoue.
1. Les informations d’échec de diffusion du message sont consignées.

   Toutes les tentatives échouées de diffusion d’un message sont consignées afin que le débogage puisse être effectué pour déterminer la cause racine d’un échec donné ou d’une série d’échecs.

1. Échec de l’URL incrémenté.
1. Le nombre de tentatives de messages est incrémenté.
1. Calculez le délai jusqu’à ce que la diffusion de ce message soit de nouveau envoyée.
1. Le message est placé dans la file d’attente des reprises de message.

   Comme illustré dans l’organigramme précédent, la file d’attente des messages utilisée pour le traitement des reprises de diffusion des messages est une file d’attente distincte de celle qui traite la tentative de diffusion initiale pour chaque message. Cela permet au flux de messages en temps quasi réel de continuer sans être entravé par l’échec d’un sous-ensemble de messages.

1. L’état du circuit URL est évalué. L’une des opérations suivantes se produit :

   * Si le circuit est ouvert et que les diffusions ne sont pas autorisées à ce stade, redémarrez le processus à l’étape 5.
   * Si le circuit est à moitié ouvert, cela signifie que notre circuit est actuellement ouvert, mais un temps suffisant a été nécessaire pour permettre le test de l’URL pour voir si le problème de l’envoi vers lui a été résolu.
   * Si les limites des tentatives de diffusion du message ont été atteintes (48 heures après une nouvelle tentative), le message est abandonné.

1. Si le circuit d’URL est fermé et autorise les diffusions, essayez de diffuser le message. Si cette diffusion échoue, le message redémarre à l’étape 1.

1. Si le circuit d’URL est fermé et autorise les diffusions, essayez de diffuser le message. Si cette diffusion échoue, le message redémarre à l’étape 1.

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront disables Event Subscriptions when both of the following criteria are met:
   <ul>
   <!--
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">The Event Subscription has failed 1000 delivery attempts consecutively</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">48 hours have passed since the last successful delivery</li>
   </ul></li>
   -->
