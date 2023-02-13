---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Présentation de la date de passation des tâches
description: La date de remise correspond à la date à laquelle une tâche est disponible pour le travail. Cela signifie généralement que ses prédécesseurs ont résolu le problème et que la personne désignée de la tâche peut commencer à travailler dessus.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 39efbf1d678cf85e9b6b61744fb046664992370c
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 3%

---

# Présentation de la date de passation des tâches

La date de remise correspond à la date à laquelle une tâche est disponible pour le travail. Cela signifie généralement que ses prédécesseurs ont résolu le problème et que la personne désignée de la tâche peut commencer à travailler dessus.

>[!TIP]
>
>Il n’existe pas de date de remise pour les problèmes et les projets.

## Méthode de calcul de la date de remise par Adobe Workfront

>[!NOTE]
>
>La date de remise n’est calculée que si l’état du projet correspond aux états suivants :
>
>* Suspendu
>* Actuel
>* Terminé
>* Immobilisé
>


Workfront applique les règles suivantes pour calculer la date de remise d’une tâche :

* **Lorsque la tâche a un prédécesseur incomplet**: La date de remise de la tâche est nulle.
* **Lorsque la tâche a un prédécesseur complet**: La Date de remise est identique à la Date de fin réelle de la tâche précédente. Si le prédécesseur a un retard, Workfront calcule la Date de passation de la tâche qui lui succède à l’aide de la formule suivante :

   `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

   Pour plus d’informations sur le délai, voir [Présentation des types de balise](../use-prdcssrs/lag-types.md).

   Si la tâche qui lui succède comporte plusieurs prédécesseur, la date de passation est calculée en fonction de la dernière date d’achèvement réelle des prédécesseurs. Par exemple, si les dates d’achèvement réelles des deux prédécesseurs sont le 8 novembre 2022 et le 20 novembre 2022, la date de passation du successeur est le 20 novembre 2022.

   >[!NOTE]
   >
   >   Le calcul de la date de remise d’une tâche de remplacement en fonction de la date de fin réelle ou d’une tâche prédécesseur est le même que le prédécesseur soit appliqué ou non. Pour plus d’informations sur les prédécesseurs appliqués, voir [Application des prédécesseurs](../use-prdcssrs/enforced-predecessors.md).


* **Lorsque la tâche n’a pas de prédécesseur et**:

   * **La date de début planifiée se situe dans le passé.**: La date de remise est identique à la date de début planifiée du projet.
   * **La Date de début planifiée se situe dans le futur (toute date postérieure à la date actuelle)**: La date de remise est identique à la date de début planifiée du projet.

>[!NOTE]
>
>Lorsque la tâche a un prédécesseur multi-projet, la date de remise du successeur ne se recalcule que lorsque l’un des événements suivants se produit :
>
>* Vous pouvez recalculer manuellement la chronologie du projet du successeur. Pour recalculer la chronologie, vous devez disposer des autorisations de gestion du projet.
>* La chronologie du projet du successeur est automatiquement recalculée la nuit.
>
>Pour plus d’informations sur le recalculage de la chronologie du projet, voir [Recalculer les calendriers du projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Lorsque la tâche présente une contrainte pour les dates prévues**: La date de remise est toujours identique à la date définie par la contrainte, indépendamment de toute autre condition.\
   Les contraintes suivantes sont imposées sur les tâches :

   * Il Faut Commencer Le
   * Il Faut Finir Le
   * Commencer Au Plus Tôt
   * Commencer Au Plus Tard
   * Date fixe

## Localisation de la date de remise

Vous pouvez afficher la Date de remise d&#39;une tâche dans un rapport de tâche ou l&#39;affichage d&#39;une liste de tâches.\
Pour plus d’informations sur la création d’un rapport, voir [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
