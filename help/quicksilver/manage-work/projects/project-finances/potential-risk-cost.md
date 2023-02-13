---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcul du coût du risque potentiel
description: Le coût des risques potentiels d’un projet tient compte des coûts potentiels des risques du projet et de leur probabilité de réalisation.
author: Alina
feature: Work Management
exl-id: f4dc1950-efd8-4936-83fd-1280ee465923
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# Calcul du coût du risque potentiel

Le coût des risques potentiels d’un projet tient compte des coûts potentiels des risques du projet et de leur probabilité de réalisation.

## Présentation du coût potentiel de risque d’un projet

Adobe Workfront calcule le coût potentiel de risque d’un projet à l’aide de la formule suivante :

```
Potential Risk Cost =SUM(Potential Risk Costs * Risk Probability)
```

Tenez compte des points suivants lorsque vous passez en revue le coût potentiel de risque d’un projet :

* Le coût du risque prévu d&#39;un projet est identique à celui du risque potentiel. 
* Le coût du risque potentiel n&#39;est pas inclus dans le coût prévu d&#39;un projet. Elle est utilisée à la place pour déterminer sa valeur nette. .

## Localisation du coût potentiel de risque d’un projet

Vous pouvez trouver les risques pour un projet et leur coût potentiel dans les domaines suivants de Workfront :

* Dans l’onglet Risques du projet.
* Dans le résumé des analyses de cas.\
   Pour plus d’informations sur l’analyse de cas d’un projet, reportez-vous à l’article [Création d’une analyse de cas pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).
* Dans un rapport de projet, lorsque vous ajoutez le champ Coût des risques planifiés aux colonnes du rapport.\
   Pour plus d’informations sur la création de rapports dans Workfront, reportez-vous à l’article [Création d’un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Dans Portfolio Optimizer, lorsque le projet est associé à un Portfolio, dans la colonne Risque .\
   La somme de tous les coûts potentiels de tous les projets du portfolio s’ajoute au risque du Portfolio.\
   Pour plus d’informations sur Portfolio Optimizer, reportez-vous à l’article [Portfolio Optimizer - Aperçu](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Pour plus d’informations sur la création de risques sur un projet, consultez l’article [Créer et modifier des risques sur les projets](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)

Pour plus d’informations sur l’analyse de cas d’un projet, reportez-vous à l’article [Création d’une analyse de cas pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).
