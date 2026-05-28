---
title: Principes de base des API de planification d’Adobe Workfront
description: L’API Planning d’Adobe Workfront a pour objectif de simplifier la création d’intégrations avec Planning en introduisant une architecture REST-ful qui fonctionne via HTTP. Ce document suppose que vous connaissez les réponses REST et JSON et décrit l’approche adoptée par l’API Planning.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: fdbe3945f59306fc26424d7e88b799d9dcaea4da
workflow-type: tm+mt
source-wordcount: '2206'
ht-degree: 4%

---


# Principes de base des API Adobe Workfront Planning

{{planning-important-intro}}

<!--

Lilit asked me to hide everything in this current article and replace it with her version of it. I kept just the Field type and search modifier section. The rest of the article is a re-write of the original from Lilit. 

She also said we need to reword how we organize the version features, after we get more versions released but for now, she calls out what's different in V1 than the current (V2) with almost every feature. 

-->

L’API Planning d’Adobe Workfront a pour objectif de simplifier la création d’intégrations avec Planning en introduisant une architecture RESTful qui fonctionne via HTTP. Ce document suppose que vous connaissez les réponses REST et JSON.

Pour obtenir une référence complète des points d’entrée, des schémas de requête/réponse et des détails spécifiques à la version, consultez la [documentation du développeur de l’API Workfront Planning](https://developer.adobe.com/wf-planning).

## Authentification

L’API Workfront Planning utilise OAuth 2.0 pour l’authentification. Les informations d’identification sont configurées via le Adobe Developer Console.

Nous prenons en charge les deux flux suivants en fonction de votre type d’intégration :

* **Authentification de serveur à serveur (JWT)** : pour les intégrations automatisées et les services back-end sans interaction utilisateur. Utilise les informations d’identification de serveur à serveur OAuth (octroi des informations d’identification client — votre application s’authentifie directement à l’aide de son identifiant client et de son secret pour obtenir un jeton d’accès, sans connexion de l’utilisateur ni étape de consentement).

  Pour plus d’informations, voir [Authentification de serveur à serveur](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/).

* **Authentification de l’utilisateur (flux de code d’autorisation)** : pour les intégrations agissant pour le compte d’un utilisateur spécifique. Utilise les informations d’identification de l’application web OAuth ou de l’application monopage (octroi du code d’autorisation : l’utilisateur se connecte et donne son consentement, après quoi votre application reçoit un code d’autorisation qu’elle échange contre un jeton d’accès).

  Pour plus d’informations, voir [Authentification utilisateur](https://developer.adobe.com/developer-console/docs/guides/authentication/UserAuthentication/).

Pour commencer, créez un projet dans Adobe Developer Console et ajoutez l’API Workfront Planning pour obtenir vos informations d’identification.

Pour configurer les informations d’identification, créez une application OAuth2 dans Workfront.

Pour plus d’informations, voir [Création d’applications OAuth2 pour les intégrations Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

>[!NOTE]
>
>Le point d’entrée `/login` et l’authentification par clé API ne sont pas pris en charge pour Workfront Planning. N’utilisez pas de paramètres `sessionID` ou `apiKey`.


## Contrôle de version des API

Le contrôle de version de l’API Planning s’effectue via le chemin URL.

Voici les versions actuellement prises en charge :

| Version | Date de publication |
|-----------|----------------|
| Version 1 | Juillet 2024 |
| Version 2 | Mai 2026 |

<!--

(*****************add deprecation date column above, when we have one*****************)

-->


Pour plus d’informations sur les versions actuellement prises en charge, consultez l’article [Documentation destinée aux développeurs et développeuses de l’API Workfront Planning](https://developer.adobe.com/wf-planning).

Nous vous recommandons de cibler explicitement une version dans toutes les intégrations :

```
https://{customer-domain}/maestro/api/v2/...
```

Lorsqu’une nouvelle version majeure est publiée, la version précédente reste disponible jusqu’à ce qu’une date d’obsolescence soit communiquée.

Consultez les notes de mise à jour de Workfront pour rester informé des modifications apportées à l’API.


## Structure et opérations de l’URL

Les objets sont manipulés en envoyant une requête HTTP à leur URI unique. L’opération est spécifiée par la méthode HTTP.

| Méthode | Opération |
|----------|----------------------------------------------------------------------|
| GET | Récupérer un seul objet par ID ou rechercher/répertorier des objets |
| POST | Créer un nouvel objet |
| PUT | Remplacer un objet existant (mise à jour complète) |
| PATCH | Mettre à jour partiellement un objet existant (seuls les champs fournis sont modifiés) |
| SUPPRIMER | Suppression d’un objet |

>[!NOTE]
>
>**Remarque pour la version 1 :** `PATCH` n’est pas pris en charge dans la version 1. Utilisez `PUT` pour toutes les mises à jour.


Pour obtenir des chemins d’accès complets aux points d’entrée et des exemples de requête/réponse, consultez la **référence d’API** à l’adresse [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning).

## Codes d’état HTTP

L’API Planning renvoie des codes d’état HTTP standard :

| Code | Signification |
|------------------------|-------------------------------------------------|
| 200 OK | GET, PUT ou PATCH réussi |
| 201 Créé | POST réussi (ressource créée) |
| 204 Pas de contenu | DELETE réussie |
| 207 Statut multiple | Opération en bloc terminée avec des résultats mitigés, où certains éléments ont réussi et d’autres ont échoué. Vérifiez les réponses de chaque élément pour plus de détails. |
| 400 Requête Incorrecte | Requête non valide — voir la réponse d’erreur pour plus de détails |
| 401 Non Autorisé | Jeton d’authentification manquant ou non valide |
| 403 Interdit | Autorisations authentifiées mais insuffisantes |
| 404 Introuvable | La ressource n’existe pas |
| 409 Conflit | Conflit d&#39;écriture, la ressource a été modifiée par une autre requête. Réessayez avec la dernière version. |
| 429 Too Many Requests | Limite de taux dépassée |

>[!NOTE]
>
>**Remarque sur la version 1 :** la version 1 renvoie des `200 OK` pour toutes les opérations réussies, y compris POST et DELETE.


## Gestion des erreurs

L’API Planning renvoie des erreurs dans un format cohérent. Chaque réponse d’erreur comprend un message lisible par l’utilisateur, un code d’erreur lisible par la machine et un identifiant de demande pour l’escalade de l’assistance.

Exemple de réponse d’erreur :

```
json
{
  "title": "Validation failed",
  "status": 400,
  "detail": "Request validation failed. See 'errors' for details.",
  "errorCode": "VALIDATION_FAILED",
  "requestId": "req-123",
  "errors": [
    { "field": "name", "message": "must not be blank" }
  ]
}
```

Utilisez `errorCode` (non `status`) pour piloter la gestion des erreurs de programmation. Il fournit la classification la plus spécifique de l’échec.

>[!NOTE]
>
>**Note de la version 1 :** les réponses d’erreur de la version 1 utilisent un champ de `type` numérique (par exemple, `40001`) au lieu d’un `errorCode` de chaîne, et encapsulent les détails dans un objet `report` plutôt que dans un champ de `detail` de niveau supérieur.

## Filtrer les enregistrements

Utilisez le paramètre `filter` dans les demandes de recherche d’enregistrements pour renvoyer uniquement les enregistrements correspondant à des critères spécifiques. Pour les requêtes POST, `filter` est une propriété JSON dans le corps de la requête. Pour les requêtes GET, `filter` est un paramètre de requête contenant un groupe de filtres codés JSON. Les filtres utilisent une structure composite typée avec des opérateurs logiques explicites.

```
json
{
  "filter": {
    "operator": "AND",
    "conditions": [
      { "fieldId": "<fieldId>", "condition": "IS", "value": "Active" },
      { "fieldId": "<fieldId>", "condition": "CONTAINS", "value": "marketing" }
    ]
  }
}
```

Les filtres peuvent être imbriqués à l’aide d’opérateurs `AND`/`OR` pour créer des conditions composites :

```
json
{
  "filter": {
    "operator": "OR",
    "conditions": [
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "BETWEEN", "value": ["2024-03-31T20:00:00.000Z", "2024-04-01T20:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "active" }
        ]
      },
      {
        "operator": "AND",
        "conditions": [
          { "fieldId": "<fieldId>", "condition": "IS_BETWEEN", "value": ["2024-04-15T00:00:00.000Z", "2024-04-16T00:00:00.000Z"] },
          { "fieldId": "<fieldId>", "condition": "IS", "value": "planned" }
        ]
      }
    ]
  }
}
```

>[!NOTE]
>
>**Remarque sur la version 1 :** la version 1 utilise des opérateurs non typés de style Mongo dans un objet `filters`. Les opérateurs sont précédés du préfixe `$` (par exemple, `$and`, `$or`, `$is`, `$contains`, `$isBetween`). Les paramètres de pagination (`offset`, `limit`) et `recordTypeId` sont transmis dans le corps de la requête plutôt que comme chemin d’URL et paramètres de requête.


## Types de champs et modificateurs de recherche

Vous pouvez utiliser des modificateurs et des filtres avec des champs pour contrôler les données qui seront renvoyées dans les résultats.

Pour obtenir des exemples, consultez la documentation du développeur de l’API Workfront Planning [&#128279;](https://developer.adobe.com/wf-planning/).

### Utilisation des modificateurs de recherche

Workfront Planning prend en charge les modificateurs de recherche suivants :


<table style="table-layout:auto"> 
  <colgroup><col class="c1"><col class="c2"><col class="c3"><col class="c4"></colgroup>
  <thead>
    <tr>
      <th>Modificateur</th>
      <th>Exemple</th>
      <th>Description</th>
      <th>Valeurs possibles</th>
    </tr>
  </thead>
  <tbody>
    <tr><td class="modifier">CONTIENT</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« CONTAINS »,« value »:« product »}</td><td>Retourne les enregistrements dont la valeur du champ contient le filtre</td><td class="possible">« Nouveau lancement de produit »</td></tr>
    <tr><td class="modifier">NE_CONTIENT_PAS</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« Does_NOT_CONTAIN »,« value »:« product »}</td><td>Renvoie les enregistrements dont la valeur du champ ne contient pas le filtre</td><td class="possible">« Nouveau lancement »</td></tr>
    <tr><td class="modifier">EST</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« IS »,« value »:« nouveau lancement de produit »}</td><td>Renvoie les enregistrements dont la valeur du champ correspond exactement au filtre</td><td class="possible">« Nouveau lancement de produit »</td></tr>
    <tr><td class="modifier">IS_NOT</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« IS_NOT »,« value »:« product »}</td><td>Renvoie les enregistrements dont la valeur du champ ne correspond pas exactement au filtre</td><td class="possible">« Nouveau lancement de produit »</td></tr>
    <tr><td class="modifier">IS_EMPTY</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« IS_EMPTY »}</td><td>Retourne les enregistrements dont la valeur du champ est vide</td><td class="possible">« » ou nul</td></tr>
    <tr><td class="modifier">IS_NOT_EMPTY</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« IS_NOT_EMPTY »}</td><td>Retourne les enregistrements dont la valeur du champ n’est pas vide</td><td class="possible">« Nouveau lancement de produit »</td></tr>
    <tr><td class="modifier">GREATER_THAN</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« GREATER_THAN »,« value »:« 10 »}</td><td>Renvoie les enregistrements dont la valeur du champ est supérieure au filtre</td><td class="possible">"11"</td></tr>
    <tr><td class="modifier">GREATER_THAN_OR_EQUAL</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« GREATER_THAN_OR_EQUAL »,« value »:« 10 »}</td><td>Renvoie les enregistrements dont la valeur du champ est supérieure ou égale au filtre</td><td class="possible">"10", "11"</td></tr>
    <tr><td class="modifier">INFÉRIEUR À</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« LESS_THAN »,« value »:« 10 »}</td><td>Renvoie les enregistrements dont la valeur du champ est inférieure au filtre</td><td class="possible">"9"</td></tr>
    <tr><td class="modifier">LESS_THAN_OR_EQUAL</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« LESS_THAN_OR_EQUAL »,« value »:« 10 »}</td><td>Renvoie les enregistrements dont la valeur du champ est inférieure ou égale au filtre</td><td class="possible">"9", "10"</td></tr>
    <tr><td class="modifier">IS_BETWEEN</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« IS_BETWEEN »,« value »:[« 2024-01-01 »,« 2024-12-31 »]}</td><td>Renvoie les enregistrements dont la valeur du champ est comprise entre les deux valeurs de filtre</td><td class="possible">["2024-03-01","2024-06-30"]</td></tr>
    <tr><td class="modifier">IS_NOT_BETWEEN</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« IS_NOT_BETWEEN »,« value »:[« 2024-01-01 »,« 2024-12-31 »]}</td><td>Renvoie les enregistrements dont la valeur du champ ne se situe pas entre les deux valeurs de filtre</td><td class="possible">["2023-01-01","2025-06-30"]</td></tr>
    <tr><td class="modifier">IS_AFTER</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« IS_AFTER »,« value »:« 2024-01-01 »}</td><td>Renvoie les enregistrements dont la valeur du champ de date est postérieure au filtre</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_BEFORE</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« IS_BEFORE »,« value »:« 2024-12-31 »}</td><td>Renvoie les enregistrements dont la valeur du champ de date est antérieure au filtre</td><td class="possible">"2024-06-01"</td></tr>
    <tr><td class="modifier">IS_ANY_OF</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« IS_ANY_OF »,« value »:[« Active »,« Planned »]}</td><td>Renvoie les enregistrements dont la valeur du champ correspond à n’importe quelle valeur de la liste de filtres</td><td class="possible">[« Actif »,« Prévu »,« Terminé »]</td></tr>
    <tr><td class="modifier">IS_NONE_OF</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« IS_NONE_OF »,« value »:[« Active »,« Planned »]}</td><td>Renvoie les enregistrements dont la valeur du champ ne correspond à aucune des valeurs de la liste de filtres</td><td class="possible">[« Actif »,« Prévu »]</td></tr>
    <tr><td class="modifier">HAS_ANY_OF</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« HAS_ANY_OF »,« value »:[« Tag1 »,« Tag2 »]}</td><td>Renvoie les enregistrements dont le champ à plusieurs valeurs contient l’une des valeurs de filtre</td><td class="possible">[« Tag1 »,« Tag2 »]</td></tr>
    <tr><td class="modifier">HAS_ALL_OF</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« HAS_ALL_OF »,« value »:[« Tag1 »,« Tag2 »]}</td><td>Renvoie les enregistrements dont le champ à plusieurs valeurs contient toutes les valeurs de filtre</td><td class="possible">[« Tag1 »,« Tag2 »]</td></tr>
    <tr><td class="modifier">IS_EXACTLY</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« IS_EXACTLY »,« value »:[« Tag1 »]}</td><td>Renvoie les enregistrements dont le champ à plusieurs valeurs contient exactement les valeurs de filtre et aucune autre</td><td class="possible">[« Tag1 »]</td></tr>
    <tr><td class="modifier">HAS_NONE_OF</td><td class="example">{« fieldId »:« &lt;id&gt; »,« condition »:« HAS_NONE_OF »,« value »:[« Tag1 »]}</td><td>Renvoie les enregistrements dont le champ à plusieurs valeurs ne contient aucune des valeurs de filtre</td><td class="possible">[« Tag1 »]</td></tr>
  </tbody>
</table>


>[!NOTE]
>
>Note de la version 1 : les noms de modificateurs V1 utilisent `$-prefixed camelCase` (par exemple `$contains`, `$isNot`, `$isEmpty`, `$greaterThan`, `$greaterThanOrEqual`, `$lessThan`, `$lessThanOrEqual`, `$isBetween`, `$isNotBetween`, `$isAnyOf`, `$hasAllOf`). Le comportement de chaque modificateur est le même.


## Conditions de filtrage prises en charge par type de champ

| Type de champ | Conditions prises en charge |
|-----------------------------|--------------------------------------------------------------------------------------------------------------|
| texte, texte long | CONTAINS, Does_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| nombre, pourcentage, devise | IS, IS_NOT, GREATER_THAN, GREATER_THAN_OR_EQUAL, LESS_THAN, LESS_THAN_OR_EQUAL, IS_EMPTY, IS_NOT_EMPTY |
| Date | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY, IS_NOT_EMPTY |
| à sélection unique | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| sélection multiple, utilisateur | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| booléen | EST |
| formule | CONTAINS, Does_NOT_CONTAIN, IS, IS_NOT, IS_EMPTY, IS_NOT_EMPTY |
| created-by | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF |
| mis à jour par | IS, IS_NOT, IS_ANY_OF, IS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| created-at | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN |
| updated-at | IS, IS_NOT, IS_AFTER, IS_BEFORE, IS_BETWEEN, IS_NOT_BETWEEN, IS_EMPTY, IS_NOT_EMPTY, IS_NOT_EMPTY |
| référence | HAS_ANY_OF, HAS_ALL_OF, IS_EXACTLY, HAS_NONE_OF, IS_EMPTY, IS_NOT_EMPTY |
| recherche | Dépend du type de champ lié |

>[!NOTE]
>
>**Remarque sur la version 1 :** la version 1 utilise des noms d’opérateurs avec préfixe `$` (par exemple `$contains`, `$greaterThan`, `$isAnyOf`, `$hasAllOf`). L’ensemble des conditions prises en charge par type de champ est le même.

## Filtrer par champs Personnes

Les filtres de champ de personne (`user`, `created-by`, `updated-by`, `approved-by`) acceptent les ID utilisateur Adobe IMS et Workfront. Une valeur de chaîne simple est interprétée comme un identifiant utilisateur Adobe IMS.

Pour définir le type d’identifiant afin de vérifier l’ID utilisateur Workfront, vous devez transmettre explicitement les paramètres `id` et `idType`. Les valeurs prises en charge pour `idType` sont « `WF` » pour les ID utilisateur Workfront et « `IMS` » pour les ID utilisateur Adobe IMS.

```
{ 
  "filter": { 
   "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<userFieldId>", 
        "condition": "HAS_ANY_OF", 
        "value": [ 
          { "id": "63e3b13000078c1795146248182d15dc", "idType": "WF" } 
        ] 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
> Remarque pour la version 1 : la version 1 prend uniquement en charge le filtrage par identifiant IMS des utilisateurs.

## Filtrer les champs de référence externes par ID externe

Les champs de référence externes lient les enregistrements aux objets d’autres systèmes Adobe (tels que les projets Workfront ou AEM Assets). En interne, Planning affecte des ID d&#39;enregistrement Planning à ces objets. Pour filtrer ces champs directement en fonction de leur ID d’objet d’origine, ajoutez des `"matchExternalId": true` à une condition de filtre.

Cet indicateur n&#39;est valide que pour les champs de référence où `referenceOptions.isExternal` est `true` ; il est ignoré pour les champs de référence non externes. Si une valeur de chaîne unique ne peut pas être résolue, la requête échoue avec `400 Bad Request`. Si une valeur de liste est fournie, les entrées non résolues passent inchangées et ne correspondent tout simplement pas.

```
{ 
  "filter": { 
    "operator": "AND", 
    "conditions": [ 
      { 
        "fieldId": "<externalReferenceFieldId>", 
        "condition": "IS_ANY_OF", 
        "value": [ 
          "5f6a4f6e00000123456789abcdef0123", 
          "/content/dam/wknd/en/adventures/bali-surf-camp" 
        ], 
        "matchExternalId": true 
      } 
    ] 
  } 
} 
```

>[!NOTE]
>
>Remarque concernant la version 1 : la version V1 ne prend pas en charge le filtrage par ID d’objets externes.

## Champs de connexion externe

Les types d&#39;enregistrements Planning peuvent héberger des champs de référence externes qui lient des enregistrements à des objets dans d&#39;autres systèmes Adobe au lieu d&#39;autres types d&#39;enregistrements Planning.

Pour créer un champ de référence externe via l’API, définissez `referenceOptions.recordTypeId` sur un nouveau champ de `REFERENCE` l’identifiant du type d’enregistrement externe souhaité. Le serveur dérive automatiquement les `referenceOptions.isExternal=true` et les métadonnées de connexion (`connectionName, objectName`) du type d’enregistrement cible.

Les types d’objets externes pris en charge comprennent les objets Workfront (projets, tâches, programmes, portfolios, entreprises, groupes, équipes, utilisateurs) et AEM Assets (ressources, fragments de contenu).

>[!NOTE]
>
>Remarque concernant la version 1 : la version V1 ne prend pas en charge la création de champs de connexion externe.


## Tri

Triez les résultats en fonction de n’importe quel champ en incluant un tableau de `sort` dans votre requête :

```
json
{
  "sort": [
    { "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" },
    { "fieldId": "F658afcbd4a0273c67c346fd5", "direction": "desc" }
  ]
}
```

Plusieurs champs de tri sont évalués dans l’ordre. Appliquez toujours un tri lors de la pagination afin de garantir un ordre cohérent sur toutes les pages.

Pour regrouper des résultats, incluez un tableau de groupe à côté de trier :

```
{ 
  "sort": [{ "fieldId": "F001", "direction": "asc" }], 
  "group": [{ "fieldId": "F002", "direction": "asc" }] 
} 
```

>[!NOTE]
>
>Remarque concernant la version 1 : la version 1 utilise `sorting` (non `sort`), `groupingFieldIds` (tableau d’identifiants de champ et non d’objets `group`) et la `rowOrderViewId` désormais obsolète pour appliquer l’ordre des lignes d’une vue existante. Aucun de ces paramètres V1 n’est pris en charge dans la version

## Projection de champ

Pour limiter les champs renvoyés dans une réponse, utilisez les paramètres de requête `fieldIds` ou `fieldAliases` avec une liste séparée par des virgules. Cela réduit la taille de la payload de réponse et est recommandé pour les intégrations à volume élevé ou sensibles à la latence.

>[!NOTE]
>
>**Note pour la version 1 :** la version 1 utilise le `?attributes=` pour la projection (par exemple `?attributes=data,createdBy`) plutôt que le `?fieldIds=` ou le `?fieldAliases=`.

## Pagination

L’API Planning prend en charge les réponses paginées pour gérer les jeux de données volumineux.

* La **pagination basée sur le curseur** est utilisée pour les espaces de travail, les types d’enregistrements, les champs et les vues. Transmettez une valeur `cursor` de la réponse précédente pour récupérer la page suivante. Les réponses basées sur le curseur incluent un indicateur hasMore pour indiquer s’il y a d’autres pages ou non.
* La **pagination basée sur la page** est utilisée pour la recherche d’enregistrements. Utilisez `page` et `size` comme paramètres de requête. Appliquez toujours un tri lors de la pagination afin de garantir un ordre cohérent sur toutes les pages. Notez que la pagination est basée sur zéro. Par conséquent, pour récupérer les résultats de la deuxième page, utilisez « `page=1` » comme paramètre.

Par exemple, utilisez la requête suivante pour récupérer la deuxième page de 500 enregistrements à partir d’une recherche d’enregistrements :

```
POST /v2/record-types/{recordTypeId}/records/search?page=1&size=500 
{ 
  "sort": [{ "fieldId": "F6527ecb25df57c441d92b9fc", "direction": "asc" }], 
  "filter": { "operator": "AND", "conditions": [ 
    { "fieldId": "<fieldId>", "condition": "IS", "value": "active" } 
  ] } 
} 
```

Toutes les réponses paginées incluent une enveloppe structurée indiquant si d’autres résultats sont disponibles. Appliquez toujours un tri lors de la pagination afin de garantir un ordre cohérent sur toutes les pages.

>[!NOTE]
>
> **Note pour la version 1 :** la version V1 utilise `offset` et `limit` transmises dans le corps de la requête (500 par défaut, 2 000 max.). Pour récupérer les enregistrements 2001-4000, définissez « `offset` »: « `2000` », « `limit` »: « `2000` » dans le corps de la requête. La réponse renvoie un tableau d’enregistrements plats avec un champ `totalCount`.

## Opérations en masse

L’API Planning prend en charge la création, la mise à jour, l’application de correctifs et la suppression en bloc d’enregistrements dans une seule requête. Consultez la **référence d’API** à l’adresse [developer.adobe.com/wf-planning](https://developer.adobe.com/wf-planning) pour connaître les chemins de point d’entrée, les formats de requête et les limites d’enregistrement par opération.

>[!NOTE]
>
>**Remarque sur la version 1 :** les opérations en bloc ne sont pas disponibles dans la version 1.


## Autorisations

Les autorisations d’entités sont gérées par le biais d’une API d’autorisations dédiée, distincte des points d’entrée des ressources eux-mêmes. Vous pouvez ainsi lire les autorisations actuelles, gérer la liste de partage et gérer les demandes d’accès indépendamment des opérations sur les données. Pour plus d’informations, consultez la section « Références de l’API » dans l’article [API Workfront Planning](https://developer.adobe.com/wf-planning).

>[!NOTE]
>
>**Remarque sur la version 1 :** la version 1 n’expose pas d’API d’autorisations publiques. Le niveau d’autorisation est directement incorporé dans les DTO de réponse de ressource.

## Utilisation de l’API Planning avec des formulaires personnalisés Workfront

Vous pouvez appeler l’API Planning à partir d’un champ de recherche externe dans un formulaire personnalisé Workfront pour faire apparaître les données Planning directement dans les objets Workfront. Pour plus d’informations, voir [Exemples du champ de recherche externe dans un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## Ressources connexes

Pour plus d’informations sur les API, consultez également les articles suivants :

* [API Workfront Planning](https://developer.adobe.com/wf-planning) documentation et référence pour les développeurs
* [Commencer à utiliser Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md)
* [Vue d’ensemble de l’accès à Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md)
* [Créer des applications OAuth2 pour les intégrations Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md)

<!--

Our version of this article before Lilit replaced it with the above: 

The goal for the Adobe Workfront Planning API is to simplify building integrations with Planning by introducing a REST-ful architecture that operates over HTTP. This document assumes you are familiar with REST and JSON responses and describes the approach taken by the Planning API.  

A familiarity with the Workfront Planning schema will assist you in understanding the database relationships that can be utilized to pull data out of Workfront Planning for integration purposes. 

You can call the planning API from an External lookup field in a Workfront custom form.

For more information on External lookup fields, see [Examples of the External lookup field in a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>When using the Planning API, all user-related information will be returned using the Adobe Identity Management System (IMS) user ID, and not the Workfront user ID.
>
>For information, see [Manage users in the Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).  

## Workfront Planning API versions

* Version 1 - released in July 2024 

  For more information, see the section [Workfront Planning API Version 1](#workfront-planning-api-version-1) in this article. 

* Version 2 - released in May 2026

  For more information, see the section [Workfront Planning API Version 2](#workfront-planning-api-version-2) in this article.


## Workfront Planning API Version 1

Workfront Planning API Version 1 was released in July 2024.

The following sections described functionality that was made available in the Workfront API Version 1. 

All future API version will contain the same functionality, unless otherwise specified. 

### Operations 

Objects are manipulated by sending an HTTP request to their unique URI. The operation to be performed is specified by the HTTP method. 

The standard HTTP methods correspond to the following operations: 

* **GET** - Retrieves an object by ID, searches for all objects by a query 
* **POST** - Inserts a new object 
* **PUT** - Edits an existing object 
* **DELETE** - Deletes an object 

For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

### Field types and search modifiers used with them 

You can use modifiers and filters with fields to control what data will be returned in results. 

For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).

#### Using search modifiers 

Workfront Planning supports the following search modifiers: 

<table>
    <tr>
        <td><b>Modifier</b></td>
        <td><b>Example</b></td>
        <td><b>Description</b></td>
        <td><b>Possible Values</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Returns records whose field value contains the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Returns records where the field value does not contain the filter  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Returns records whose field value exactly match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Returns records whose field value exactly is not match the filter  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is empty  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Returns records whose field value is not empty  </td>
        <td>"New Product Launch"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Returns records whose field value is greater than the filter  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is greater than or equal the filter  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Returns records whose field value is less than the filter  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Returns records whose field value is less than or equal the filter </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is after the filter  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Returns records whose field value is before the filter </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is between the filter  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Returns records whose field value is not between the filter  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is any of the filter  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is none of the filter </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has any of the filter  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has all of the filter  </td>
        <td><ul><li>["active", "completed"]   </li><li>["active", "completed", "finished"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value has none of the filter </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Returns records whose field value is exactly the filter  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>
 
#### Field types 

Below is the list of supported field types and what search modifiers can be used with each of those field types  

| Field Type | Supported search modifiers |
|---|---|
| text |$contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| number | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| percentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| single-select | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| boolean | $is |
| user | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| formula | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| updated-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| lookup | Depends on the linked field |

### Using "And" and "Or" statements 

In the API call you can have filters that are based on several criteria combined by $and" and "$or" statements  

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### Using the fields request parameter 

You can use the fields request parameter to specify a comma-separated list of specific fields that should be returned. These field names are case-sensitive.  

For example, the request 

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
..
```

returns a response similar to the following: 

  
```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Sorting query results in the API 

You can sort your results by any field if you append the following to your API call: 


`/v1/records/search`

Request body:

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### Query limits and paginated responses 

By default, Planning API requests return 500 results, starting from the beginning of the list. To override the default limitation for number of results, you can use the `limit` parameter in your requests and set it to a different number, up to 2000 results.  

We recommend that you consider using paginated responses for large datasets by adding the `offset` parameter to your requests. Paginated responses allow you to specify the location of the first result that should be returned. 

For example, if you want to return the results 2001-4000, you can use the following request. This example returns 2000 records that are in active status, starting from the 2001st result: 

`POST /v1/records/search`


Request body: 

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

To make sure your results are properly paginated, use a sorting parameter. This allows the results to be returned in the same order, so that the pagination does not repeat or skip results. 

For more information on sorting, see [Sorting query results in the API](#sorting-query-results-in-the-api) in this article.


Lilit did not want this organized like this - keeping this for reference: 

## Workfront Planning API Version 2

Version of the Workfront Planning API was released in May 2026. 

In addition to all the information contained in Version 1, the following enhancements were added in Version 2: 

* Search by the user's Workfront ID field instead of the user's IMS ID.

    This is applicable to custom People fields, as well as system fields such as Created By and Last Updated By fields.

* Ability to search by external connections (Workfront or AEM objects) via the API.

* Ability to link cross-workspace shared records through API. 

* Support all CRUD operations for workspaces, record types, fields, and views. 

* Enable permissions sharing for all sharable entities via API. 

    This includes workspaces, record types, and views. (***********and in the future also records and fields.*********)

* Support for uploading record thumbnail through API. 

-->