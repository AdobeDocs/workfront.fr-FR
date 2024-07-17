---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Vue d’ensemble de l’optimisateur de portfolio
description: '[!UICONTROL Portfolio Optimizer] est l’outil utilisé pour l’évaluation et la comparaison de projets. Le processus de vérification et de comparaison des valeurs des Business Case pour les projets affectés à un portefeuille consiste à déterminer comment un gestionnaire de portefeuille peut hiérarchiser les projets et générer le plus de valeur pour une organisation.'
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: 1fd3b135682c096f1715e5da0455fed12e882582
workflow-type: tm+mt
source-wordcount: '1629'
ht-degree: 0%

---

# [!UICONTROL Portfolio Optimizer] - Aperçu

<!-- Audited: 01/2024 -->

[!UICONTROL Portfolio Optimizer] est l’outil utilisé pour l’évaluation et la comparaison de projets. Le processus de vérification et de comparaison des valeurs [!UICONTROL Business Case] pour les projets affectés à un portefeuille consiste à déterminer comment un gestionnaire de portefeuille peut hiérarchiser les projets et générer le plus de valeur pour une organisation.

![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

L’ [!UICONTROL  optimiseur de portefeuille] a pour but de fournir une interface par laquelle un gestionnaire de portefeuille, un comité de pilotage ou un bureau de gestion de produits peut consulter des informations récapitulatives sur l’analyse de cas de chaque projet. Les projets peuvent ensuite être classés par ordre de priorité en fonction des valeurs et des objectifs stratégiques ou de leur note globale.

L’ [!UICONTROL Portfolio Optimizer] ne peut vous aider que si vous avez rempli les conditions préalables suivantes :

* Les [!UICONTROL affaires] ont été effectuées sur les projets. Pour plus d’informations, reportez-vous aux articles de la section [Définition d’un cas d’affaire : index d’article](../../projects/define-a-business-case/define-business-case.md).
* Un portfolio est défini dans la section Aperçu du projet de la section Détails du projet pour les projets que vous souhaitez consulter.
* Vous avez indiqué le budget du projet et les avantages prévus pour les projets que vous souhaitez passer en revue. Le coût fixe et les recettes fixes sont facultatifs, mais ils ajoutent une valeur supplémentaire. Pour plus d’informations, reportez-vous à la section [Le projet finance les champs](../../projects/project-finances/project-finances-overview-1.md).

Pour plus d’informations sur la localisation de [!UICONTROL Portfolio Optimizer], voir [Localisation de l’[!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finances dans [!UICONTROL Portfolio Optimizer]

Vous pouvez consulter l’état financier de votre portefeuille à tout moment pendant la durée de vie de vos projets lors de l’utilisation de [!UICONTROL Portfolio Optimizer].

Tenez compte de ce qui suit lorsque vous utilisez des finances dans [!UICONTROL Portfolio Optimizer] :

* Les projets reçoivent chacun un score lorsque leurs [!UICONTROL affaires] sont terminées en fonction des critères qu’ils correspondent dans [!UICONTROL Portfolio Optimizer]. Par exemple, les projets à faible coût ou d’alignement élevé reçoivent un score plus élevé.

  Pour plus d’informations sur le calcul du score d’optimisation de portefeuille d’un projet, voir [Présentation de la note [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* Les calculs financiers pour [!UICONTROL Portfolio Optimizer] utilisent le [!UICONTROL coût budgété] dans l’ [!UICONTROL analyse de cas] du projet.
* Vous pouvez donner la priorité manuellement à vos projets dans [!UICONTROL Portfolio Optimizer], en prenant en compte toutes les informations les concernant. Cela inclut les données financières, l’alignement sur leurs fiches d’évaluation et le retour sur investissement, par exemple.

### Les zones financières de [!UICONTROL Portfolio Optimizer] {#the-financial-areas-in-the-portfolio-optimizer}

Vous pouvez afficher des informations financières dans les zones suivantes de [!UICONTROL Portfolio Optimizer] :

* **[!UICONTROL En-tête de Portfolio]** : cette zone affiche les informations financières recueillies sur tous les projets du portefeuille. Il s’affiche sur chaque onglet de l’objet de Portfolio.
* **[!UICONTROL Finances par Portfolio pour les projets sélectionnés]** : cette zone affiche les informations financières rassemblées à partir des projets sélectionnés dans [!UICONTROL Portfolio Optimizer]. Vous pouvez ajouter ou supprimer des projets et comprendre comment cela affectera les finances du portefeuille en consultant les informations dans ce domaine.
* **[!UICONTROL Projets financiers]** : cette zone affiche les informations financières de chaque projet répertorié dans [!UICONTROL Portfolio Optimizer].

### Les champs financiers de [!UICONTROL Portfolio Optimizer] {#the-financial-fields-in-the-portfolio-optimizer}

Les champs financiers suivants s’affichent dans [!UICONTROL Portfolio Optimizer] :

* [En-tête de Portfolio](#portfolio-header)
* [Finances Portfolios pour des projets sélectionnés](#portfolio-finances-for-selected-projects)

#### En-tête de Portfolio {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] calcule les champs financiers de l’en-tête de portefeuille à l’aide des informations provenant de projets dont les états correspondent uniquement à [!UICONTROL Approuvé] ou [!UICONTROL Actuel].

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
   <td> <p>Pourcentage de projets du portefeuille considérés comme étant [!UICONTROL à l’heure]. Cette option est visible à partir de n’importe quel onglet d’un portfolio.</p> <p>Un projet est considéré comme étant [!UICONTROL À l’heure] lorsque le projet <strong>[!UICONTROL Condition]</strong> est <strong>[!UICONTROL Sur Target]</strong>. <br>Pour plus d’informations sur les [!UICONTROL Conditions du projet], consultez l’article <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Présentation de la condition et du type de condition du projet</a>.</p> <p>Le pourcentage <strong>[!UICONTROL À l’heure]</strong> est calculé à l’aide de la formule suivante :</p> <p><em>[!UICONTROL Pourcentage Portfolio horaire] = Nombre de projets / Nombre total de projets dans un état [!UICONTROL actuel] ou [!UICONTROL Approuvé]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sur Le Budget]</td> 
   <td> <p>Pourcentage de projets du portefeuille considérés comme étant [!UICONTROL sur le budget]. Ceci est visible à partir de n’importe quel onglet d’un [!UICONTROL portfolio].</p> <p>Les projets sont <strong>[!UICONTROL Sur le budget]</strong> lorsqu’ils n’ont pas dépassé leur budget prédéfini. <br>Pour plus d’informations sur le budget d’un projet, consultez l’article <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">[!UICONTROL Gérer] dans la zone Finance du projet </a>.</p> <p>Le pourcentage [!UICONTROL On Budget] est calculé à l’aide de la formule suivante :</p> <p><em>[!UICONTROL En pourcentage sur le Portfolio budgétaire] = Nombre de projets / Nombre total de projets </em><em> dans un état [!UICONTROL Actuel] ou [!UICONTROL Approuvé]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (pour le portefeuille)</td> 
   <td> <p>Le [!UICONTROL Retour sur investissement] (ROI) du portefeuille est calculé en prenant en compte l’[!UICONTROL Avantage] total du [!UICONTROL Portfolio] et le total des [!UICONTROL Coûts budgétés] des projets. Cette option est visible à partir de n’importe quel onglet d’un portfolio.</p> <p>La valeur du ROI Portfolio est calculée à l’aide de la formule suivante :</p> <p><em>ROI Portfolio = ([!UICONTROL Total des avantages] - [!UICONTROL Total des coûts budgétés])/ [!UICONTROL Coût total] * 100</em> </p> <p>Pour plus d’informations sur le mode de calcul du retour sur investissement pour un projet, consultez l’article <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Calcul du retour sur investissement (ROI)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aligné] ou [!UICONTROL Score d’alignement] </td> 
   <td> <p>Moyenne de toutes les valeurs [!UICONTROL Score d’alignement du projet], qui sont calculées après avoir rempli la [!UICONTROL Fiche d’évaluation] dans l’[!UICONTROL Analyse de cas] du projet. Le score d’alignement de chaque projet est répertorié dans la colonne [!UICONTROL Alignement] de [!UICONTROL Portfolio Optimizer]. Cette option est visible à partir de n’importe quel onglet d’un portfolio.</p> <p>Pour plus d’informations sur la génération d’un score d’alignement pour un projet, consultez l’article <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Application d’une fiche d’évaluation à un projet et génération d’une note d’alignement</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Net Value]</td> 
   <td> <p>La somme de toutes les [!UICONTROL valeurs nettes] de tous les projets du portefeuille. Cette option est visible à partir de n’importe quel onglet d’un portfolio.</p> <p>Pour plus d’informations sur le mode de calcul de [!UICONTROL Net Value] pour un projet, consultez l’article <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calculate Net Value</a>.</p> </td> 
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
   <th><strong>Description</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nombre de projets]</td> 
   <td> <p>Nombre total de projets actifs dans le portfolio. Les projets considérés comme actifs dans un portfolio peuvent avoir l’un des états suivants :</p> 
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
   <td> <p>Le budget restant après l'ensemble des [!UICONTROL Coûts budgétés] sur tous les projets du portefeuille a été soustrait du budget du portefeuille.</p> <p>Le [!UICONTROL Budget Portfolio restant] est calculé à l’aide de la formule suivante :</p> <p><em>[!UICONTROL Restant du budget Portfolio] = [!UICONTROL Total du budget Portfolio] - Total [!UICONTROL Coût budgété] de tous les projets de Portfolio{1</em> </p> <p>L’[!UICONTROL Coût budgété] global de tous les projets du portefeuille est représenté dans la barre d’indicateurs située sous le champ Budget . </p> <p>Pour plus d’informations sur le suivi des coûts sur un projet, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracker les coûts</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Coût total]</td> 
   <td> <p>Somme des coûts de tous les projets affichés dans [!UICONTROL Portfolio Optimizer]. Le coût de chaque projet est le même que le coût [!UICONTROL Budget] du projet, tel qu’il est affiché dans le [!UICONTROL Résumé du cas d’entreprise]. </p> <p>Pour plus d’informations sur les champs financiers des projets dans l’[!UICONTROL Business Case], consultez la section "Présentation des champs financiers dans l’analyse de cas" de l’article <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Créer une analyse de cas pour un projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risque] </td> 
   <td> <p>Somme de tous les [!UICONTROL Risques potentiels] de tous les projets du portefeuille. Le [!UICONTROL Coût des risques potentiels] de chaque projet est répertorié dans la colonne [!UICONTROL Risque] de [!UICONTROL Optimizer de Portfolio]. </p> <p>Pour plus d’informations sur le calcul des risques pour les projets, consultez l’article <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calculer le coût du risque potentiel</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Avantage]</td> 
   <td> <p>Somme de toutes les valeurs [!UICONTROL Advertising] de tous les projets du portefeuille. La valeur des avantages prévus de chaque projet est répertoriée dans la colonne [!UICONTROL Avantage] de [!UICONTROL Optimizer de Portfolio]. </p> <p>Pour plus d’informations sur l’[!UICONTROL Bénéfice planifié] d’un projet, consultez l’article <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Présentation de l’avantage planifié du projet</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Indicateur [!UICONTROL Risque jusqu’à la valeur nette]</td> 
   <td> <p>Mesure la valeur [!UICONTROL Risque potentiel] en prenant en compte la [!UICONTROL Valeur nette] fournie par tous les projets du portefeuille. Pour optimiser l’efficacité au sein du portefeuille, vous souhaitez vérifier que l’indicateur [!UICONTROL Risque] est faible et que l’indicateur [!UICONTROL Valeur nette] est élevé. </p> <p>Pour plus d’informations sur le calcul du risque à [!UICONTROL Valeur nette], consultez l’article <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Calculer le risque à la valeur nette dans un portefeuille</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnaliser [!UICONTROL Portfolio Optimizer]

Vous pouvez personnaliser uniquement la zone de liste de projets de l’ [!UICONTROL Portfolio Optimizer] en utilisant les paramètres pour modifier les informations de la liste.

Les icônes et options suivantes sont disponibles pour [!UICONTROL Portfolio Optimizer] :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Icône dans Portfolio Optimizer</strong></td> 
   <td><strong>Nom</strong></td> 
   <td><strong>Fonction</strong></td> 
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
    </ul><p>Pour plus d’informations sur l’optimisation de votre portefeuille, consultez l’article <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Optimisation des projets dans [!UICONTROL Portfolio Optimizer]</a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>Icônes [!UICONTROL Annuler]/ [!UICONTROL Rétablir]</td> 
   <td>Utilisez ces icônes pour annuler ou rétablir les modifications apportées à [!UICONTROL Portfolio Optimizer] avant de les enregistrer.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>Projets [!UICONTROL Afficher]/[!UICONTROL Masquer] non cochés</td> 
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
      <li> <p>Tous les [!DNL Workfront] champs standard ne peuvent pas être ajoutés aux colonnes. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Vous pouvez ajouter uniquement les champs personnalisés dont la valeur est autre que zéro dans l’un des projets du portfolio.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
