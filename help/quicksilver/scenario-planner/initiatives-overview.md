---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Présentation des initiatives dans le planificateur de scénarios
description: Le planificateur de scénario n’est disponible que dans la nouvelle expérience Adobe Workfront et nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénario Workfront, consultez la présentation du planificateur de scénario.
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# Aperçu des initiatives dans la section [!DNL Scenario Planner]

Le [!DNL Scenario Planner] n’est disponible que dans la nouvelle [!DNL Adobe Workfront] et nécessite une licence supplémentaire. Pour plus d’informations sur la variable [!DNL Workfront Scenario Planner], voir [Le [!DNL Scenario Planner] aperçu](../scenario-planner/scenario-planner-overview.md).
En tant que chef d’entreprise, vous pouvez créer des initiatives pour les plans dans le [!DNL Adobe Workfront Scenario Planner]. Pour plus d’informations sur la création de plans, voir l’article [Créez et modifiez des plans dans le [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Présentation des initiatives

En utilisant la variable [!DNL Workfront Scenario Planner], vous pouvez estimer et examiner les informations suivantes pour chaque initiative :

* Estimez le type et le nombre de rôles de tâche qui peuvent être requis pour terminer l’initiative. Cela ajoute au nombre de rôles d’emploi requis pour le plan et calcule le coût des personnes que vous pouvez évaluer pour une initiative.
* Estimez les coûts fixes associés au travail nécessaire pour terminer l’initiative.
* Estimez l’avantage planifié que votre entreprise peut obtenir une fois l’initiative terminée.

Pour afficher des informations sur vos initiatives, vous pouvez accéder à des initiatives individuelles dans un plan. Pour plus d’informations sur la création d’initiatives et l’accès à celles-ci, reportez-vous à l’article [Créez et modifiez des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Remarques sur les initiatives

Tenez compte des points suivants lors de la création d’initiatives :

* Vous devez créer un plan avant de pouvoir créer une initiative.
* Vous pouvez créer des initiatives de toutes pièces ou importer des projets dans un plan. Les projets deviennent des initiatives dans le cadre du plan.

   Pour plus d’informations sur la création entièrement nouvelle d’une initiative, voir [Créez et modifiez des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   Pour plus d’informations sur l’importation de projets dans un plan de création d’initiatives à partir de projets, voir [Importation de projets dans des plans dans [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Les initiatives sont des unités de planification plus petites que les plans et elles ne sont créées que dans le cadre d&#39;un plan.
* L’initiative la plus courte peut avoir une durée d’un mois. La plus longue initiative peut avoir une durée de 5 ans.
* Vous ne pouvez pas réellement travailler sur une initiative. Au niveau de l&#39;initiative, vous pouvez définir les ressources nécessaires et les coûts que ces ressources entraîneront pour que vous puissiez commencer à exécuter l&#39;une des exigences du plan. Par exemple, si votre entreprise prévoit de développer et d’acquérir un nouveau bureau dans un nouvel emplacement, votre service peut avoir une initiative pour installer l’infrastructure réseau pour ce nouvel emplacement.
* Vous pouvez créer plusieurs initiatives dans un plan. Avec chaque initiative, vous pouvez définir une stratégie de haut niveau pour accomplir le travail dans votre département.
* Vous pouvez hiérarchiser les initiatives au sein d’un plan, de sorte que l’initiative la plus importante reçoive le plus de budget et de ressources.
* Lorsque vous créez des initiatives au sein d’un plan, tous ceux qui le consultent peuvent également voir toutes les initiatives du plan.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* Vous pouvez publier des initiatives pour créer des projets ou pour mettre à jour les projets qui y sont liés. Pour plus d’informations sur les initiatives de publication, voir [Mettez à jour ou créez des projets en publiant des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Informations financières sur les initiatives

Vous pouvez consulter des informations financières sur les initiatives individuelles pour comprendre comment les initiatives s’inscrivent dans le plan. Pour plus d’informations sur l’accès à une initiative, voir l’article [Créez et modifiez des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Vous pouvez afficher les indicateurs financiers suivants sur une initiative en y accédant dans le cadre d’un plan :

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Montant total des coûts]</td> 
   <td> <p style="font-weight: normal;">Il s’agit d’un calcul du coût total d’une initiative. </p> <p style="font-weight: normal;">[!DNL Workfront] calcule la valeur totale des coûts d’une initiative à l’aide de cette formule :</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Coûts fixes]</td> 
   <td> <p><span style="font-weight: normal;">Il s’agit d’une entrée manuelle dans laquelle vous pouvez estimer <span>un montant mensuel des coûts fixes pour chaque mois de l’initiative.</span> Cela n’inclut pas les coûts associés aux rôles ajoutés à l’initiative, qui sont capturés dans le champ [!UICONTROL Coût des personnes] .</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Coûts des personnes]</td> 
   <td> <p style="font-weight: normal;">Il s’agit d’un calcul total des coûts associés aux rôles de travail de l’initiative pour la durée de l’initiative. Ce nombre dépend du nombre d’ETR ou d’heures estimé pour un rôle d’emploi pour chaque mois de l’initiative. </p> 
     <p><b>CONSEILS</b>  
     <ul> 
      <li> <p>Le nombre d’EFS mensuels pour le même rôle de tâche peut être différent d’un mois à l’autre.</p> </li> 
      <li> <p>[!DNL Workfront] considère qu’il y a 160 heures de travail en un mois. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] calcule les [!UICONTROL Coûts des personnes] d’une initiative à l’aide de la formule suivante :</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] calcule les coûts mensuels des personnes pour chaque mois pendant la durée de l’initiative à l’aide de la formule suivante :</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>EXEMPLE</b></p>
      <p>Si vous avez une initiative d’une durée de 6 mois qui nécessite 1 Designer avec un taux horaire de 50 $ pour 1 EPT par mois et un concepteur web avec un taux horaire de 100 $ pour 2 mois de l’initiative, les coûts d’utilisation de l’initiative sont calculés comme suit :</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bénéfice prévu]</td> 
   <td>Il s’agit d’une entrée manuelle dans laquelle vous pouvez estimer les avantages globaux que votre service pourrait tirer de cette initiative. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Montant de la valeur nette]</td> 
   <td> <p style="font-weight: normal;">Cela représente la valeur de votre initiative en tenant compte des coûts globaux et de l’avantage prévu estimé pour l’initiative. [!DNL Workfront] calcule la valeur nette d’une initiative à l’aide de la formule suivante :</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted content from People Costs:
(NOTE: drafted below)</p> 
       <p>Depending on whether the plan is set up to use FTEs or hours, Workfront uses the following formulas to calculate People Cost:</p> 
       <ul> 
        <li> <p>When using FTEs: </p> <p><code>People Costs = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, where 160 is the total number of working hours in a month. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> When estimating resources using FTEs,(NOTE: drafted and yellow and fix the rest of the sentence)
      <p>When using hours:</p> 
      <p><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> 
      <p>For information about setting up the plan to use hours or FTE, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>.</p>-->

## Informations sur l’initiative dans les rapports

Vous pouvez afficher les informations sur l’initiative dans les rapports, comme décrit dans le tableau ci-dessous. Ces informations ne sont disponibles dans votre instance Workfront que si votre entreprise a acheté une licence de planificateur de scénario Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Type de rapport</b></td> 
   <td><b>Informations sur l’initiative</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>Nom, Durée, Dates de début et de fin, Entrés par, ID, Date de dernière publication*, Tous les champs du projet, y compris les champs personnalisés*</td> 
  </tr> 
  <tr> 
   <td>Rôle de tâche de l’'initiative [!UICONTROL]</td> 
   <td>Toutes les informations d’initiative comme indiqué ci-dessus, ID (rôle de tâche), Projet*, Attribution de projet Heures planifiées*, Initiative Heures de rôle de tâche, (rôle de tâche), Tous les champs de projet, y compris les champs personnalisés*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Project]*</p></td> 
   <td> <p>Toutes les informations sur l’initiative répertoriées ci-dessus*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Ces champs renseignent les informations du projet liées à l’initiative, uniquement lorsque l’initiative a été créée à partir d’un projet ou a été publiée au moins une fois dans un projet. Pour plus d’informations sur les initiatives de publication, voir [Mettez à jour ou créez des projets en publiant des initiatives dans le [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
