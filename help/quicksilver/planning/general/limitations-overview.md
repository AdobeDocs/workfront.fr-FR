---
title: Présentation des limites des objets de planification Adobe Workfront
description: Adobe Workfront Planning comporte des limites quant au nombre d’objets que vous pouvez créer dans votre instance. Des limites d’objet sont en place pour améliorer les performances du produit et améliorer votre expérience avec Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 63%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Présentation des limites des objets de la planification Adobe Workfront

Adobe Workfront Planning comporte des limites quant au nombre d’objets que vous pouvez créer dans votre instance. Des limites d’objet sont en place pour améliorer les performances du produit et améliorer votre expérience avec Workfront Planning.

Le tableau suivant indique les limites du nombre d’objets que vous pouvez créer dans Workfront Planning. Les limites peuvent changer au fur et à mesure que nous entrons dans les phases suivantes de développement.

| Objet Adobe Workfront Planning | Limite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Nombre d’espaces de travail pour une instance Workfront | 1 000 |
| Nombre de sections d’un espace de travail | 50 |
| Nombre de types d’enregistrement d’un espace de travail | 1 000 (y compris les types d’enregistrement de toutes les sections et ceux créés lors de l’utilisation d’un modèle d’espace de travail) |
| Nombre d’enregistrements d’un type d’enregistrement | 50 000 |
| Nombre de champs d’un type d’enregistrement ou d’une taxonomie | 500 |
| Nombre de caractères d’un champ de texte | 1 000 caractères |
| Taille de fichier que vous pouvez coller dans un tableau de type enregistrement | 1 Mo |
| Taille de fichier que vous pouvez importer via l’API pour un tableau de type enregistrement | 1,5 Mo |
| Taux auquel les demandes d’API peuvent être effectuées | 200 demandes par minute |
| Nombre de vues qu’un utilisateur peut créer pour un type d’enregistrement | 100 |

<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->

<!--At GA, replace the table above with this:

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   unlimited*                                                                                                        |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   25,000                                                                                                        |
|     Number of records for one workspace                                               |   25,000 for customers with the Planning plan <br> 500,000 for customers with the Planning Plus  plan                                                                                                         |
|     Number of total records for one instance of Workfront Planning type                                               |   500,000 for customers with the Planning plan <br>2 million for customers with the Planning Plus plan                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

*We recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.

****************KEEP THIS COMMENTED OUT:
| Size of CSV of Excel file you can import** | 5MB |
**This functionality has been temporarily removed and it will be available at a later date.**********************
-->