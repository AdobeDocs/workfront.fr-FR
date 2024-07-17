---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Vue d’ensemble du score de l’optimiseur de portfolio
description: Vous trouverez le score Portfolio Optimizer dans Portfolio Optimizer. Il s’affiche dans la colonne [!UICONTROL Score] pour chaque projet. Ceci représente un score pour chaque projet du portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# Score [!UICONTROL Portfolio Optimizer] - Aperçu

Vous pouvez trouver le score [!UICONTROL Portfolio Optimizer] dans [!UICONTROL Portfolio Optimizer]. Il s’affiche dans la colonne **[!UICONTROL Score]** pour chaque projet. Ceci représente un score pour chaque projet du portfolio.

Pour plus d’informations sur la localisation de [!UICONTROL Portfolio Optimizer], reportez-vous à l’article [[!UICONTROL Portfolio Optimizer] overview](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Pour plus d’informations sur la façon dont [!DNL Adobe Workfront] utilise la note du projet et d’autres informations sur le projet pour optimiser les projets dans [!UICONTROL Portfolio Optimizer], voir [Optimisation des projets dans Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

## Différence entre le [!UICONTROL score d’alignement] et le [!UICONTROL  score d’optimisation de Portfolio]

Il existe une différence entre le score d’alignement et le score d’optimisation de portefeuille d’un projet.

Le score d’alignement d’un projet est calculé en fonction des points obtenus après avoir rempli la fiche d’évaluation. Ce score est ensuite utilisé pour déterminer le score d’alignement du portfolio. Le score d&#39;alignement s&#39;affiche en pourcentage.\
Le score d’alignement d’un projet s’affiche dans la colonne **[!UICONTROL Alignement]** de [!UICONTROL Portfolio Optimizer] ou dans le champ [!UICONTROL Alignement] de la [!UICONTROL synthèse des analyses de cas].

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

Pour plus d’informations sur la génération du score d’alignement d’un projet, consultez l’article [Application d’une fiche d’évaluation à un projet et génération d’une note d’alignement](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Le score [!UICONTROL optimiseur de portefeuille] est un classement automatiquement calculé dans l’ [!UICONTROL Portfolio Optimizer] par lequel les projets peuvent être classés par priorité. Le score d’optimisation de portefeuille s’affiche en tant qu’icône d’indicateur accompagnée d’un nombre et s’affiche dans la colonne **[!UICONTROL Score]** de l’ [!UICONTROL Portfolio Optimizer].

>[!NOTE]
>
>Un projet ne peut être noté dans [!UICONTROL Portfolio Optimizer] que si son analyse de cas a été terminée. Pour plus d’informations sur l’exécution d’une analyse de cas, consultez l’article [[!UICONTROL Créer une analyse de cas] pour un projet](../../../manage-work/projects/define-a-business-case/create-business-case.md).

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

Le score de chaque projet est calculé en fonction de l&#39;importance des catégories suivantes :

* [!UICONTROL Cost]
* [!UICONTROL Alignement]
* [!UICONTROL Valeur réseau]
* [!UICONTROL  Risque de bénéfice ]
* [!UICONTROL ROI]

## Calcul du score [!UICONTROL Portfolio Optimizer]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront] produit un score à l’aide de [!UICONTROL Portfolio Optimizer] qui est un classement permettant de hiérarchiser les projets. Les valeurs du portfolio sont basées sur les valeurs renseignées dans les affaires des projets et sont utilisées pour calculer un score pour le projet. Les projets dont le score est plus élevé peuvent être considérés comme ayant une plus grande importance et ils peuvent être prioritairement terminés en premier.

Pour connaître le classement d’un projet, procédez comme suit :

1. Accédez à [!UICONTROL Portfolio Optimizer].
1. Passez la souris sur l’icône de classement pour afficher le score d’optimisation de portefeuille d’un projet.

![ranking_icon_in_portfolio_optimizer_new.png](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

L’algorithme de calcul des scores prend en compte les valeurs définies dans les Analyses de cas des projets et les poids qu’ils portent. Il attribue un score à chaque projet de l’optimiseur et normalise ce score afin qu’il y ait toujours un projet avec un score de 100. Cela donne un score élevé au meilleur projet.

**Exemple :** Par exemple, si vous faites de [!UICONTROL alignement supérieur] le seul facteur à prendre en compte, le projet dont l’alignement est le plus élevé obtient un score de 100.

Vous trouverez ci-dessous des critères pour lesquels vous pouvez noter un projet en :

* [!UICONTROL Cost]
* [!UICONTROL Alignement]
* [!UICONTROL Valeur]
* [!UICONTROL  Risque de bénéfice ]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

Pour plus d’informations sur l’optimisation des projets dans le portefeuille, voir [Optimisation des projets dans [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

Chaque critère du panneau de configuration ([!UICONTROL Cost], [!UICONTROL Alignement], [!UICONTROL ROI], [!UICONTROL Net Value], [!UICONTROL Risk to Avantage]) reçoit sa pondération dans la plage 0 à 100 en fonction de ce que vous avez sélectionné.

Pour chaque projet avec une analyse de cas complète, un score par critère est généré à l’aide de la formule suivante :

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**Exemple :** Pour le [!UICONTROL score d’alignement] pour le projet A, vous aurez les éléments suivants :

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

Une fois que tous les [!UICONTROL Score par critère] sont calculés, vous pouvez les ajouter en prenant en compte leur poids pour obtenir le score complet par projet. Le score du projet est calculé à partir de la formule suivante :

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

Pour le coût du projet et le [!UICONTROL risque], la logique fonctionne en sens inverse de la façon dont les autres critères fonctionnent : si vous souhaitez que le [!UICONTROL faible coût] soit important pour vous, il n’augmentera pas mais diminuera le score global du projet de `Cost Score * Cost Weight`.

Une fois que les scores sont calculés pour chaque projet, la [!UICONTROL note d’optimisation] est définie pour les projets de la manière suivante :

1. Les scores [!UICONTROL Minimum] et [!UICONTROL Maximum] sont définis.
1. La plage entre ces valeurs est calculée.
1. Pour chaque projet, le [!UICONTROL score d’optimisation] est calculé à l’aide de la formule suivante :

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
