---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Vue d’ensemble de la réconciliation des affectations de ressources entre les projets et les initiatives
description: Vue d’ensemble de la réconciliation des affectations de ressources entre les projets et les initiatives
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 7%

---

# Vue d’ensemble de la réconciliation des affectations de ressources entre les projets et les initiatives

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Vous pouvez associer les projets à des initiatives pour vous assurer que vos plans stratégiques et le travail réel sont synchronisés. Lorsque vous définissez vos plans stratégiques et initiatives dans le [!DNL Scenario Planner] et que vous planifiez le travail réel dans un projet, vous pouvez vous assurer que vos ressources sur le projet et les initiatives correspondent, de sorte que vous ne les surestimerez pas ou ne les sous-utiliserez pas.

## Conditions préalables

Avant de commencer, vous devez disposer des éléments suivants :

* Un plan dans le [!DNL Scenario Planner] avec une initiative connectée à un projet.
* Affectation des rôles requis pour l’initiative.
* Tâches ou problèmes sur le projet qui ont des heures planifiées et qui sont affectés à l’une des tâches suivantes :

   * Fonctions
   * Utilisateurs associés aux rôles de tâche

## Connexion de projets et d’initiatives

>[!NOTE]
>
>Vous pouvez créer des initiatives et les connecter à des projets uniquement si votre entreprise a acheté une licence supplémentaire pour le [!DNL Workfront Scenario Planner].

Vous pouvez connecter des projets à des initiatives en effectuant l’une des opérations suivantes :

* Importer des projets dans un plan, en tant que nouvelles initiatives

  Pour plus d’informations, voir [Importation de projets dans des plans dans le  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Initiatives Publish vers les projets

  Pour plus d’informations, voir [Mise à jour ou création de projets en publiant des initiatives dans  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Les deux processus créent un lien entre les projets et leurs initiatives correspondantes. Une fois connectés, vous pouvez gérer leurs allocations de ressources en les comparant et en veillant à ce qu’elles correspondent.

## Considérations sur la réconciliation des ressources sur les projets et initiatives liés

>[!NOTE]
>
>Vous pouvez afficher les initiatives, les connecter aux projets et afficher leurs allocations de ressources sur un projet uniquement si votre organisation a acheté une licence supplémentaire pour le [!DNL Workfront Scenario Planner].

* Vous pouvez affecter des utilisateurs, des équipes et des rôles de tâche aux tâches d’un projet, ainsi que des rôles de tâche aux initiatives. Par conséquent, vous ne pouvez réconcilier que les rôles de tâche entre les projets et les initiatives.

  >[!TIP]
  >
  >Pour réconcilier le temps passé par les utilisateurs sur un projet avec les attributions de rôles sur les initiatives, vous devez associer les utilisateurs à des rôles de tâche.

* Vous pouvez afficher l’attribution du rôle d’initiative sur un projet lié dans les zones suivantes du projet :

   * [!DNL Scenario Planner] de la zone [!UICONTROL Détails du projet] sur un projet. Pour plus d’informations, consultez les articles suivants :

      * [ Mettez à jour ou créez des projets en publiant des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Gérer les informations dans la zone [!UICONTROL Overview] du projet](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >Vous ne pouvez pas voir les informations sur les rôles de tâche du projet et de l’initiative côte à côte dans la section [!DNL Scenario Planner] des [!UICONTROL détails du projet].

   * Le panneau [!UICONTROL Affectation de rôle] dans les domaines suivants :

      * [!UICONTROL équilibreur de charge de travail] du projet

        Pour plus d’informations sur la manière d’afficher et de concilier les attributions de rôles entre l’initiative et le projet lié dans l’ [!UICONTROL équilibreur de charge de travail], voir [Afficher l’allocation de rôles pour les projets et les initiatives dans l’ [!UICONTROL équilibreur de charge de travail]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * Section [!UICONTROL Tâches]

        Pour plus d’informations sur la manière de réconcilier les attributions de rôles entre l’initiative et le projet lié dans la section [!UICONTROL Tâches], voir [Afficher l’attribution des rôles pour les projets et les initiatives dans la liste des tâches](../scenario-planner/show-role-allocation-task-list-nwe.md).

     >[!TIP]
     >
     >Vous pouvez afficher les informations sur les rôles de tâche du projet et de l’initiative côte à côte dans le panneau [!UICONTROL Affectation de rôle] .

* Vous ne pouvez pas afficher l’attribution des rôles de tâche pour un projet sur une initiative liée. Pour plus d’informations, voir [Importation de projets dans des plans dans le  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
