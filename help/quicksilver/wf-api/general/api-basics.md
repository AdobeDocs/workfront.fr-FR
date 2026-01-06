---
content-type: api
navigation-topic: general-api
title: Bases d’API
description: Bases d’API
author: Becky
feature: Workfront API
role: Developer
exl-id: d8c27915-8e1b-4804-9ef8-3a2efd57caac
source-git-commit: 319c45bc6617269f358af1e7b5f6132a8694710b
workflow-type: tm+mt
source-wordcount: '4396'
ht-degree: 97%

---


# Bases d’API

L’objectif de l’API Adobe Workfront est de simplifier la création d’intégrations avec Workfront en introduisant une architecture REST qui fonctionne sur HTTP. Ce document suppose que vous connaissez les réponses REST et JSON et décrit l’approche adoptée par l’API Workfront.

Une bonne connaissance du schéma Workfront vous aidera à comprendre les relations entre les bases de données qui peuvent être utilisées pour extraire des données de Workfront à des fins d’intégration.

## Politiques et directives

Pour garantir des performances cohérentes du système Workfront à la demande, l’API Workfront limite les threads d’API simultanés. Ce mécanisme de sécurisation empêche les problèmes système causés par des appels API abusifs. L’environnement Sandbox a la même limite de threads d’API simultanés en place, ce qui permet aux clients et aux partenaires de tester avec précision les appels d’API avant de publier le code en production.

Pour les environnements de production, de prévisualisation et de test, les demandes des utilisateurs et utilisatrices finaux ont une longueur maximale d’URI de 8 892 octets parce qu’elles sont acheminées par le CDN de Workfront (Akamai). Cette limite ne s’applique qu’aux URI acheminés par le CDN.

### Avertissement

Toute utilisation de l’API doit être testée dans l’environnement Beta de Workfront avant d’être exécutée dans l’environnement de production. Si un client ou une cliente utilise l’API pour un processus que Workfront considère raisonnablement comme une charge pour le logiciel à la demande (c’est-à-dire que le processus a un effet négatif important sur la performance du logiciel pour d’autres clientes et clients), Workfront se réserve le droit de demander au client ou à la cliente d’interrompre ce processus. Si le client ou la cliente ne se conforme pas et que le problème persiste, Workfront se réserve le droit de mettre fin au processus.

## URL de l’API Workfront

Pour plus d’informations sur l’URL que vous utiliserez pour appeler l’API Workfront, voir [Format de domaine pour les appels API Adobe Workfront](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md).

## Concepts de base de REST

Cette section fournit une introduction de haut niveau sur la façon d’interagir avec l’API REST de Workfront pour les principes REST suivants :

### URI d’objet

Chaque objet du système se voit attribuer un URI unique composé du type d’objet et de l’ID. Les exemples suivants montrent des URI décrivant trois objets uniques :

```
/attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
/attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d1
/attask/api/v15.0/issue/4c78821c0000d6fa8d5e52f07a1d54d2
```

Le type d’objet n’est pas sensible à la casse et peut être soit le code ObjCode abrégé (tel que proj), soit le nom alternatif de l’objet (projet).

Pour obtenir la liste des objets, des ObjCodes valides et des champs d&#39;objet, voir  [Explorateur d’API](../../wf-api/general/api-explorer.md).

>[!NOTE]
>
>Dans le contexte de l’API Workfront, un formulaire personnalisé est un objet `Category` et un champ personnalisé est un objet `Parameter`.

### Opérations

Les objets sont manipulés en envoyant une requête HTTP à leur URI unique. L’opération à effectuer est spécifiée par la méthode HTTP.

Les méthodes HTTP standard correspondent aux opérations suivantes :

* **GET** - Permet de récupérer un objet par son ID, de rechercher tous les objets par une requête, d’exécuter des rapports ou des requêtes nommées.
* **POST** - Insère un nouvel objet.
* **PUT** - Modifie un objet existant.
* **DELETE** - Supprime un objet.

Afin de contourner les déficiences du client ou les limites de longueur du protocole, le paramètre de méthode peut être utilisé pour modifier le comportement du protocole HTTP. Par exemple, une opération GET peut être mise en œuvre en publiant l’URI suivant :
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=get<br>GET /attask/api/v15.0/project/4c78...54d0?method=get</pre>

### Réponse

Chaque requête reçoit une réponse au format JSON. La réponse comporte soit un attribut data si la demande a abouti, soit un attribut error en cas de problème. Par exemple, la requête

```
GET /attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5
```

renvoie une réponse JSON similaire à la suivante :


<pre>{<br>    "data": [<br>        {<br>            "percentComplete": 0,<br>            "status": "CUR",<br>            "priority": 2,<br>            "name": "Brand New Project",<br>            "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Lors de l’exécution d’une requête GET via la barre d’adresse de votre navigateur, il n’est pas nécessaire d’inclure le sessionID dans la requête.

Une sécurité particulière a été ajoutée pour les requêtes PUT, POST et DELETE. Toute requête d’écriture ou de suppression dans la base de données ne peut être exécutée que si **sessionID=abc123** est inclus dans l’URI. Les exemples suivants montrent ce que cela donnerait pour une requête DELETE :
<pre>GET /attask/api/v15.0/project?id=4c78...54d0&amp;method=delete&amp;sessionID=abc123<br>GET /attask/api/v15.0/project/4c78...54d0?method=delete&amp;sessionID=abc123</pre>

### Authentification

L’API authentifie chaque demande pour s’assurer que le client a le droit d’afficher ou de modifier l’objet concerné par la requête.

L’authentification s’effectue en transmettant un ID de session qui peut être fourni en utilisant l’une des méthodes suivantes :

#### Authentification de l’en-tête de la demande

La méthode d’authentification préférée consiste à transmettre un en-tête de requête nommé SessionID contenant le jeton de session. Cela présente l’avantage d’être à l’abri des attaques [Cross-site Request Forgery (CSRF)](https://fr.wikipedia.org/wiki/Cross-site_request_forgery) et de ne pas interférer avec l’URI à des fins de mise en cache.

Voici un exemple d’en-tête de requête :

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

#### Authentification basée sur les cookies

L’API utilise la même authentification basée sur les cookies que celle utilisée par l’interface web du système. Ainsi, si un client ou une cliente se connecte à Workfront à l’aide de l’interface web, tous les appels AJAX effectués à partir du même navigateur utilisent la même authentification.

>[!NOTE]
>
>Afin de se protéger contre les attaques CSRF (Cross Site Request Forgery), cette méthode d’authentification n’est disponible que pour les opérations en lecture seule.

## Connexion

>[!IMPORTANT]
>
>Workfront ne recommande plus l’utilisation du point d’entrée `/login` ou des clés API. Utilisez plutôt l’une des méthodes d’authentification suivantes :
>
>* Authentification du serveur avec JWT
>* Authentification des utilisateurs et utilisatrices avec OAuth2
>
>Pour obtenir des instructions sur la configuration de ces méthodes d’authentification, voir [Créer des applications OAuth2 pour les intégrations Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>
>Pour obtenir des instructions sur l’utilisation de l’authentification du serveur dans Workfront, voir [Configurer et utiliser les applications OAuth 2 personnalisées de votre organisation à l’aide du flux JWT](../../wf-api/api/oauth-app-jwt-flow.md).
>
>Pour obtenir des instructions sur l’utilisation de l’authentification des utilisateurs et utilisatrices dans Workfront, voir [Configurer et utiliser les applications OAuth 2 personnalisées de votre organisation à l’aide du flux de code d’autorisation](../../wf-api/api/oauth-app-code-token-flow.md).

>[!NOTE]
>
>La procédure décrite dans cette section ne s’applique qu’aux organisations qui n’ont pas encore été intégrées à Adobe Business Platform. La connexion à Workfront via l’API Workfront n’est pas disponible si votre entreprise a été intégrée à Adobe Business Platform.
>
>Pour une liste des procédures qui diffèrent selon que votre entreprise a été intégrée ou non à Adobe Business Platform, voir [Différences d’administration en fonction de la plateforme (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

À l’aide d’un nom d’utilisateur ou d’utilisatrice et d’un mot de passe valides, vous pouvez utiliser la requête suivante pour obtenir un ID de session :

```
POST /attask/api/v15.0/login?username=admin&password=user
```

Cela permet de créer un cookie pour authentifier les futures requêtes et de renvoyer une réponse JSON contenant l’ID de session nouvellement créé, l’ID de la personne connectée et d’autres attributs de session.

>[!NOTE]
>
>Si vous avez un utilisateur ou une utilisatrice API désigné qui est également administrateur ou administratrice, Workfront vous suggère fortement d’utiliser une clé API pour vous connecter.

**Génération d’une clé API**

Vous pouvez générer une clé API lorsque vous vous connectez au système en tant qu’utilisateur ou utilisatrice, comme le montre l’exemple suivant :


```
PUT /attask/api/v15.0/user?action=generateApiKey&username= username&password=password&method=put
```

**Récupération d’une clé API précédemment générée**

Vous pouvez également récupérer une clé API qui a été précédemment générée pour un utilisateur ou une utilisatrice en particulier en exécutant getApiKey :


```
PUT /attask/api/v15.0/user?action=getApiKey&username=user@email.com&password=userspassword&method=put
```

Vous pouvez ensuite utiliser ce résultat pour authentifier tout appel API en ajoutant « apiKey » comme paramètre de requête avec cette valeur à la place d’un sessionID ou d’un nom d’utilisateur ou d’utilisatrice et d’un mot de passe. Cela est bénéfique du point de vue de la sécurité.

La requête suivante est un exemple de récupération de données d’un projet à l’aide de la clé API :

```
GET /attask/api/v15.0/project/abc123xxxxx?apiKey=123abcxxxxxxxxx
```

**Invalider une clé API**

Si la valeur apiKey a été compromise, vous pouvez exécuter « clearApiKey », ce qui invalide la clé API actuelle, comme le montre l’exemple suivant :

```
GET /attask/api/v15.0/user?action=clearApiKey&username=user@email.com&password=userspassword&method=put
```

Une fois la clé effacée, vous pouvez relancer getApiKey pour générer une nouvelle clé API.

### Déconnexion

Lorsqu’une session est terminée, vous pouvez utiliser la requête suivante pour déconnecter l’utilisateur ou l’utilisatrice, en empêchant tout accès ultérieur avec l’ID de session.

```
GET /attask/api/v15.0/logout?sessionID=abc1234
```

L’ID de session à déconnecter peut être spécifié sous la forme d’un cookie, d’un en-tête de requête ou d’un paramètre de requête.

Pour déconnecter un utilisateur ou une utilisatrice :

1. Accédez à votre écran de connexion, mais ne vous connectez pas.
1. Modifiez l’URL en /attask/api/v15.0/project/search.\
   Remarquez que la page est introuvable.
1. Remplacez le mot *search* par login?username=admin&amp;password=user, en remplaçant votre nom d’utilisateur ou d’utilisatrice et votre mot de passe pour *admin* et *user.\
   *Cette session est stockée dans le navigateur sous la forme d’un cookie et n’a pas besoin d’être répétée dans chaque requête GET ultérieure.

1. Remplacez l’URL par **/attask/api/v15.0/project/search**.
1. Remarquez la réponse fournie.

Vous devez toujours inclure le sessionID fourni après la connexion lorsque vous effectuez des requêtes PUT, POST et DELETE.

## Comportement GET

Utilisez la méthode HTTP GET pour récupérer un ou plusieurs objets et pour exécuter des rapports.

### Récupération d’objets

Vous pouvez améliorer la recherche d’objets à l’aide de modificateurs et de filtres.

#### Récupération d’un objet à l’aide de l’ID de l’objet

Si vous connaissez l’identifiant d’un objet, vous pouvez le retrouver en accédant à son URI unique. Par exemple, la requête

```
GET /attask/api/v15.0/project/4c78821c0000d6fa8d5e52f07a1d54d0
```

renvoie une réponse similaire à la suivante :

<pre>{<br>    "percentComplete": 0,<br>    "status": "CUR",<br>    "priority": 2,<br>    "name": "Brand New Project",<br>    "ID": "4c7c08b20000002de5ca1ebc19edf2d5" <br>}</pre>


Vous pouvez récupérer plusieurs objets dans la même requête en spécifiant le paramètre de requête ID et en donnant une liste des identifiants séparés par des virgules, comme le montre l’exemple suivant :


```
GET /attask/api/v15.0/project?id=4c78...54d0,4c78...54d1
```

Notez que la requête /attask/api/v15.0/project?id=... est identique à la requête `/attask/api/v15.0/project/...`.

#### Récupérer un objet à l’aide de l’URI

Si vous souhaitez récupérer un objet en fonction de critères autres que l’identifiant, vous pouvez rechercher l’URI.

Par exemple, vous pouvez utiliser la requête suivante pour obtenir une liste de tous les projets dans le système :

```
GET /attask/api/v15.0/project/search
```

Vous pouvez spécifier des filtres en utilisant les paramètres de la requête sous forme de paires nom-valeur. Par exemple, l’exemple suivant montre une requête qui recherche tous les projets en cours :

```
GET /attask/api/v15.0/project/search?status=CUR
```

La requête suivante trouve toutes les tâches qui ne sont pas encore terminées et qui sont affectées à un utilisateur nommé John.

```
GET /attask/api/v15.0/task/search?percentComplete=100
&percentComplete_Mod=lt &assignedTo:firstName=John
```

#### Utiliser les modificateurs de recherche

Le tableau suivant répertorie certains des modificateurs que vous pouvez utiliser avec l’API Workfront.

| **Modificateur** | **Description** | **Exemple** |
| --- | --- | --- |
| eq | renvoie les résultats qui ont le statut « Fermé ». | <pre>...status=cls&amp;status_Mod=eq...</pre> |
| ne | renvoie les résultats qui n’ont pas le statut « Fermé ». | <pre>...status=cls&amp;status_Mod=ne...</pre> |
| gte | renvoie les résultats affichant un pourcentage d’achèvement supérieur ou égal à 50. | <pre>...percentComplete=50&amp;percentComplete_Mod=gte...</pre> |
| lte | renvoie les résultats affichant un pourcentage d’achèvement inférieur ou égal à 50. | <pre>...percentComplete=50&amp;percentComplete_Mod=lte...</pre> |
| isnull | renvoie les résultats dont la description est « Null ». | <pre>...description_Mod=isnull...</pre> |
| notnull | renvoie les résultats dont la description n’est pas « Null ». | <pre>...description_Mod=notnull...</pre> |
| contient | renvoie les résultats dont le nom contient « Workfront ». | <pre>...name=Workfront&amp;name_Mod=contains...</pre> |
| entre | renvoie les résultats dont la date de saisie se situe dans les 7 derniers jours. | <pre>...entryDate=$$TODAY-7d&amp;entryDate_Range=$$TODAY&amp;entryDate_Mod=between...</pre> |

{style="table-layout:auto"}

>[!NOTE]
>
>Les requêtes de recherche sont sensibles à la casse. Si vous recevez une erreur, assurez-vous que **_Mod** et **_Range** ont la bonne casse.

#### Utiliser des instructions OR (OU)

Vous pouvez améliorer une recherche en ajoutant un paramètre comprenant « OR » ainsi qu’un nombre pour indiquer le niveau d’un filtre ou d’une série de filtres.

Une instruction OR renvoie uniquement les enregistrements de l’appel API qui répondent aux critères de filtrage de l’instruction OR. Les filtres ne sont pas nécessairement appliqués à tous les niveaux de l’instruction OR.

Par exemple, si vous souhaitez filtrer les éléments suivants :

* Tâches dont le nom contient « Planning » OR
* Tâches dans un portfolio nommé « FixedAssets » AND (ET) affectées à une personne dont le nom contient « Steve » OR
* Tâches dont la tâche parent s’appelle « Final Task » (tâche finale)

alors utilisez l’appel API suivant avec ses multiples instructions OR :
<pre>GET /attask/api/v15.0/task/search?name=Planning<br>&amp;name_Mod=contains<br>&amp;OR:1:portfolio:name=FixedAssets<br>&amp;OR:1:portfolio:name_Mod=eq<br>&amp;OR:1:assignedTo:name=Steve<br>&amp;OR:1:assignedTo:name_Mod=cicontains<br>&amp;OR:2:parent:name=Final Task<br>&amp;OR:2:parent:name_Mod=eq
</pre>

#### Utiliser les paramètres du filtre

L’un des inconvénients potentiels de l’utilisation de paramètres URL pour les filtres de recherche est que Workfront analyse certains paramètres avant de vérifier les différentes méthodes d’authentification (par exemple, nom d’utilisateur ou d’utilisatrice, mot de passe, apiKey, cookie). Dans ce cas, les paramètres ne sont pas utilisés comme filtres dans l’appel. 

Pour éviter ce problème, vous pouvez placer ces valeurs dans des paramètres de filtre avec un formatage JSON. Par exemple, si vous voulez filtrer le nom d’utilisateur ou d’utilisatrice testuser, au lieu d’utiliser
<pre>/attask/api/v15.0/user/search?username=testuser@workfront.com</pre>faites passer le paramètre URL dans un filtre, comme le montre l’exemple suivant :
<pre>/attask/api/v15.0/user/search?filters={"username":"testuser@workfront.com"}</pre>

#### Utiliser le paramètre de requête Map

Par défaut, les données renvoyées par une recherche sont sous la forme d’un tableau JSON. Selon votre cas d’utilisation, il peut être plus efficace d’obtenir le résultat sous la forme d’un objet JSON indexé par ID. Pour ce faire, il convient d’utiliser le paramètre de requête Map. Par exemple, la requête
<pre>/attask/api/v15.0/task/search?map=true</pre>renvoie une réponse indexée par ID similaire à ce qui suit :
<pre>{<br>    "data": {<br>        "4c9a97db0000000f13ee4446b9aead9b": {<br>            "percentComplete": 0,<br>            "status": "NEW",<br>            "name": "first task",<br>            "ID": "4c9a97db0000000f13ee4446b9aead9b",<br>            "taskNumber": 1 <br>        },<br>        "4ca28ba600002024cd49e75bd43cf601": {<br>            "percentComplete": 0,<br>            "status": "INP:A",<br>            "name": "second task",<br>            "ID": "4ca28ba600002024cd49e75bd43cf601",<br>            "taskNumber": 2 <br>        } <br>    } <br>}</pre>

#### Utiliser le paramètre de requête Fields

Par défaut, la récupération d‘un objet ne renvoie que le sous-ensemble de champs le plus couramment utilisé.

Vous pouvez utiliser le paramètre de requête Fields pour spécifier une liste de champs spécifiques séparés par des virgules. Par exemple, la requête
<pre>/attask/api/v15.0/task/search?fields=plannedStartDate,priority</pre>renvoie une réponse similaire à la suivante :
<pre>{<br>    "priority": 2,<br>    "name": "first task",<br>    "ID": "4c7c08fa0000002ff924e298ee148df4",<br>    "plannedStartDate": "2010-08-30T09:00:00:000-0600" <br>}</pre>

>[!NOTE]
>
>Les noms de ces champs sont sensibles à la casse.

Pour obtenir une liste des références de champs possibles, consultez l’[Explorateur d’API](../../wf-api/general/api-explorer.md).

#### Rechercher des objets imbriqués

Vous pouvez rechercher des objets imbriqués. Par défaut, les objets imbriqués sont renvoyés avec seulement le nom et l’ID. Par exemple, pour obtenir tous les problèmes avec leurs personnes propriétaires, utilisez la requête suivante :
<pre>/attask/api/v15.0/issue/search?fields=owner</pre>Si vous avez besoin de plus d’informations, vous pouvez demander un champ imbriqué en utilisant la syntaxe des deux points. Par exemple, la requête suivante permet de rechercher tous les problèmes ainsi que le nom, l’ID, le titre et le numéro de téléphone de la personne propriétaire.
<pre>/attask/api/v15.0/issue/search?fields=owner:title,owner:phoneNumber</pre>et de renvoyer ce qui suit :
<pre>{<br>    "name": "an important issue",<br>    "ID": "4c78285f00000908ea8cfd66e084939f",<br>    "owner": {<br>        "title": "Operations Specialist",<br>        "phoneNumber": "555-1234",<br>        "name": "Admin User",<br>        "ID": "4c76ed7a0000054c172b2c2d9f7f81c3" <br>    } <br>}</pre>

#### Récupérer des collections imbriquées

Vous pouvez récupérer des collections imbriquées d’objets. Par exemple, pour obtenir un projet avec toutes ses tâches, utilisez la requête suivante :
<pre>/attask/api/v15.0/project/search?fields=tasks</pre>La requête suivante récupère des affectations de tâches :
<pre>/attask/api/v15.0/task/search?fields=assignments</pre>

#### Rechercher plusieurs champs imbriqués

Par défaut, seuls le nom et l’ID de chaque tâche sont renvoyés, mais des champs imbriqués supplémentaires peuvent être spécifiés à l’aide de la syntaxe des deux points. Pour afficher tous les champs disponibles pour un objet ou une collection connexe, il suffit d’ajouter deux points et un astérisque à la référence de l’objet ou de la collection.
<pre>/attask/api/v15.0/task/search?fields=assignments:*</pre>

#### Récupérer des données personnalisées

Vous pouvez récupérer des champs de données personnalisés en utilisant le préfixe « DE: ». Par exemple, pour demander un projet avec un paramètre appelé « CustomText », utilisez la requête suivante :
<pre>/attask/api/v15.0/project/search?fields=DE:CustomText</pre>qui renvoie
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    "DE:CustomText": "task b" <br>}</pre>Vous pouvez également récupérer toutes les données personnalisées d’un objet en interrogeant le champ parameterValues. Par exemple,
<pre>/attask/api/v15.0/project/search?fields=parameterValues</pre>renvoie des données similaires à celles qui suivent :
<pre>{<br>    "name": "custom data project",<br>    "ID": "4c9a954f0000001afad0687d7b1b4e43",<br>    parameterValues: { <br>        "DE:CustomText": "task b", <br>        "DE:CustomNumber": 1.4, <br>        "DE:CustomCheckBoxes": ["first", "second", "third"] <br>    } <br>}</pre>

#### Utiliser les requêtes nommées

Certains types d’objets ont des recherches nommées qui sont couramment exécutées et sont disponibles en ajoutant le nom de la requête à la fin de l’URI du type d’objet. Par exemple, la requête suivante permet de récupérer les éléments de travail (tâches et problèmes) qui sont actuellement affectés à l’utilisateur ou l’utilisatrice :
<pre>/attask/api/v15.0/work/myWork</pre>Les requêtes nommées permettent d’utiliser le paramètre fields pour récupérer des champs supplémentaires. Certaines requêtes nommées acceptent également des filtres supplémentaires. Pour obtenir la liste des requêtes nommées autorisées pour un objet, voir l’onglet Action de l’objet dans le  [API Explorer](https://developer.adobe.com/workfront/api-explorer/).

#### Utiliser `Count`

Vous pouvez utiliser `count` pour obtenir le nombre de résultats correspondant à votre requête. Cela peut être utile lorsque vous n’avez pas besoin des données dans les résultats. En ne renvoyant que le nombre, le serveur peut traiter la requête plus rapidement et économiser de la bande passante. Par exemple, la requête
<pre>GET /attask/api/v15.0/project/count?status=CUR</pre>renvoie le nombre de résultats dans le format suivant :
<pre>{<br>    "count": 3 <br>}</pre>Le fait de renvoyer un nombre représente un transfert de données beaucoup moins important que si les objets complets étaient renvoyés. La syntaxe est identique à celle de la commande de recherche.

### Demander un rapport

Vous pouvez demander un rapport, où seul l’agrégat de certains champs avec un ou plusieurs regroupements est nécessaire. Comme le montre l’exemple suivant, la syntaxe du rapport est la même que celle de l’API SOAP :
<pre>GET /attask/api/v15.0/hour/report?project:name_1_GroupBy=true&amp;hours_AggFunc=sum</pre>qui renvoie le résultat suivant
<pre>{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>     "Second Project": { <br>        "sum_hours": 30 <br>    } <br>}</pre>L’ajout du paramètre $$ROLLUP=true permet d’inclure un total à chaque niveau de regroupement :
<pre>{<br>    "First Project": { <br>        "sum_hours": 15 <br>    }, <br>    "Second Project": { <br>        "sum_hours": 30 <br>    }, <br>    "$$ROLLUP": { <br>        "sum_hours": 45 <br>    } <br>}</pre>

### Trier les résultats d’une requête dans l’API

Vous pouvez trier vos résultats selon n’importe quel champ si vous ajoutez les éléments suivants à votre appel API :

&amp;entryDate_Sort=asc

Par exemple, si vous souhaitez trier les tâches en fonction de leur date de début prévue, supprimez entryDate et remplacez-la par plannedCompletionDate.

Cela fonctionne pour la plupart des champs de Workfront.

### Prendre en compte les limites des requêtes

Lorsque vous interrogez un objet, il convient de tenir compte des relations entre les objets connexes et des limites de la recherche.Par exemple, comme le montre le tableau suivant, une requête portant sur les projets ne peut pas renvoyer plus de 2 000 projets. Ces 2 000 projets sont considérés comme des « objets principaux ». Si vous interrogez le champ Tâches sur les projets, le champ Tâches, qui est une collection, devient un objet secondaire par rapport à l’objet principal Projet. Une requête du champ Tâches peut inclure des milliers de tâches sur des projets. Au total, le nombre combiné d’objets (projets et tâches) renvoyés ne peut dépasser le maximum de 50 000.

Pour garantir des performances optimales, le tableau suivant indique les limites imposées aux requêtes de recherche. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Résultat de la requête</th> 
   <th>Limite</th> 
   <th>Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td width="200">Nombre de résultats par défaut</td> 
   <td>100</td> 
   <td> Si aucune limite n’est spécifiée dans le filtre de la requête (c’est-à-dire $$LIMIT), le résultat ne peut pas contenir plus de 100 objets principaux. <br>Voir <a href="#using-paginated-responses" class="MCXref xref">Utiliser les réponses paginées</a> pour savoir comment contourner cette limite. </td> 
  </tr> 
  <tr> 
   <td>Nombre maximal de résultats</td> 
   <td>2 000</td> 
   <td>Le filtre de requête (c’est-à-dire $$LIMIT) ne peut renvoyer plus de 2 000 résultats. Pour plus d’informations, voir « Réponses paginées ».</td> 
  </tr> 
  <tr> 
   <td>Profondeur de champ maximale</td> 
   <td>4</td> 
   <td>Lorsque vous identifiez les champs que vous souhaitez afficher, vous ne pouvez pas vous éloigner de plus de quatre niveaux de l’objet concerné par la requête.</td> 
  </tr> 
  <tr> 
   <td>Nombre maximal d’objets</td> 
   <td>50 000</td> 
   <td>L’ensemble des résultats ne peut pas inclure 50 000 objets principaux et secondaires.</td> 
  </tr> 
  <tr> 
   <td>Nombre maximal de champs</td> 
   <td nowrap>1 000 000</td> 
   <td>Lorsque l’ensemble des résultats est inférieur à 50 000 objets, vos résultats peuvent comprendre au maximum 1 000 000 de champs.</td> 
  </tr> 
  <tr> 
   <td>Nombre maximal de créations/mises à jour de lots</td> 
   <td>100</td> 
   <td>La limite maximale de créations ou de mises à jour de lots est de 100.</td> 
  </tr> 
 </tbody> 
</table>

### Utiliser les réponses paginées {#using-paginated-responses}

Pour passer outre la limite du nombre de résultats par défaut et autoriser 200 résultats, vous pouvez inclure le filtre `$$LIMIT=200` dans votre requête, comme dans l’exemple suivant :
<pre>GET /attask/api/v15.0/project/search?$$LIMIT=200</pre>

Pour garantir la fiabilité et les performances des autres clientes et clients du système, la limite maximale des résultats autorisés par requête est de 2 000 objets. Toute tentative de spécifier une limite plus importante entraîne un message d’erreur `IllegalArgumentException`.

Par conséquent, nous vous recommandons d’utiliser des réponses paginées pour les jeux de données volumineux. Pour spécifier le premier résultat à renvoyer, ajoutez le filtre `$$FIRST`. Par exemple, la demande suivante renvoie les résultats 201-250 pour une requête :
<pre>GET /attask/api/v15.0/project/search?$$FIRST=200&amp;$$LIMIT=50</pre>

Notez que dans l’exemple ci-dessus, `$$FIRST=200` renvoie le 201e résultat. `$$FIRST=0` renverrait le premier résultat. Il peut être utile de considérer la valeur $$FIRST comme le nombre de résultats que vous souhaitez ignorer avant de renvoyer les résultats.

Pour vous assurer que vos résultats sont correctement paginés, utilisez un paramètre de tri. Cela permet de renvoyer les résultats dans le même ordre, de sorte que la pagination ne répète pas ou n’ignore pas de résultats. Par exemple, pour trier à l’aide de l’ID de l’objet, utilisez `ID_Sort=asc`.

### Créer une règle d’accès

Vous pouvez créer une règle d’accès pour déterminer qui peut accéder à un objet. Voici des exemples de règles d’accès que vous pouvez définir :

Pour configurer un projet de manière à ce qu’il ne soit partagé qu’avec un utilisateur ou une utilisatrice dont l’ID est « abc123 », utilisez la requête suivante :
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=put &amp;updates={ accessRules: [ {accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'} ] }</pre>Il est également possible de ne partager qu’avec une nouvelle personne et de conserver intactes les autorisations existantes :
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?method=put&amp;accessorID=abc123&amp;accessorObjCode=USER&amp;coreAction=VIEW</pre>Pour récupérer les règles d’accès existantes :
<pre>GET /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?fields=accessRules:*</pre>

## Comportement de la requête POST

POST insère un nouvel objet. La syntaxe est identique à celle de PUT, à quelques exceptions près. Comme le nouvel objet n’existe pas encore, il n’a pas d’ID. Pour cette raison, l’URI n’inclut pas l’ID.

### Créer un objet

Voici un exemple de requête de création d’un projet :
<pre>POST /attask/api/v15.0/project?name=New Project</pre>La réponse comprend le projet qui vient d’être créé avec son nouvel ID et tous les autres champs spécifiés.

### Copier un objet

Certains objets peuvent être copiés. Pour ces types d’objets, il est possible de créer de nouveaux objets en les publiant avec un paramètre copySourceID. Par exemple, la requête suivante copie le projet donné et lui donne un nouveau nom :

```
POST /attask/api/v15.0/project?copySourceID=4c7...&name=Copied Project
```

### Charger des documents

Vous pouvez charger des documents par l’intermédiaire de l’URL d’API suivante :
<pre>POST /attask/api/v15.0/upload</pre>L’API s’attend à ce que le type de contenu soit multipart/form-data. Le nom du paramètre pour le fichier doit être uploadedFile. Le serveur renvoie les données JSON suivantes :
<pre>{<br>    "handle": "4c7c08fa0000002ff924e298ee148df4"<br>}</pre>Vous pouvez utiliser la poignée et poster à l’URL suivante lors de la création d’un document Workfront :
<pre>POST /attask/api/v15.0/document?updates={<br>    name: aFileName,<br>    handle: abc...123, (handle from the file upload)<br>    docObjCode: PROJ, (or TASK, OPTASK, etc)<br>    objID: abc...123,<br>    currentVersion:{version:v1.0,fileName:aFileName}<br>}</pre>

## Comportement de la requête PUT

PUT est utilisée pour mettre à jour un objet existant.

La réponse à une requête PUT est identique à celle d’une GET. Dans les deux cas, le serveur renvoie le nouvel état de l’objet après la mise à jour. Toutes les règles utilisées pour modifier une réponse à une requête GET fonctionnent également avec PUT, comme la spécification de champs supplémentaires à renvoyer, de données personnalisées, etc.

### Modifier des objets

Les mises à jour des objets sont toujours effectuées par ID en utilisant l’URI unique de l’objet. Les champs à mettre à jour sont spécifiés en tant que paramètres de la requête. Par exemple, pour modifier le nom d’un projet, vous pouvez envoyer une requête similaire à la suivante :
<pre>PUT /attask/api/v15.0/project/4c7...?name=New Project Name <br>PUT /attask/api/v15.0/project?id=4c7...&amp;name=New Project Name</pre>La mise à jour nécessitant un ID, cette opération échouera (sans insertion) si l’objet n’existe pas sur le serveur.

### Spécifier les modifications JSON

Comme le montre l’exemple suivant, vous pouvez utiliser le paramètre de requête updates pour spécifier les champs à mettre à jour en utilisant la syntaxe JSON :
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>{<br>     name: "New Project Name", <br>     status: "CUR", <br>     ... <br>}</pre>

### Effectuer des mises à jour imbriquées

Certains objets possèdent des collections privées qui peuvent être mises à jour. Par exemple, l’exemple suivant montre comment remplacer les affectations existantes pour une tâche donnée :
<pre>PUT /attask/api/v15.0/task/4c7...?updates= <br>{<br>    assignments: [ <br>        { <br>            assignedToID: "2222...54d0, <br>            assignmentPercent: 50.0 <br>        },{ <br>            roleID: "1111...54d0"<br>        } <br>    ] <br>}</pre>

>[!NOTE]
>
>Alors que les mises à jour effectuées au niveau supérieur sont peu nombreuses, les mises à jour d’une collection ou d’un objet imbriqué remplacent complètement la collection existante. Pour modifier une seule affectation sur une tâche sans effet sur les objets, utilisez une requête PUT sur l’affectation plutôt que sur la tâche.

L’exemple suivant fait d’un projet une file d’attente publique pour le centre d’assistance. Notez que les propriétés existantes de la file d’attente sont remplacées.
<pre>PUT /attask/api/v15.0/project/4c7...?updates= <br>{ <br>    queueDef: { <br>        isPublic: 1 <br>    } <br>}</pre>

### Utiliser le paramètre de requête Action

Certains objets permettent d’effectuer des actions supplémentaires, en plus des simples modifications. Vous pouvez spécifier ces actions à l’aide du paramètre de requête Action. Par exemple, la requête suivante recalcule la chronologie d’un projet donné :
<pre>PUT /attask/api/v15.0/project/4c7...?action=calculateTimeline<br><br>or<br><br>PUT /attask/api/v15.0/project/4c7.../calculateTimeline </pre>

### Déplacer des objets

La syntaxe suivante permet de déplacer une tâche d’un projet à un autre :
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>Un exemple pour chaque type d’action est fourni ici : (??)
<pre>PUT /attask/api/v15.0/project/1234/approveApproval<br><br>PUT /attask/api/v15.0/project/1234/calculateFinance<br><br>PUT /attask/api/v15.0/project/1234/calculateTimeline<br><br>PUT /attask/api/v15.0/project/1234/calculateDataExtension<br><br>PUT /attask/api/v15.0/project/1234/recallApproval<br><br>PUT /attask/api/v15.0/project/1234/rejectApproval<br><br>PUT /attask/api/v15.0/task/1234/move<br><br>PUT /attask/api/v15.0/workitem/1234/markViewed</pre>L’identification d’attributs supplémentaires est nécessaire uniquement pour l’action de déplacement afin de spécifier le projet dans lequel l’élément de travail doit être déplacé.

Voici un exemple de chaque type d’action :
<pre>PUT /attask/api/v15.0/project/1234?method=put&amp;updates={accessRules:[{accessorID: 'abc123', accessorObjCode: 'USER', coreAction: 'VIEW'}]}</pre>

### Partager des objets

La syntaxe suivante permet de partager un projet avec une équipe :
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx/share?accessorID=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx&amp;accessorObjCode=TEAMOB</pre>Lors de la modification d’un objet, vous pouvez remplacer toutes les règles d’accès sur un objet en effectuant une requête PUT et en envoyant des mises à jour comme dans l’exemple suivant :
<pre>PUT /attask/api/v15.0/project/123abcxxxxxxxxxxxxxxxxxxxxxxxxxx?method=PUT&amp;updates={accessRules:[{accessorID:'123abcxxxxxxxxxxxxxxxxxxxxxxxxxx',accessorObjCode:'TEAMOB',coreAction:'VIEW'}]}</pre>La syntaxe suivante permet de déplacer une tâche d’un projet à un autre :
<pre>PUT /attask/api/v15.0/task/4c7.../move?projectID=5d8...</pre>

## Comportement de la requête DELETE

La requête DELETE supprime un objet. Dans tous les cas, l’URI peut inclure le paramètre force=true pour que le serveur supprime les données spécifiées et leurs éléments dépendants. Exécuter la méthode HTTP DELETE permet de supprimer une tâche sur un URI :
<pre>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0 <br>DELETE /attask/api/v15.0/task/4c78821c0000d6fa8d5e52f07a1d54d0?force=true <br>DELETE /attask/api/v15.0/task?id=4c78821c0000d6fa8d5e52f07a1d54d0?force=true</pre>

## Mises à jour en masse

Une instruction de mises à jour en masse met à jour plusieurs objets en même temps dans le cadre d’un seul appel API. Un appel API de création en masse est conçu de la même manière qu’un appel de mise à jour normal, comme le montrent les exemples suivants :
<pre>PUT /attask/api/v15.0/proj?updates=[{"name":"Test_Project_1"},{"name":"Test_Project_2"}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>ou <pre>PUSH /attask/api/v15.0/proj?updates=[{« name »:« Test_Project_1 »},{« name »:« Test_Project_2 »}]&amp;method=POST&amp;apiKey=123ab-cxxxxxxxxxxxxxxxxxxxxxxxx</pre>ce qui se traduit par un retour similaire à ce qui suit :
<pre>data: [{<br>    ID: "53ff8d3d003b438b57a8a784df38f6b3",<br>    name: "Test_Project_1",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>},<br>{<br>    ID: "53ff8d49003b43a2562aa34eea3b6b10",<br>    name: "Test_Project_2",<br>    objCode: "PROJ",<br>    percentComplete: 0usi,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:12:00:000-0400",<br>    status: "CUR"<br>}]</pre>Vous pouvez également effectuer une mise à jour en masse similaire à ce qui suit :
<pre>PUT /attask/api/v15.0/proj?Umethod=PUT&amp;updates=[{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_1_ Edit"},{"ID":"123abcxxxxxxxxxxxxxxxxxxxxxxxxxx","name":"Test_Project_2_Edit"}]&amp;apiKey=123abcxxxxxxxxxxxxxxxxxxxxxxxxxx</pre>ce qui se traduit par un retour similaire à ce qui suit :
<pre>data: [ {<br>     ID: "53ff8e15003b461d4560f7f65a440078",<br>     name: "Test_Project_1_Edit",<br>     objCode: "PROJ",<br>     percentComplete: 0,<br>     plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>     plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>     priority: 0,<br>     projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>     status: "CUR"<br>},<br>{<br>    ID: "53ff8e19003b46238a58d303608de502",<br>    name: "Test_Project_2_Edit",<br>    objCode: "PROJ",<br>    percentComplete: 0,<br>    plannedCompletionDate: "2014-08-28T11:00:00:000-0400",<br>    plannedStartDate: "2014-08-28T11:00:00:000-0400",<br>    priority: 0,<br>    projectedCompletionDate: "2014-08-28T16:16:00:000-0400",<br>    status: "CUR"<br>}]</pre>Si vous souhaitez que toutes les opérations se déroulent dans la même transaction, ajoutez « atomic=true » à votre appel API par lots en tant que paramètre de requête. Ainsi, si l’une des opérations échoue, toutes les opérations sont annulées.

>[!NOTE]
>
>Les opérations atomiques par lots ne peuvent renvoyer que « success: true » ou une erreur.

