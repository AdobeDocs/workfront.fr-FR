---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Vue d’ensemble de l’optimiseur de portfolio
description: L’[!UICONTROL optimisateur de portfolio] est l’outil utilisé pour l’évaluation et la comparaison des projets. Le processus de vérification et de comparaison des valeurs des Business Case pour les projets affectés à un portfolio consiste à déterminer comment un ou une gestionnaire de portfolio peut hiérarchiser les projets et générer le plus de valeur pour une organisation.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: b07b4926ab1b1eee9b7698a445644e1cd312fa09
workflow-type: tm+mt
source-wordcount: '1649'
ht-degree: 98%

---

# Vue d’ensemble de l’[!UICONTROL optimisateur de portfolio]

<!-- Audited: 01/2024 -->

L’[!UICONTROL optimisateur de portfolio] est l’outil utilisé pour l’évaluation et la comparaison des projets. Les personnes gestionnaires de portfolio peuvent hiérarchiser les projets et générer un maximum de valeur pour l’entreprise grâce au processus de révision et de comparaison des valeurs de [!UICONTROL business case] pour les projets affectés à un portfolio.

![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

L’[!UICONTROL optimisateur de portfolio] a pour fonction de fournir une interface permettant aux personnes gestionnaires de portfolio, à un comité de direction ou à un bureau de gestion de produits d’afficher des informations récapitulatives sur le business case de chaque projet. Les projets peuvent ensuite être hiérarchisés en fonction des valeurs et des objectifs stratégiques, ou selon leur score global.

L’[!UICONTROL optimisateur de portfolio] ne peut vous aider que si vous avez rempli les conditions préalables suivantes :

* Les [!UICONTROL business cases] ont été terminés sur les projets. Pour plus d’informations, voir les articles dans [Définir un business case : index des articles](../../projects/define-a-business-case/define-business-case.md).
* Un portfolio est défini dans la zone Vue d’ensemble du projet de la section Détails du projet pour les projets que vous souhaitez réviser.
* Vous avez indiqué le budget du projet et le bénéfice prévu pour les projets que vous souhaitez réviser. Le coût fixe et les revenus fixes sont facultatifs, mais ils apportent une valeur supplémentaire. Pour plus d’informations, voir [Champs financiers d’un projet](../../projects/project-finances/project-finances-overview-1.md).

Pour plus d’informations sur la localisation de l’[!UICONTROL optimisateur de portfolio], voir [Localiser l’[!UICONTROL optimisateur de portfolio]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finances dans l’[!UICONTROL optimisateur de portfolio]

Vous pouvez consulter l’état financier de votre portfolio à tout moment au cours de vos projets par le biais de l’[!UICONTROL optimisateur de portfolio].

Tenez compte des points suivants lorsque vous travaillez avec les finances dans l’[!UICONTROL optimisateur de portfolio] :

* Chaque projet se voit attribuer un score lorsque son [!UICONTROL business case] est complété selon les critères auxquels ils correspondent dans l’[!UICONTROL optimisateur de portfolio]. Par exemple, les projets à faible coût ou d’alignement élevé reçoivent un meilleur score.

  Pour plus d’informations sur le calcul du score de l’optimisateur de portfolio d’un projet, voir [Vue d’ensemble du [!UICONTROL score de l’optimisateur de portfolio]](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* Les calculs financiers pour l’[!UICONTROL optimisateur de portfolio] utilisent le [!UICONTROL coût budgété] dans le [!UICONTROL business case] du projet.
* Vous pouvez hiérarchiser manuellement vos projets dans l’[!UICONTROL optimisateur de portfolio], en tenant compte de toutes les informations les concernant. Ces informations incluent par exemple les données financières, l’alignement sur leurs cartes de score et le retour sur investissement.

### Zones financières de l’[!UICONTROL optimisateur de portfolio] {#the-financial-areas-in-the-portfolio-optimizer}

Vous pouvez afficher des informations financières dans les zones suivantes de l’[!UICONTROL optimisateur de portfolio] :

* **[!UICONTROL En-tête de portfolio]** : cette zone affiche les informations financières recueillies sur tous les projets du portfolio. Il s’affiche sur chaque onglet de l’objet Portfolio.
* **[!UICONTROL Finances du portfolio pour les projets sélectionnés]** : cette zone affiche les informations financières recueillies sur les projets sélectionnés dans l’[!UICONTROL optimisateur de portfolio]. Vous pouvez ajouter ou supprimer des projets et comprendre quel sera l’impact sur les finances du portfolio en consultant les informations dans cette zone.
* **[!UICONTROL Finances des projets]** : cette zone affiche les informations financières de chaque projet répertorié dans l’[!UICONTROL optimisateur de portfolio].

### Champs financiers dans l’[!UICONTROL optimisateur de portfolio] {#the-financial-fields-in-the-portfolio-optimizer}

Les champs financiers suivants s’affichent dans l’[!UICONTROL optimisateur de portfolio] :

* [En-tête de portfolio](#portfolio-header)
* [Finances du portfolio pour les projets sélectionnés](#portfolio-finances-for-selected-projects)

#### En-tête de portfolio {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] calcule les champs financiers de l’en-tête du portfolio grâce aux informations provenant de projets dont le statut correspond uniquement à [!UICONTROL Approuvé] ou [!UICONTROL Actuel].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nom du champ</strong> </th> 
   <th><strong>Description</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL On Time]</td> 
   <td> <p>Pourcentage des projets du portfolio considérés comme [!UICONTROL On Time]. Cet élément est visible dans tout onglet d’un portfolio.</p> <p>Un projet est considéré comme [!UICONTROL On Time] lorsque le <strong>[!UICONTROL Condition]</strong> du projet est <strong>[!UICONTROL On Target]</strong>. <br>Pour plus d’informations sur les [!UICONTROL Project Conditions], voir l’article <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Vue d’ensemble du statut du projet et du type de statut</a>.</p> <p>Le pourcentage <strong>[!UICONTROL On Time]</strong> est calculé à partir de la formule suivante :</p> <p><em>[!UICONTROL On Time Portfolio Percentage] = Nombre de projets [!UICONTROL On Time] / Nombre total de projets avec un statut [!UICONTROL Current] ou [!UICONTROL Approved]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL On Budget]</td> 
   <td> <p>Pourcentage des projets du portfolio considérés comme [!UICONTROL On Budget]. Cet élément est visible dans tout onglet d’un [!UICONTROL portfolio].</p> <p>Les projets sont <strong>[!UICONTROL On Budget]</strong> lorsqu’ils n’ont pas dépassé leur budget prédéfini. <br>Pour plus d’informations sur le budget d’un projet, consultez l’article <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Informations [!UICONTROL Manage] dans la zone Finance du projet</a>.</p> <p>Le pourcentage [!UICONTROL On Budget] est calculé à l’aide de la formule suivante :</p> <p><em>[!UICONTROL On Budget Portfolio Percentage] = Nombre de projets [!UICONTROL On Budget] / Nombre total de projets </em><em>avec le statut [!UICONTROL Current] ou [!UICONTROL Approved]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>Retour sur investissement (du portfolio)</td> 
   <td> <p>Le [!UICONTROL Return on Investment] (ROI) du portfolio est calculé en prenant en compte le [!UICONTROL Benefit] total du [!UICONTROL Portfolio] et le total des [!UICONTROL Budgeted Costs] des projets. Cet élément est visible dans tout onglet d’un portfolio.</p> <p>La valeur du retour sur investissement du portfolio est calculée à l’aide de la formule suivante :</p> <p><em>Retour sur investissement du portfolio = ([!UICONTROL Total Benefit] - [!UICONTROL Total Budgeted Cost]) / [!UICONTROL Total Cost] * 100</em> </p> <p>Pour plus d’informations sur le mode de calcul du retour sur investissement d’un projet, voir l’article <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Calcul du retour sur investissement (ROI)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aligned] ou [!UICONTROL Alignment Score] </td> 
   <td> <p>Moyenne de toutes les valeurs [!UICONTROL Project Alignment Score], qui sont calculées après avoir rempli la [!UICONTROL Scorecard] dans l’[!UICONTROL Business Case] du projet. Le score d’alignement de chaque projet est répertorié dans la colonne [!UICONTROL Alignment] de [!UICONTROL Portfolio Optimizer]. Cet élément est visible dans tout onglet d’un portfolio.</p> <p>Pour plus d’informations sur la génération d’un score d’alignement pour un projet, voir l’article <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Appliquer une carte de performance à un projet et générer un score d’alignement</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Net Value]</td> 
   <td> <p>La somme de toutes les [!UICONTROL Net Values] de tous les projets du portfolio. Cet élément est visible dans tout onglet d’un portfolio.</p> <p>Pour plus d’informations sur le calcul de la [!UICONTROL Net Value] d’un projet, voir l’article <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calculer la valeur nette</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Finances du portfolio pour les projets sélectionnés {#portfolio-finances-for-selected-projects}

![](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nom du champ</strong> </th> 
   <th><strong>Description</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Number of projects]</td> 
   <td> <p>Nombre total de projets actifs dans le portfolio. Les projets considérés comme actifs dans un portfolio peuvent avoir l’un des statuts suivants :</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL Planning]</li> 
     <li>[!UICONTROL Approved]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget]</td> 
   <td>Vous pouvez mettre à jour manuellement ce champ pour indiquer le budget total de l’ensemble du portfolio. Ce budget est utilisé pour tous les projets du portfolio. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Remaining]</td> 
   <td> <p>Le budget restant après l’ensemble des [!UICONTROL Budgeted Costs] sur tous les projets du portfolio a été soustrait du budget du portfolio.</p> <p>Le [!UICONTROL Remaining Portfolio Budget] est calculé à l’aide de la formule suivante :</p> <p><em>[!UICONTROL Remaining Portfolio Budget] = [!UICONTROL Total Portfolio Budget] - total du [!UICONTROL Budgeted Cost] de tous les projets du portfolio</em> </p> <p>Le [!UICONTROL Budgeted Cost] global de tous les projets du portfolio est représenté dans la barre d’indicateurs située sous le champ Budget. </p> <p>Pour plus d’informations sur le suivi des coûts d’un projet, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivre les coûts</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Cost]</td> 
   <td> <p>Somme des coûts de tous les projets affichés dans [!UICONTROL Portfolio Optimizer]. Le coût de chaque projet est le même que le [!UICONTROL Budgeted Cost] du projet, tel qu’il est affiché dans le [!UICONTROL Business Case Summary]. </p> <p>Pour plus d’informations sur les champs financiers des projets dans l’[!UICONTROL Business Case], voir la section « Comprendre les champs financiers dans l’analyse de rentabilité » de l’article <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Créer une analyse de rentabilité pour un projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk] </td> 
   <td> <p>Somme de tous les [!UICONTROL Potential Risk Costs] de tous les projets du portfolio. Le [!UICONTROL Potential Risk Cost] de chaque projet est répertorié dans la colonne [!UICONTROL Risk] de [!UICONTROL Portfolio Optimizer]. </p> <p>Pour plus d’informations sur le calcul des risques pour les projets, voir l’article <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculer le coût potentiel des risques</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefit]</td> 
   <td> <p>Somme de toutes les valeurs du [!UICONTROL Planned Benefit] de tous les projets du portfolio. La valeur du bénéfice prévu de chaque projet est répertoriée dans la colonne [!UICONTROL Benefit] de [!UICONTROL Portfolio Optimizer]. </p> <p>Pour plus d’informations sur le [!UICONTROL Planned Benefit] d’un projet, voir l’article <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Vue d’ensemble du bénéfice prévu d’un projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Indicateur [!UICONTROL Risk to Net Value]</td> 
   <td> <p>Mesure la valeur de [!UICONTROL Potential Risk] en prenant en compte la [!UICONTROL Net Value] fournie par tous les projets du portfolio. Pour optimiser l’efficacité au sein du portfolio, vous devez voir que l’indicateur [!UICONTROL Risk] est faible et que l’indicateur [!UICONTROL Net Value] est élevé. </p> <p>Pour plus d’informations sur le calcul du rapport Risque/[!UICONTROL Net Value], consultez l’article <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Calculer le rapport risque/valeur nette d’un portfolio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnaliser l’[!UICONTROL optimisateur de portfolio]

Vous pouvez personnaliser uniquement la zone de liste des projets de l’[!UICONTROL optimisateur de portfolio] en utilisant les paramètres pour modifier les informations de la liste.

Les icônes et options suivantes sont disponibles pour l’[!UICONTROL optimisateur de portfolio] :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Icône dans l’optimisateur de portfolio</strong></td> 
   <td><strong>Nom</strong></td> 
   <td><strong>Fonction</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Set project priority]</td> 
   <td><p>Utilisez cette icône lorsque vous souhaitez enregistrer l’ordre des projets en fonction de leur priorité.</p>
   <p>Vous devez disposer des autorisations de gestion pour tous les projets de la liste pour pouvoir utiliser <b>Définir la priorité du projet</b></p>.
    </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL Optimize portfolio]</td> 
   <td>Utilisez cette icône pour optimiser le portfolio en fonction des valeurs financières suivantes des projets :
    <ul>
     <li>[!UICONTROL Cost]</li>
     <li>[!UICONTROL Alignment]</li>
     <li>[!UICONTROL Value]</li>
     <li>[!UICONTROL Risk to Benefit]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>Pour plus d’informations sur l’optimisation de votre portfolio, voir l’article <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Optimiser des projets dans l’[!UICONTROL Portfolio Optimizer]</a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>Icônes [!UICONTROL Undo]/ [!UICONTROL Redo]</td> 
   <td>Utilisez ces icônes pour annuler ou rétablir les modifications apportées au [!UICONTROL Portfolio Optimizer] avant de les enregistrer.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>Projets [!UICONTROL Show]/[!UICONTROL Hide] décochés</td> 
   <td>Utilisez ces icônes pour afficher ou masquer les projets du portfolio que vous avez décochés.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Utilisez cette icône pour exporter les données de la zone [!UICONTROL Project Prioritization] de l’[!UICONTROL Portfolio Optimizer]. Vous pouvez les exporter aux formats suivants :</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Tab] délimité</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL Preferences]</td> 
   <td> <p>Utilisez cette icône pour modifier les champs du projet affichés dans les colonnes de l’[!UICONTROL Portfolio Optimizer] ou pour modifier les projets que vous affichez dans l’[!UICONTROL Optimizer] en fonction de leur statut. </p> <p>Conseil :  
     <ul> 
      <li> <p>Tous les champs standard [!DNL Workfront] ne peuvent pas être ajoutés dans les colonnes. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Vous pouvez ajouter uniquement les champs personnalisés dont la valeur est autre que zéro dans l’un des projets du portfolio.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
