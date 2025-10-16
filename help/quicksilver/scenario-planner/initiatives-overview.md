---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Présentation des initiatives dans le planificateur de scénarios
description: Le planificateur de scénarios n’est disponible que dans la nouvelle expérience Adobe Workfront et nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénario Workfront, consultez la Vue d’ensemble du planificateur de scénario.
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 99%

---

# Vue d’ensemble des initiatives dans le [!DNL Scenario Planner]

En tant que personne à la tête d’une entreprise, vous pouvez créer des initiatives pour les plans dans le [!DNL Adobe Workfront Scenario Planner]. Pour plus d’informations sur la création de plans, voir l’article [Créer et modifier des plans dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Vue d’ensemble des initiatives

En utilisant le [!DNL Workfront Scenario Planner], vous pouvez estimer et examiner les informations suivantes pour chaque initiative :

* Estimez le type et le nombre de fonctions qui peuvent être requises pour terminer l’initiative. Cela s’ajoute au nombre de fonctions requises pour le plan et calcule les coûts des ressources humaines que vous pouvez évaluer pour une initiative.
* Estimez les coûts fixes associés au travail nécessaire pour terminer l’initiative.
* Estimez le bénéfice prévu que votre entreprise peut obtenir une fois l’initiative terminée.

Pour afficher des informations sur vos initiatives, vous pouvez accéder à des initiatives individuelles dans un plan. Pour plus d’informations sur la création d’initiatives et l’accès à celles-ci, consultez l’article [Créer et modifier des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Remarques sur les initiatives

Tenez compte des points suivants lors de la création d’initiatives :

* Vous devez créer un plan avant de pouvoir créer une initiative.
* Vous pouvez créer des initiatives de toutes pièces ou importer des projets dans un plan. Les projets deviennent des initiatives dans le cadre du plan.

  Pour plus d’informations sur la création d’une initiative de toutes pièces, voir [Créer et modifier des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

  Pour plus d’informations sur l’import de projets dans un plan pour créer des initiatives à partir de projets, voir [Importer des projets dans des plans dans le  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Les initiatives sont des unités de planification plus petites que les plans et elles ne sont créées que dans le cadre d’un plan.
* L’initiative la plus courte peut avoir une durée d’un mois. L’initiative la plus longue peut avoir une durée de 5 ans.
* Vous ne pouvez pas réellement travailler sur une initiative. Au niveau de l’initiative, vous pouvez définir les ressources nécessaires et les coûts que ces ressources entraîneront pour que vous puissiez commencer à exécuter l’une des exigences du plan. Par exemple, si votre entreprise prévoit de développer et d’acquérir un nouveau bureau dans un nouvel emplacement, votre service peut avoir une initiative pour installer l’infrastructure réseau pour ce nouvel emplacement.
* Vous pouvez créer plusieurs initiatives dans un plan. Avec chaque initiative, vous pouvez définir une stratégie de haut niveau pour accomplir le travail dans votre service.
* Vous pouvez hiérarchiser les initiatives au sein d’un plan, afin de vous assurer que l’initiative la plus importante reçoive le plus de budget et de ressources.
* Lorsque vous créez des initiatives au sein d’un plan, toutes les personnes consultent ce dernier peuvent également voir toutes les initiatives du plan.
* Vous pouvez publier des initiatives pour créer des projets ou pour mettre à jour les projets qui leur sont liés. Pour plus d’informations sur la publication d’initiatives, voir [Mettre à jour ou créer des projets en publiant des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Informations financières sur les initiatives

Vous pouvez consulter des informations financières sur les initiatives individuelles pour comprendre comment les initiatives s’inscrivent dans le plan. Pour plus d’informations sur l’accès à une initiative, voir l’article [Créer et modifier des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Vous pouvez afficher les indicateurs financiers suivants sur une initiative en y accédant dans le cadre d’un plan :

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs total amount]</td> 
   <td> <p style="font-weight: normal;">Il s’agit d’un calcul du coût total d’une initiative. </p> <p style="font-weight: normal;">[!DNL Workfront] Cela calcule la valeur totale des coûts d’une initiative à l’aide de cette formule :</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fixed Costs]</td> 
   <td> <p><span style="font-weight: normal;">Il s’agit d’une entrée manuelle dans laquelle vous pouvez estimer <span>un montant mensuel des coûts fixes pour chaque mois de l’initiative.</span> Cela n’inclut pas les coûts associés aux rôles ajoutés à l’initiative, qui sont capturés dans le champ [!UICONTROL People Cost].</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL People Costs]</td> 
   <td> <p style="font-weight: normal;">Il s’agit d’un calcul total des coûts associés aux fonctions de l’initiative pour la durée de l’initiative. Ce nombre dépend du nombre d’équivalents temps complet ou d’heures estimé pour une fonction pour chaque mois de l’initiative. </p> 
     <p><b>CONSEILS</b>  
     <ul> 
      <li> <p>Le nombre d’équivalents temps complet mensuels pour la même fonction peut être différent d’un mois à l’autre.</p> </li> 
      <li> <p>[!DNL Workfront] Cela considère qu’il y a 160 heures de travail dans un mois. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] Cela calcule les [!UICONTROL People Costs] d’une initiative à l’aide de la formule suivante :</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] calcule les coûts mensuels des ressources humaines pour chaque mois pendant la durée de l’initiative à l’aide de la formule suivante :</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>EXEMPLE</b></p>
      <p>Si vous avez une initiative d’une durée de 6 mois qui nécessite une personne chargée de la conception avec un taux horaire de 50 $ pour 1 équivalent temps complet par mois et une personne chargée de la conception web avec un taux horaire de 100 $ pour 2 mois de l’initiative, les coûts des ressources hulaines de l’initiative sont calculés comme suit :</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Benefit]</td> 
   <td>Il s’agit d’une entrée manuelle dans laquelle vous pouvez estimer les bénéfices globaux que votre service pourrait tirer de cette initiative. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Net Value amount]</td> 
   <td> <p style="font-weight: normal;">Cela représente la valeur de votre initiative en tenant compte des coûts globaux et du bénéfice prévu estimé pour l’initiative. [!DNL Workfront] calcule la valeur nette d’une initiative à l’aide de la formule suivante :</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
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
   <td>Nom, Durée, Dates de début et de fin, Enregistré par, ID, Date de dernière publication*, Tous les champs du projet, y compris les champs personnalisés*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>Toutes les informations d’initiative comme indiqué ci-dessus, ID (fonction), Projet*, Nombre d’heures prévues pour l’affectation du projet*, Nombre d’heures d’une fonction liée à une initiative, Nombre (fonction), Tous les champs de projet, y compris les champs personnalisés*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Project]*</p></td> 
   <td> <p>Toutes les informations sur l’initiative répertoriées ci-dessus*</p> </td> 
  </tr> 
 </tbody> 
</table>

* Ces champs renseignent les informations du projet liées à l’initiative, uniquement lorsque l’initiative a été créée à partir d’un projet ou a été publiée au moins une fois dans un projet. Pour plus d’informations sur la publication des initiatives, voir [Mettre à jour ou créer des projets en publiant des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
