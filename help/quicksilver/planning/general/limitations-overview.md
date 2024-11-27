---
title: Présentation des limites des objets de planification Adobe Workfront
description: Adobe Workfront Planning comporte des limites quant au nombre d’objets que vous pouvez créer dans votre instance. Des limites d’objet sont en place pour améliorer les performances du produit et améliorer votre expérience avec Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
source-git-commit: d962d60294295dd1f3771d1f0b737c9d1f03dfef
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 35%

---

<!--check the workfront.com/plans article linked below to see if there is content in there about Planning - after August 28, 2024-->

# Présentation des limites des objets de la planification Adobe Workfront

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients. Après les versions mensuelles de Production, les mêmes fonctionnalités sont également disponibles dans l’environnement Production pour les clients qui ont activé les versions rapides. </span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation de versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}


Adobe Workfront Planning comporte des limites quant au nombre d’objets que vous pouvez créer dans votre instance. Des limites d’objet sont en place pour améliorer les performances du produit et améliorer votre expérience avec Workfront Planning.

Le tableau suivant indique les limites du nombre d’objets que vous pouvez créer dans Workfront Planning. Les limites peuvent changer au fur et à mesure que nous entrons dans les phases suivantes de développement.

| Objet Adobe Workfront Planning | Limite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Nombre d’espaces de travail pour une instance Workfront | unlimited* |
| Nombre de sections d’un espace de travail | 50 |
| Nombre de types d’enregistrement d’un espace de travail | 1 000 (y compris les types d’enregistrement de toutes les sections et ceux créés lors de l’utilisation d’un modèle d’espace de travail) |
| Nombre d’enregistrements d’un type d’enregistrement | 25 000 |
| Nombre d&#39;enregistrements pour un espace de travail | 25 000 pour les clients ayant une planification <br> 500 000 pour les clients ayant une planification plus |
| Nombre total d’enregistrements pour une instance de la planification Workfront | 500 000 pour les clients ayant le plan de planification <br>2 millions pour les clients ayant le plan Plus |
| Nombre de champs pour un type d’enregistrement ou une taxonomie | 500 |
| Nombre de caractères d’un champ de texte d’une seule ligne | 1 000 caractères |
| Nombre de caractères d’un champ de paragraphe | 10 000 caractères |
| Nombre de champs de paragraphe pour un type d’enregistrement | 20 champs de paragraphe |
| Taille du fichier que vous pouvez coller dans un tableau de type d’enregistrement | 1 Mo |
| Taille du fichier que vous pouvez importer via l’API pour un tableau de type d’enregistrement | 1,5 Mo |
| Vitesse à laquelle les demandes d’API peuvent être effectuées | 200 demandes par minute |
| Nombre de vues qu’un utilisateur peut créer pour un type d’enregistrement | 100 |
| Taille du fichier CSV d’Excel que vous pouvez importer pour créer des types d’enregistrement | 5 Mo |
| <span class="preview">Nombre de lignes que vous pouvez importer dans un fichier CSV ou Excel pour créer des types d’enregistrement</span> | 10 000 |
| <span class="preview">Nombre de colonnes que vous pouvez importer dans un fichier CSV ou Excel pour créer des types d’enregistrement</span> | 500 |

*Nous vous recommandons de ne pas avoir trop d’espaces de travail, car ils peuvent devenir difficiles à gérer et vos workflows peuvent être trop fragmentés.

Pour plus d’informations sur le prix et le package de Workfront Planning, voir [Prix et package Adobe Workfront](https://business.adobe.com/products/workfront/pricing.html).

<!--
****************KEEP THIS COMMENTED OUT:

**This functionality has been temporarily removed and it will be available at a later date.**********************
-->


<!--OLD limitations (before GA:)

|       Adobe Workfront Planning  object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of sections for one workspace                                      |   50                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes record types from all sections and those that are created when using a workspace template)  |
|     Number of records for one record type                                               |   50,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text field                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     The rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Number of views one user can create for one record type | 100 |

-->
<!--| Size of CSV of Excel file you can import* | 5MB |-->

<!--[!IMPORTANT]
>
>*This functionality has been temporarily removed and it will be available at a later date.-->
