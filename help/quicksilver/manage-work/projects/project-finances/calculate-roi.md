---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer le retour sur investissement (ROI)
description: Le retour sur investissement (ROI) est une mesure d’Adobe Workfront qui permet aux gestionnaires de portefeuille de déterminer rapidement les performances du projet par rapport aux avantages prévus et au coût budgétaire initial du projet.
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 3%

---

# Calculer le retour sur investissement (ROI)

Le retour sur investissement (ROI) est une mesure d’Adobe Workfront qui permet aux gestionnaires de portefeuille de déterminer rapidement les performances du projet par rapport aux avantages prévus et au coût budgétaire initial du projet.

## Présentation du retour sur investissement (ROI) du projet

Workfront calcule le ROI à l’aide de la formule suivante :

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

Les champs suivants affectent le retour sur investissement d’un projet :

* **Bénéfice prévu du projet** : il s’agit d’une entrée manuelle spécifiée par le propriétaire du projet lors de l’achèvement de la zone Informations sur le projet de l’analyse de cas client. Il s’agit d’une estimation de ce que vous, en tant que propriétaire du projet, pensez que l’avantage du projet pourrait être si vous terminez le projet. Il s’agit d’un montant spécifique de la devise et il doit s’agir d’une valeur positive.\
  Pour plus d’informations sur les avantages prévus d’un projet, consultez la section &quot;Informations sur le projet&quot; dans l’article [Créer un cas d’entreprise pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Coût budgété du projet** : coût total associé au projet tel qu’estimé lors du premier lancement du projet.

  Le **Coût budgété** utilise la valeur **Coût du travail budgété** qui est calculée dans la zone Ressource/Budget de l’analyse de performances et qui prend en compte les heures budgétisées pour vos rôles de travail dans le planificateur de ressources et le taux de coût par heure de chaque rôle de tâche.\
  Pour plus d’informations, voir [Calculer le coût budgété](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Localisation du retour sur investissement du projet

Vous pouvez afficher la valeur du retour sur investissement d’un projet dans les zones suivantes de Workfront :

* Dans Portfolio Optimizer si le projet est associé à un portfolio

  >[!NOTE]
  >
  >Le total de toutes les valeurs du ROI du projet correspond au ROI du portfolio.

  Pour plus d’informations sur Portfolio Optimizer, reportez-vous à l’article [Présentation de Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Dans le champ ROI du projet , dans les listes et rapports suivants : 

   * Projet
   * Tâche
   * Problème
   * Projet (données financières)

  Pour plus d’informations sur la création de rapports dans Workfront, reportez-vous à l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
