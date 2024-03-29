---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Déplacement d’objets d’un environnement à un autre
description: La fonctionnalité Promotion de l’environnement est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Il ne prend pas en charge la possibilité de déplacer des objets transactionnels (à quelques exceptions près).
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: dd3c29df-4583-463a-b27a-bbfc4dda8184
source-git-commit: 8d0cfe9bdf32b3be8f44fde0c921abdd1ba9920b
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 2%

---

# Déplacer des objets entre [!DNL Workfront] à l’aide des [!DNL Workfront] API de promotion d’environnement

La fonctionnalité Promotion de l’environnement est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Vous pouvez déplacer ces objets à l’aide de l’API Workfront, comme décrit dans cet article.

Pour plus d’informations sur le déplacement d’objets entre les environnements à l’aide de l’application Workfront, voir :

* [Créer ou modifier un package de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
* [Installer un package de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plan</td> 
   <td> <p>Enterprise, Prime ou Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] license</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Autorisations d’objet</p> </td> 
   <td> <p>Tout</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Package de support</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Privilégié] ou [!UICONTROL Enterprise]</p> <p>Le package de prise en charge standard n’a pas accès à l’environnement de test d’actualisation personnalisée, mais il a accès à l’environnement de test d’aperçu.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Conditions préalables

Le point de terminaison Créer un module de promotion suppose que vous avez déjà configuré l’environnement source. Cet appel API nécessite la création manuelle d’une carte d’objet de [!DNL Workfront] objCodes et GUID d’objet. La structure spécifique de cette carte est décrite ci-dessous.

## Objets pris en charge pour la promotion de l’environnement

La fonctionnalité Promotion de l’environnement est conçue pour permettre de déplacer des objets liés à la configuration d’un environnement à un autre. Il ne prend pas en charge la possibilité de déplacer des objets transactionnels (à quelques exceptions près).

Pour obtenir la liste des objets promotionnels et de leurs sous-objets promotionnels inclus, voir [Objets pris en charge pour la promotion de l’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) dans l’article [Présentation du déplacement d’objets entre les environnements Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).

## Authentification

L’API authentifie chaque requête pour s’assurer que le client a accès à l’affichage ou à la modification d’un objet demandé.

L’authentification est effectuée en transmettant un ID de session ou une clé d’API, qui peut être fournie à l’aide de la méthode suivante :

### Authentification de l’en-tête de requête

La méthode d’authentification privilégiée consiste à transmettre un en-tête de requête nommé SessionID contenant le jeton de session. Cela a l’avantage d’être en sécurité contre [Cross-site Request Forgery (CSRF)](https://en.wikipedia.org/wiki/Cross-site_request_forgery) n’interfère pas avec l’URI à des fins de mise en cache.

Voici un exemple d’en-tête de requête :

```
GET /attask/api/v15.0/project/search
SessionID: abc1234
```

## Points de terminaison API

* [Création d’un package](#create-a-package)
* [Obtention d’une liste de packages](#get-a-list-of-packages)
* [Obtention d’un package par ID](#get-a-package-by-id)
* [Mettre à jour les propriétés spécifiques d’un package](#update-specific-properties-of-a-package)
* [Suppression d’un package](#delete-a-package)
* [Exécution d’une pré-exécution](#execute-a-pre-run)
* [Exécution d’une installation](#execute-an-installation)
* [Obtenir la liste des installations pour un package spécifique](#get-a-list-of-installations-for-a-specific-package)
* [Obtention des détails d’installation d’une installation](#get-the-installation-details-for-an-installation)

### Création d’un package

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel exécute un processus en plusieurs étapes.

La première étape entraîne la création d’un package de promotion vide dans le statut &quot;ASSEMBLEMENT&quot;.

La deuxième étape utilise la méthode `objectCollections` tableau fourni dans le corps du POST pour assembler les enregistrements demandés à partir de Workfront. Cette étape peut prendre plusieurs minutes, en fonction du nombre d’enregistrements demandés et de votre configuration Workfront. À la fin de ce processus, le module de promotion vide est mis à jour avec la variable `packageEntities` et l’état est automatiquement défini sur &quot;BROUILLON&quot;.


>[!NOTE]
>
>Notez la structure de la variable `objectCollections`  tableau.
>
>Chaque élément du tableau contient une `objCode` qui correspond au code d’objet documenté dans l’explorateur d’API Workfront.
>
>Chaque élément contient également un `entities` collection. Cela suppose que la variable `ID` champ . Il peut également accepter une `name` pour faciliter la recherche de ce que la variable `ID` représente .
>
>Pour obtenir la liste des codes d’objet autorisés à être demandés dans la variable `objectCollections` , voir [Objets pris en charge pour la promotion de l’environnement](#supported-objects-for-environment-promotion) dans cet article.

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

### Obtention d’une liste de packages

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /packages</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel renvoie une liste non filtrée des packages de promotion appartenant au client.

La réponse comprend tous les modules créés à partir de n’importe quelle instance de test, d’aperçu ou de production du client de Workfront.

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

&lt;!—Vérifiez &quot;status&quot; ci-dessus—a-t-il été ajouté ?—>

### Obtention d’un package par ID

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

### Mettre à jour les propriétés spécifiques d’un package

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>PATCH /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel met à jour tout le contenu du module de promotion fourni dans le corps du PATCH.

Les attributs modifiables sont les suivants :

1. name (string)
1. description (string)
1. status (chaîne avec validation de valeur)

Pour une description détaillée des états disponibles, voir [Statuts de promotion d’environnement](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#environment-promotion-statuses) dans l’article [Présentation du déplacement d’objets entre les environnements Workfront](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md).


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

### Suppression d’un package

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>DELETE /packages/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel supprime l’enregistrement du kit de promotion. Cette action est irréversible.

>[!NOTE]
>
>Au lieu de supprimer un package de promotion, il est recommandé de modifier le statut du package en Désactivé. Cela permet de récupérer le package et conserve l’historique d’installation de l’emplacement où il a été déployé.

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

### Exécution d’une pré-exécution

>[!IMPORTANT]
>
>Avant de pouvoir exécuter une installation, vous devez exécuter cette pré-exécution. Vous utiliserez l’identifiant généré par cet appel lorsque vous exécuterez l’installation.

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST  {customer-domain}/environment-promotion/api/v1/packages/{id}/prepare-installation</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel effectue une comparaison entre la définition de package et l’environnement cible identifié dans l’URL.

Le résultat est un corps JSON qui identifie si un objet de promotion est trouvé ou non dans l’environnement cible.

Pour chaque objet de promotion, l’un des éléments suivants `actions`  est définie sur :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>CREATE</td> 
   <td><p>Lorsqu’un enregistrement correspondant est introuvable dans l’environnement cible, l’action est définie sur CRÉER.</p><p>Lorsque cette action est définie dans la variable <code>translationmap</code> qui est fourni au <code>/install</code> , le service d’installation crée l’enregistrement.</p></td> 
  </tr> 
  <tr> 
   <td>USEEXISTANT</td> 
   <td><p>Lorsqu’un enregistrement correspondant est trouvé dans l’environnement cible, l’action est définie sur USEEXISTING et une <code>targetId</code> est également capturé dans la variable <code>translationmap</code>.</p><p>Lorsque cette action est définie dans la variable <code>translationmap</code> qui est fourni au <code>/install</code> endpoint, le service d’installation ne crée pas l’enregistrement. Cependant, il utilisera la variable <code>targetId</code> inclus dans l’entrée map pour d’autres objets qui peuvent avoir une référence à cet enregistrement.</p><p>Par exemple, un "groupe par défaut" se trouve dans l’environnement cible dans lequel un package est déployé. Il n’est pas possible d’avoir deux enregistrements "Groupe par défaut". Le service d’installation utilisera donc le GUID du groupe existant dans toute autre action de création d’objet qui inclura une référence au "Groupe par défaut", comme un projet, un formulaire ou toute autre entité liée à ce groupe.</p><p><b>Remarque :</b> <ul><li><p>Lorsque l'action USEEXISTING est affectée, l'enregistrement existant dans l'environnement cible ne sera pas modifié. </p><p>Par exemple, si la description du "Groupe par défaut" a changé dans l’environnement de test à partir duquel le package a été créé et que la valeur de description est différente dans l’environnement cible, la valeur reste inchangée après une installation avec cette méthode <code>translationmap</code>.</li></ul></td> 
  </tr> 
  <tr> 
   <td>REMPLACEMENT</td> 
   <td><p>Cette action ne sera pas définie automatiquement.</p><p>Cette action permet de mettre à jour un objet existant dans l’environnement cible. Il permet de remplacer manuellement une action CRÉER ou UTILISER EXISTANTE affectée avant d’exécuter la fonction <code>/install</code> appelez .<ul><li>Un utilisateur peut mettre à jour un objet dans l’environnement de test, puis utiliser l’action REMPLACER pour mettre à jour cet objet dans l’environnement cible.</p></li><li><p>Si l’utilisateur installe d’abord un package de promotion, puis qu’un nouveau package (ou mis à jour) contiendra à l’avenir des modifications apportées aux objets dans le package initial, l’utilisateur peut utiliser l’option OVERWRITING pour remplacer (remplacer) les objets précédemment installés. </p></li><ul></td> 
  </tr> 
  <tr> 
   <td>IGNORER</td> 
   <td><p>Cette action ne sera pas définie automatiquement.</p><p>Il permet de remplacer manuellement une action CRÉER ou UTILISER EXISTANTE affectée avant d’exécuter la fonction <code>/install</code> appelez .</p><p><b>Remarques : </b><ul><li><p>Si un enregistrement qui a été initialement défini sur CRÉER est défini sur IGNORER, tous les enregistrements enfants doivent également être définis sur IGNORER.</p><p>Par exemple, si un enregistrement de modèle a été mappé avec une action CREATE et que l’utilisateur qui installe souhaite l’exclure du déploiement, il peut définir l’action du modèle sur IGNORE.</p><p>Dans ce cas, si l’utilisateur qui installe n’a pas également défini les tâches du modèle, les affectations de tâches du modèle, les prédécesseurs de tâches du modèle, la définition de la file d’attente, les rubriques de la file d’attente, les règles de routage, etc., sur IGNORE, le déploiement entraîne l’échec de la tentative d’installation.</p></li><li><p>Si un enregistrement qui était initialement défini sur USEEXISTING est défini sur IGNORE, il peut y avoir des effets négatifs pendant le processus d’installation.</p><p>Par exemple, si un enregistrement Group a été mappé avec l’action USEEXISTING et que l’utilisateur qui installe l’action change IGNORE, pour les objets nécessitant un groupe (par exemple, un projet ne peut pas exister sans qu’un groupe soit affecté), le groupe par défaut système sera affecté à ce projet.</p></li><li><p>Si un enregistrement qui était initialement défini sur USEEXISTING est défini sur CREATE, il peut y avoir des effets négatifs pendant le processus d’installation, car de nombreuses entités Workfront ont des contraintes de nom uniques.</p><p>Par exemple, si un enregistrement "Groupe par défaut" a été mappé avec l’action USEEXISTING et que l’utilisateur qui installe l’action passe à CREATE, car il existe déjà un "Groupe par défaut", la tentative d’installation échoue à toutes les étapes. Les noms de groupe doivent être uniques.</p><p>Certaines entités n’ont pas de contrainte de nom unique. Pour ces objets, la modification entraîne deux enregistrements portant le même nom. Par exemple, les modèles, les projets, les vues, les filtres, les groupes, les rapports et les tableaux de bord ne nécessitent pas de contraintes de nom unique. Il est recommandé d’attribuer des noms uniques à ces enregistrements, mais cela n’est pas appliqué.</p></li></ul></p></td> 
  </tr> 
  </tbody> 
</table>

Il n’existe actuellement aucune prise en charge pour une mise à jour `action` dans les fonctionnalités alpha de ce service. L’option permettant d’autoriser une mise à jour `action` c&#39;est quelque chose que nous recherchons.

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
>L’identifiant dont vous aurez besoin pour exécuter l’installation est : `id` champ . Dans cet exemple, la variable `id` est troisième à partir du haut et a une valeur commençant par `c0bc79bd`.

### Exécution d’une installation

>[!IMPORTANT]
>
>Avant de pouvoir exécuter une installation, vous devez exécuter une pré-exécution. Vous utiliserez l’identifiant généré à partir de la pré-exécution lorsque vous exécuterez l’installation.
>
>Si des modifications ont été apportées à l’environnement de destination (l’environnement sur lequel le package est déployé) après l’exécution de la pré-exécution, nous vous recommandons d’exécuter à nouveau la pré-exécution. Si vous n’exécutez pas à nouveau la pré-exécution, votre exécution risque de ne pas s’achever correctement ou l’installation peut échouer.
>
>Pour plus d’informations sur l’exécution d’une pré-exécution, voir [Exécution d’une pré-exécution](#execute-a-pre-run).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>POST /install</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel lance une tentative d’installation d’un package de promotion dans l’environnement cible identifié dans l’URL du POST.

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

Les résultats incluent les événements d’installation de tous les environnements dans lesquels le module a été déployé. Elles ne se limitent pas aux installations pour l’environnement par lequel la demande est faite. Vous pouvez ainsi identifier les environnements qui ont reçu ce package.

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

### Obtention des détails d’installation d’une installation

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td><code>GET /installations/{id}</code></td> 
  </tr> 
  </tbody> 
</table>

Cet appel renvoie la valeur finale `translationMap` produit par le service d’installation pour une installation spécifique.

Chaque enregistrement indique ce qui est prescrit. `action` et si cette action a réussi ou non.

Pour les enregistrements avec une méthode CREATE `action` la valeur `targetId` est défini avec la valeur de l’enregistrement nouvellement créé dans le système cible. En outre, la variable `installationStatus` est défini sur INSTALLLED.

Pour les enregistrements avec l’instruction USEEXISTING `action` la valeur `targetId` est également défini, et la variable `installationStatus` est défini sur ENREGISTRÉ. Cela signifie que le processus de mappage a été terminé et que le service d’installation reconnaît avoir évalué l’enregistrement et qu’il n’y a rien à faire.

Si l’enregistrement comporte une propriété CREATE `action` mais il ne parvient pas à créer l’enregistrement, puis l’événement `installationStatus` est défini sur ÉCHEC et la raison de l’échec est également fournie.

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
