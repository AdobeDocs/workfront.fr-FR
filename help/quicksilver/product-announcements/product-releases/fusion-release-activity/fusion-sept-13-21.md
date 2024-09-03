---
title: 'Activité Version Workfront Fusion : semaine du 13 septembre 2021'
description: 'Activité Version Workfront Fusion : semaine du 13 septembre 2021'
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: d9056d6f-a62d-4516-930e-4c3f4fbaec3e
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 100%

---

# Activité Version Workfront Fusion : semaine du 13 septembre 2021

Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion au cours de la semaine du 23 septembre 2021.

Pour obtenir la liste de toutes les modifications récentes, voir [Activité de publication d’Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Pour obtenir la liste des correctifs récents dans Workfront Fusion, reportez-vous à la page [Mises à jour de maintenance Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) et recherchez toutes les mises à jour intitulées Mise à jour de maintenance de Workfront Fusion.

## Filtrer et trier l’historique d’exécution d’un scénario Workfront Fusion

Pour faciliter la recherche d’exécutions de scénarios spécifiques, nous avons autorisé le filtrage sur davantage de champs dans l’historique d’exécution des scénarios. Désormais, en plus des filtres existants, vous pouvez effectuer un filtrage selon les critères suivants :

* Durée d’exécution
* Nombre d’opérations
* Quantité de données transférées
* Type d’action (exécution ou mise à jour)

Auparavant, l’historique d’exécution ne pouvait être filtré que par heure de début ou statut.

Nous avons également intégré la possibilité de trier l’historique d’exécution des scénarios. Vous pouvez trier les éléments selon les valeurs suivantes :

* Heure de début de l’exécution
* Statut d’exécution
* Durée d’exécution
* Nombre d’opérations
* Quantité de données transférées

Pour plus d’informations sur le filtrage et le tri de l’historique d’exécution, voir la section [Afficher l’historique d’exécution d’un scénario dans Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Les liens d’aide dans Fusion mènent désormais à des articles spécifiques.

Afin de vous aider à trouver plus facilement les informations dont vous avez besoin, nous avons mis à jour les liens d’aide dans Fusion afin de vous diriger directement vers l’article concernant la zone de Fusion dans laquelle vous travaillez.

Vous pouvez cliquer sur l’icône d’aide dans n’importe quelle zone de Fusion pour accéder à l’article traitant de cette zone. Par exemple, le lien d’aide du panneau Paramètres du scénario mène à l’article décrivant ce panneau, tandis que le lien d’aide d’un module Workfront renvoie à l’article décrivant la configuration des modules Workfront. Vous pouvez également cliquer sur les liens en surbrillance dans le texte explicatif pour consulter l’article correspondant, par exemple une liste des formats de date et d’heure pris en charge.

Auparavant, les liens d’aide de Fusion ouvraient la documentation de Workfront Fusion, où vous pouviez ensuite effectuer des recherches, dans la rubrique de votre choix.

## L’historique d’exécution des scénarios n’affiche le bouton Détails que lorsque des détails sont disponibles.

Pour plus de clarté dans le tableau d’exécution des scénarios, nous avons rendu le bouton Détails visible uniquement pour les exécutions dont les détails sont disponibles. Vous pouvez maintenant déterminer en un coup d’œil si les détails d’une exécution ont été archivés. La fonctionnalité du bouton Détails n’a pas été modifiée.

Auparavant, toutes les exécutions comportaient un bouton Détails. Or, il arrivait que les utilisateurs et utilisatrices cliquent dessus mais constataient qu’il ne contenait aucune information.

Pour plus d’informations, voir la section [Afficher l’historique d’exécution d’un scénario dans Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Délai d’expiration du connecteur de traduction gérée par SDL augmenté à 120 secondes

Pour réduire les expirations du connecteur de traduction gérée par SDL, nous avons augmenté le délai d’attente à 120 secondes.

Auparavant, la traduction gérée par SDL suivait le mécanisme de sécurisation de l’expiration de Workfront Fusion de 40 secondes.
