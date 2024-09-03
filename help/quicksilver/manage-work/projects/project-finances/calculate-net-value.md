---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer la valeur nette
description: La valeur nette d’un projet correspond à la valeur totale attendue du projet après avoir calculé ses avantages et supprimé les coûts.
author: Alina
feature: Work Management
exl-id: 44e3f211-c816-4ee1-aafc-c40fc8732f1a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 100%

---

# Calculer la valeur nette

La valeur nette d’un projet correspond à la valeur totale attendue du projet après avoir calculé ses avantages et supprimé les coûts. 

## Vue d’ensemble de la valeur nette des projets

Adobe Workfront calcule la valeur nette d’un projet à l’aide de la formule suivante :

```
Project Net Value = Planned Benefit - Budgeted Cost - Potential Risk Cost
```

Les champs suivants peuvent affecter la valeur nette d’un projet :

* **Bénéfice prévu** : il s’agit d’une entrée manuelle spécifiée par la personne propriétaire du projet lors du remplissage de la zone **Informations sur le projet** du business case.\
  Pour plus d’informations sur le bénéfice prévu d’un projet, voir la section [Informations sur le projet](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) de l’article [Vue d’ensemble des zones du business case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* **Coût budgété** : il s’agit du coût total associé au projet tel qu’il a été estimé lors de son lancement.

  Le **coût budgété** utilise la valeur **Coût budgété de la main-d’œuvre**, qui est calculée dans la zone Établissement du budget de ressources du business case et prend en compte les heures budgétées pour vos fonctions dans le planificateur de ressources et le taux de coût horaire de chaque fonction.\
  Le coût budgété affecte la **valeur nette** du projet.Pour plus d’informations sur le calcul du coût budgété, voir [Calculer le coût budgété](../../../manage-work/projects/project-finances/budgeted-cost.md).

* **Coût potentiel des risques** : il s’agit du coût associé aux risques du projet, tels qu’ils sont définis dans le business case ou dans l’onglet Risques du projet.\
  Pour plus d’informations sur le calcul du coût potentiel des risques d’un projet, voir l’article [Calculer le coût potentiel des risques](../../../manage-work/projects/project-finances/potential-risk-cost.md).

   

## Localiser la valeur nette du projet

Vous pouvez trouver la valeur nette d’un projet dans les zones suivantes de Workfront :

* Dans la zone Récapitulatif du business case du business case.\
  Pour plus d’informations sur la zone Récapitulatif du business case, voir la section « Comprendre le Récapitulatif du business case » de l’article [Créer un business case pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md) [Créer un business case pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

  ![](assets/net-value-on-business-case-summary-highlighted-350x444.png)

* Dans l’optimisateur de portfolio, si le projet est associé à un portfolio.

  >[!TIP]
  >
  >Le total des valeurs nettes de tous les projets est la valeur nette du portfolio.

  Pour plus d’informations sur l’optimisateur de portfolio, voir [Vue d’ensemble de l’optimisateur de portfolio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Dans le champ Valeur nette du projet des listes et rapports suivants :

   * Projet
   * Tâche
   * Problème
   * Projet (données financières)

  Pour plus d’informations sur la création d’un rapport, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
