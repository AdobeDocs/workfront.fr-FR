---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Présentation du rapprochement des allocations de ressources entre les projets et les initiatives
description: Vue d’ensemble de la réconciliation des affectations de ressources entre les projets et les initiatives
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 98%

---

# Vue d’ensemble de la réconciliation des affectations de ressources entre les projets et les initiatives

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Pour garantir la synchronisation entre vos plans stratégiques et le travail effectif, vous avez la possibilité de connecter les projets aux initiatives. Lorsque vous définissez vos plans stratégiques et vos initiatives dans le [!DNL Scenario Planner] et que vous planifiez le travail effectif dans un projet, vous pouvez vous assurer que vos ressources sur le projet et les initiatives correspondent, pour éviter tout excès ou manque d’affectations.

## Conditions préalables

Avant de commencer, vous devez disposer des éléments suivants :

* Un plan dans le [!DNL Scenario Planner] avec une initiative liée à un projet.
* Affectations des fonctions requises pour l’initiative.
* Tâches ou problèmes du projet qui ont un nombre d’heures prévues et qui sont affectées à l’un des éléments suivants :

   * Fonctions
   * Utilisateurs et utilisatrices à qui des fonctions ont été associées

## Connecter les projets et les initiatives

>[!NOTE]
>
>Vous ne pouvez créer des initiatives et les connecter à des projets que si votre organisation a acheté une licence supplémentaire pour le [!DNL Workfront Scenario Planner].

Vous pouvez connecter des projets et des initiatives en effectuant l’une des opérations suivantes :

* Importer des projets dans un plan, en tant que nouvelles initiatives

  Pour plus d’informations, consultez la section [Importer des projets dans des plans dans le  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Publier des initiatives dans des projets

  Pour plus d’informations, consultez la section [Mettre à jour ou créer des projets en publiant des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Ces deux processus créent une connexion entre les projets et les initiatives correspondantes. Après les avoir connectés, vous pouvez gérer leurs affectations de ressources en les comparant et en veillant à ce qu’elles correspondent.

## Considérations relatives à la réconciliation des ressources entre les projets et les initiatives connectés

>[!NOTE]
>
>Vous ne pouvez afficher les initiatives, les connecter à des projets et voir leurs affectations de ressources sur un projet que si votre organisation a acheté une licence supplémentaire pour le [!DNL Workfront Scenario Planner].

* Vous pouvez affecter des utilisateurs, des utilisatrices, des équipes et des fonctions aux éléments de travail d’un projet et affecter des fonctions aux initiatives. Par conséquent, vous ne pouvez réconcilier les fonctions qu’entre les projets et les initiatives.

  >[!TIP]
  >
  >Pour réconcilier le temps passé sur un projet par les utilisateurs et les utilisatrices avec les affectations de rôles sur les initiatives, vous devez affecter des fonctions aux utilisateurs et aux utilisatrices.

* Vous pouvez afficher l’affectation d’une fonction liée à une initiative sur un projet lié dans les zones suivantes du projet :

   * Section de la zone [!UICONTROL Détails du projet] d’un projet dans le [!DNL Scenario Planner]. Pour plus d’informations, consultez les articles suivants :

      * [Mettre à jour ou créer des projets en publiant des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Gérer les informations dans la zone [!UICONTROL Vue d’ensemble] du projet](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >Vous ne pouvez pas voir les informations relatives à la fonction du projet et de l’initiative côte à côte dans la section [!DNL Scenario Planner] des [!UICONTROL Détails du projet].

   * Panneau [!UICONTROL Affectation des rôles] dans les zones suivantes :

      * [!UICONTROL Équilibreur de charge de travail] du projet

        Pour plus d’informations sur l’affichage et la réconciliation des affectations de rôles entre l’initiative et le projet lié dans l’[!UICONTROL équilibreur de charge de travail], consultez la section [Afficher l’affectation des rôles pour les projets et les initiatives dans l’[!UICONTROL équilibreur de charge de travail]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * Section [!UICONTROL Tâches]

        Pour plus d’informations sur la réconciliation des affectations de rôles entre l’initiative et le projet lié dans la zone [!UICONTROL Tâches], consultez la section [Afficher l’affectation des rôles pour les projets et les initiatives dans la liste des tâches](../scenario-planner/show-role-allocation-task-list-nwe.md).

     >[!TIP]
     >
     >Vous pouvez voir les informations sur les fonctions du projet et de l’initiative côte à côte dans le panneau [!UICONTROL Affectation des rôles].

* Vous ne pouvez pas afficher l’affectation des fonctions pour un projet sur une initiative liée. Pour plus d’informations, consultez la section [Importer des projets dans des plans dans le  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
