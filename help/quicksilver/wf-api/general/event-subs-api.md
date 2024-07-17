---
content-type: api
navigation-topic: general-api
title: API d’abonnement aux événements
description: API d’abonnement aux événements
author: Becky
feature: Workfront API
role: Developer
exl-id: c3646a5d-42f4-4af8-9dd0-e84977506b79
source-git-commit: c08bd3311892d24a9bd40af138169957f5ea2ca4
workflow-type: tm+mt
source-wordcount: '2147'
ht-degree: 4%

---


# API d’abonnement aux événements

<!--BOB clean this up-->

<!--
{{highlighted-preview}}
-->

Lorsqu’une action se produit sur un objet Adobe Workfront pris en charge par les abonnements aux événements, vous pouvez configurer Workfront pour envoyer une réponse au point de terminaison souhaité. Cela signifie que les applications tierces peuvent recevoir des mises à jour provenant d’interactions Workfront via l’API Workfront peu après leur apparition. En règle générale, vous pouvez vous attendre à recevoir des notifications webhook en moins de 5 secondes à partir du changement de données en cours de journalisation. En moyenne, les clients reçoivent des notifications webhook en moins d’une seconde à partir du changement de données en cours de journalisation.  

Pour recevoir les payloads d’abonnement aux événements par le biais de votre pare-feu, vous devez ajouter les adresses IP suivantes à votre liste autorisée :

**Pour les clients en Europe :**

* 52.30.133.50
* 52.208.159.124
* 54.220.93.204
* 52.17.130.201
* 34.254.76.122
* 34.252.250.191

**Pour les clients situés à des endroits autres que l’Europe :**

* 54.244.142.219
* 44.241.82.96
* 52.36.154.34
* 34.211.224.9
* 54.218.48.56
* 52.39.217.230

Les rubriques suivantes prennent en charge l’API Event Subscription :

## Objets pris en charge par les abonnements à un événement

Les objets Workfront suivants sont pris en charge par les abonnements aux événements.

* Affectation
* Entreprise
* Tableau de bord
* Document
* Frais
* champ
* Heure
* Problème
* Note
* Portfolio
* Programme
* Projet
* Enregistrement
* Type d’enregistrement
* Rapport
* Tâche
* Modèle
* Feuille de temps
* l’utilisateur ou de l’utilisatrice
* Espace de travail

Pour obtenir la liste des champs pris en charge par les objets d’abonnement d’événement, voir [Champs de ressource d’abonnement d’événement](../../wf-api/api/event-sub-resource-fields.md).

## Authentification de l’abonnement à un événement

Pour créer, interroger ou supprimer un abonnement à un événement, l’utilisateur de Workfront doit disposer des éléments suivants :

* Un niveau d’accès &quot;Administrateur système&quot; est requis pour utiliser les abonnements à un événement.
* Un en-tête `sessionID` est nécessaire pour utiliser l’API d’abonnements à un événement

  Pour plus d’informations, voir [Authentification](api-basics.md#authentication) dans [Principes de base des API](api-basics.md).

## Formation de la ressource d’abonnement

La ressource d&#39;abonnement contient les champs suivants.

* objId (facultatif)

   * **String** - ID de l’objet objCode spécifié pour lequel les événements sont déclenchés. Si ce champ n’est pas spécifié, l’utilisateur reçoit des événements pour tous les objets du type spécifié.

* objCode (obligatoire)

   * **String** - objCode de l’objet abonné aux modifications. Les valeurs possibles pour objCode sont répertoriées dans le tableau ci-dessous.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <thead> 
       <tr> 
        <th><p>Objet</p></th> 
        <th><p>objCode</p></th> 
       </tr> 
      </thead> 
      <tbody> 
       <tr> 
        <td scope="col">Affectation</td> 
        <td scope="col"><p>ASSGN</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Société </td> 
        <td scope="col"><p>CMPY</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Tableau de bord</td> 
        <td scope="col">PTLTAB</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Document</p></td> 
        <td scope="col">DOCU </td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Frais</p></td> 
        <td scope="col">EXPNS</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>champ</p></td> 
        <td scope="col"><p>CHAMP</p></td> 
       </tr> 
      <tr> 
        <td scope="col"><p>Heure</p></td> 
        <td scope="col">HOUR</td> 
       </tr> 
       <tr> 
        <td scope="col">Problème</td> 
        <td scope="col"><p>OPTASK</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Note</td> 
        <td scope="col">NOTE</td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Portfolio</p></td> 
        <td scope="col"><p>PORT</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Programme</p></td> 
        <td scope="col"><p>PRGM</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Projet</p></td> 
        <td scope="col"><p>PROJ</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Enregistrement</p></td> 
        <td scope="col"><p>ENREGISTRER</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Type d’enregistrement</p></td> 
        <td scope="col"><p>RECORD_TYPE</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Rapport</p></td> 
        <td scope="col"><p>PTLSEC</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Tâche</p></td> 
        <td scope="col"><p>TÂCHE</p></td> 
       </tr> 
       <tr> 
        <td scope="col"><p>Modèle</p></td> 
        <td scope="col"><p>TMPL</p></td> 
       </tr> 
       <tr> 
        <td scope="col">Feuille de temps</td> 
        <td scope="col">TSHET</td> 
       </tr> 
       <tr> 
        <td scope="col">l’utilisateur ou de l’utilisatrice</td> 
        <td scope="col">UTILISATEUR</td> 
       </tr> 
       <tr> 
        <td scope="col">Espace de travail</td> 
        <td scope="col">WORKSPACE</td> 
       </tr> 
      </tbody> 
     </table>

* eventType (obligatoire)

   * **String** - Valeur qui représente le type d’événement auquel l’objet est abonné. Les types d’événement disponibles sont les suivants :

      * CREATE
      * DELETE 
      * UPDATE

* url (obligatoire)

   * **String** - URL du point de terminaison auquel les payloads d’événement d’abonnement sont envoyées via HTTP.

* authToken (obligatoire)

   * **String** - Jeton de porteur OAuth2 utilisé pour s’authentifier avec l’URL spécifiée dans le champ &quot;URL&quot;. 

## Création de requêtes d’API d’abonnement à un événement

Une fois que l’utilisateur a accès en tant qu’administrateur et qu’il a créé la ressource d’abonnement, vous êtes prêt à créer des abonnements à des événements.

Utilisez la syntaxe suivante pour construire l’URL.

**URL de requête :**


```
POST https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**En-têtes de requête :**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nom de l’en-tête</p> </th> 
   <th> <p>Valeur d’en-tête</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Content-type</p> </td> 
   <td> <p>application/json</p> </td> 
  </tr> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valeur sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Exemple de corps de requête :**

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua",
                "authToken": "EauthTokenWorkfrontRocks1234_"
            }
```

| Code de réponse | Description |
|---|---|
| 201 (Créé) | L’abonnement à l’événement a bien été créé. |
| 400 (Requête incorrecte) | Le champ URL de la ressource d&#39;abonnement a été considéré comme non valide. |
| 401 (Non autorisé) | L’ID de session fourni était vide ou considéré comme non valide. |
| 403 (Interdit) | L’utilisateur qui correspond à l’ID de session fourni ne dispose pas d’un accès administrateur. |

La transmission d’une ressource d’abonnement en tant que corps d’une requête (le type de contenu étant &quot;application/json&quot;) entraîne la création d’un abonnement d’événement pour l’objet spécifié. Un code de réponse 201 (Créé) indique que l’abonnement a été créé. Un code de réponse autre que 201 signifie que l’abonnement a été **NOT** créé.

>[!NOTE]
>
> L’en-tête de réponse &quot;Emplacement&quot; contient l’URI de l’abonnement d’événement nouvellement créé.

**Exemple d’en-têtes de réponse :**

| En-têtes de réponse | Exemple |
|---|---|
| Content-Length | `→0` |
| Date | `→Wed, 05 Apr 2017 21:23:33 GMT` |
| Emplacement | `→https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/750a636c-5628-48f5-ba26-26b7ce537ac2` |
| Serveur | `→Apache-Coyote/1.1` |

## Requête sur les abonnements aux événements

Lors de l’interrogation de Workfront HTTP, utilisez la méthode GET. Il existe deux manières de rechercher des abonnements à un événement : effectuer une requête par ID d’abonnement (voir ci-dessous) ou interroger tous les abonnements à un événement.

### Requête sur tous les abonnements aux événements

Vous pouvez interroger tous les abonnements à des événements pour un client ou utiliser les éléments suivants pour gérer la réponse. Vous pouvez également utiliser les options suivantes pour gérer la réponse :

* **page** : option de paramètre de requête pour spécifier le nombre de pages à renvoyer. La valeur par défaut est 1.
* **limit** : option de paramètre de requête pour spécifier le nombre de résultats à renvoyer par page. La valeur par défaut est 100 avec un maximum de 1 000.

La syntaxe de requête pour répertorier tous les abonnements d’événement pour un client spécifique est la suivante :

**URL de requête :**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions
```

**En-têtes de requête :**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nom de l’en-tête</p> </th> 
   <th> <p>Valeur d’en-tête</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valeur sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Codes de réponse :**

| Code de réponse | Description |
|---|---|
| 200 (OK) | La requête renvoyée avec tous les abonnements d’événement trouvés pour le client correspondant à l’ID de session fourni. |
| 401 (Non autorisé) | L’ID de session fourni était vide. |
| 403 (Interdit) | L’utilisateur, qui correspond à l’ID de session fourni, ne dispose pas d’un accès administrateur. |


**Exemple d’en-têtes de réponse :**

| En-tête de réponse | Exemple |
|---|---|
| Content-Type | `→application/json;charset=UTF-8` |
| Date | `→Wed, 05 Apr 2017 21:29:32 GMT` |
| Serveur | `→Apache-Coyote/1.1` |
| Transfer-Encoding | `→chunked` |


**Exemple de corps de réponse :**

<!-- [Copy](javascript:void(0);) -->

```
                {
                "subscriptions":                
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": "ObjId1234",
                "objCode": "TASK",
                "url": "http://test.test.net/test/1234",
                "eventType": "UPDATE",
                "authToken": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
                ],
                "meta":
                {
                "page": 1,
                "page_count": 2,
                "limit": 100,
                "total_count": 150
                }
                }            
```

Où

* **page** et **limit** sont les valeurs fournies dans la requête ou la valeur par défaut si aucune valeur n’est fournie.
* **page_count** est le nombre total de pages pouvant être interrogées.
* **total_count** est le nombre total d’abonnements correspondant à la requête.

### Requête par identifiant d’abonnement à l’événement

Vous pouvez rechercher des abonnements à des événements par identifiant d’abonnement à l’événement. La syntaxe de requête pour répertorier les abonnements d’événement est la suivante :

**URL de requête :**

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**En-têtes de requête :**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nom de l’en-tête</p> </th> 
   <th> <p>Valeur d’en-tête</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p>valeur sessionID</p> </td> 
  </tr> 
 </tbody> 
</table>

**Codes de réponse :**

| Code de réponse | Description |
|---|---|
| 200 (OK) | La requête renvoyée avec l’abonnement à l’événement correspondant à l’ID d’abonnement fourni. |
| 401 (Non autorisé) | L’ID de session fourni était vide. |
| 403 (Interdit) | L’utilisateur, qui correspond à l’ID de session fourni, ne dispose pas d’un accès administrateur. |


**Exemple de corps de réponse :**

<!-- [Copy](javascript:void(0);) -->

```
{
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customerId": "504f9640000013401be513579fbebffa",
                "objId": null,
                "objCode": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "eventType": "UPDATE",
                "authToken": "authTokenWorkfrontRocks1234_"
                }
```

## Filtrage des abonnements des événements

Le filtrage des abonnements aux événements peut être utilisé pour vous assurer que vous ne recevez que les messages pertinents. La création de filtres pour vos abonnements peut diminuer considérablement le nombre de messages que votre point de terminaison doit consommer.

Par exemple, un abonnement à un événement **UPDATE - TASK** peut être défini pour se déclencher uniquement lorsque l’événement **newState** d’une charge utile d’événement définit **taskStatus** comme **current**.

>[!IMPORTANT]
>
>Les attributs suivants s’appliquent au filtrage des abonnements aux événements

* Lorsqu’un champ de filtre a une valeur non vide, seuls les messages avec un **newState** contenant les clés de filtre et les valeurs sont envoyés à l’URL abonnée.
* Vous pouvez filtrer par données personnalisées incluses dans l’objet **newState** ET/OU **oldState**
* Les filtres sont évalués uniquement s’ils sont égaux ou non à une valeur spécifique.
* Si la syntaxe de votre filtre est incorrecte ou ne correspond à aucune donnée contenue dans le **newState** de la payload, un message de validation n’est pas renvoyé pour indiquer qu’une erreur s’est produite.
* Les filtres ne peuvent pas être mis à jour sur un abonnement existant ; un nouvel abonnement doit être créé avec de nouveaux paramètres de filtre.
* Plusieurs filtres peuvent être appliqués à un seul abonnement et celui-ci ne sera diffusé que lorsque toutes les conditions de filtre auront été remplies.
* L’application de plusieurs filtres à un seul abonnement équivaut à l’utilisation d’un opérateur logique **AND**.
* Plusieurs abonnements d’événement peuvent être appliqués à un seul objet tant qu’un ou plusieurs paramètres de champ d’abonnement d’événement sont différents entre chaque abonnement d’événement.
* Lorsque plusieurs abonnements d’événement sont attribués à un seul objet, tous les abonnements d’événement associés à cet objet peuvent être renvoyés à un seul point de terminaison. Cette pratique peut être utilisée comme alternative équivalente à l&#39;opérateur logique **OR** qui ne peut pas être défini à l&#39;aide des paramètres de filtre.

### Utilisation des opérateurs de comparaison

Vous pouvez spécifier un champ de comparaison avec le champ de filtrage. Utilisez un opérateur de comparaison dans ce champ pour filtrer les résultats comparatifs. Par exemple, vous pouvez créer un abonnement UPDATE - TASK qui envoie uniquement une charge utile si l’état de la tâche n’est PAS égal à actif. Vous pouvez utiliser les opérateurs de comparaison suivants :

#### eq : égal

Ce filtre permet aux messages de passer si la modification survenue correspond exactement à `fieldValue` dans le filtre. La valeur `fieldValue` est sensible à la casse.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "eq"
        }
    ]
}
```

#### ne : différent de

Ce filtre permet aux messages de passer si la modification survenue ne correspond pas exactement à `fieldValue` dans le filtre. La valeur `fieldValue` est sensible à la casse.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "ne"
        }
    ]
}
```

#### gt : supérieur à

Ce filtre permet aux messages de passer si la mise à jour de la `fieldName` spécifiée est supérieure à la valeur de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gt"
        }
    ]
}
```

#### gte : supérieur ou égal à

Ce filtre permet de transmettre des messages si la mise à jour de la `fieldName` spécifiée est supérieure ou égale à la valeur de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-11T16:00:00.000-0800",
            "comparison": "gte"
        }
    ]
}
```

#### lt : inférieur à

Ce filtre permet aux messages de passer si la mise à jour de la `fieldName` spécifiée est inférieure à la valeur de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lt"
        }
    ]
}
```

#### lte : inférieur ou égal à

Ce filtre permet de transmettre des messages si la mise à jour de la `fieldName` spécifiée est inférieure ou égale à la valeur de `fieldValue`.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "plannedCompletionDate",
            "fieldValue": "2022-12-18T16:00:00.000-0800",
            "comparison": "lte"
        }
    ]
}
```

#### contient

Ce filtre permet aux messages de passer si la modification survenue contient le `fieldValue` dans le filtre. La valeur `fieldValue` est sensible à la casse.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        }
    ]
}
```

#### modifier

Ce filtre permet aux messages de passer uniquement si le champ spécifié (`fieldName`) a une valeur différente dans les états ancien et nouveau. La mise à jour d’autres champs en plus de celui spécifié (`fieldName`) ne renverra pas cette modification.

>[!NOTE]
>
>`fieldValue` dans le tableau de filtres ci-dessous n’a aucun effet.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "",
            "comparison": "changed"
        }
    ]
}
```

#### state

Ce connecteur fait en sorte que le filtre s’applique au nouvel état ou à l’ancien état de l’objet créé ou mis à jour. Cela s’avère utile lorsque vous souhaitez savoir où une modification a été apportée d’un élément à un autre.
`oldState` n’est pas possible sur CREATE `eventTypes`.

>[!NOTE]
>
>L’abonnement ci-dessous avec le filtre donné renvoie uniquement les messages où le nom de la tâche contient `again` sur le `oldState`, ce qu’il était avant qu’une mise à jour ait été effectuée sur la tâche.
>Un cas pratique pour cela serait de trouver les messages objCode qui ont changé d’une chose à l’autre. Par exemple, pour connaître toutes les tâches qui ont changé de &quot;Recherche et nom&quot; en &quot;Nom de l’équipe de recherche Certains nom&quot;.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains",
            "state": "oldState"
        }
    ]
}
```

### Utilisation des champs de connecteur

Le champ `filterConnector` de la payload de l’abonnement vous permet de choisir comment les filtres doivent être appliqués. La valeur par défaut est &quot;AND&quot;, où les filtres doivent tous être `true` pour que le message d’abonnement passe. Si &quot;OR&quot; est spécifié, un seul filtre doit correspondre pour que le message d’abonnement passe.

```
{
    "objCode": "TASK",
    "eventType": "UPDATE",
    "authToken": "token",
    "url": "https://domain-for-subscription.com/API/endpoint/UpdatedTasks",
    "filters": [
        {
            "fieldName": "name",
            "fieldValue": "again",
            "comparison": "contains"
        },
        {
            "fieldName": "name",
            "fieldValue": "also",
            "comparison": "contains"
        }
    ],
    "filterConnector": "AND"
}
```

## Suppression d’abonnements à un événement

Lors de la suppression d’un HTTP Workfront, utilisez la méthode DELETE. La syntaxe de requête pour la suppression d’un abonnement d’événement unique par ID d’abonnement est la suivante :

**URL de requête :**

<!-- [Copy](javascript:void(0);) -->

```
DELETE https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/<SUBSCRIPTION ID>
```

**En-têtes de requête :**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nom de l’en-tête</p> </th> 
   <th> <p>Valeur d’en-tête</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> valeur sessionID </p> </td> 
  </tr> 
 </tbody> 
</table>

**Codes de réponse :**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Code de réponse</p> </th> 
   <th> Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (Aucun contenu)</td> 
   <td>Le serveur a supprimé l’abonnement à l’événement correspondant à l’ID d’abonnement fourni.</td> 
  </tr> 
  <tr> 
   <td>401 (Non autorisé)</td> 
   <td>L’ID de session fourni était vide.</td> 
  </tr> 
  <tr> 
   <td>403 (Interdit)</td> 
   <td>L’utilisateur qui correspond à l’ID de session fourni ne dispose pas d’un accès administrateur.</td> 
  </tr> 
  <tr> 
   <td>404 (Introuvable)</td> 
   <td>Le serveur n’a pas pu trouver un abonnement d’événement correspondant à l’ID d’abonnement fourni pour la suppression.</td> 
  </tr> 
 </tbody> 
</table>

**Exemple d’en-têtes de réponse :**

| En-tête de réponse | Exemple |
|---|---|
| Date | `→Wed, 05 Apr 2017 21:33:41 GMT` |
| Serveur | `→Apache-Coyote/1.1` |


**Exemple de corps de réponse :** S.O.

## Exemples de payloads d’événement

La payload qu’un utilisateur reçoit varie en fonction du type d’objet, mais il existe un format cohérent pour la diffusion de ces payloads variables.

Par exemple, les propriétés suivantes restent cohérentes pour toutes les payloads d’événement :

* eventType
* subscriptionId
* oldState
* newState
* eventTime

Bien que le format soit cohérent, les valeurs contenues dans les propriétés varient selon les objets et les types d’objets.

Les exemples de payloads pour un événement UPDATE et un événement CREATE sont présentés ci-dessous. Notez dans l’exemple UPDATE que les objets oldState et newState sont identiques, alors que dans l’exemple CREATE, l’objet oldState est vide (pas NULL).

Voici un exemple de payload pour un événement UPDATE :

<!-- [Copy](javascript:void(0);) -->

```
{
                  "eventType": "UPDATE",
                   "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                   "eventTime": {
                       "nano": 998000000,
                       "epochSecond": 1507319336
                   },
                   "newState": {
                "ID": "59d7ddf7000002322d791eb08bafddfb", 
                       "name": "EventSub Test updated",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:56.980-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,       "categoryID": null,
                      "status": "CUR",
                      "parameterValues": {}
                   },
                   "oldState": {
                       "ID": "59d7ddf7000002322d791eb08bafddfb",
                       "name": "EventSub Test 180fd595-63fb-4fa9-bd47-58bf6e53d964",
                       "objCode": "PROJ",
                       "entryDate": "2017-10-06T13:48:07.776-0600",
                       "accessorIDs": [
                           "544820df0000142362741fc0c368de19"
                       ],
                       "lastUpdateDate": "2017-10-06T13:48:07.792-0600",
                       "groupID": "544820df0000140f6a9c1faa7cacadd3",
                       "sponsorID": null,
                       "description": null,
                       "plannedCompletionDate": "2017-10-06T09:00:00.000-0600",
                       "enteredByID": "544820df0000142362741fc0c368de19",
                       "ownerID": "544820df0000142362741fc0c368de19",
                       "templateID": null,
                       "priority": 0,
                       "companyID": null,<
                       "portfolioID": null,
                       "referenceNumber": 1894,
                       "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                       "customerID": "544820df0000135b7719dcca654391f6",
                       "currency": null,
                       "categoryID": null,
                       "status": "CUR",
                       "parameterValues": {}
                   }
                }
```

Voici un exemple de payload pour un événement CREATE :

<!-- [Copy](javascript:void(0);) -->

```
{
                "eventType": "CREATE",
                "subscriptionId": "4028e3815ebf03a7015ebfa53b6d0002",
                "eventTime": {
                "nano": 232000000,
                "epochSecond": 1506453831
                },
                "newState": {
                "ID": "59caa946000000e07b0afc3383230c67",
                "name": "EventSub Test fe16d470-0a40-4290-92f4-6a0389fb536c",
                "objCode": "PROJ",
                "entryDate": "2017-09-26T13:23:50.746-0600",
                "accessorIDs": ["544820df0000142362741fc0c368de19"],
                "lastUpdateDate": "2017-09-26T13:23:50.927-0600",
                "groupID": "544820df0000140f6a9c1faa7cacadd3",
                "sponsorID": null,
                "description": null,
                "plannedCompletionDate": "2017-09-26T09:00:00.000-0600",
                "enteredByID": "544820df0000142362741fc0c368de19",
                "ownerID": "544820df0000142362741fc0c368de19",
                "templateID": null,
                "priority": 0,
                "companyID": null,
                "portfolioID": null,
                "referenceNumber": 1750,
                "lastUpdatedByID": "544820df0000142362741fc0c368de19",
                "customerID": "544820df0000135b7719dcca654391f6",
                "currency": null,
                "categoryID": null,
                "status": "CUR",
                "parameterValues": {}
                },
                "oldState": {}
            }
```

## Codage de base 64

Si un abonnement à un événement est rejeté en raison d&#39;un conflit entre les caractères spéciaux contenus dans vos abonnements à un événement et vos paramètres réseau, vous pouvez utiliser l&#39;encodage Base64 pour transmettre vos abonnements à un événement. Base64 est un ensemble de schémas de codage qui peuvent traduire n&#39;importe quelle donnée arbitraire dans un format de chaîne ASCII. Il est important de noter que Base64 n&#39;est pas une forme de cryptage de sécurité.

### Champ de codage de base 64

Le champ de codage base64Encoding est un champ facultatif qui est utilisé pour activer le codage Base64 des payloads d’abonnement aux événements. La valeur par défaut est false et les valeurs possibles sont : true, false et &quot;&quot; (vide).

### Exemple de requête utilisant le champ base64Encoding

Si une requête est effectuée à l’aide du champ de codage base64Encoding défini sur true, les objets **newState** et **oldState** de la payload sont fournis sous forme de chaînes de codage de base 64. Si le champ de codage base64Encoding est défini sur false, laissez le champ vide ou n’est pas inclus dans la requête, la payload renvoyée ne sera pas codée en base 64.

Voici un exemple de requête qui utilise le champ base64Encoding :

<!-- [Copy](javascript:void(0);) -->

```
{
                "objCode": "PROJ",
                "eventType": "UPDATE",
                "url": "http://requestb.in/ua5hi2ua"",
                "authToken": "EauthTokenWorkfrontRocks1234_",
                "base64Encoding": "true"
            }
```

### Exemples de payloads de réponse dans le codage de base 64

<!-- [Copy](javascript:void(0);) -->

```
                {
                "eventType": "UPDATE",
                "subscriptionId": "8a0d839d5ef32c9a015ef336a5ed0002",
                "eventTime": {
                "nano": 998000000,
                "epochSecond": 1507319336
                },
                "newState": "ewogICAgICAgIklEIjogIjU5ZDdkZGY3MDAwMDAyMzIyZDc5MWViMDhiYWZkZGZiIiwgCiAgICAgICAibmFtZSI6ICJFdmVudFN1YiBUZXN0IHVwZGF0ZWQiLAogICAgICAgIm9iakNvZGUiOiAiUFJPSiIsCiAgICAgICAiZW50cnlEYXRlIjogIjIwMTctMTAtMDZUMTM6NDg6MDcuNzc2LTA2MDAiLAogICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICI1NDQ4MjBkZjAwMDAxNDIzNjI3NDFmYzBjMzY4ZGUxOSIKICAgICAgIF0sCiAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODo1Ni45ODAtMDYwMCIsCiAgICAgICAiZ3JvdXBJRCI6ICI1NDQ4MjBkZjAwMDAxNDBmNmE5YzFmYWE3Y2FjYWRkMyIsCiAgICAgICAic3BvbnNvcklEIjogbnVsbCwKICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAicGxhbm5lZENvbXBsZXRpb25EYXRlIjogIjIwMTctMTAtMDZUMDk6MDA6MDAuMDAwLTA2MDAiLAogICAgICAgImVudGVyZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICJ0ZW1wbGF0ZUlEIjogbnVsbCwKICAgICAgICJwcmlvcml0eSI6IDAsCiAgICAgICAiY29tcGFueUlEIjogbnVsbCwKICAgICAgICJwb3J0Zm9saW9JRCI6IG51bGwsCiAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICJsYXN0VXBkYXRlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgImN1c3RvbWVySUQiOiAiNTQ0ODIwZGYwMDAwMTM1Yjc3MTlkY2NhNjU0MzkxZjYiLAogICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICJjYXRlZ29yeUlEIjogbnVsbCwKICAgICAgICJzdGF0dXMiOiAiQ1VSIiwKICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ==",
                "oldState": "ewogICAgICAgICJJRCI6ICI1OWQ3ZGRmNzAwMDAwMjMyMmQ3OTFlYjA4YmFmZGRmYiIsCiAgICAgICAgIm5hbWUiOiAiRXZlbnRTdWIgVGVzdCAxODBmZDU5NS02M2ZiLTRmYTktYmQ0Ny01OGJmNmU1M2Q5NjQiLAogICAgICAgICJvYmpDb2RlIjogIlBST0oiLAogICAgICAgICJlbnRyeURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43NzYtMDYwMCIsCiAgICAgICAgImFjY2Vzc29ySURzIjogWwogICAgICAgICAgICAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiCiAgICAgICAgXSwKICAgICAgICAibGFzdFVwZGF0ZURhdGUiOiAiMjAxNy0xMC0wNlQxMzo0ODowNy43OTItMDYwMCIsCiAgICAgICAgImdyb3VwSUQiOiAiNTQ0ODIwZGYwMDAwMTQwZjZhOWMxZmFhN2NhY2FkZDMiLAogICAgICAgICJzcG9uc29ySUQiOiBudWxsLAogICAgICAgICJkZXNjcmlwdGlvbiI6IG51bGwsCiAgICAgICAgInBsYW5uZWRDb21wbGV0aW9uRGF0ZSI6ICIyMDE3LTEwLTA2VDA5OjAwOjAwLjAwMC0wNjAwIiwKICAgICAgICAiZW50ZXJlZEJ5SUQiOiAiNTQ0ODIwZGYwMDAwMTQyMzYyNzQxZmMwYzM2OGRlMTkiLAogICAgICAgICJvd25lcklEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAidGVtcGxhdGVJRCI6IG51bGwsCiAgICAgICAgInByaW9yaXR5IjogMCwKICAgICAgICAiY29tcGFueUlEIjogbnVsbCw8CiAgICAgICAgInBvcnRmb2xpb0lEIjogbnVsbCwKICAgICAgICAicmVmZXJlbmNlTnVtYmVyIjogMTg5NCwKICAgICAgICAibGFzdFVwZGF0ZWRCeUlEIjogIjU0NDgyMGRmMDAwMDE0MjM2Mjc0MWZjMGMzNjhkZTE5IiwKICAgICAgICAiY3VzdG9tZXJJRCI6ICI1NDQ4MjBkZjAwMDAxMzViNzcxOWRjY2E2NTQzOTFmNiIsCiAgICAgICAgImN1cnJlbmN5IjogbnVsbCwKICAgICAgICAiY2F0ZWdvcnlJRCI6IG51bGwsCiAgICAgICAgInN0YXR1cyI6ICJDVVIiLAogICAgICAgICJwYXJhbWV0ZXJWYWx1ZXMiOiB7fQogICAgfQ=="
                }
 
```

## Méthode obsolète pour interroger tous les abonnements à un événement

Le point de terminaison d’API suivant est obsolète et ne doit pas être utilisé pour les nouvelles implémentations. Nous vous recommandons également de passer d’anciennes implémentations à la méthode dans la section **Abonnements à des événements de requêtage** décrite ci-dessus.

Vous pouvez interroger tous les abonnements à un événement pour un client, comme spécifié par la valeur sessionID . La syntaxe de requête permettant de répertorier tous les abonnements d’événement pour un client spécifique est l’URL suivante :

<!-- [Copy](javascript:void(0);) -->

```
GET https://<HOSTNAME>/attask/eventsubscription/api/v1/subscriptions/list
```

**En-têtes de requête :**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Nom de l’en-tête</p> </th> 
   <th> <p>Valeur d’en-tête</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>sessionID</p> </td> 
   <td> <p> valeur sessionID </p> </td> 
  </tr> 
 </tbody> 
</table>

**Codes de réponse :**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Code de réponse</p> </th> 
   <th> Description</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>200 (Aucun contenu)</td> 
   <td>La requête a renvoyé avec succès tous les abonnements d’événement trouvés pour l’utilisateur.</td> 
  </tr> 
  <tr> 
   <td>401 (Non autorisé)</td> 
   <td>L’ID de session fourni était vide.</td> 
  </tr> 
  <tr> 
   <td>403 (Interdit)</td> 
   <td>L’utilisateur qui correspond à l’ID de session fourni ne dispose pas d’un accès administrateur.</td> 
  </tr> 
 </tbody> 
</table>

 

### Exemple de corps de réponse

<!-- [Copy](javascript:void(0);) -->

```
                [
                {
                "id": "37c4bcf5-e0b5-4256-aba3-a51cba7bf997",
                "customer_id": "504f9640000013401be513579fbebffa",
                "obj_id": "ObjId1234",
                "obj_code": "TASK",
                "url": "http://test.test.net/test/1234",
                "event_type": "UPDATE",
                "auth_token": "auth_token"
                },
                {
                "id": "750a636c-5628-48f5-ba26-26b7ce537ac2",
                "customer_d": "504f9640000013401be513579fbebffa",
                "obj_id": null,
                "obj_code": "PROJ",
                "url": "http://requestb.in/ua5hi2ua",
                "event_type": "UPDATE",
                "auth_token": "authTokenWorkfrontRocks1234_"
                }                
                ]
```
