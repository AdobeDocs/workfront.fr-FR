---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Déplacer des objets d’un environnement à un autre
description: La fonctionnalité Promotion environnementale est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Elle n’offre pas la possibilité de déplacer des objets transactionnels (à quelques exceptions près).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 99%

---

# Déplacer des objets entre des environnements [!DNL Workfront] à l’aide de l’API Promotion environnementale [!DNL Workfront]

La fonctionnalité Promotion environnementale vous permet de déplacer des objets liés à la configuration d’un environnement à un autre. Vous pouvez déplacer ces objets à l’aide de l’API Workfront, comme décrit dans cet article.

Pour obtenir des instructions sur le déplacement d’objets entre des environnements à l’aide de l’application Workfront, voir :

* [Créer ou modifier un package de promotion environnementale](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [Installer un package de promotion environnementale](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)


## Conditions d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td>Package Adobe Workfront
   </td>
   <td> <p>Prime ou Ultimate</p>
   </td>
  </tr>
  <tr>
   <td><strong>Licences Workfront</strong>
   </td>
   <td> <p>Standard</p>&gt;
   </td>
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td><p>Vous devez être un administrateur ou une administratrice Workfront.</p>
   </td>
  </tr>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Conditions préalables

Le point d’entrée Créer un package de promotion part du principe que vous avez déjà configuré l’environnement source. Cet appel API nécessite la création manuelle d’un mappage d’objets objCodes [!DNL Workfront] et de GUID d’objets. La structure spécifique de ce mappage est décrite ci-dessous.

## Objets pris en charge pour la promotion environnementale

La fonctionnalité Promotion environnementale est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Elle n’offre pas la possibilité de déplacer des objets transactionnels (à quelques exceptions près).

Pour obtenir la liste des objets pouvant être promus et de leurs sous-objets pouvant être promus inclus, voir [Objets pris en charge pour la promotion environnementale](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) dans l’article [Vue d’ensemble du déplacement d’objets entre des environnements Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## Authentification

L’API authentifie chaque demande pour s’assurer que le client a le droit d’afficher ou de modifier l’objet concerné par la requête.

L’authentification s’effectue en transmettant un identifiant de session ou une clé API, qui peuvent être fournis à l’aide de la méthode suivante :

### Authentification de l’en-tête de la demande

La méthode d’authentification préférée consiste à transmettre un en-tête de requête nommé SessionID contenant le jeton de session. Cela présente l’avantage d’être à l’abri des attaques [Cross-site Request Forgery (CSRF)](https://fr.wikipedia.org/wiki/Cross-site_request_forgery) et de ne pas interférer avec l’URI à des fins de mise en cache.

Voici un exemple d’en-tête de requête :

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## Points d’entrée API

* [Créer un package](#create-a-package)
* [Obtenir une liste de packages](#get-a-list-of-packages)
* [Obtenir un package par identifiant](#get-a-package-by-id)
* [Mettre à jour des propriétés spécifiques d’un package](#update-specific-properties-of-a-package)
* [Supprimer un package](#delete-a-package)
* [Effectuer une exécution préalable](#execute-a-pre-run)
* [Exécuter une installation](#execute-an-installation)
* [Obtenir la liste des installations pour un package spécifique](#get-a-list-of-installations-for-a-specific-package)
* [Obtenir les détails d’installation d’une installation](#get-the-installation-details-for-an-installation)

### Créer un package

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel exécute un processus à plusieurs étapes.

La première étape entraîne la création d’un package de promotion vide avec le statut « ASSEMBLING ».

La deuxième étape utilise le tableau `objectCollections` fourni dans le corps POST pour assembler les enregistrements demandés à partir de Workfront. Cette étape peut prendre plusieurs minutes, en fonction du nombre d’enregistrements demandés et de votre configuration Workfront. À la fin de ce processus, le package de promotion vide est mis à jour avec les `packageEntities` et le statut est automatiquement défini sur « BROUILLON ».


>[!NOTE]
>
>Observez la structure du tableau `objectCollections`.
>
>Chaque élément du tableau contient une clé `objCode` qui correspond au code d’objet documenté dans l’explorateur d’API Workfront.
>
>Chaque élément contient également une collection d’`entities`. Le champ `ID` est ainsi attendu. Il peut également accepter un attribut `name` facultatif pour permettre de savoir plus facilement ce que représente `ID`.
>
>Pour obtenir la liste des codes d’objet pouvant être demandés dans la liste `objectCollections`, voir la section [Objets pris en charge pour la promotion environnementale](#supported-objects-for-environment-promotion) dans cet article.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### En-têtes

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Ou

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corps

```json
{
    "name": "Agency Onboarding - 2023-06-06",
    "description": "This promotion package contains configuration to support the agency onboarding processes...",
    "source": "https://{domain}.{environment}.workfront.com",
    "objectCollections": [
        {
            "objCode": "PROJ",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597ba1",
                    "name": "Agency Request"
                }
            ]
        },
        {
            "objCode": "TMPL",
            "entities": [
                {
                    "ID": "6419b8b9001151ee258921a4f7597bb2",
                    "name": "New Agency Onboarding"
                },
                {
                    "ID": "6419b8b9001151ee258921a4f7597bc3",
                    "name": "New Agency Offboarding"
                }
            ]
        },
        {
            "objCode": "PTLTAB",
            "entities": [
                {
                    "ID": "645e6435000b4aaebe4776f4a42ed5ad",
                    "name": "Agency Performance and Readiness"
                }
            ]
        }
    ]
}
```

#### Réponse

```json
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ASSEMBLING",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "createdById": "61aa9d0e0005fcee8f212835bdaa2619",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d"
    }
}
```

### Obtenir une liste de packages

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel renvoie une liste non filtrée des packages de promotion appartenant au client ou à la cliente.

La réponse comprend tous les packages créés à partir de n’importe quelle instance Workfront de sandbox, de prévisualisation ou de production du client ou de la cliente.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages
```

#### En-têtes

```json
{
    "apikey": "**********"
}
```

Ou

```json
{
    "sessionID": "*****************"
}
```

#### Corps

_Vide_

#### Réponse

```
200
```

```json
{
    "data": [
        {
            "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
            "name": "Agency Onboarding - 2023-06-06",
            "description": "This promotion package contains configuration to support the agency onboarding processes...",
            "status": "ASSEMBLING",
            "createdAt": "2023-06-06T17:29:21.600Z",
            "deletedAt": null
},
        {...}
    ]
}
```

&lt;!--Vérifiez le « statut » ci-dessus. A-t-il été ajouté ?-->

### Obtenir un package par identifiant

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel renvoie les détails d’un package de promotion demandé.

La demande peut être effectuée par l’intermédiaire de n’importe quel environnement, quelle que soit la source d’origine du package de promotion.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### En-têtes

```json
{
    "apikey": "**********"
}
```

Ou

```json
{
    "sessionID": "*****************"
}
```

#### Corps

_Vide_

#### Réponse

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "DRAFT",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": null,
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "null"
                   - or -
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Mettre à jour des propriétés spécifiques d’un package

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel met à jour tout le contenu du package de promotion fourni dans le corps PATCH.

Les attributs modifiables sont les suivants :

1. name (chaîne)
1. description (chaîne)
1. status (chaîne avec validation de valeur)

Pour une description détaillée des statuts disponibles, voir [Statuts de promotion environnementale](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) dans l’article [Vue d’ensemble du déplacement d’objets entre des environnements Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


#### URL

```
PATCH https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```


#### En-têtes

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Ou

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corps

```json
{
    "status": "ACTIVE"
}
```

#### Réponse

```
200
```

```json
{
    "data": {
        "id": "1d5693b9-b7b5-492d-8219-c21f34bcaca6",
        "name": "Agency Onboarding - 2023-06-06",
        "description": "This promotion package contains configuration to support the agency onboarding processes...",
        "source": "https://{domain}.{environment}.workfront.com",
        "status": "ACTIVE",
        "version": 1,
        "createdAt": "2023-06-06T17:29:21.600Z",
        "publishedAt": "2023-06-06T19:39:01.600Z",
        "customerId": "61aa9d090005fa42152c1cb66659f38d",
        "packageEntities": {
            "GROUP": [
               {
                   "id": "52aa9d0e0005fcee8f212835bdaa2691",
                   "name": "Default Group",
                   "description": "..."
               }
            ],
            "ROLE": [
               {...}
            ],
            ...
        }
   }
}
```

### Supprimer un package

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel supprime l’enregistrement du package de promotion. Cette action est irréversible.

>[!NOTE]
>
>Au lieu de supprimer un package de promotion, il est recommandé de modifier le statut du package en DISABLED. Cela permet la récupération du package et conserve l’historique d’installation de l’emplacement où il a été déployé.

#### URL

```
DELETE https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}
```

#### En-têtes

```json
{
    "apikey": "**********"
}
```

Ou

```json
{
    "sessionID": "*****************"
}
```

#### Corps

_Vide_

#### Réponse

```
200
```

```
Deleted
```

### Effectuer une exécution préalable

>[!IMPORTANT]
>
>Avant de pouvoir exécuter une installation, vous devez effectuer cette exécution préalable. Vous utilisez l’identifiant généré par cet appel lorsque vous exécutez l’installation.

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel effectue une comparaison entre la définition du package et l’environnement cible identifié dans l’URL.

Le résultat est un corps JSON qui identifie si un objet de promotion est présent ou non dans l’environnement cible.

Pour chaque objet de promotion, une des `actions` suivantes est définie :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>CREATE</td> 
   <td><p>Lorsqu’un enregistrement correspondant est introuvable dans l’environnement cible, l’action est définie sur CREATE.</p><p>Lorsque cette action est définie dans la <code>translationmap</code> qui est fournie au point d’entrée <code>/install</code>, le service d’installation crée l’enregistrement.</p></td> 
  </tr> 
  <tr> 
   <td>USEEXISTING</td> 
   <td><p>Lorsqu’un enregistrement correspondant est trouvé dans l’environnement cible, l’action est définie sur USEEXISTING et un <code>targetId</code> est également capturé dans la <code>translationmap</code>.</p><p>Lorsque cette action est définie dans la <code>translationmap</code> qui est fournie au point d’entrée <code>/install</code>, le service d’installation ne crée pas l’enregistrement. Cependant, il utilisera les <code>targetId</code> inclus dans l’entrée de mappage pour les autres objets qui peuvent avoir une référence à cet enregistrement.</p><p>Par exemple, un « Groupe par défaut » peut se trouver dans l’environnement cible dans lequel un package est déployé. Il n’est pas possible d’avoir deux enregistrements « Groupe par défaut ». Le service d’installation utilise donc le GUID du groupe existant pour toute autre action de création d’objet qui inclut une référence au « Groupe par défaut », comme un projet, un formulaire ou toute autre entité liée à ce groupe.</p><p><b>Note :</b> <ul><li><p>Lorsque l’action USEEXISTING est affectée, l’enregistrement existant dans l’environnement cible n’est pas modifié. </p><p>Par exemple, si la description du « Groupe par défaut » a changé dans le sandbox à partir duquel le package a été créé et que la valeur de description est différente dans l’environnement cible, la valeur reste inchangée après une installation avec ce <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>OVERWRITING</td> 
   <td><p>Cette action n’est pas définie automatiquement.</p><p>Cette action permet de mettre à jour un objet existant dans l’environnement cible. Elle permet de remplacer manuellement une action CREATE ou USEEXISTING affectée avant d’appeler le <code>/install</code>.<ul><li>Un utilisateur ou une utilisatrice peut mettre à jour un objet dans l’environnement de test, puis utiliser l’action OVERWRITING pour mettre à jour cet objet dans l’environnement cible.</p></li><li><p>Si l’utilisateur ou l’utilisatrice installe d’abord un package de promotion, puis qu’un nouveau package (ou un package mis à jour) contient des modifications apportées aux objets dans le package initial, l’utilisateur ou l’utilisatrice peut utiliser l’action OVERWRITING pour remplacer les objets précédemment installés. </p><p>Pour plus d’informations sur le remplacement, voir la section [Remplacement](#overwriting) de cet article.</li><ul></td> 
  </tr> 
  <tr> 
   <td>IGNORE</td> 
   <td><p>Cette action n’est pas définie automatiquement.</p><p>Elle permet de remplacer manuellement une action CREATE ou USEEXISTING affectée avant d’exécuter l’appel <code>/install</code>.</p><p><b>Notes : </b><ul><li><p>Si un enregistrement qui a été initialement défini sur CREATE est défini sur IGNORE, tous les enregistrements enfant doivent également être définis sur IGNORE.</p><p>Par exemple, si un enregistrement de modèle a été mappé avec une action CREATE et que l’utilisateur ou l’utilisatrice qui effectue l’installation souhaite l’exclure du déploiement, celui-ci peut définir l’action du modèle sur IGNORE.</p><p>Dans ce cas, si l’utilisateur ou l’utilisatrice qui effectue l’installation ne définit pas également sur IGNORE les tâches du modèle, les affectations des tâches du modèle, les prédécesseurs des tâches du modèle, la définition de la file d’attente, les rubriques de la file d’attente, les règles de routage, etc., le déploiement entraîne l’échec de la tentative d’installation.</p></li><li><p>Si un enregistrement qui était initialement défini sur USEEXISTING est défini sur IGNORE, il peut se produire des effets indésirables lors du processus d’installation.</p><p>Par exemple, si un enregistrement Groupe a été mappé avec l’action USEEXISTING et que l’utilisateur ou l’utilisatrice qui effectue l’installation modifie l’action en IGNORE, pour les objets nécessitant un groupe (par exemple, un projet ne peut pas exister sans qu’un groupe lui soit affecté), le groupe par défaut du système est affecté à ce projet.</p></li><li><p>Si un enregistrement qui était initialement défini sur USEEXISTING est défini sur CREATE, il peut y avoir des effets indésirables lors du processus d’installation, car de nombreuses entités Workfront ont des contraintes d’unicité des noms.</p><p>Par exemple, si un enregistrement « Groupe par défaut » a été mappé avec l’action USEEXISTING et que l’utilisateur ou l’utilisatrice qui effectue l’installation modifie l’action en CREATE, étant donné qu’il existe déjà un « Groupe par défaut », la tentative d’installation ne parviendra pas à compléter l’ensemble des étapes. Les noms de groupes doivent être uniques.</p><p>Certaines entités n’ont pas de contrainte d’unicité des noms. Pour ces objets, effectuer cette modification entraîne la création de deux enregistrements portant le même nom. Par exemple, les modèles, les projets, les vues, les filtres, les regroupements, les rapports et les tableaux de bord ne sont pas soumis à une contrainte d’unicité des noms. La bonne pratique consiste à attribuer des noms uniques à ces enregistrements, mais cela n’est pas imposé.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

Il n’existe actuellement aucune prise en charge pour une `action` UPDATE dans les fonctionnalités alpha de ce service. Nous étudions comment mettre au point l’option permettant de réaliser une `action` UPDATE.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/:id/prepare-installation
```

#### En-têtes

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Ou

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corps

```json
{}
```

#### Réponse

```
200
```

```json
{
    "environmentPromotionPackageId": "45f2ae94-76c0-4b13-8f3b-f688de83043d",
    "environmentPromotionPackageVersion": 1,
    "id": "c0bc79bd-c9c1-4b5b-b118-b1241392de0e",
    "userId": "5ba38da500b752fd66439d4f6a9999a1",
    "customerId": "5ba38d9d00b74f0c7a38b1b487fc9710",
    "status": "PREPARING",
    "environment": "mmi.my.workfront.com",
    "registeredAt": "2023-10-19T20:00:16.697Z",
    "updatedAt": "2023-10-19T20:00:16.701Z",
    "translationMap": {
        "CTGY": {
            "62d9c9a0000013aeeefe7242a0a5fdb2": {
                "name": "Example Document Form",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9a0000013aeeefe7242a0a5fdb2"
            }
        },
        "PGRP": {
            "62d1eee4001c6618e6b9f9a588ba1598": {
                "name": "Asset Detail",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee4001c6618e6b9f9a588ba1598"
            }
        },
        "GROUP": {
            "5ba38da500b752b0f46d13186030b7ad": {
                "name": "Default Group",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "5ba38da500b752b0f46d13186030b7ad"
            }
        },
        "PARAM": {
            "62d1eee400f8578895166ee91a83f97a": {
                "name": "Asset Type",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee400f8578895166ee91a83f97a"
            },
            "62d1eee50001407c713514a8970b58e4": {
                "name": "Keywords",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee50001407c713514a8970b58e4"
            },
            "62d1eee5000333ac3981ea4f3df6d88e": {
                "name": "Permitted Uses",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000333ac3981ea4f3df6d88e"
            },
            "62d1eee5000b188e9ec8039a097fc7ab": {
                "name": "File Format",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee5000b188e9ec8039a097fc7ab"
            },
            "62d1eee500100c159fd5f838ce560507": {
                "name": "CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d1eee500100c159fd5f838ce560507"
            },
            "62d9c988001c1f23954dbb9d646335b5": {
                "name": "Other CTA",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c988001c1f23954dbb9d646335b5"
            },
            "62d9c9880070f546cf4c798ea6c3eaa4": {
                "name": "Other Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c9880070f546cf4c798ea6c3eaa4"
            },
            "62d9c990006258baf1b40f2569c3eab7": {
                "name": "Target Audience",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "62d9c990006258baf1b40f2569c3eab7"
            }
        }
    }
}
```

>[!NOTE]
>
>L’identifiant dont vous aurez besoin pour effectuer l’installation est le champ `id`. Dans cet exemple, le champ `id` est le troisième à partir du haut et a une valeur commençant par `c0bc79bd`.

### Exécuter une installation

>[!IMPORTANT]
>
>Avant de pouvoir exécuter une installation, vous devez effectuer cette exécution préalable. Vous utiliserez l’identifiant généré à partir de l’exécution préalable lorsque vous effectuerez l’installation.
>
>Si des modifications ont été apportées à l’environnement de destination (l’environnement sur lequel le package est déployé) après le lancement de l’exécution préalable, nous vous recommandons de lancer à nouveau l’exécution préalable. Si vous ne la lancez pas, votre exécution risque de ne pas s’achever correctement ou l’installation peut échouer.
>
>Pour plus d’informations sur le lancement d’une exécution préalable, consultez la section [Effectuer une exécution préalable](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel lance une tentative d’installation d’un package de promotion dans l’environnement cible identifié dans l’URL de la requête POST.

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}/install
```

#### En-têtes

```json
{
    "apikey": "**********",
    "Content-Type": "application/json"
}
```

Ou

```json
{
    "sessionID": "*****************", 
    "Content-Type": "application/json"
}
```

#### Corps

```json
{
}
```

#### Réponse

```
202
```


```json
{}
```

### Obtenir la liste des installations pour un package spécifique

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
</code></td> 
  </tr> 
  </tbody> 
</table>

Les résultats incluent les événements d’installation de tous les environnements dans lesquels le module a été déployé. Ils ne se limitent pas aux installations pour l’environnement par lequel la requête est faite. Vous pouvez ainsi identifier les environnements qui ont reçu ce package.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations?environmentPromotionPackageId={environmentPromotionPackageId}
```

#### En-têtes

```json
{
    "apikey": "**********"
}
```

Ou

```json
{
    "sessionID": "*****************"
}
```

#### Corps

_Vide_

#### Réponse

```
200
```

```json
[
    {
        "id": "2892b936-e09e-455a-935f-e1462ab9753c",
        "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
        "environmentPromotionPackageVersion": 1,
        "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
        "customerId": "54286d78b064451096752b99bf968481",
        "status": "INSTALLED",
        "environment": "https://{domain}.{environment}.workfront.com",
        "registeredAt": "2021-03-16T02:21:31.908Z",
        "updatedAt": null,
        "translationMap": {
            "ROLE": {
                "5f6d114f006883209828ddd9088e63b3": {
                    "name": "DAM Curator",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f4bed00028a718599f29575840053"
                },
                "ad535a9ebe647361e053a7656a0a1575": {
                    "name": "Copywriter",
                    "action": "USEEXISTING",
                    "isValid": true,
                    "targetId": "600f162700001ca051081c06667b14a4"
                },
                ...
            },
            "TMPL": {
                "5f9b317c00b3db5af69abcd1ed5f82aa": {
                    "name": "Digital Asset Production (Integrated)",
                    "action": "CREATE",
                    "isValid": true,
                    "targetId": "6054cda40000d5af63dc811d9c2b3a07"
                },
                ...
            },
            ...
        }
    },
    {...}
]
```

### Obtenir les détails d’installation d’une installation

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel renvoie le dernier `translationMap` produit par le service d’installation pour une installation spécifique.

Chaque enregistrement indique l’`action` prescrite et le succès ou l’échec de l’action.

Pour les enregistrements avec une valeur `action` CREATE, le champ `targetId` sera remplacé par la valeur de l’enregistrement nouvellement créé dans le système cible. De plus, le champ `installationStatus` sera défini sur INSTALLED.

Pour les enregistrements comportant l’`action` USEEXISTING, le champ `targetId` sera également défini, et le champ `installationStatus` sera défini comme REGISTERED. Le processus de mappage est terminé, signifiant que le service d’installation reconnaît avoir évalué l’enregistrement et qu’il n’y a rien à faire.

Si l’enregistrement a une `action` CREATE mais qu’il ne parvient pas à être créé, le `installationStatus` sera défini comme FAILED et la raison de l’échec sera également fournie.

#### URL

```
GET https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/installations/{id}
```

#### En-têtes

```json
{
    "apikey": "**********"
}
```

Ou

```json
{
    "sessionID": "*****************"
}
```

#### Corps

_Vide_

#### Réponse

```
200
```

```json
{
    "id": "2892b936-e09e-455a-935f-e1462ab9753c",
    "environmentPromotionPackageId": "4fae2b9d-d315-45f4-909f-a0c0d79fc65d",
    "environmentPromotionPackageVersion": 1,
    "userId": "8fbbc5bcf4f94a5b862483ee05573e73",
    "customerId": "54286d78b064451096752b99bf968481",
    "status": "INSTALLED",
    "environment": "https://{domain}.{environment}.workfront.com",
    "registeredAt": "2021-03-16T02:21:31.908Z",
    "updatedAt": null,
    "translationMap": {
        "ROLE": {
            "5f6d114f006883209828ddd9088e63b3": {
                "name": "DAM Curator",
                "action": "USEEXISTING",
                "isValid": true,
                "targetId": "600f4bed00028a718599f29575840053"
            },
            ...
        },
        "TMPL": {
            "5f9b317c00b3db5af69abcd1ed5f82aa": {
                "name": "Digital Asset Production (Integrated)",
                "action": "CREATE",
                "isValid": true,
                "targetId": "6054cda40000d5af63dc811d9c2b3a07"
            },
            ...
        },
        ...
    }
}
```

## Remplacement

Il s’agit d’un processus en 3 étapes.

1. Créez une carte de traduction (analogue à la phase de « préparation de l’installation »).
1. Modifiez la carte de traduction générée, en définissant les champs  et  pour tout objet qui doit être remplacé. `action` `targetId` L’action doit être `OVERWRITING`, et le `targetId` doit être l’UUID de l’objet qui doit être remplacé.
1. Exécutez l’installation.

* [Étape 1 : créer une carte de traduction](#step-1---create-a-translation-map)
* [Étape 2 : modifier la carte de traduction](#step-2---modify-the-translation-map)
* [Étape 3 : installer](#step-3---install)

### **Étape 1 : créer une carte de traduction**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/translation-map
```

#### Corps

Aucun

#### Réponse

Une carte de traduction, avec un statut `202 - OK`

```json
{
    {objcode}: {
        {object uuid}: {
            "targetId": {uuid of object in destination},
            "action": {installation action},
            "name": {name of the object},
            "isValid": true
        },
        {...more objects}
    },
    {...more objcodes}
}
```


#### Exemple

```json
{
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "CREATE",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
```

### Étape 2 : modifier la carte de traduction

Il n’existe aucun point d’entrée pour cette étape.

1. Dans la carte de traduction renvoyée dans l’[Étape 1 : créer une carte de traduction](#step-1---create-a-translation-map), examinez la liste des objets qui seront installés.
1. Mettez à jour le champ d’action sur chaque objet en fonction de l’action d’installation souhaitée.
1. Validez `targetId` sur chaque objet. Si l’action définie est `USEEXISTING` ou `OVERWRITING`, `targetId` doit être défini sur l’UUID de l’objet cible dans l’environnement de destination. Pour toute autre action, l’ID de cible doit être une chaîne vide.

   >[!NOTE]
   >
   >`targetId` est déjà renseigné si une collision a été détectée.

### **Étape 3 : installer**

#### URL

```
POST https://{domain}.{environment}.workfront.com/environment-promotion/api/v1/packages/{id}/install
```

#### Corps

Il s’agit d’un objet avec un seul champ. `translationMap`, qui doit être égal à la carte de traduction modifiée de l’[Étape 2 : modifier la carte de traduction](#step-2---modify-the-translation-map).

```json
{
    "translationMap": {
        {objcode}: {
            {object uuid}: {
                "targetId": {uuid of object in destination},
                "action": {installation action},
                "name": {name of the object},
                "isValid": true
            },
            {...more objects}
        },
        {...more objcodes}
    }
}
```


#### Exemple

```json
{
    "translationMap": {
    "UIVW": {
        "109f611680bb3a2b0c0a8c1f5ec63f6d": {
            "targetId": "6643a26b0001401ff797ccb318f97aa6",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIGB": {
        "edb4c6c127d38910e4860eb25569a5cc": {
            "targetId": "6643a26b000178fb5cc27b74cc1e87ec",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "UIFT": {
        "f97b662e229fd09ee595d8d359ec88bd": {
            "targetId": "6643a26b00015cdd6727b76d6fda1d1d",
            "action": "OVERWRITING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "PTLSEC": {
        "4bb80aa88a96420296a7f47bf866f162": {
            "targetId": "4bb80aa88a96420296a7f47bf866f162",
            "action": "USEEXISTING",
            "name": "Actual Portfolio Cost by Program",
            "isValid": true
        }
    },
    "EXTSEC": {
        "65f8637900015e4dceb6fe079bd5409d": {
            "targetId": "65f8637900015e4dceb6fe079bd5409d",
            "action": "USEEXISTING",
            "name": "Asnyc List",
            "isValid": true
        }
    },
    "PTLTAB": {
        "65f8638a00016422a83ddc3508852d0f": {
            "targetId": "65f8638a00016422a83ddc3508852d0f",
            "action": "CREATEWITHALTNAME",
            "name": "Cool 2.0 The Best",
            "isValid": true
        }
    }
}
}
```

#### Réponse

La réponse comprend `{uuid of the created installation}` et un statut `202 - ACCEPTED`.

Exemple : `b6aa0af8-3520-4b25-aca3-86793dff44a6`

<!--table templates

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

<table style="table-layout:fixed"> 
 <col> 
 <tbody> 
  <tr> 
   <td><b></b></td> 
  </tr> 
  <tr> 
   <td><pre></pre></td> 
  </tr> 
  </tbody> 
</table>
-->
