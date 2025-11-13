---
title: Améliorations des rapports du premier trimestre 2026
description: Améliorations des rapports du premier trimestre 2026
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 00483638948941c933e5f8bc8cb3edaf8e43fea1
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 11%

---

# Améliorations des rapports du premier trimestre 2026

Cette page décrit les améliorations apportées aux rapports avec la version du premier trimestre 2026 dans l’environnement Aperçu. Ces améliorations seront rendues disponibles comme indiqué, dans l’environnement de production.

Pour obtenir la liste de toutes les modifications disponibles à ce stade du cycle de publication de la version du premier trimestre 2026, consultez l’article [Vue d’ensemble de la version du premier trimestre 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Duplication d’un rapport dans un tableau de bord de zone de travail

>[!NOTE]
>
>Version préliminaire : vendredi 23 octobre 2025
>Version de production pour toute la clientèle : vendredi 23 octobre 2025
>[!BADGE Hors programme ]{type=Neutral}

Vous pouvez désormais dupliquer un rapport d’indicateur de performance clé, de tableau ou de graphique dans un tableau de bord de zone de travail après sa création. Une fois dupliqué, vous pouvez modifier le rapport selon vos besoins avant d’enregistrer.

## Suppression des options de champ des filtres de rapport

>[!NOTE]
>
>Aperçu : 6 novembre 2025
>Version rapide de production : 13 novembre 2025
>Production pour tous : 15 janvier 2026

Nous avons supprimé les options de champ suivantes qui étaient auparavant disponibles lors de l’application d’un filtre à un rapport :

* Autres ID de groupe
* ID d&#39;autres rôles
* Autres ID d&#39;équipe

Ils ont été supprimés en raison de problèmes associés aux opérateurs Non égal à et Est vide . Si un filtre existant utilise l’un de ces champs, il continuera à fonctionner comme prévu. Vous pouvez également continuer à utiliser ces champs en <code>mode texte)</code>, mais il est recommandé d’éviter d’utiliser les opérateurs Non égal à ou Est vide lorsque vous le faites.

Les options de champ suivantes sont disponibles en tant qu’alternatives :

* Autres groupes : ID
* Autres rôles : ID
* Autres équipes : ID

## Amélioration de l’affichage du nombre de regroupements dans les tableaux de bord de la zone de travail

>[!NOTE]
>
>Aperçu : 6 novembre 2025
>Version rapide de production : 13 novembre 2025
>Production pour tous : 15 janvier 2026

Lorsqu’un rapport tabulaire comporte plusieurs pages de résultats et que le tableau est configuré avec des regroupements, le tableau affiche désormais à la fois la quantité d’enregistrements de la page active et le nombre total d’enregistrements de toutes les pages. Par exemple, si votre rapport de tableau comporte 7 regroupements et que la première page affiche 3, le tableau affiche 3 de 7.


## Nouveaux mécanismes de sécurisation pour améliorer les temps de chargement dans les tableaux de bord de la zone de travail

>[!NOTE]
>
>Aperçu : 6 novembre 2025
>Version rapide de production : 13 novembre 2025
>Production pour tous : 15 janvier 2026

Pour éviter les retards de chargement et améliorer les performances globales dans les tableaux de bord de la zone de travail, nous avons appliqué des limites au nombre de composants de tableau de bord pouvant être ajoutés à un tableau de bord :

* Rapports par tableau de bord : limite de 25
* Regroupements sur les vues de la table : 5 limite
* Distance par rapport à l&#39;objet de base du rapport : limite de 10
* Colonnes dans une vue Tableau : limite de 25
* Invites de filtre au niveau du tableau de bord : limite de 10