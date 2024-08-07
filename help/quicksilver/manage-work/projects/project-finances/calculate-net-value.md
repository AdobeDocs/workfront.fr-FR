---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer la valeur nette
description: La valeur nette d’un projet est la valeur totale attendue du projet après avoir calculé ses avantages et supprimé les coûts.
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 3%

---

# Calculer la valeur nette

La valeur nette d’un projet est la valeur totale attendue du projet après avoir calculé ses avantages et supprimé les coûts. 

## Présentation de la valeur nette du projet

Adobe Workfront calcule la valeur nette d’un projet à l’aide de la formule suivante : 

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

Les champs suivants peuvent affecter la valeur nette d’un projet :

* **Avantage planifié** : il s’agit d’une entrée manuelle spécifiée par le propriétaire du projet lors de l’achèvement de la zone **Informations sur le projet** de l’analyse de cas client.\
  Pour plus d’informations sur les avantages prévus d’un projet, consultez la section [Informations sur le projet](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) de l’article [Présentation des domaines de l’analyse de cas](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Coût budgété** : coût total associé au projet tel qu’estimé lors du premier lancement du projet.

  Le **Coût budgété** utilise la valeur **Coût du travail budgété** qui est calculée dans la zone Ressource/Budget de l’analyse de performances et qui prend en compte les heures budgétisées pour vos rôles de travail dans le planificateur de ressources et le taux de coût par heure de chaque rôle de tâche.\
  Le coût budgété affecte la **valeur nette** du projet. Pour plus d’informations sur le mode de calcul du coût budgété, voir [Calcul du coût budgété](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Coût des risques potentiels** : coût associé à tout risque sur le projet, tel qu’il est défini dans l’analyse de cas ou dans l’onglet Risques du projet.\
  Pour plus d’informations sur le calcul du coût potentiel de risque d’un projet, consultez l’article [Calculer le coût potentiel de risque](../../../manage-work/projects/project-finances/potential-risk-cost.md).

   

## Localisation de la valeur nette du projet

Vous trouverez la valeur nette d’un projet dans les zones suivantes de Workfront :

* Dans la zone Résumé des cas d’entreprise de l’analyse de cas \
  Pour plus d’informations sur la zone de résumé de l’analyse de cas, reportez-vous à la section &quot;Comprendre le résumé de l’analyse de cas&quot; de l’article [Créer une analyse de cas pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Créer une analyse de cas pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

  ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* Dans Portfolio Optimizer si le projet est associé à un portfolio

  >[!TIP]
  >
  >Le total de toutes les valeurs nettes du projet est la valeur nette du portefeuille.

  Pour plus d’informations sur Portfolio Optimizer, consultez la [présentation de Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Dans le champ Valeur nette du projet des listes et rapports suivants :

   * Projet
   * Tâche
   * Problème
   * Projet (données financières)

  Pour plus d’informations sur la création d’un rapport, consultez l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
