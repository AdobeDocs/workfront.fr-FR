---
content-type: api;faq
navigation-topic: general-api
title: Questions fréquentes - Abonnements aux événements
description: Questions fréquentes - Abonnements aux événements
author: Becky
feature: Workfront API
role: Developer
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: 77c07c7c7104d37360cc7630a89dd72836da477c
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 97%

---

# Questions fréquentes - Abonnements aux événements

<!--
{{highlighted-preview}}
-->

Vous trouverez ci-dessous les questions fréquentes sur les abonnements à des événements :

## Qu’est-ce qu’un abonnement ?

Un abonnement est un ensemble de données utilisé pour faire correspondre et diffuser des événements Adobe Workfront vers le point d’entrée HTTP d’un client ou d’une cliente. Cette ressource est composée de 4 attributs principaux :

* customer_id
* obj_code
* obj_id
* url

Un abonnement peut également posséder d’autres attributs, tels que son propre identifiant unique et sa date de création, mais les attributs répertoriés ci-dessus sont principalement utilisés pour faire correspondre les événements et les diffuser aux clientes et aux clients.

## Puis-je sélectionner les événements à envoyer à un point d’entrée en fonction de certains critères inclus dans un payload d’événement ?

Les filtres d’abonnements aux événements permettent de trier les abonnements aux événements selon des critères spécifiés. Il est recommandé d’appliquer des filtres aux abonnements aux événements, car cela peut réduire considérablement le nombre de messages qu’un point d’entrée doit consommer. Pour plus d’informations, consultez [Filtrage des abonnements aux événements](../../wf-api/general/event-subs-api.md#event).

## Pourquoi l’API renvoie-t-elle un code de réponse « 409 Conflict » ?

Si vous tentez de créer un abonnement à un événement et que vous recevez un code de réponse « 409 Conflict », l’abonnement que vous avez tenté de créer est un doublon. Workfront ne permet pas la création d’abonnements en double.

## Que dois-je faire si mes messages ne sont pas diffusés vers mon point d’entrée ?

Examinez les scénarios suivants et utilisez la solution recommandée :

* Assurez-vous que votre point d’entrée de l’abonnement, défini par le champ **url**, renvoie un code de réponse HTTP 2xx. Si ce n’est pas le cas, contactez l’assistance Workfront ou consultez les [Exigences de diffusion des abonnements aux événements](../../wf-api/general/setup-event-sub-endpoint.md).

* La demande de diffusion d’événement peut expirer avant qu’elle ne soit terminée. Assurez-vous que votre point d’entrée répond régulièrement en moins de 5 secondes. Il s’agit du délai d’expiration par défaut défini pour la requête HTTP pour la diffusion d’un message d’abonnement à un événement. Si votre point d’entrée ne répond pas dans les 5 secondes, contactez l’assistance Workfront ou consultez les [Exigences de diffusion des abonnements aux événements](../../wf-api/general/setup-event-sub-endpoint.md).
* Les événements peuvent ne pas se générer de la manière que vous pensez. Assurez-vous de ne pas faire d’hypothèses sur la manière ou le moment du déclenchement prévu et réel des événements. Par exemple, vous pouvez penser que la mise à jour d’un document sur une tâche génère un événement de mise à jour de tâche, mais cette mise à jour génère en fait un événement de création de document ou de mise à jour de document.
* Votre abonnement peut ne pas être configuré comme prévu. Vous pouvez créer des abonnements à des événements dans différents environnements et vous attendre à ce qu’ils soient transférés comme leurs autres données Workfront. Toutefois, les données d’abonnement aux événements ne sont pas configurées pour être copiées ou promues dans d’autres environnements. Assurez-vous d’émettre des demandes d’API dans l’environnement approprié et que les abonnements dans cet environnement sont configurés comme prévu.
* Le payload n’a pas été reçu, car l’adresse IP Workfront nécessaire n’a pas été ajoutée à la liste autorisée de votre pare-feu. Les événements d’abonnement aux événements ne sont envoyés que par quelques adresses IP. Assurez-vous que le réseau de destination comporte toutes les exceptions IP nécessaires pour recevoir les payloads des abonnements aux événements Workfront.
* La payload n’a pas été reçue, car elle dépassait 1 Mo. Les messages d&#39;abonnement à un événement ou l&#39;objet ne peuvent pas dépasser 1 Mo.

## Pourquoi mes messages prennent autant de temps pour atteindre mon point d’entrée ?

Certains des scénarios suivants peuvent être responsables :

* Une opération de grande envergure (une mise à jour en masse, par exemple) dans le système peut provoquer la mise en file d’attente d’un grand nombre de messages en même temps, ce qui peut prendre du temps à traiter.
* Des calculs de longue durée ou de chronologie sur des projets volumineux peuvent entraîner un retard dans la publication des messages à consommer par les abonnements aux événements.
* L’abonnement a peut-être été désactivé.

   * Après un délai de grâce de 100 messages, si une URL spécifique, qui peut être associée à un ou plusieurs abonnements, échoue plus de 70 % du temps ou si l’URL ne parvient pas à diffuser après 2 000 tentatives consécutives, toute tentative de diffusion des messages correspondant à des abonnements avec la même URL est abandonnée. Ces messages sont immédiatement placés en file d’attente pour une reprise.

     Toutes les 10 minutes après la désactivation d’une URL, nous tentons de diffuser le message suivant qui passe pour être traité. Si ce message réussit, nous réactivons cette URL et par la suite tous les abonnements correspondants. Si l’envoi de ce message échoue, ce retardateur de 10 minutes se réinitialise et nous réessayons après son expiration.

     Ce comportement peut être perçu comme incohérent ou comme des diffusions retardées, mais il suit simplement nos politiques de gestion des messages d’abonnement aux événements.

   * Une URL d’abonnement à un événement sera désactivée de manière irréversible si l’une des conditions suivantes est remplie :

      * L’URL d’abonnement n’a pas pu diffuser pendant 7 jours et au moins 2 000 tentatives de diffusion consécutives ont échoué au cours des dernières 72 heures.
      * L’URL d’abonnement n’a pas pu remettre 50 000 tentatives consécutives.

## Que dois-je faire si je reçois un statut de réponse 500 lorsque je tente d’appeler l’API d’abonnement aux événements ?

Veuillez contacter le support Workfront. Pour savoir comment contacter le support, voir [Contacter l’assistance clientèle](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Quels types d’authentification différents puis-je utiliser avec les abonnements aux événements Workfront ?

Vous pouvez utiliser n’importe quelle authentification utilisant un jeton porteur. Le champ **authToken** d’un abonnement est une chaîne qui représente un jeton porteur OAuth2 utilisé pour s’authentifier avec l’URL spécifiée dans le champ **url**. En théorie, ce jeton peut prendre n’importe quelle valeur tant que le point d’entrée de destination sait comment gérer son codage, à savoir **utf-8**.

## Combien de temps doit s’écouler avant que je ne reçoive ma payload d’événement des abonnements aux événements Workfront ?

En règle générale, vous pouvez vous attendre à recevoir les demandes de diffusion d’événement d’abonnement aux événements en moins de 5 secondes à partir de la modification des données consignée. En moyenne, les notifications de webhook sont reçues en moins d’une seconde à partir du moment où la modification des données est effectuée. Cependant, le service peut recevoir des messages en si grande quantité qu’il peut également prendre plus de temps.

## Ressources supplémentaires

* **Documentation de l’API** : [API d’abonnement aux événements](../../wf-api/general/event-subs-api.md)

* **Bonnes pratiques** : [Bonnes pratiques en matière d’abonnement aux événements](../../wf-api/general/event-sub-best-practice.md)

* **Champs déclenchant des payloads d’abonnement aux événements** : [Champs de ressources de l’abonnement à un événement](../../wf-api/api/event-sub-resource-fields.md)

* **Présentation des reprises pour les abonnements aux événements**: [Reprises pour les abonnements aux événements](../../wf-api/api/event-sub-retries.md)

* **Configurer votre pare-feu pour Workfront**: [Configurer la liste autorisée de votre pare-feu](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
