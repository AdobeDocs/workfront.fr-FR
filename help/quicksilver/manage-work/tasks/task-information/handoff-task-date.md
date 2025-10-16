---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Aperçu de la date de remise de la tâche
description: La date de remise est la date à laquelle une tâche est disponible pour le travail. Cela signifie généralement que ses tâches antérieures sont terminées et que la personne cessionnaire de la tâche peut commencer à travailler dessus.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 99%

---

# Vue d’ensemble de la date de remise de la tâche

La date de remise est la date à laquelle une tâche est disponible pour le travail. Cela signifie généralement que ses tâches antérieures sont terminées et que la personne cessionnaire de la tâche peut commencer à travailler dessus.

>[!TIP]
>
>Il n’existe pas de date de remise pour les problèmes et les projets.

## Méthode de calcul de la date de remise par Adobe Workfront

>[!NOTE]
>
>La date de remise n’est calculée que si le statut du projet correspond aux statuts suivants :
>
>* Suspendu
>* Actuel
>* Terminé
>* Immobilisé
>

Workfront applique les règles suivantes pour calculer la date de remise d’une tâche :

* **Lorsque la tâche a une tâche antérieure incomplète** : la date de remise de la tâche est nulle.
* **Lorsque la tâche a une tâche antérieure complète** : la date de remise est identique à la date d’achèvement réelle de la tâche antérieure. Si la tâche antérieure a un décalage, Workfront calcule la Date de remise de la tâche qui lui succède à l’aide de la formule suivante :

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  Pour plus d’informations sur le décalage, voir [Vue d’ensemble des types de décalage](../use-prdcssrs/lag-types.md).

  Si la tâche qui lui succède comporte plusieurs tâches antérieures, la date de remise est calculée en fonction de la dernière date d’achèvement réelle des tâches antérieures. Par exemple, si les dates d’achèvement réelles des deux tâches antérieures sont le 8 novembre 2022 et le 20 novembre 2022, la date de remise de la tâche ultérieure est le 20 novembre 2022.

  >[!NOTE]
  >
  >   Le calcul de la date de remise d’une tâche ultérieure en fonction de la date d’achèvement réelle ou d’une tâche antérieure est le même que la tâche antérieure soit appliquée ou non. Pour plus d’informations sur l’application des tâches antérieures, voir [Forcer les tâches antérieures](../use-prdcssrs/enforced-predecessors.md)


* **Lorsque la tâche n’a pas de tâche antérieure et que** :

   * **La date de début prévue se situe dans le passé.** : la date de remise est identique à la date de début prévue du projet si aucune contrainte forcée n’est définie pour la tâche. Pour les cas où les tâches ont des contraintes forcées, voir la section « Lorsque la tâche a une contrainte forcée pour les dates prévues » ci-dessous.
   * **La date de début prévue se situe dans le futur (toute date postérieure à la date actuelle)** : la date de remise est identique à la date de début prévue de la tâche si aucune contrainte forcée n’est définie pour celle-ci. Pour les cas où les tâches ont des contraintes forcées, voir la section « Lorsque la tâche a une contrainte forcée pour les dates prévues » ci-dessous.

>[!NOTE]
>
>Lorsque la tâche a un projet transversal antérieur, la date de remise du projet ultérieur ne se recalcule que lorsque l’un des événements suivants se produit :
>
>* Vous pouvez recalculer manuellement la chronologie du projet du projet ultérieur. Pour recalculer la chronologie, vous devez disposer des autorisations de gestion du projet.
>* La chronologie du projet du projet ultérieure st automatiquement recalculée la nuit.
>
>Pour plus d’informations sur le recalcul de la chronologie du projet, voir [Recalculer les chronologies d’un projet](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **Lorsque la tâche présente une contrainte forcée pour les dates prévues** : la date de remise varie selon le type de contrainte et selon que la tâche possède ou non une date de début effective.\
  Les contraintes suivantes sont imposées sur les tâches :

   * Il Faut Commencer Le
   * Il Faut Finir Le
   * Commencer Au Plus Tôt
   * Commencer Au Plus Tard
   * Date fixe

  Les scénarios suivants sont possibles :

   * **Lorsque la tâche présente une contrainte Doit démarrer le ou Ne pas démarrer au plus tôt** : si la date de la contrainte de tâche se situe dans le passé et qu’il n’existe pas de date de début effective sur la tâche (la tâche n’a pas encore démarré), la date de remise est la date la plus proche à laquelle la tâche peut être démarrée. Si la tâche a commencé, la date de remise correspond à la date de début du projet.
   * **Lorsque la tâche présente une contrainte Doit se terminer le ou Ne pas démarrer plus tard que** : si la date de la contrainte de tâche se situe dans le futur et qu’il n’y a pas de date de début effective sur la tâche (la tâche n’a pas encore démarré), la date de remise est la date de début prévue de la tâche. S’il existe une date de début effective sur la tâche, la date de remise correspond à la date de début du projet.
   * **Lorsque la tâche présente une contrainte de dates fixes** : la date de remise est la date de début prévue de la tâche, qu’elle ait ou non une tâche antérieure et que celle-ci soit terminée ou non.

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## Localiser la date de remise

Vous pouvez afficher la date de remise d’une tâche dans un rapport de tâche ou la vue de liste de tâches.\
Pour plus d’informations sur la création d’un rapport, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
