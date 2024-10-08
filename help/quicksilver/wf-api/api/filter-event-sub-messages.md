---
filename: filter-event-sub-messages
content-type: api
navigation-topic: api-navigation-topic
title: Filtrer les messages d’abonnement aux événements
description: Filtrer les messages d’abonnement aux événements
author: Becky
feature: Workfront API
role: Developer
exl-id: 8364c4b9-5604-47ab-8b4b-db6836dcd8ca
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1767'
ht-degree: 100%

---

# Filtrer les messages d’abonnement aux événements

Vous pouvez créer des composants de traitement intermédiaires qui peuvent vous aider à filtrer et à traiter uniquement les messages d’abonnement aux événements dont votre entreprise a besoin.

Pour en savoir plus sur les abonnements aux événements, voir [API d’abonnement aux événements](../../wf-api/general/event-subs-api.md).

## Filtrer les messages d’événement

Cette section contient des fragments de code de filtrage que vous pouvez implémenter pour réduire la quantité de messages d’abonnement aux événements.  Pour illustrer les différences dans la syntaxe des différents langages, ces fragments de code illustrent le même ensemble de filtres écrits dans les langages suivants :

Vous pouvez consulter des exemples de filtrage sur la page [https://github.com/workfront/workfront-event-subscription-filter-examples](https://github.com/workfront/workfront-event-subscription-filter-examples). Vous pouvez voir les différences de syntaxe pour chaque langage et les moyens d’interaction avec le SDK AWS. Ces exemples sont écrits sous la forme de fonction Lambda AWS, qui est une méthode courante pour utiliser les composants de filtrage et de traitement intermédiaires.

Les fragments de code suivants sont prêts pour le déploiement et peuvent être utilisés comme point de départ pour vous aider à écrire vos propres filtres et composants de traitement plus complexes.

### Java

L’exemple suivant en Java montre comment filtrer les payloads du projet en fonction de l’ID de groupe du projet, comme dans [ProjectGroupFiltering.java:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/java/src/main/java/com/workfront/lambda/ProjectGroupFiltering.java)

1. Définissez l’ID de groupe que vous recherchez et créez-le en tant que constante statique.

   ```
   private static final String DESIRED_GROUP_ID = "VaqTTVaB0UcbPu4n6824WIYYIV953Mg3";
   ```

   Dans cet exemple, la méthode handleRequest, qui est un nom de méthode standard AWS Lambda, prend un type Map comme premier paramètre, qui est le contenu du message d’abonnement à l’événement.\
   Le deuxième paramètre nécessaire est le contexte de la demande actuelle de proxy Lambda.\
   L’objet Context est utilisé pour obtenir un enregistreur Lambda, qui est utilisé pour écrire un message aux CloudWatchLogs.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
      ...
   }
   ```

2. Lors de l’appel de la méthode handleRequest, obtenez l’attribut « newState » du message d’abonnement à l’événement, qui représente l’état mis à jour de la ressource.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        Map<String, Object> newState = (Map<String, Object>) webHookPayload.get("newState");
        ...
   }
   ```

   Pour en savoir plus sur le format newState, voir [Format du message sortant pour les abonnements aux événements](../../wf-api/api/message-format-event-subs.md).

3. Après avoir analysé le mappage de l’attribut « newState » du message, assurez-vous que l’ID de groupe de l’objet correspond à l’ID de groupe que vous avez identifié à l’étape 1.

4. (Le cas échéant) Si les ID **ne correspondent pas**, abandonnez le message afin qu’une réponse vide soit renvoyée.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
    String projectGroupId = (String) newState.get("groupID");
    logger.log("String projectGroupID is - " + projectGroupId);    
    if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        ...
      }
    return "";
   }
   ```

   >[!NOTE]
   >
   >Il est essentiel de renvoyer une réponse de succès vide. Tout élément autre qu’une réponse 200 est considéré comme un échec de la diffusion.

5. Traitez le message.

   ```
   public String handleRequest(Map<String, Object> webHookPayload, Context context) 
   {
        ...
        if (DESIRED_GROUP_ID.equals(projectGroupId)) {
        //process the message
        logger.log("Processing Event Subscription message matching groupId " + DESIRED_GROUP_ID + "...");
   
        AWSLambda client = AWSLambdaClientBuilder.standard().build();
        InvokeRequest request = new InvokeRequest()
                .withFunctionName("MyFunction")
                .withInvocationType("Event")
                .withLogType("Tail")
                .withPayload(jsonParser.toJson(webHookPayload))
        InvokeResult response = client.invoke(request);
      }
    ... 
   }
   ```

   Le SDK AWS est utilisé pour appeler une autre fonction Lambda, chargée de diffuser le message filtré vers le point d’entrée souhaité.

   L’objectif de la transmission de la responsabilité de diffusion du message à une autre fonction Lambda est d’éviter un délai d’expiration de la demande de diffusion provenant du service d’abonnement à un événement. Actuellement, le délai d’expiration autorisé pour la diffusion est défini sur cinq secondes. Si le filtre prend plus de temps que celui prévu par le paramètre, vous pouvez traiter la demande, mais le service d’abonnement à un événement expire et tombe dans une boucle de reprises jusqu’à ce qu’il reçoive une réponse 200 dans le délai d’expiration.

   Pour en savoir plus sur la gestion de la diffusion des messages, voir [Améliorer la diffusion des messages tout en tenant compte des délais d’expiration](#improving-message-delivery-while-accommodating-timeouts).

### Python

La principale différence entre les exemples Java et Python réside dans le fait que dans l’exemple Java, le message d’abonnement à l’événement est reçu comme premier paramètre, et dans l’exemple Python, le premier paramètre est un « événement » de proxy Lambda, qui contient le message d’abonnement à l’événement ainsi que des informations sur la demande de proxy AWS Lambda.

L’exemple suivant en Python montre comment filtrer les payloads du projet en fonction de l’ID de groupe du projet, comme dans [projectGroupFiltering.py:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/py/projectGroupFiltering.py)

1. Définissez l’ID de groupe que vous recherchez et créez-le en tant que constante statique.

   ```
   DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3'
   ```

   Le premier paramètre est l’« événement » du proxy Lambda, qui contient le message d’abonnement à l’événement et certaines informations supplémentaires qui doivent être analysées.\
   Le second paramètre est le contexte de la requête actuelle de proxy Lambda.\
   Dans cet exemple, l’objet Context est utilisé pour obtenir un enregistreur Lambda, qui est utilisé pour écrire un message aux CloudWatchLogs.

   ```
   def project_group_filter_handler(event, context):
       ...
   ```

1. Analysez le message de l’événement.

   ```
   event_subscription_message = json.loads(event['body'])
   ```

1. Obtenez l’attribut « newState » du message d’abonnement à l’événement.\
   L’attribut newState représente l’état mis à jour de la ressource.

   ```
   new_state = json.loads(event_subscription_message['newState'])
   ```

   Pour en savoir plus sur le format newState, voir [Format du message sortant pour les abonnements aux événements](../../wf-api/api/message-format-event-subs.md).

1. Après avoir analysé le mappage de l’attribut « newState » du message, assurez-vous que l’ID de groupe de l’objet correspond à l’ID de groupe que vous avez indiqué à l’étape 1.

1. (Le cas échéant) Si les ID ne correspondent pas, abandonnez le message afin qu’une réponse vide soit renvoyée.

   ```
   if new_state['groupID'] == DESIRED_GROUP_ID:
      # Process the message
      print('matched group ID')
      process_message(event_subscription_message)
   
   return {
   'statusCode': 200
   ```

   >[!NOTE]
   >
   >Il est essentiel de renvoyer une réponse de succès vide. Tout élément autre qu’une réponse 200 est considéré comme un échec de la diffusion.

1. Traitez le message.

   ```
   def process_message(event_subscription_message):
      aws_lambda.invoke(
         FunctionName='forwardMessageOntoMyEndpoint',
         InvocationType='Event',
         LogType='None',
         Payload=event_subscription_message
      )
   ```

   Le SDK AWS est utilisé pour appeler une autre fonction Lambda, chargée de diffuser le message filtré vers le point d’entrée souhaité.

   L’objectif de la transmission de la responsabilité de diffusion du message à une autre fonction Lambda est d’éviter un délai d’expiration de la demande de diffusion provenant du service d’abonnement à un événement. Actuellement, le délai d’expiration de la diffusion est défini sur cinq secondes. Si le filtre prend plus de temps que celui prévu par le paramètre, vous pouvez traiter la demande, mais le service d’abonnement à un événement expire et tombe dans une boucle de reprises jusqu’à ce qu’il reçoive une réponse 200 dans le délai d’expiration.


### Node.js

L’exemple Node.js de filtrage des ID de groupe de projet est similaire aux exemples Java et Python. Comme pour l’exemple Python, le premier paramètre est un événement proxy Lambda et le second est le contexte Lambda.

L’exemple suivant dans Node.js montre comment filtrer les payloads du projet en fonction de l’ID de groupe du projet, comme effectué dans [projectGroupFiltering.js:](https://github.com/Workfront/workfront-event-subscription-filter-examples/blob/master/lambda/js/projectGroupFiltering.js)

1. Définissez l’ID de groupe que vous recherchez et créez-le en tant que constante statique.

   ```
   const DESIRED_GROUP_ID = 'VaqTTVaB0UcbPu4n6824WIYYIV953Mg3';
   ```

   Le premier paramètre est l’« événement » du proxy Lambda, qui contient le message d’abonnement à l’événement et certaines informations supplémentaires qui doivent être analysées.\
   Le second paramètre est le contexte de la requête actuelle de proxy Lambda.\
   Dans cet exemple, l’objet Context est utilisé pour obtenir un enregistreur Lambda, qui est utilisé pour écrire un message aux CloudWatchLogs.

   ```
   exports.myProjectGroupFilterHandler = function (event, context) {
      ...
   }
   ```

2. Analysez le message de l’événement.

   ```
   let eventSubscriptionMessage = JSON.parse(event.body);
   ```

3. Récupérez l’attribut projectGroupID à partir de l’attribut « newState » du message d’abonnement à l’événement, puis faites-le correspondre à l’ID de groupe du groupe que vous avez identifié à l’étape 1.

   ```
   let projectGroupId = eventSubscriptionMessage.newState.groupID; 
   ```

   Pour en savoir plus sur le format newState, voir [Format du message sortant pour les abonnements aux événements](../../wf-api/api/message-format-event-subs.md).

4. (Le cas échéant) Si les ID ne correspondent pas, abandonnez le message afin qu’une réponse vide soit renvoyée.\
   L’exemple suivant présente les ID de groupe correspondants :

   ```
   if (projectGroupId === DESIRED_GROUP_ID) {
      // Process the message
      console.log('Processing Event Subscription message matching groupId ' + DESIRED_GROUP_ID + '...');
      forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context);
   } else {
      endLambdaRequest(context);
   }
   ```

   >[!NOTE]
   >
   >Il est essentiel de renvoyer une réponse de succès vide. Tout élément autre qu’une réponse 200 est considéré comme un échec de la diffusion.

5. Traitez le message.

   ```
   function forwardMessageOntoMyEndpoint(eventSubscriptionMessage, context) {
      let lambdaParams = {
         FunctionName: 'forwardMessageOntoMyEndpoint',
         InvocationType: 'Event',
         LogType: 'None',
         Payload: new Buffer(JSON.stringify(eventSubscriptionMessage))
      };
   
      lambda.invoke(lambdaParams, function (err, data) {
         if (err) {
            console.error(err, err.stack);
         } else {
            console.log('data = ' + data);
         }
         endLambdaRequest(context);
      });
   }
   ```

   Le SDK AWS est utilisé pour appeler une autre fonction Lambda, chargée de diffuser le message filtré vers le point d’entrée souhaité.\
   L’objectif de la transmission de la responsabilité de diffusion du message à une autre fonction Lambda est d’éviter un délai d’expiration de la demande de diffusion provenant du service d’abonnement à un événement. Actuellement, le délai d’expiration de la diffusion est défini sur cinq secondes. Si le filtre prend plus de temps que celui prévu par le paramètre, vous pouvez traiter la demande, mais le service d’abonnement à un événement expire et tombe dans une boucle de reprises jusqu’à ce qu’il reçoive une réponse 200 dans le délai d’expiration.\
   Pour en savoir plus sur la gestion de la diffusion des messages, voir [Amélioration de la diffusion des messages tout en tenant compte des dépassements de délai](#improving-message-delivery-while-accommodating-timeouts).

## Amélioration de la diffusion des messages tout en tenant compte des dépassements de délai

Le service d’abonnement à un événement a un délai d’expiration strict de **cinq secondes** pour toutes les demandes de diffusion. Dans le cas où la diffusion d’un message dépasse le temps autorisé, le service d’abonnement à un événement lance un cycle de reprise pour ce message.

Par exemple, vous créez un filtre d’ID de groupe de projet similaire à l’un des exemples trouvés dans la section [Filtrage des messages d’événement](#filtering-event-messages) et vous incluez une recherche de base de données pour déterminer si le message est nécessaire. Il est possible que la recherche dans la base de données, ainsi que le temps nécessaire au traitement requis et au démarrage à froid de Lambda, puisse prendre plus de cinq secondes, ce qui provoquerait une nouvelle tentative de remise du message par le service d’abonnement à un événement.

Vous pouvez éviter une nouvelle tentative en séparant les parties chronophages du processus de la logique responsable de déterminer si le message est un message que vous souhaitez traiter et diffuser. Ce faisant, vous pouvez accepter le message et renvoyer une réponse de niveau 200 au service d’abonnement à l’événement, tout en continuant de manière asynchrone à traiter ou filtrer le message en arrière-plan (voir l’étape 5 dans [Java](#java) par exemple).


Même si le traitement ou le filtrage ne dépasse pas le délai de cinq secondes, il est toujours avantageux de séparer le premier point de contact du filtrage ou du traitement des messages des autres étapes de traitement ou de diffusion côté client. Ainsi, la remise du message à la destination à partir du service d’abonnement à un événement a un impact minimal sur le temps et les performances pour les deux parties.

Pour en savoir plus sur le mécanisme de reprise, voir [Reprises d’abonnement à un événement](../../wf-api/api/event-sub-retries.md).

## Mise en oeuvre de filtres hébergés dans l’architecture sans cloud

Si vous ne parvenez pas à utiliser une architecture cloud pour le filtrage des abonnements aux événements, vous pouvez toujours utiliser les exemples de la section [Filtrage des messages d’événement](#filtering-event-messages) comme feuilles de route de la mise en œuvre de vos propres filtres hébergés ou composants de traitement.

### Ajustement d’exemples de filtrage pour les services autonomes

Avant d&#39;utiliser les exemples de filtrage dans un environnement sans cloud, procédez comme suit :

* Omettez les éléments spécifiques à Lambda des exemples, tels que le paramètre Contexte.

* Remplacez les appels d’autres Lambdas dans les exemples par des requêtes HTTP asynchrones supplémentaires envoyées à d’autres filtres ou composants de traitement que vous hébergez.

* Si vous vous référez aux exemples Python et Node.js, remplacez le premier paramètre d’événement par le premier paramètre de payload affiché dans l’exemple Java. Voir Étape 1 dans [Java](#java).

* Déployez les filtres ou les processeurs avec une API web.

### Prévention des messages d’abonnement aux événements manqués

Dans une architecture sans cloud, les services chargés de recevoir les messages d’abonnement aux événements peuvent parfois être inatteignables. Dans ce cas, les messages peuvent dépasser la limite de reprise et être perdus, sans moyen de récupérer les informations dans les messages.

Nous vous recommandons d’implémenter, au démarrage de votre service, une requête demandant l’état le plus récent de toutes les ressources qui peuvent avoir été incluses dans les messages manqués. Comme illustré dans l’exemple suivant, vous pouvez utiliser les critères de filtre pour rechercher les ressources qui correspondent à ces critères, puis traiter leur état actuel.

```
public static List<Map<String, Object>> projectGroupFilteringStartupRecoveryQuery(LambdaLogger logger) {
    HttpClient httpClient = HttpClientBuilder.create().build();

    // Produces a URL of https://<my-domain>.workfront.com/attask/api/v15.0/PROJ/search?groupID=<DESIRED_GROUP_ID>
    replacing <...> with the appropriate values
    URI projectGroupQueryUri = generateProjectRecoveryQueryURI(logger);

    HttpUriRequest projectGroupIdGetRequest = new HttpGet(projectGroupQueryUri);

    // Our preferred method of authentication 
    projectGroupIdGetRequest.addHeader("apiKey", WORKFRONT_API_KEY);
 
    List<Map<String, Object>> projects = null;
    try 
    {
        HttpResponse response = httpClient.execute(projectGroupIdGetRequest);
        InputStream responseBodyStream = response.getEntity().getContent();
        Reader reader = new InputStreamReader(responseBodyStream);
        Type listType = new TypeToken<List<Map<String, Object>>>(){}.getType();
        projects = new GsonBuilder().create().fromJson(reader, listType);
      } catch (IOException e) {
        logger.log("An IOException was thrown while executing a request to Workfront for projects matching the group ID " + DESIRED_GROUP_ID);
    }
    return projects;
}
```

En demandant des ressources, vous vous assurez que vos systèmes d’intégration disposent de la version la plus récente des ressources.

### Mise en œuvre d’un traitement asynchrone dans la diffusion de messages

Tous les exemples de la section [Filtrage des messages d’événement](#filtering-event-messages) transfère la responsabilité de diffuser des messages filtrés à un autre AWS Lambda. Cela permet d’éviter de dépasser le délai d’expiration de cinq secondes dans la demande de diffusion, qui est appliquée par le service d’abonnement à un événement qui émet la demande.

Dans une architecture sans cloud, vous devrez peut-être mettre en œuvre un mécanisme de traitement asynchrone similaire à la manière dont le SDK AWS permet des appels asynchrones à d’autres AWS Lambdas. La plupart des langages de programmation modernes disposent de bibliothèques tierces ou principales qui gèrent le traitement asynchrone, ce qui vous permet d’exploiter le style asynchrone de traitement mise en œuvre dans nos exemples.
