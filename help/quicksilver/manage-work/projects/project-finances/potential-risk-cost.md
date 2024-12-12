---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calculer le coût potentiel des risques
description: Le coût potentiel des risques d’un projet tient compte des coûts potentiels des risques du projet et de la probabilité qu’ils se produisent.
author: Lisa
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 85%

---

# Calculer le coût potentiel des risques

Le coût potentiel des risques d’un projet tient compte des coûts potentiels des risques du projet et de la probabilité qu’ils se produisent.

## Vue d’ensemble du coût potentiel des risques d’un projet

Adobe Workfront calcule le coût potentiel de risque d’un projet à l’aide de la formule suivante :

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

Tenez compte des points suivants lorsque vous passez en revue le coût potentiel de risque d’un projet :

* Le coût prévu des risques d’un projet est identique au coût potentiel des risques.
* Le coût potentiel des risques n’est pas inclus dans le coût prévu d’un projet. Elle est utilisée à la place pour déterminer sa valeur nette.

## Localisation du coût potentiel de risque d’un projet

Vous pouvez trouver les risques d’un projet et leur coût potentiel dans les zones suivantes de Workfront :

* Dans l’onglet Risques du projet.
* Dans le récapitulatif du business case.\
  Pour plus d’informations sur le business case d’un projet, voir l’article [Créer un business case pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* Dans un rapport de projet, lorsque vous ajoutez le champ Coût prévu des risques aux colonnes du rapport.\
  Pour plus d’informations sur la création de rapports dans Workfront, voir l’article [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Dans l’optimisateur de portfolio, lorsque le projet est associé à un portfolio, dans la colonne Risque.\
  La somme de tous les coûts potentiels des risques de tous les projets du portfolio s’ajoute au risque du portfolio.\
  Pour plus d’informations sur l’optimisateur de portfolio, voir l’article [Vue d’ensemble de l’optimisateur de portfolio](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Pour plus d’informations sur la création de risques sur un projet, voir l’article [Créer et modifier des risques sur les projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

Pour plus d’informations sur le business case d’un projet, voir l’article [Créer un business case pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).
