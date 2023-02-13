---
content-type: reference
product-area: projects
navigation-topic: financials
title: Calcul du coût budgété
description: Calculer la progression du projet de suivi des coûts budgété avec un rapport d’utilisation"
author: Alina
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 2%

---

# Calcul du coût budgété

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

Le coût budgété d’un projet est le coût total associé au projet, estimé lors de la planification du projet.

## Présentation du coût budgétaire dans un projet

Vous ne pouvez pas modifier manuellement le coût budgété d’un projet. Adobe Workfront calcule le coût budgété à l’aide de la formule suivante :

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* Le **Coût de la main-d’oeuvre budgété du planificateur de ressources** dans le calcul ci-dessus, vous trouverez le coût associé aux rôles de tâche dans le projet.

   Vous pouvez effectuer le suivi du Coût de la main-d’oeuvre budgété d’un projet dans la zone Budget des ressources de l’Analyse de cas ou du planificateur de ressources.

   >[!TIP]
   >
   >  Le Coût de la main-d’oeuvre budgété d’un projet dans l’Analyse de cas affiche le Coût de la main-d’oeuvre budgété du planificateur de ressources dans les rapports et les listes.

   Pour plus d’informations sur les coûts de main-d’oeuvre budgétés, voir l’article [Présentation de l’option Coût de la main-d’oeuvre budgétisé et heures budgétisées pour les projets](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* Le **Coût des dépenses budgétisées** dans le calcul ci-dessus se trouve le Coût planifié associé aux dépenses du projet, telles qu&#39;elles sont calculées dans la zone Dépenses de l&#39;Analyse de cas ou dans l&#39;onglet Dépenses du projet.\
   Pour plus d’informations sur les dépenses relatives à un projet, consultez l’article [Gestion des dépenses de projet](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Le **Coût fixe** dans le calcul ci-dessus est le montant fixe associé au coût du projet, tel que défini dans la section Finances de la section Détails du projet.\
   Pour plus d’informations sur le sous-onglet Finance d’un projet, consultez l’article [Gestion des informations dans la zone Finance du projet](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront calcule toutes les informations de coût à l’aide de la devise du projet. Si vous définissez des Heures budgétées pour vos ressources dans le planificateur de ressources, l’option permettant de modifier la devise du projet est désactivée.
>
>Pour plus d’informations sur la modification de la devise d’un projet, consultez l’article . [Modification de la devise du projet](../../../manage-work/projects/project-finances/change-project-currency.md).

## Localisation du coût budgété d’un projet

Le Coût budgété tel qu&#39;il est reflété dans la zone Budget des ressources de l&#39;Analyse de cas ou du Plan des ressources s&#39;affiche dans les zones suivantes de Workfront sous les noms suivants :

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Nom d’affichage Coût planifié</strong></td> 
     <td><strong>Zone de Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Coût budgété</td> 
     <td> <p>Récapitulatif du business case</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Coûts</td> 
     <td> <p>Portfolio Optimizer</p> <p>Conseil : Le total de toutes les valeurs de l’option Coût budgété du projet correspond à l’option Coût budgété du portefeuille.</p> </td> 
    </tr> 
    <tr> 
     <td>Coût budgété du projet</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>Rapport Projet</p> <p>Rapport Projet (données financières)</p> <p>Rapport Tâches</p> <p>Rapport sur les problèmes</p> <p>Rapport Heure budgétisée</p> <p>Pour plus d’informations sur la création d’un rapport, reportez-vous à l’article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Création d’un rapport personnalisé</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
