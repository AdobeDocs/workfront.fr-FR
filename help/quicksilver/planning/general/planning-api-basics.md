---
title: Principes de base des API de planification Adobe Workfront
description: L’objectif de l’API de planification d’Adobe Workfront est de simplifier la création d’intégrations avec la planification en introduisant une architecture REST-ful qui fonctionne sur HTTP. Ce document suppose que vous connaissez les réponses REST et JSON et décrit l’approche adoptée par l’API de planification.
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: 20e8d45264f9441d9576c7d4d5521e4f6053a7f3
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 12%

---


# Principes de base des API de planification Adobe Workfront

{{planning-important-intro}}

L’objectif de l’API de planification d’Adobe Workfront est de simplifier la création d’intégrations avec la planification en introduisant une architecture REST-ful qui fonctionne sur HTTP. Ce document suppose que vous connaissez les réponses REST et JSON et décrit l’approche adoptée par l’API de planification.

Une familiarité avec le schéma de planification Workfront vous aidera à comprendre les relations de base de données qui peuvent être utilisées pour extraire des données de la planification Workfront à des fins d’intégration.

Vous pouvez appeler l’API de planification à partir d’un champ de recherche externe dans un formulaire personnalisé Workfront.

Pour plus d’informations sur les champs de recherche externes, voir [Exemples du champ de recherche externe dans un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

## URL de l’API de planification Workfront

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### Opérations

Les objets sont manipulés en envoyant une requête HTTP à leur URI unique. L’opération à effectuer est spécifiée par la méthode HTTP.

Les méthodes HTTP standard correspondent aux opérations suivantes :

* **GET** - Récupère un objet par identifiant, recherche tous les objets par une requête
* **POST** - Insère un nouvel objet.
* **PUT** - Modifie un objet existant.
* **DELETE** - Supprime un objet.

Pour plus d’informations et d’exemples sur chaque opération, consultez la [documentation destinée aux développeurs de l’API de planification Workfront](https://developer.adobe.com/wf-planning/).

### Types de champ et modificateurs de recherche utilisés avec eux

Vous pouvez utiliser des modificateurs et des filtres avec des champs pour contrôler les données qui seront renvoyées dans les résultats.

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### Utilisation des modificateurs de recherche

Workfront Planning prend en charge les modificateurs de recherche suivants :

<table>
    <tr>
        <td><b>Modificateur</b></td>
        <td><b>Exemple</b></td>
        <td><b>Description</b></td>
        <td><b>Valeurs possibles</b></td>
    </tr>
    <tr>
        <td>$contains </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ contient le filtre  </td>
        <td>"Nouveau lancement de produit"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>Renvoie les enregistrements pour lesquels la valeur du champ ne contient pas le filtre  </td>
        <td>"New Launch"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>Renvoie les enregistrements dont la valeur de champ correspond exactement au filtre  </td>
        <td>"Nouveau lancement de produit"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ ne correspond pas exactement au filtre  </td>
        <td>"Nouveau lancement de produit"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>Renvoie les enregistrements dont la valeur de champ n’est pas vide  </td>
        <td><ul><li>« » </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>Renvoie les enregistrements dont la valeur de champ n’est pas vide  </td>
        <td>"Nouveau lancement de produit"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ est supérieure au filtre  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ est supérieure ou égale au filtre  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>$lessThan </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ est inférieure au filtre  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ est inférieure ou égale au filtre </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ est postérieure au filtre  </td>
        <td>"2024-05-15T20:00:00.000Z"  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ est antérieure au filtre </td>
        <td>"2024-05-12T20:00:00.000Z" </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ est comprise entre le filtre  </td>
        <td><ul><li>"2024-05-12T20:00:00.000Z" </li><li>"2024-05-14T20:00:00.000Z" </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ n'est pas comprise entre le filtre  </td>
        <td><ul><li>"2024-05-09T20:00:00.000Z"  </li><li>"2024-05-17T20:00:00.000Z"  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ correspond à l’un des filtres  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ ne correspond à aucun des filtres </td>
        <td><ul><li>"finished"  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ contient l’un des filtres  </td>
        <td><ul><li>["active", "fixed"]  </li><li>["fixed", "completed", "finished"]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ contient tout le filtre  </td>
        <td><ul><li>["active", "completed"]   </li><li>["actif", "terminé", "terminé"]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ ne comporte aucun filtre </td>
        <td>["fixed", "finished"]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>Renvoie les enregistrements dont la valeur de champ correspond exactement au filtre  </td>
        <td>["active", "completed"]  </td>
    </tr>
</table>

#### Types de champ

Vous trouverez ci-dessous la liste des types de champ pris en charge et les modificateurs de recherche pouvant être utilisés avec chacun de ces types de champ.

| Type de champ | Modificateurs de recherche pris en charge |
|---|---|
| Texte | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| long-text | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| Nombre | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| pourcentage | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| currency | $is, $isNot, $greaterThan, $greaterThanOrEqual, $lessThan, $lessThanOrEqual, $isEmpty, $isNotEmpty |
| Date | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| sélection unique | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| multi-select | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| booléen | $is |
| utilisateur | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| formule | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| url | $contains, $doesNotContain, $is, $isNot, $isEmpty, $isNotEmpty |
| created-by | $is, $isNot, $isAnyOf, $isNoneOf |
| created-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween |
| updated-by | $is, $isNot, $isAnyOf, $isNoneOf, $isEmpty, $isNotEmpty |
| update-at | $is, $isNot, $isAfter, $isBefore, $isBetween, $isNotBetween, $isEmpty, $isNotEmpty |
| reference | $hasAnyOf, $hasAllOf, $isExactly, $hasNoneOf, $isEmpty, $isNotEmpty |
| recherche | Dépend du champ lié |

### Utilisation d’instructions &quot;Et&quot; et &quot;Ou&quot;

Dans l’appel API, vous pouvez avoir des filtres qui sont basés sur plusieurs critères combinés par des instructions $and&quot; et &quot;$or&quot;.

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

### Utilisation du paramètre de requête de champs

Vous pouvez utiliser le paramètre de requête de champs pour spécifier une liste de champs spécifiques séparés par des virgules qui doivent être renvoyés. Les noms de ces champs sont sensibles à la casse.

Par exemple, la requête

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
....
```

renvoie une réponse similaire à la suivante :


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### Trier les résultats d’une requête dans l’API

Vous pouvez trier vos résultats selon n’importe quel champ si vous ajoutez les éléments suivants à votre appel API :


`/v1/records/search`

Corps de la requête :

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

### Limites de requête et réponses paginées

Par défaut, les demandes d’API de planification renvoient 500 résultats, à partir du début de la liste. Pour contourner la limitation par défaut du nombre de résultats, vous pouvez utiliser le paramètre `limit` dans vos requêtes et le définir sur un nombre différent, jusqu’à 2 000 résultats.

Nous vous recommandons d’utiliser des réponses paginées pour les jeux de données volumineux en ajoutant le paramètre `offset` à vos requêtes. Les réponses paginées vous permettent de spécifier l’emplacement du premier résultat qui doit être renvoyé.

Par exemple, si vous souhaitez renvoyer les résultats 2001-4000, vous pouvez utiliser la requête suivante. Cet exemple renvoie les 2 000 enregistrements qui sont en état actif, à partir du résultat 2001st :

`POST /v1/records/search `



Corps de la requête :

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

Pour vous assurer que vos résultats sont correctement paginés, utilisez un paramètre de tri. Cela permet de renvoyer les résultats dans le même ordre, de sorte que la pagination ne se répète pas ou n’ignore pas les résultats.

Pour plus d’informations sur le tri, voir [Tri des résultats de requête dans l’API](#sorting-query-results-in-the-api) de cet article.
