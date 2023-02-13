---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio Optimizer - Aperçu
description: Le [!UICONTROL Portfolio Optimizer] est l’outil utilisé pour l’évaluation et la comparaison des projets. Le processus de vérification et de comparaison des valeurs des Business Case pour les projets affectés à un portefeuille consiste à déterminer comment un gestionnaire de portefeuille peut hiérarchiser les projets et générer le plus de valeur pour une organisation.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '1654'
ht-degree: 0%

---

# [!UICONTROL Portfolio Optimizer] aperçu

Le [!UICONTROL Portfolio Optimizer] est l’outil utilisé pour l’évaluation et la comparaison des projets. Processus de révision et de comparaison [!UICONTROL Analyse de cas] les valeurs pour les projets affectés à un portefeuille sont la manière dont un gestionnaire de portefeuille peut hiérarchiser les projets et générer le plus de valeur pour une organisation.

L’objet de la variable [!UICONTROL optimiseur de portefeuille] est de fournir une interface permettant à un gestionnaire de portefeuille, à un comité de pilotage ou à un bureau de gestion de produits d’afficher des informations récapitulatives sur l’analyse de performances de chaque projet. Les projets peuvent ensuite être classés par ordre de priorité en fonction des valeurs et des objectifs stratégiques ou de leur note globale.

Le [!UICONTROL Portfolio Optimizer] ne peut vous aider que si vous avez rempli les conditions préalables suivantes :


* Le [!UICONTROL Analyses de cas] ont été réalisés sur les projets. Pour plus d’informations, voir les articles de la section [Définition d’un cas d’entreprise](../../projects/define-a-business-case/define-business-case.md).
* Un portfolio est défini dans la section Aperçu du projet de la section Détails du projet pour les projets que vous souhaitez consulter.
* Vous avez indiqué le budget du projet et les avantages prévus pour les projets que vous souhaitez passer en revue. Le coût fixe et les recettes fixes sont facultatifs, mais ils ajoutent une valeur supplémentaire. Pour plus d’informations, voir [Champs de financement du projet](../../projects/project-finances/project-finances-overview-1.md).


Pour plus d’informations sur la localisation de la variable [!UICONTROL Portfolio Optimizer], voir [Recherchez la variable [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finances dans [!UICONTROL Portfolio Optimizer]

* [Les domaines financiers dans la [!UICONTROL Portfolio Optimizer]](#the-financial-areas-in-the-portfolio-optimizer)
* [Les champs financiers du [!UICONTROL Portfolio Optimizer]](#the-financial-fields-in-the-portfolio-optimizer)

Vous pouvez consulter l’état financier de votre portefeuille à tout moment pendant la durée de vos projets lors de l’utilisation de la variable [!UICONTROL Portfolio Optimizer].

Tenez compte de ce qui suit lorsque vous utilisez des ressources dans le [!UICONTROL Portfolio Optimizer]:

* Les projets reçoivent chacun un score lorsque leur [!UICONTROL Analyses de cas] sont remplis selon les critères qu’ils correspondent dans la variable [!UICONTROL Portfolio Optimizer]. Par exemple, les projets à faible coût ou d’alignement élevé reçoivent un score plus élevé.

   Pour plus d’informations sur le calcul du score d’optimisation de portefeuille d’un projet, consultez l’article . [Présentation de la variable [!UICONTROL Portfolio Optimizer] Score](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* Les calculs financiers pour la variable [!UICONTROL Portfolio Optimizer] utilisez la méthode [!UICONTROL Coût budgété] dans le [!UICONTROL Analyse de cas] du projet.
* Vous pouvez hiérarchiser manuellement vos projets dans la [!UICONTROL Portfolio Optimizer], en prenant en compte toutes les informations les concernant. Cela inclut les données financières, l’alignement sur leurs fiches d’évaluation, le retour sur investissement, par exemple.

### Les domaines financiers dans la [!UICONTROL Portfolio Optimizer] {#the-financial-areas-in-the-portfolio-optimizer}

Vous pouvez afficher des informations financières dans les zones suivantes du [!UICONTROL Portfolio Optimizer]:

* **[!UICONTROL En-tête de Portfolio]**: Ce domaine présente les informations financières recueillies sur tous les projets du portfolio. Il s’affiche sur chaque onglet de l’objet de Portfolio.
* **[!UICONTROL Finances de Portfolio pour les projets sélectionnés]**: Cette zone affiche les informations financières recueillies sur les projets sélectionnés dans la [!UICONTROL Portfolio Optimizer]. Vous pouvez ajouter ou supprimer des projets et comprendre comment cela affectera les finances du portefeuille en consultant les informations dans ce domaine.
* **[!UICONTROL Finances des projets]**: Cette zone affiche les informations financières de chaque projet répertoriées dans le [!UICONTROL Portfolio Optimizer].

### Les champs financiers du [!UICONTROL Portfolio Optimizer] {#the-financial-fields-in-the-portfolio-optimizer}

Les champs financiers suivants s’affichent dans la variable [!UICONTROL Portfolio Optimizer]:

* [En-tête de Portfolio](#portfolio-header)
* [Finances Portfolios pour des projets sélectionnés](#portfolio-finances-for-selected-projects)

#### En-tête de Portfolio {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] calcule les champs financiers de l’en-tête de portefeuille à l’aide des informations provenant de projets dont le statut est égal uniquement à [!UICONTROL Approuvé] ou [!UICONTROL Actuel].

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
   <td>[!UICONTROL Heure d’activation]</td> 
   <td> <p>Pourcentage de projets du portefeuille considérés comme étant [!UICONTROL à l’heure]. Cette option est visible à partir de n’importe quel onglet d’un Portfolio.</p> <p>Un projet est considéré comme étant [!UICONTROL Heure d’activation] lorsque le projet <strong>[!UICONTROL Condition]</strong> is <strong>[!UICONTROL Sur Target]</strong>. <br>Pour plus d’informations sur les [!UICONTROL Conditions du projet], voir l’article <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Présentation de la condition et du type de condition du projet</a>.</p> <p>Le <strong>[!UICONTROL Heure d’activation]</strong> Le pourcentage est calculé à l’aide de la formule suivante :</p> <p><em>[!UICONTROL Pourcentage Portfolio d’activation] = Nombre de projets / Nombre total de projets dans un état [!UICONTROL Actuel] ou [!UICONTROL Approuvé]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sur Le Budget]</td> 
   <td> <p>Pourcentage de projets du portefeuille considérés comme étant [!UICONTROL sur le budget]. Ceci est visible à partir de n’importe quel onglet dans un [!UICONTROL Portfolio].</p> <p>Les projets sont <strong>[!UICONTROL Sur Le Budget]</strong> lorsqu’ils n’ont pas dépassé leur budget prédéfini. <br>Pour plus d’informations sur le budget d’un projet, consultez l’article <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Informations [!UICONTROL Gérer] dans la zone Finance du projet</a>.</p> <p>Le pourcentage [!UICONTROL Sur le budget] est calculé à l’aide de la formule suivante :</p> <p><em>[!UICONTROL Sur Le Pourcentage Du Portfolio Budgétaire] = Nombre De Projets / Nombre Total De Projets </em><em>dans un état [!UICONTROL Actuel] ou [!UICONTROL Approuvé]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (pour le portefeuille)</td> 
   <td> <p>Le [!UICONTROL Retour sur investissement] (ROI) du portefeuille est calculé en prenant en compte l’[!UICONTROL Avantage] total du [!UICONTROL Portfolio] et le total des [!UICONTROL Coûts budgétés] des projets. Cette option est visible à partir de n’importe quel onglet d’un Portfolio.</p> <p>La valeur du ROI Portfolio est calculée en utilisant la formule suivante :</p> <p><em>ROI Portfolio = ([!UICONTROL Total des avantages] - [!UICONTROL Total des coûts budgétés])/ [!UICONTROL Coût total] * 100</em> </p> <p>Pour plus d’informations sur le mode de calcul du ROI d’un projet, consultez l’article . <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Calcul du retour sur investissement</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aligné] ou [!UICONTROL Score d’alignement] </td> 
   <td> <p>Moyenne de toutes les valeurs [!UICONTROL Score d’alignement du projet] calculées après avoir rempli la [!UICONTROL Fiche d’évaluation] dans l’[!UICONTROL Analyse de cas] du projet. Le score d’alignement de chaque projet est répertorié dans la colonne [!UICONTROL Alignement] de [!UICONTROL Portfolio Optimizer]. Cette option est visible à partir de n’importe quel onglet d’un portfolio.</p> <p>Pour plus d’informations sur la génération d’un score d’alignement pour un projet, reportez-vous à l’article <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Application d’une fiche d’évaluation à un projet et génération d’une note d’alignement</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Net Value]</td> 
   <td> <p>La somme de toutes les [!UICONTROL valeurs nettes] de tous les projets du portefeuille. Cette option est visible à partir de n’importe quel onglet d’un portfolio.</p> <p>Pour plus d’informations sur le calcul de [!UICONTROL Net Value] pour un projet, reportez-vous à l’article <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calculer la valeur nette</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Finances Portfolios pour des projets sélectionnés {#portfolio-finances-for-selected-projects}

![](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nom du champ</strong> </th> 
   <th> <p><strong>Description</strong> </p> <p> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nombre de projets]</td> 
   <td> <p>Nombre total de principaux projets du portfolio. Les projets considérés comme principaux dans un portfolio peuvent avoir l’un des états suivants :</p> 
    <ul> 
     <li>[!UICONTROL Actuel]</li> 
     <li>[!UICONTROL Planning]</li> 
     <li>[!UICONTROL Approuvé]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget]</td> 
   <td>Vous pouvez mettre à jour manuellement ce champ pour indiquer le budget total de l'ensemble du portfolio. Ce budget est utilisé pour tous les projets du portefeuille. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Restant]</td> 
   <td> <p>Le budget restant après l'ensemble des [!UICONTROL Coûts budgétés] sur tous les projets du portefeuille a été soustrait du budget du portefeuille.</p> <p>Le [!UICONTROL Budget Portfolio restant] est calculé à l’aide de la formule suivante :</p> <p><em>[!UICONTROL Restant du budget Portfolio] = [!UICONTROL Total du budget Portfolio] - Total [!UICONTROL Coût budgété] de tous les projets de Portfolio</em> </p> <p>L’[!UICONTROL Coût budgété] global de tous les projets du portefeuille est représenté dans la barre d’indicateurs située sous le champ Budget . </p> <p>Pour plus d’informations sur le suivi des coûts sur un projet, consultez l’article .<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivi des coûts</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût total]</td> 
   <td> <p>Somme des coûts de tous les projets affichés dans [!UICONTROL Portfolio Optimizer]. Le coût de chaque projet est le même que le coût [!UICONTROL Budget] du projet, tel qu’il est affiché dans le [!UICONTROL Résumé du cas d’entreprise]. </p> <p>Pour plus d’informations sur les champs financiers des projets dans l’[!UICONTROL Business Case], consultez la section "Présentation des champs financiers dans l’analyse de cas" de l’article . <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Création d’une analyse de cas pour un projet </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risque] </td> 
   <td> <p>Somme de tous les [!UICONTROL Risques potentiels] de tous les projets du portefeuille. Le [!UICONTROL Coût des risques potentiels] de chaque projet est répertorié dans la colonne [!UICONTROL Risque] de [!UICONTROL Optimizer de Portfolio]. </p> <p>Pour plus d’informations sur le calcul des risques pour les projets, voir l’article <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcul du coût du risque potentiel </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Avantage]</td> 
   <td> <p>Somme de toutes les valeurs [!UICONTROL Advertising] de tous les projets du portefeuille. La valeur des avantages prévus de chaque projet est répertoriée dans la colonne [!UICONTROL Avantage] de [!UICONTROL Optimizer de Portfolio]. </p> <p>Pour plus d’informations sur les [!UICONTROL Avantages planifiés] d’un projet, consultez l’article . <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Aperçu des avantages prévus du projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Indicateur [!UICONTROL Risque jusqu’à la valeur nette]</td> 
   <td> <p>Mesure la valeur du [!UICONTROL Risque potentiel] en tenant compte de la [!UICONTROL Valeur nette] fournie par tous les projets du portefeuille. Pour optimiser l’efficacité au sein du portefeuille, vous souhaitez vérifier que l’indicateur [!UICONTROL Risque] est faible et que l’indicateur [!UICONTROL Valeur nette] est élevé. </p> <p>Pour plus d’informations sur le calcul du risque à [!UICONTROL Net Value], consultez l’article . <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Calcul du risque par rapport à la valeur nette d’un portefeuille</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnalisez le [!UICONTROL Portfolio Optimizer]

Vous pouvez personnaliser uniquement la zone de liste des projets de la variable [!UICONTROL Portfolio Optimizer] en utilisant les paramètres pour modifier les informations de la liste.

Les icônes et options suivantes sont disponibles pour la fonction [!UICONTROL Portfolio Optimizer]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Icône dans Portfolio Optimizer</td> 
   <td>Nom</td> 
   <td>Fonction</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Définir la priorité du projet]</td> 
   <td>Utilisez cette icône lorsque vous souhaitez enregistrer l’ordre du projet en fonction de leur priorité. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL Optimisation de portefeuille]</td> 
   <td>Utilisez cette icône pour optimiser le portefeuille en fonction des valeurs financières suivantes des projets :
    <ul>
     <li>Coût [!UICONTROL]</li>
     <li>[!UICONTROL Alignement]</li>
     <li>[!UICONTROL Value]</li>
     <li>[!UICONTROL Risque à mettre au profit]</li>
     <li>ROI [!UICONTROL]</li>
    </ul><p>Pour plus d’informations sur l’optimisation de votre portefeuille, reportez-vous à l’article <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Optimisation des projets dans [!UICONTROL Portfolio Optimizer] </a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>Icônes [!UICONTROL Annuler]/ [!UICONTROL Rétablir]</td> 
   <td>Utilisez ces icônes pour annuler ou rétablir les modifications apportées à [!UICONTROL Portfolio Optimizer] avant de les enregistrer.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Afficher]/ [!UICONTROL Masquer les projets non cochés]</td> 
   <td>Utilisez ces icônes pour afficher ou masquer les projets du portfolio que vous avez décochés.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Utilisez cette icône pour exporter les données de la zone [!UICONTROL Project Prioritization] de [!UICONTROL Portfolio Optimizer]. Vous pouvez l’exporter aux formats suivants :</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Onglet] Délimité</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL Preferences]</td> 
   <td> <p>Utilisez cette icône pour modifier les champs du projet affichés dans les colonnes de [!UICONTROL Portfolio Optimizer] ou pour modifier les projets que vous affichez dans [!UICONTROL Optimizer] en fonction de leur état. </p> <p>Conseil :  
     <ul> 
      <li> <p>Pas tous [!DNL Workfront] des champs standard peuvent être ajoutés dans les colonnes. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Vous pouvez ajouter uniquement les champs personnalisés dont la valeur est autre que zéro dans l’un des projets du portfolio.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
