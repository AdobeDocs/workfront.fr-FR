---
title: Activité Publication de fusion Workfront :&nbsp;Semaine du 13 septembre 2021
description: Activité Publication de fusion Workfront :&nbsp;Semaine du 13 septembre 2021
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: d9056d6f-a62d-4516-930e-4c3f4fbaec3e
hidefromtoc: true
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Activité Publication de fusion Workfront : semaine du 13 septembre 2021

Cette page décrit toutes les améliorations apportées à Adobe Workfront Fusion au cours de la semaine du 23 septembre 2021.

Pour obtenir la liste de toutes les modifications récentes, voir [Activité Publication de fusion Adobe Workfront](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Pour obtenir la liste des correctifs récents dans Workfront Fusion, reportez-vous à la section [Mises à jour de maintenance de Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) et recherchez toutes les mises à jour intitulées Mise à jour de maintenance de la fusion Workfront.

## Filtrage et tri de l’historique d’exécution du scénario Workfront Fusion

Pour faciliter la recherche d&#39;exécutions de scénarios spécifiques, nous avons rendu possible le filtrage par davantage de champs dans l&#39;historique d&#39;exécution des scénarios. Désormais, en plus des filtres existants, vous pouvez les filtrer selon les critères suivants :

* Durée d’exécution
* Nombre d’opérations
* Quantité de données transférée
* Type d’action (exécution ou mise à jour)

Auparavant, l’historique de l’exécution ne pouvait être filtré que par heure de début ou état.

Nous avons également permis de trier l&#39;historique d&#39;exécution des scénarios. Vous pouvez trier selon les valeurs suivantes :

* Heure de début de l&#39;exécution
* Etat d&#39;exécution
* Durée d’exécution
* Nombre d’opérations
* Quantité de données transférée

Pour plus d’informations sur le filtrage et le tri de l’historique d’exécution, voir [Affichage de l’historique d’exécution d’un scénario dans Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Les liens d’aide dans Fusion mènent désormais à des articles spécifiques.

Afin de vous aider à trouver plus facilement les informations dont vous avez besoin, nous avons mis à jour les liens d’aide dans Fusion afin de vous diriger directement vers l’article sur l’espace de Fusion dans lequel vous travaillez.

Vous pouvez cliquer sur l&#39;icône d&#39;aide dans n&#39;importe quelle zone de Fusion pour accéder à l&#39;article traitant de cette zone. Par exemple, le lien d’aide du panneau Paramètres du scénario mène à l’article décrivant le panneau Paramètres du scénario, tandis que le lien d’aide d’un module Workfront renvoie à l’article décrivant la configuration des modules Workfront. Vous pouvez également cliquer sur les liens en surbrillance dans le texte explicatif pour renvoyer à l’article correspondant à ce texte explicatif, par exemple une liste de formats de date et d’heure pris en charge.

Auparavant, les liens d’aide de Fusion ouvraient la documentation de Workfront Fusion, que vous pouviez ensuite rechercher dans la rubrique de votre choix.

## L’historique d’exécution du scénario affiche uniquement le bouton Détails lorsque des détails sont disponibles.

Pour plus de clarté dans le tableau d’exécution du scénario, nous avons rendu le bouton Détails visible uniquement pour les exécutions dont les détails sont disponibles. Vous pouvez maintenant savoir en un coup d’oeil si les détails d’une exécution ont été archivés. La fonctionnalité du bouton Détails n’a pas été modifiée.

Auparavant, toutes les exécutions comportaient un bouton Détails, et il arrivait que les utilisateurs cliquent dans les détails pour constater qu’aucun détail n’était disponible.

Pour plus d’informations, voir [Affichage de l’historique d’exécution d’un scénario dans Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Délai d’expiration du connecteur de traduction gérée SDL augmenté à 120 secondes.

Pour réduire les dépassements de délai sur le connecteur de traduction gérée par SDL, nous avons augmenté le délai d’attente à 120 secondes.

Auparavant, la traduction gérée par SDL suivait la barrière de sécurité de délai d’expiration de Workfront Fusion de 40 secondes.
