---
content-type: reference
product-area: projects
navigation-topic: financials
title: Calculer le coût budgété
description: Calculer la progression du projet de suivi des coûts budgétés avec un rapport d'utilisation
author: Lisa
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: 13621c29f32a514af46489fb58397f3e96f640ce
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 97%

---

# Calculer le coût budgété

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

Le coût budgété d’un projet correspond au coût total associé au projet tel qu’il a été estimé lors de la planification du projet.

## Vue d’ensemble du coût budgété dans un projet

Vous ne pouvez pas modifier manuellement le coût budgété d’un projet. Adobe Workfront calcule le coût budgété à l’aide de la formule suivante :

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* Le **coût budgété de la main-d’œuvre du planificateur de ressources** dans le calcul ci-dessus correspond au coût associé aux fonctions dans le projet.

  Vous pouvez suivre le coût budgété de la main-d’œuvre d’un projet dans la zone de budgétisation des ressources du business case ou du planificateur de ressources.

  >[!TIP]
  >
  >  Le coût budgété de la main-d’œuvre d’un projet dans le business case s’affiche en tant que coût budgété de la main-d’œuvre du planificateur de ressources dans les rapports et les listes.

  Pour plus d’informations sur les coûts budgétés de la main-d’œuvre, voir l’article [Comprendre le coût budgété de la main-d’œuvre et les heures budgétées pour les projets](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* Le **coût des dépenses budgétées** dans le calcul ci-dessus correspond au coût prévu associé aux dépenses du projet, tel qu’il est calculé dans la zone des dépenses du business case ou dans l’onglet des dépenses du projet.\
  Pour plus d’informations sur les dépenses d’un projet, voir l’article [Gérer les dépenses d’un projet](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Le **coût fixe** dans le calcul ci-dessus représente le montant fixe associé au coût du projet, tel qu’il est défini dans la zone Finances de la section Détails du projet.\
  Pour plus d’informations sur le sous-onglet Finances d’un projet, voir l’article [Gérer les informations dans la zone Finances du projet](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront calcule toutes les informations relatives aux coûts en utilisant la devise du projet. Si vous spécifiez des heures budgétées pour vos ressources dans le planificateur de ressources, l’option permettant de changer la devise du projet est désactivée.
>
>Pour plus d’informations sur le changement de devise d’un projet, voir l’article [Changer la devise d’un projet](../../../manage-work/projects/project-finances/change-project-currency.md).

## Localiser le coût budgété d’un projet

Le coût budgété, tel qu’il apparaît dans la zone de budgétisation des ressources du business case ou du planificateur de ressources, s’affiche dans les zones suivantes de Workfront, sous les noms suivants :

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nom d’affichage du coût budgété</strong></td> 
     <td><strong>Zone de Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Coût budgété</td> 
     <td> <p>Récapitulatif du business case</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Coûts</td> 
     <td> <p>Optimisateur de portfolio</p> <p>Conseil : le total de toutes les valeurs de coût budgété du projet correspond au coût budgété du portfolio.</p> </td> 
    </tr> 
    <tr> 
     <td>Coût budgété du projet</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>Rapport du projet</p> <p>Rapport du projet (données financières)</p> <p>Rapport sur la tâche</p> <p>Rapport sur le problème</p> <p>Rapport sur les heures budgétées</p> <p>Pour plus d’informations sur la création d’un rapport, voir l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Créer un rapport personnalisé</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
