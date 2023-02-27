---
content-type: api
navigation-topic: general-api
title: Bases d’API
description: Bases d’API
author: Becky
feature: Workfront API
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '4405'
ht-degree: 0%

---


# Bases d’API

L’objectif de l’API Adobe Workfront est de simplifier la création d’intégrations avec Workfront en introduisant une architecture REST-ful qui fonctionne sur HTTP. Ce document suppose que vous connaissez les réponses REST et JSON et décrit l’approche adoptée par l’API Workfront.

Une familiarité avec le schéma Workfront vous aidera à comprendre les relations de base de données qui peuvent être utilisées pour extraire des données de Workfront à des fins d’intégration.

## Limites et directives

Pour garantir des performances système à la demande constantes de Workfront, chaque client est limité à 10 threads API simultanés. L’environnement Sandbox a la même limite en place, ce qui permet aux clients et aux partenaires de tester précisément les appels d’API avant de publier du code en production.

Pour les environnements de production, de prévisualisation et de test, les requêtes des utilisateurs finaux ont une longueur URI maximale de 8 892 octets, car elles sont acheminées via le réseau de diffusion de contenu Workfront (Akamai). Cette limite s’applique uniquement aux URI qui sont acheminés par le réseau CDN.

>[!NOTE]
>
>cette limite ne s’applique pas aux environnements de test, car les environnements de test ne sont pas acheminés par le réseau de diffusion de contenu.

### Clause de non-responsabilité

Toute utilisation de l’API doit être testée dans l’environnement bêta de Workfront avant d’être exécutée dans l’environnement de production. Si un client utilise l’API pour un processus que Workfront considère raisonnablement comme pesant sur le logiciel à la demande (c’est-à-dire que le processus a un effet matériellement négatif sur les performances du logiciel pour les autres clients), Workfront se réserve le droit de demander au client d’interrompre ce processus. Si le client ne se conforme pas et que le problème persiste, Workfront se réserve le droit de mettre fin au processus.

## Notions de base de REST

Cette section présente de manière générale comment interagir avec l’API REST Workfront pour les principes REST suivants :

### URI de l’objet

Chaque objet du système reçoit un URI unique composé du type d’objet et de l’identifiant. Les exemples suivants présentent des URI décrivant trois objets uniques :

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

Le type d’objet n’est pas sensible à la casse et peut être l’ObjCode abrégé (comme proj) ou l’autre nom d’objet (projet).

Pour obtenir une liste des codes ObjCodes valides, voir  [Explorateur d’API](../../wf-api/general/api-explorer.md).

### Opérations

Les objets sont manipulés en envoyant une requête HTTP à leur URI unique. L’opération à effectuer est spécifiée par la méthode HTTP.

Les méthodes HTTP standard correspondent aux opérations suivantes :

* **GET** - Récupère un objet par identifiant, recherche tous les objets par une requête, exécute des rapports ou exécute des requêtes nommées
* **POST** - Insère un nouvel objet
* **PUT** - Modification d’un objet existant
* **DELETE** - Supprime un objet

Pour contourner les défaillances du client ou les limites de longueur du protocole, le paramètre de méthode peut être utilisé pour remplacer le comportement HTTP. Par exemple, une opération de GET peut être implémentée en publiant l’URI suivant :
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### réponse

Chaque requête reçoit une réponse au format JSON. La réponse comporte un attribut data si la requête a réussi ou un attribut error en cas de problème. Par exemple, la requête

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

renvoie une réponse JSON similaire à ce qui suit :


<pre>{<br>    "data": [<br>        {<br>            "percentComplete" : 0,<br>            "status": "CUR",<br>            "priority": 2,<br>            "name": "Brand New Project",<br>            "ID" : "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Lors de l’exécution d’une requête de GET via la barre d’adresse de votre navigateur, il n’est pas nécessaire d’inclure l’ID de session dans la requête.

Une sécurité spéciale a été ajoutée pour les demandes de PUT, de POST et de DELETE. Toute requête qui entraîne l’écriture ou la suppression dans la base de données ne peut être exécutée que si la variable **sessionID=abc123** est inclus dans l’URI. Les exemples suivants illustrent la recherche d’une requête de DELETE :
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### Authentification

L’API authentifie chaque requête pour s’assurer que le client a accès à l’affichage ou à la modification d’un objet demandé.

L’authentification est effectuée en transmettant un ID de session qui peut être donné à l’aide de l’une des méthodes suivantes :

#### Authentification de l’en-tête de requête

La méthode d’authentification privilégiée consiste à transmettre un en-tête de requête nommé SessionID contenant le jeton de session. Cela a l’avantage d’être en sécurité contre [Cross-site Request Forgery (CSRF)](http://en.wikipedia.org/wiki/Cross-site_request_forgery) n’interfère pas avec l’URI à des fins de mise en cache.

Voici un exemple d’en-tête de requête :

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Authentification du paramètre de requête

Vous pouvez vous authentifier en transmettant un paramètre de requête nommé sessionID, comme illustré dans l’exemple suivant : 

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0?sessionID=abc1234
```

#### Authentification basée sur les cookies

L’API utilise la même authentification basée sur les cookies que celle utilisée par l’interface utilisateur web pour le système. Lorsqu’un client se connecte à Workfront à l’aide de l’interface utilisateur web, les appels AJAX effectués à partir du même navigateur utilisent la même authentification.

>[!NOTE]
>
>Afin de se protéger contre la possibilité d’attaques CSRF (Cross Site Request Forgery, Falsification de requête inter-sites), cette méthode d’authentification est uniquement disponible pour les opérations en lecture seule.

## Connexion

>[!IMPORTANT]
Workfront ne recommande plus l’utilisation de la variable `/login` point d’entrée ou clés d’API. Utilisez plutôt l’une des méthodes d’authentification suivantes :
* Authentification du serveur avec JWT
* Authentification de l’utilisateur avec OAuth2
>
Pour obtenir des instructions sur la configuration de ces méthodes d’authentification, voir [Création d’applications OAuth2 pour les intégrations Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md)
Pour plus d’informations sur l’utilisation de l’authentification du serveur dans Workfront, voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux JWT](../../wf-api/api/oauth-app-jwt-flow.md)
Pour plus d’informations sur l’utilisation de l’authentification des utilisateurs dans Workfront, voir [Configuration et utilisation des applications OAuth 2 personnalisées de votre entreprise à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md)

>[!NOTE]
La procédure décrite dans cette section s’applique uniquement aux organisations qui n’ont pas encore été intégrées à Adobe Business Platform. La connexion à Workfront par le biais de l’API Workfront n’est pas disponible si votre organisation a été intégrée à Adobe Business Platform.
Pour obtenir une liste des procédures différentes selon que votre organisation a été intégrée à Adobe Business Platform, voir [Différences d’administration basées sur les plateformes (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

En utilisant un nom d’utilisateur et un mot de passe valides, vous pouvez utiliser la requête suivante pour obtenir un ID de session :

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Cela définit un cookie pour authentifier les futures requêtes et renvoyer une réponse JSON avec le nouvel ID de session, l’ID utilisateur de l’utilisateur connecté et d’autres attributs de session.

>[!NOTE]
Si vous disposez d’un utilisateur désigné de l’API, également administrateur, Workfront vous recommande vivement d’utiliser une clé API pour vous connecter.

**Génération d’une clé API**

Vous pouvez générer une clé API lorsque vous vous connectez au système en tant que cet utilisateur, comme illustré dans l’exemple suivant :


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Récupération d’une clé API générée précédemment**

Vous pouvez également récupérer une clé API qui a été générée précédemment pour un utilisateur particulier en exécutant getApiKey :


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Vous pouvez ensuite utiliser ce résultat pour authentifier tout appel API en ajoutant &quot;apiKey&quot; comme paramètre de requête avec cette valeur au lieu d’un ID de session ou d’un nom d’utilisateur et d’un mot de passe. Cela est bénéfique du point de vue de la sécurité.

La requête suivante est un exemple de récupération de données d’un projet à l’aide de l’apiKey :

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Invalidation d’une clé API**

Si la valeur apiKey a été compromise, vous pouvez exécuter &quot;clearApiKey&quot; qui invalide la clé API actuelle, comme illustré dans l’exemple suivant :

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Une fois effacé, vous pouvez exécuter à nouveau getApiKey pour générer une nouvelle clé API.

### Déconnexion

Une fois la session terminée, vous pouvez utiliser la requête suivante pour déconnecter l’utilisateur, ce qui empêche tout accès ultérieur à l’aide de l’ID de session.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

L’ID de session à déconnecter peut être spécifié sous la forme d’un cookie, d’un en-tête de requête ou d’un paramètre de requête.

Pour déconnecter un utilisateur :

1. Accédez à l’écran de connexion, mais ne vous connectez pas.
1. Remplacez l’URL par /attask/api/v15.0/project/search.\
   Notez que la page est introuvable.
1. Remplacer le mot *search* avec login?username=admin&amp;password=user, en substituant votre nom d’utilisateur et votre mot de passe pour *admin* et *user\
   *Cette session est stockée dans le navigateur sous forme de cookie et n’a pas besoin d’être redémarrée dans chaque demande de GET suivante.

1. Remplacez l’URL par **/attask/api/v15.0/project/search**.
1. Notez la réponse fournie.

Vous devez toujours inclure l’ID de session fourni après connexion lors de l’exécution de requêtes de PUT, de POST et de DELETE.

## Comportement des GET

Utilisez la méthode de GET HTTP pour récupérer un ou plusieurs objets et exécuter des rapports.

### Récupération d’objets

Vous pouvez améliorer la recherche d’objets à l’aide de modificateurs et de filtres.

#### Récupération d’un objet à l’aide de l’ID d’objet

Si vous connaissez l’identifiant d’un objet, vous pouvez le récupérer en accédant à son URI unique. Par exemple, la requête

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

renvoie une réponse similaire à celle-ci :

<pre>{<br>    "percentComplete" : 0,<br>    "status": "CUR",<br>    "priority": 2,<br>    "name": "Brand New Project",<br>    "ID" : "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


Vous pouvez récupérer plusieurs objets dans la même requête en spécifiant le paramètre de requête d’identifiant et en fournissant une liste d’identifiants séparés par des virgules, comme illustré dans l’exemple suivant :


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

Notez que la requête /attask/api/v15.0/project?id=... est identique à la requête `/attask/api/v15.0/project/...` requête.

#### Récupération d’un objet à l’aide de l’URI

Si vous souhaitez récupérer un objet selon des critères autres que l’ID, vous pouvez rechercher l’URI.

Par exemple, vous pouvez utiliser la requête suivante pour renvoyer une liste de tous les projets du système :

```
GET /attask/api/v15.0/project/search
```

Vous pouvez spécifier des filtres à l’aide des paramètres de requête en tant que paires nom-valeur. Par exemple, l’exemple suivant illustre une requête qui recherche tous les projets en cours :

```
GET /attask/api/v15.0/project/search?status=CUR
```

La requête suivante recherche toutes les tâches qui ne sont pas encore terminées et qui sont affectées à un utilisateur nommé John.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Utilisation des modificateurs de recherche

Le tableau suivant répertorie certains des modificateurs que vous pouvez utiliser avec l’API Workfront.

| **Modificateur** | **Description** | **Exemple** |
|---|---|---|
| eq | renvoie les résultats qui se trouvent dans l’état &quot;fermé&quot; | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | renvoie les résultats qui ne sont pas à l’état fermé | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | renvoie des résultats dont le pourcentage est supérieur ou égal à 50. | <pre>...percentComplete=50&amp;percentComplete_Mod=gte...</pre> |
| lte | renvoie des résultats dont le pourcentage est inférieur ou égal à 50 ; | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | renvoie des résultats pour lesquels la description est nulle. | <pre>...description_Mod=isnull...</pre> |
| notnull | renvoie des résultats pour lesquels la description n’est pas nulle. | <pre>...description_Mod=notnull...</pre> |
| contient | renvoie des résultats pour lesquels le nom contient &quot;Workfront&quot;. | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| entre | renvoie les résultats dont la date d’entrée est comprise dans les 7 derniers jours. | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=entre...</pre> |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
Les requêtes de recherche sont sensibles à la casse. Si une erreur s’affiche, assurez-vous que  **_Mod** et **_Plage** possèdent la bonne casse.

#### Utilisation d’instructions OU

Vous pouvez améliorer une recherche en ajoutant un paramètre qui inclut &quot;OR&quot; ainsi qu’un nombre pour indiquer le niveau d’un filtre ou d’une série de filtres.

Une instruction OU renvoie uniquement les enregistrements de l’appel API qui répondent aux critères de filtrage de l’instruction OU. Les filtres ne sont pas implicites entre les niveaux d’instruction OU.

Par exemple, si vous souhaitez filtrer pour

* Tâches dont le nom contient &quot;Planning&quot; OU
* Tâches dans un portfolio nommé &quot;FixedAssets&quot; ET affectées à une personne dont le nom contient &quot;Steve&quot; OU
* Tâches dont la tâche parent est nommée &quot;Tâche finale&quot;

Utilisez ensuite l’appel API suivant avec ses instructions OU multiples :
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_Mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_Mod=contains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### Utilisation des paramètres de filtre

L’utilisation des paramètres d’URL pour les filtres de recherche peut entraîner un échec : Workfront analyse certains paramètres avant de rechercher différentes méthodes d’authentification (nom d’utilisateur, mot de passe, apiKey, cookie). Dans ce cas, les paramètres ne sont pas utilisés comme filtres dans l’appel . 

Pour éviter ce problème, vous pouvez placer ces valeurs dans les paramètres de filtre avec la mise en forme JSON. Par exemple, si vous souhaitez filtrer par nom d’utilisateur testuser, au lieu d’utiliser 
<pre>/atask/api/v15.0/user/search?username=testuser@workfront.com</pre>transmettez le paramètre d’URL dans un filtre, comme illustré dans l’exemple suivant :
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### Utilisation du paramètre de requête de mappage

Par défaut, les données renvoyées par une recherche sont un tableau JSON. Selon votre cas d’utilisation, il peut être plus efficace d’obtenir le résultat sous la forme d’un objet JSON indexé par l’identifiant. Pour ce faire, utilisez le paramètre de requête de carte . Par exemple, la requête 
<pre>/attask/api/v15.0/task/search?map=true</pre>renvoie une réponse indexée par un identifiant similaire à ce qui suit :
<pre>{<br>    "data": {<br>        "4c9a97db0000000f13ee446b9aead9b" : {<br>            "percentComplete" : 0,<br>            "status": "NEW",<br>            "name": "première tâche",<br>            "ID" : "4c9a97db0000000f13ee446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601" : {<br>            "percentComplete" : 0,<br>            "status": "INP:A",<br>            "name": "deuxième tâche",<br>            "ID" : "4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### Utilisation du paramètre de requête Fields

Par défaut, la récupération d’un objet renvoie uniquement le sous-ensemble de champs le plus couramment utilisé.

Vous pouvez utiliser le paramètre de requête fields pour spécifier qu&#39;une liste de champs spécifiques séparés par des virgules est renvoyée. Par exemple, la requête
<pre>/attask/api/v15.0/task/search?fields=scheduledStartDate,priority</pre>renvoie une réponse similaire à celle-ci :
<pre>{<br>    "priority": 2,<br>    "name": "première tâche",<br>    "ID" : "4c7c08fa0000002ff924e298ee148df4",<br>    "scheduledStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
Ces noms de champ sont sensibles à la casse.

Pour obtenir la liste des références de champ possibles, reportez-vous à la section  [Explorateur d’API](../../wf-api/general/api-explorer.md)

#### Recherche d’objets imbriqués

Vous pouvez rechercher des objets imbriqués. Par défaut, les objets imbriqués sont renvoyés avec uniquement le nom et l’identifiant. Par exemple, pour obtenir tous les problèmes avec leurs propriétaires, utilisez la requête suivante :
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>Si davantage d’informations sont requises, vous pouvez demander un champ imbriqué à l’aide de la syntaxe deux-points. Par exemple, la requête suivante recherche tous les problèmes, ainsi que le nom, l’identifiant, le titre et le numéro de téléphone du propriétaire.
<pre>/atask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>et renvoie les éléments suivants : 
<pre>{<br>    "name": " une question importante ",<br>    "ID" : "4c78285f00000908ea8cfd66e084939f",<br>    "owner": {<br>        "title" : " spécialiste des opérations ",<br>        "phoneNumber": "555-1234",<br>        "name": "Utilisateur administrateur",<br>        "ID" : "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### Récupération des collections imbriquées

Vous pouvez récupérer des collections d’objets imbriquées. Par exemple, pour obtenir un projet avec toutes ses tâches, utilisez la requête suivante :
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>La requête suivante récupère des affectations de tâche :
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### Recherche de plusieurs champs imbriqués

Par défaut, seul le nom et l’identifiant de chaque tâche sont renvoyés, mais des champs imbriqués supplémentaires peuvent être spécifiés avec la syntaxe des deux-points. Pour afficher tous les champs disponibles pour un objet ou une collection associé, il vous suffit d’ajouter deux points et un astérisque à la référence d’objet ou de collection.
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### Récupération de données personnalisées

Vous pouvez récupérer des champs de données personnalisés à l’aide du préfixe &quot;DE:&quot;. Par exemple, pour demander un projet avec un paramètre appelé &quot;CustomText&quot;, utilisez la requête suivante :
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>qui renverra
<pre>{<br>    "name": "projet de données personnalisé",<br>    "ID" : "4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText" : "task b" <br>}</pre>Vous pouvez également récupérer toutes les données personnalisées d’un objet en demandant le champ parameterValues . Par exemple, 
<pre>/atask/api/v15.0/project/search?fields=parameterValues</pre>renvoie des données similaires aux suivantes :
<pre>{<br>    "name": "projet de données personnalisé",<br>    "ID" : "4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues : { <br>        "DE:CustomText" : "task b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes" : ["first", "second", "third"] <br>    } <br>}</pre>

#### Utilisation de requêtes nommées

Certains types d’objets possèdent des recherches nommées qui sont généralement exécutées et qui sont disponibles en ajoutant le nom de la requête à la fin de l’URI de type d’objet. Par exemple, la requête suivante récupère les tâches (tâches et problèmes) auxquelles l’utilisateur est actuellement affecté :
<pre>/attask/api/v15.0/work/myWork</pre>Les requêtes nommées prennent en charge la demande du paramètre de champs pour récupérer des champs supplémentaires. Certaines requêtes nommées acceptent également des filtres supplémentaires. Pour obtenir la liste des requêtes nommées autorisées pour un objet, voir l’onglet Action pour l’objet dans l’[Explorateur API](../../wf-api/general/api-explorer.md).

#### Utilisation du filtre de comptage

Vous pouvez spécifier le nombre de résultats qu’une recherche donnée doit renvoyer. Cela permet au serveur de traiter la demande plus rapidement et d’économiser de la bande passante. Par exemple, la requête
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>renvoie le nombre de résultats au format suivant :
<pre>{<br>    "count": 3 <br>}</pre>Le résultat est un téléchargement beaucoup plus petit que si les objets complets sont envoyés. La syntaxe du filtre est identique à la commande de recherche.

### Demande d’un rapport

Vous pouvez effectuer une requête de rapport, dans laquelle seul l’agrégat d’un champ est souhaité avec un ou plusieurs regroupements. Comme illustré dans l&#39;exemple suivant, la syntaxe du rapport est la même que celle de l&#39;API SOAP :
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>qui renvoie le résultat suivant
<pre>{<br>    "Premier projet" : { <br>        "sum_hours": 15 <br>    }, <br>     "Second Project" : { <br>        "sum_hours": 30 <br>    } <br>}</pre>L'ajout du paramètre $$ROLLUP=true inclut un total à chaque niveau de groupement :
<pre>{<br>    "Premier projet" : { <br>        "sum_hours": 15 <br>    }, <br>    "Second Project" : { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP" : { <br>        "sum_hours": 45 <br>    } <br>}</pre>

### Tri des résultats des requêtes dans l’API

Vous pouvez trier vos résultats selon n’importe quel champ si vous ajoutez les éléments suivants à votre appel API :

&amp;entryDate_Sort=asc

Par exemple, si vous souhaitez trier par date de début planifiée de la tâche, supprimez entryDate et remplacez-le par scheduledCompletionDate.

Cela fonctionne pour la plupart des champs de Workfront.

### Prise en compte des limites de requête

Lors de l’interrogation d’un objet, une attention particulière doit être accordée à la relation entre les objets associés et les limitations de recherche. Par exemple, comme le montre le tableau suivant, une requête pour des projets ne peut pas renvoyer plus de 2 000 projets. Ces 2 000 projets sont considérés comme des &quot;Principaux objets&quot;. Si vous recherchez le champ Tâches sur les projets, le champ Tâches, qui est une collection, devient un objet secondaire du projet Principal objet. Une requête pour le champ Tâches peut inclure des milliers de tâches sur les projets. Au total, le nombre combiné d’objets (projets et tâches) renvoyés ne peut pas dépasser 50 000 au maximum.

Pour garantir des performances optimales, le tableau suivant répertorie les limites imposées aux requêtes de recherche. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Résultat de la requête</th> 
   <th>Limitation</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">Nombre de résultats par défaut</td> 
   <td>100</td> 
   <td> Si aucune limite n’est spécifiée dans le filtre de requête (c’est-à-dire $$LIMIT), le résultat ne peut pas contenir plus de 100 objets Principaux. <br>Voir <a href="#using-paginated-responses" class="MCXref xref">Utilisation de réponses paginées</a> pour obtenir des instructions sur la façon de contourner cette limitation. </td> 
  </tr> 
  <tr> 
   <td>Nombre max. de résultats</td> 
   <td>2,000</td> 
   <td>Le filtre de requête (c’est-à-dire $$LIMIT) ne peut pas renvoyer plus de 2 000 résultats. Pour plus d’informations, voir "Réponses paginées" .</td> 
  </tr> 
  <tr> 
   <td>Profondeur max. de champ</td> 
   <td>4</td> 
   <td>Lors de l’identification des champs que vous souhaitez afficher, vous ne pouvez pas éloigner de plus de quatre niveaux de l’objet interrogé.</td> 
  </tr> 
  <tr> 
   <td>Nombre max. d’objets</td> 
   <td>50,000</td> 
   <td>Le jeu de résultats ne peut pas contenir 50 000 objets Principal et secondaire.</td> 
  </tr> 
  <tr> 
   <td>Nombre max. de champs</td> 
   <td nowrap>1,000,000</td> 
   <td>Lorsque le jeu de résultats contient moins de 5 000 objets, les résultats peuvent inclure au plus 1 000 000 champs.</td> 
  </tr> 
  <tr> 
   <td>Nombre max. de créations/mises à jour par lots</td> 
   <td>100</td> 
   <td>La limite maximale de création ou de mise à jour de lot est de 100.</td> 
  </tr> 
 </tbody> 
</table>

### Utilisation de réponses paginées {#using-paginated-responses}

Pour contourner la limitation de requête Nombre de résultats par défaut et autoriser 200 résultats, vous pouvez inclure le filtre $$LIMIT=200 dans votre requête, comme illustré dans l’exemple suivant :
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>Afin d’assurer la fiabilité et les performances des autres clients du système, la limite de résultats maximale autorisée par requête est de 2 000 objets. Toute tentative de spécification d’une limite plus grande entraînera un message d’erreur IllegalArgumentException . 

Par conséquent, nous vous recommandons d’utiliser des réponses paginées pour les jeux de données volumineux. Pour spécifier le premier résultat à renvoyer, ajoutez le filtre $$FIRST . Par exemple, la requête suivante renvoie les résultats 201 à 250 pour une requête :
<pre>GET /attask/api/v15.0/project/search?$$FIRST=201&amp;$$LIMIT=50</pre>

### Création d’une règle d’accès

Vous pouvez créer une règle d’accès pour déterminer qui peut accéder à un objet. Vous trouverez ci-dessous des exemples de règles d’accès que vous pouvez définir :

Pour définir un projet afin qu’il soit partagé uniquement avec un utilisateur avec l’ID &quot;abc123&quot;, utilisez la requête suivante :
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updated={ accessRules: [ {accessID: 'abc123', accesseurObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>Vous pouvez également effectuer un partage uniquement avec une nouvelle personne et conserver les autorisations existantes intactes :
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>Pour récupérer les règles d’accès existantes :
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## Comportement des POST

POST insère un nouvel objet. La syntaxe est identique à celle du PUT, à quelques exceptions près. Comme le nouvel objet n’existe pas encore, il n’a pas d’identifiant. Pour cette raison, l’URI n’inclut pas l’identifiant.

### Création d’un objet

Voici un exemple de demande de création d’un projet :
<pre>POST /attask/api/v15.0/project?name=New Project</pre>La réponse inclut le projet nouvellement créé, ainsi que son nouvel identifiant et tous les autres champs spécifiés.

### Copie d’un objet

Certains objets prennent en charge la copie. Pour ces types d’objets, il est possible de créer de nouveaux objets en les publiant avec un paramètre copySourceID . Par exemple, la requête suivante copie le projet donné et lui donne un nouveau nom :

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Téléchargement de documents

Vous pouvez télécharger des documents à l’aide de l’URL d’API suivante :
<pre>POST /attask/api/v15.0/upload</pre>L’API exige que le type de contenu soit multipart/form-data. Le nom du paramètre du fichier doit être uploadedFile. Le serveur renvoie les données JSON suivantes :
<pre>{<br>    "handle" : "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>Vous pouvez utiliser la poignée et la publication sur l’URL suivante lors de la création d’un document Workfront :
<pre>POST /attask/api/v15.0/document?update={<br>    name: aFileName,<br>    handle : abc...123, (gérer à partir du téléchargement du fichier)<br>    docObjCode : PROJ (ou TÂCHE, OPTASK, etc.)<br>    objID : abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## Comportement des PUT

PUT est utilisé pour mettre à jour un objet existant.

La réponse d’un PUT est identique à celle d’un GET. Dans les deux cas, le serveur renvoie le nouvel état de l’objet après la mise à jour. Toutes les règles utilisées pour modifier une réponse à une demande de GET fonctionnent également avec PUT, comme la spécification de champs supplémentaires à renvoyer, de données personnalisées, etc.

### Modification d’objets

Les mises à jour des objets sont toujours effectuées par l’identifiant à l’aide de l’URI unique de l’objet. Les champs à mettre à jour sont spécifiés en tant que paramètres de requête. Par exemple, pour modifier le nom d’un projet, vous pouvez envoyer une requête semblable à ce qui suit :
<pre>PUT /attask/api/v15.0/project/4c7...?name=New Project Name <br>PUT /attask/api/v15.0/project?id=4c7..&amp;name=New Project Name</pre>Comme la mise à jour nécessite un identifiant, cette opération échoue (sans insertion) si l’objet n’existe pas sur le serveur.

### Spécification des modifications JSON

Comme illustré dans l’exemple suivant, vous pouvez utiliser le paramètre de requête de mise à jour pour spécifier les champs à mettre à jour à l’aide de la syntaxe JSON :
<pre>PUT /attask/api/v15.0/project/4c7...?update= <br>{<br>     name: "Nouveau nom du projet", <br>     status : "CUR", <br>     ... <br>}</pre>

### Mise à jour imbriquées

Certains objets possèdent des collections privées qui peuvent être mises à jour. Par exemple, l’exemple suivant montre comment remplacer les affectations existantes pour une tâche donnée :
<pre>PUT /attask/api/v15.0/task/4c7...?update= <br>{<br>    assignments : [ <br>        { <br>            assignedToID: "2222...54d0, <br>            assignmentPercent : 50,0 <br>        },{ <br>            roleID : "1111...54d0"<br>        } <br>    ] <br>}</pre>

>[!NOTE]
Bien que les mises à jour apportées au niveau supérieur soient peu nombreuses, les mises à jour apportées à une collection ou à un objet imbriqué remplacent complètement la collection existante. Pour modifier une affectation unique sur une tâche sans affecter les objets, utilisez PUT sur l’affectation plutôt que sur la tâche.

L’exemple suivant fait d’un projet une file d’attente de service d’assistance publique. Notez que les propriétés de la file d’attente existante sont remplacées.
<pre>PUT /attask/api/v15.0/project/4c7...?update= <br>{ <br>    queueDef : { <br>        isPublic : 1 <br>    } <br>}</pre>

### Utilisation du paramètre de requête d’action

Certains objets prennent en charge des actions supplémentaires pouvant être effectuées en plus des modifications simples. Vous pouvez spécifier ces actions à l’aide du paramètre de requête d’action . Par exemple, la requête suivante recalcule la chronologie d’un projet donné :
<pre>PUT /attask/api/v15.0/project/4c7...?action=calculateTimeline<br><br>ou<br><br>PUT /attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### Déplacement d’objets

L’exemple suivant illustre la syntaxe du déplacement d’une tâche d’un projet à un autre :
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>Voici un exemple pour chaque type d’action : (??)
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/rappelApproval<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>Seule l’action de déplacement nécessite l’identification d’attributs supplémentaires pour spécifier le projet dans lequel l’élément de travail doit être déplacé.

Voici un exemple de chaque type d’action : 
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updated={accessRules:[{accessorID: 'abc123', accesseurObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Partage d’objets

L’exemple suivant illustre la syntaxe du partage d’un projet avec une équipe :
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>Lors de la modification d’un objet, vous pouvez remplacer toutes les règles d’accès d’un objet en effectuant un PUT et en envoyant des mises à jour similaires à l’exemple suivant :
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updated={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction :'VIEW'}]}</pre>L’exemple suivant illustre la syntaxe du déplacement d’une tâche d’un projet à un autre :
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## Comportement des DELETE

DELETE supprime un objet. Dans tous les cas, l’URI peut inclure le paramètre force=true pour que le serveur supprime les données spécifiées et ses dépendances. Dans l’exemple suivant, une tâche est supprimée en exécutant la méthode de DELETE HTTP sur un URI :
<pre>DELETE /attask/api/v15.0/task/4c78821c000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c000d6fa8d5e52f07a1d54d0?force=true</pre>

## Mises à jour en bloc

Une instruction de mise à jour en bloc met à jour plusieurs objets en même temps au sein d’un seul appel API. Un appel d’API de création en bloc est créé de la même manière qu’un appel de mise à jour normal, comme illustré dans les exemples suivants :
<pre>PUT /attask/api/v15.0/proj?update=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>qui génère un retour similaire à ce qui suit :
<pre>data: [{<br>    ID : "53ff8d3d003b438b57a8a784df38f6b3",<br>    name: "Test_Project_1",<br>    objCode : "PROJ",<br>    percentComplete : 0,<br>    scheduleCompletionDate : "2014-08-28T11:00:00:000-0400",<br>    scheduledStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority : 0,<br>    forecastCompletionDate : "2014-08-28T16:12:00:000-0400",<br>    status : "CUR"<br>},<br>{<br>    ID : "53ff8d49003b43a2562aa34eea3b6b10",<br>    name: "Test_Project_2",<br>    objCode : "PROJ",<br>    percentComplete : 0usi,<br>    scheduleCompletionDate : "2014-08-28T11:00:00:000-0400",<br>    scheduledStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority : 0,<br>    forecastCompletionDate : "2014-08-28T16:12:00:000-0400",<br>    status : "CUR"<br>}]</pre>Vous pouvez également effectuer une mise à jour en bloc semblable à ce qui suit :
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;update=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxx"xxxx", name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>qui génère un retour similaire à ce qui suit :
<pre>data: [ {<br>     ID : "53ff8e15003b461d4560f7f65a440078",<br>     name: "Test_Project_1_Edit",<br>     objCode : "PROJ",<br>     percentComplete : 0,<br>     scheduleCompletionDate : "2014-08-28T11:00:00:000-0400",<br>     scheduledStartDate: "2014-08-28T11:00:00:000-0400",<br>     priority : 0,<br>     forecastCompletionDate : "2014-08-28T16:16:00:000-0400",<br>     status : "CUR"<br>},<br>{<br>    ID : "53ff8e19003b46238a58d303608de502",<br>    name: "Test_Project_2_Edit",<br>    objCode : "PROJ",<br>    percentComplete : 0,<br>    scheduleCompletionDate : "2014-08-28T11:00:00:000-0400",<br>    scheduledStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority : 0,<br>    forecastCompletionDate : "2014-08-28T16:16:00:000-0400",<br>    status : "CUR"<br>}]</pre>Si vous souhaitez que toutes les opérations se produisent dans la même transaction, ajoutez "atomic=true" à votre appel d’API de lot en tant que paramètre de requête. Ainsi, si l’une des opérations échoue, toutes les opérations sont restaurées.

>[!NOTE]
Les opérations par lots atomiques ne peuvent renvoyer que la &quot;réussite&quot; : &quot;true&quot; ou une erreur.
