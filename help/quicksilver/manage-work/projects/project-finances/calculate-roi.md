---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer le retour sur investissement (ROI)
description: Le retour sur investissement (ROI) est une mesure Adobe Workfront qui permet aux personnes gestionnaires de portfolios de voir rapidement l’état du projet par rapport au bénéfice prévu d’origine et au coût budgété du projet.
author: Alina
feature: Work Management
exl-id: 1a3d16cb-8cb1-472e-8102-0ea8e0bc0edd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 100%

---

# Calculer le retour sur investissement (ROI)

Le retour sur investissement (ROI) est une mesure Adobe Workfront qui permet aux personnes gestionnaires de portfolios de voir rapidement l’état du projet par rapport au bénéfice prévu d’origine et au coût budgété du projet.

## Vue d’ensemble du retour sur investissement (ROI) d’un projet

Workfront calcule le ROI à l’aide de la formule suivante :

```
Project ROI = [(Project Planned Benefit - Project Budgeted Cost) / Project Budgeted Cost] x 100
```

Les champs suivants affectent le ROI d’un projet :

* **Bénéfice prévu du projet** : il s’agit d’une saisie manuelle spécifiée par la personne propriétaire du projet lorsqu’elle remplit la zone Informations sur le projet du business case. Il s’agit d’une estimation de ce que vous, en tant que personne propriétaire du projet, pensez être le bénéfice du projet si vous le menez à bien. Il s’agit d’un montant spécifique de devise qui doit être positif.\
  Pour plus d’informations sur le bénéfice prévu d’un projet, voir la section « Informations sur le projet » dans l’article [Créer un business case pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

* **Coût budgété du projet** : il s’agit du coût total associé au projet tel qu’il a été estimé lors du lancement du projet.

  Le **coût budgété** utilise la valeur **Coût budgeté de la main-d’œuvre** qui est calculée dans la zone Établissement du budget des ressources du business case et prend en compte les heures budgétées pour vos fonctions dans le planificateur de ressources et le coût horaire de chaque fonction.\
  Pour plus d’informations, voir [Calculer le coût budgété](../../../manage-work/projects/project-finances/budgeted-cost.md).

## Localiser le retour sur investissement (ROI) du projet

Vous pouvez consulter la valeur du ROI d’un projet dans les zones suivantes de Workfront :

* Dans l’optimisateur de portfolio, si le projet est associé à un portfolio.

  >[!NOTE]
  >
  >Le total des valeurs de ROI de tous les projets correspond au ROI du portfolio.

  Pour plus d’informations sur l’optimiseur de portfolio, voir l’article [Vue d’ensemble de l’optimiseur de portfolio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* Dans le champ ROI du projet dans les listes et rapports suivants :

   * Projet
   * Tâche
   * Problème
   * Projet (données financières)

  Pour plus d’informations sur la création de rapports dans Workfront, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
