---
title: Présentation Des Limites Des Objets De Planification D’Adobe Workfront
description: Adobe Workfront Planning comporte des limites quant au nombre d’objets que vous pouvez créer dans votre instance. Des limites d’objet sont en place pour améliorer les performances du produit et votre expérience avec Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 2a640cd5-f4a8-4ff3-81b6-32f85f6e4535
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 27%

---


<!--keep the 30 connection limit in yellow till Jan 2026-->

# Présentation des limitations d’objet d’Adobe Workfront Planning

<span class="preview">Les informations de cette page font référence à des fonctionnalités qui ne sont pas encore disponibles de façon générale. Elle est disponible uniquement dans l’environnement de Prévisualisation pour tous les clients. Après les versions mensuelles en production, les mêmes fonctionnalités sont également disponibles dans l’environnement de production pour les clients qui ont activé les versions rapides.</span>

<span class="preview">Pour plus d’informations sur les versions rapides, voir [Activation ou désactivation des versions rapides pour votre organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}


Adobe Workfront Planning comporte des limites quant au nombre d’objets que vous pouvez créer dans votre instance. Des limites d’objet sont en place pour améliorer les performances du produit et votre expérience avec Workfront Planning.

Le tableau suivant indique les limites du nombre d’objets que vous pouvez créer dans Workfront Planning. Les limitations peuvent changer.

| Objet Adobe Workfront Planning | Limite |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Nombre d’espaces de travail pour une instance Workfront | Illimité* |
| Nombre de sections d’un espace de travail | 50 |
| Nombre de types d’enregistrements pour un espace de travail | 100 (y compris les types d’enregistrement de toutes les sections et ceux créés lors de l’utilisation d’un modèle d’espace de travail) |
| Nombre d’enregistrements pour un type d’enregistrement | 25 000 |
| Nombre d’enregistrements pour un espace de travail | Planification Sélectionnez : 25 000 <br> Planning Prime : 500 000 <br> Planning Ultimate : 1 000 000 |
| Nombre total d&#39;enregistrements pour une instance de Workfront Planning | Planification Sélectionnez : 500 000 <br> Planning Prime : 2 000 000 <br> Planning Ultimate : Illimité |
| Nombre de champs pour un type d’enregistrement ou une taxonomie | 500 |
| Nombre de caractères d’un champ de texte monoligne | 1 000 caractères |
| Nombre de caractères d’un champ de paragraphe | 10 000 caractères |
| Nombre de champs de paragraphe pour un type d’enregistrement | 20 champs de paragraphe |
| Taille du fichier que vous pouvez coller dans un tableau de type d’enregistrement | 1 Mo |
| Taille du fichier que vous pouvez importer via l’API pour un tableau de type d’enregistrement | 1,5 Mo |
| Vitesse à laquelle les demandes d’API peuvent être effectuées | 200 demandes par minute |
| Nombre de vues qu’un utilisateur peut créer pour un type d’enregistrement | 100 |
| Taille du fichier CSV Excel que vous pouvez importer pour créer des types d’enregistrements | 5 Mo |
| Nombre de lignes que vous pouvez importer dans un fichier CSV ou Excel pour créer des types d’enregistrements | 25 000 |
| Nombre de colonnes que vous pouvez importer dans un fichier CSV ou Excel pour créer des types d’enregistrements | 500 |
| Nombre de champs de formule pour un type d&#39;enregistrement | 20 |
| <span class="preview">Nombre de champs de connexion pour un type d’enregistrement</span> | 30 <span class="preview"></span> |
| Nombre de caractères dans une expression de champ de formule | 50 000 |
| Nombre d&#39;entités (utilisateurs, rôles, équipes, sociétés, groupes) avec lesquelles vous pouvez partager un objet Planning | 100 |

*Nous vous recommandons de ne pas avoir trop d’espaces de travail, car ils pourraient devenir difficiles à gérer et vos workflows pourraient être trop fragmentés.

Pour plus d’informations sur les prix et les packages de Workfront Planning, contactez votre gestionnaire de compte.

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
