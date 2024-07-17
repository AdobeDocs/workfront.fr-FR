---
content-type: api;faq
navigation-topic: general-api
title: Questions fréquentes - Abonnements aux événements
description: Questions fréquentes - Abonnements aux événements
author: Becky
feature: Workfront API
role: Developer
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 0%

---

# Questions fréquentes - Abonnements aux événements

<!--
{{highlighted-preview}}
-->

Vous trouverez ci-dessous des questions fréquentes sur les abonnements à des événements :

## Qu’est-ce qu’un abonnement ?

Un abonnement est un ensemble de données utilisé pour faire correspondre et diffuser des événements Adobe Workfront sur le point de terminaison HTTP d’un client. Cette ressource est composée de 4 attributs principaux :

* customer_id
* obj_code
* obj_id
* url

Un abonnement peut également avoir d’autres attributs, tels que son propre identifiant unique et la date de création, mais les attributs répertoriés ci-dessus sont principalement utilisés pour faire correspondre les événements et les diffuser aux clients.

## Puis-je sélectionner les événements qui sont envoyés à un point de terminaison en fonction de certains critères dans une payload d’événement ?

Les filtres d’abonnement aux événements permettent de trier les sous-formulaires d’événement selon des critères spécifiés. Il est recommandé d’appliquer des filtres aux abonnements aux événements, car cela peut réduire considérablement le nombre de messages qu’un point de terminaison doit consommer. Pour plus d’informations, voir [Filtrage de l’abonnement à un événement](../../wf-api/general/event-subs-api.md#event).

## Pourquoi l’API renvoie-t-elle un code de réponse au conflit 409 ?

Si vous tentez de créer un abonnement à un événement et de recevoir un code de réponse : conflit 409, l’abonnement que vous avez tenté de créer est un doublon. Workfront ne permet pas la création d’abonnements en double.

## Que dois-je faire si mes messages ne sont pas remis à mon point de terminaison ?

Recherchez les scénarios suivants et utilisez la solution recommandée :

* Assurez-vous que votre point de terminaison d’abonnement (défini par le champ **url**) renvoie un code de réponse HTTP 2XX. Si ce n’est pas le cas, contactez l’assistance Workfront ou consultez la section [Conditions de diffusion de l’abonnement à un événement](../../wf-api/general/setup-event-sub-endpoint.md).

* La demande de diffusion d’événement peut être en attente avant qu’elle ne soit terminée. Assurez-vous que votre point de terminaison répond de manière cohérente dans les 5 secondes. Il s’agit du délai d’expiration par défaut défini pour la requête HTTP afin de diffuser un message d’abonnement à un événement. Si votre point de terminaison ne répond pas dans les 5 secondes, contactez l’assistance Workfront ou reportez-vous à la section [Conditions de diffusion de l’abonnement à un événement](../../wf-api/general/setup-event-sub-endpoint.md).
* Les événements peuvent ne pas générer la manière dont vous pensez. Assurez-vous de ne pas faire d’hypothèses sur la manière ou le moment où les événements doivent et doivent se déclencher. Par exemple, vous pouvez penser que la mise à jour d’un document sur une tâche génère un événement de mise à jour de tâche, mais qu’elle génère plutôt un événement de création de document ou de mise à jour de document.
* Votre abonnement peut ne pas être configuré comme prévu. Vous pouvez créer des abonnements à des événements dans différents environnements et vous attendre à ce qu’ils soient transférés comme le font leurs autres données Workfront. Toutefois, les données d’abonnement à un événement ne sont pas configurées pour être copiées ou promues dans d’autres environnements. Assurez-vous d’émettre des requêtes d’API dans l’environnement approprié et que les abonnements dans cet environnement sont configurés comme prévu.
* La payload n’a pas été reçue, car l’adresse IP Workfront nécessaire n’a pas été ajoutée à la liste autorisée de votre pare-feu. Les événements d’abonnement à un événement ne sont envoyés que par quelques adresses IP. Assurez-vous que le réseau de destination comporte toutes les exceptions IP nécessaires pour recevoir les payloads des abonnements aux événements Workfront.

## Pourquoi cela prend-il un temps excessif pour que mes messages atteignent mon point de terminaison ?

Certains des scénarios suivants peuvent être responsables :

* Une opération de grande envergure (une mise à jour en masse, par exemple) dans le système peut provoquer la mise en file d’attente d’un grand nombre de messages en même temps, ce qui peut prendre du temps à traiter.
* Des calculs de longue durée ou de chronologie sur des projets volumineux peuvent entraîner un retard dans la publication des messages à des abonnements à des événements à consommer.
* L’abonnement a peut-être été désactivé.

   * Après une période de grâce de 100 messages, si une URL spécifique, qui peut être associée à un ou plusieurs abonnements, échoue plus de 70 % du temps ou si l’URL ne parvient pas à diffuser après 2 000 tentatives consécutives, tous les messages correspondant à des abonnements avec la même URL ne sont pas tentés pour diffusion. Ces messages sont immédiatement placés en file d’attente pour une nouvelle tentative.

     Toutes les 10 minutes après la désactivation d’une URL, nous tentons de diffuser le message suivant qui passe pour être traité. Si ce message réussit, nous réactivons cette URL et par la suite tous les abonnements correspondants. Si l’envoi de ce message échoue, ce minuteur de 10 minutes se réinitialise et nous réessayons après son expiration.

     Ce comportement peut être perçu comme incohérent ou comme des diffusions différées, mais il suit simplement nos politiques de gestion des messages d’abonnement à un événement.

   * Une URL d’abonnement à un événement sera désactivée de manière irréversible si l’une des conditions suivantes est remplie :

      * L’URL d’abonnement n’a pas pu être diffusée pendant 7 jours et a échoué au moins 2 000 tentatives de diffusion consécutives au cours des dernières 72 heures.
      * L’URL d’abonnement n’a pas pu livrer 50 000 tentatives consécutives.

## Que dois-je faire si je reçois un état de réponse 500 lorsque je tente d’appeler l’API d’abonnement à un événement ?

Veuillez contacter l’assistance de Workfront. Pour savoir comment contacter l’assistance, voir [Contacter le service clientèle](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Quels types d’authentification différents puis-je utiliser avec les abonnements à des événements Workfront ?

Vous pouvez utiliser n’importe quelle authentification utilisant un jeton porteur. Le champ **authToken** d&#39;un abonnement est une chaîne qui représente un jeton porteur OAuth2 utilisé pour s&#39;authentifier avec l&#39;URL spécifiée dans le champ **url**. En théorie, cette valeur de jeton peut être n’importe quelle valeur tant que le point de terminaison de destination sait comment gérer son encodage, qui est **utf-8**.

## Quelle doit être la durée avant que je ne reçoive la payload de l’événement des abonnements à Workfront Event ?

En règle générale, vous pouvez vous attendre à recevoir les demandes de remise d’événement d’abonnement à un événement en moins de 5 secondes à partir du changement de données en cours de journalisation. En moyenne, les notifications de webhook sont reçues en moins d’une seconde à partir du moment où la modification des données est effectuée. Cependant, le service peut recevoir des messages en si grande quantité qu’il peut également prendre plus de temps.

## Ressources supplémentaires

* **Documentation de l’API** : [API d’abonnement à un événement](../../wf-api/general/event-subs-api.md)

* **Bonnes pratiques** : [Bonnes pratiques en matière d’abonnement à un événement](../../wf-api/general/event-sub-best-practice.md)

* **Champs qui déclenchent des payloads d’abonnement à un événement** : [Champs de ressources d’abonnement à un événement](../../wf-api/api/event-sub-resource-fields.md)

* **Comprendre les reprises d’abonnement à un événement** : [Reprises d’abonnement à un événement](../../wf-api/api/event-sub-retries.md)

* **Configuration de votre pare-feu pour Workfront** : [Configuration de la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
