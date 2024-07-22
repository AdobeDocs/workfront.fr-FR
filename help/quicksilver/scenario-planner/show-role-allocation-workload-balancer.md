---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Afficher l’affectation de rôle pour les projets et les initiatives dans l’équilibreur de charge de travail
description: Une fois que vous avez connecté les projets et les initiatives, vous pouvez gérer leur allocation de ressources côte à côte afin de vous assurer qu’elles
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 5%

---

# Afficher l’attribution des rôles pour les projets et les initiatives dans l’ [!UICONTROL équilibreur de charge de travail]

<!--Audited: 07/2024-->

Une fois que vous avez connecté les projets et les initiatives, vous pouvez gérer leur allocation de ressources côte à côte afin de vous assurer qu’elles correspondent. Cela permet d’éviter de les surestimer ou de les sous-utiliser.

Cet article décrit comment vous pouvez réconcilier des ressources à l’aide du panneau [!UICONTROL Affectation de rôle] dans l’ [!UICONTROL équilibreur de charge de travail] d’un projet.

Pour obtenir des informations générales sur la réconciliation des ressources entre les projets et les initiatives, y compris les conditions préalables, voir [Présentation de la réconciliation des allocations de ressources entre les projets et les initiatives](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] forfait*</p> </td> 
   <td> <p>Actuel : [!UICONTROL Entreprise] ou version ultérieure</p>
   <p>Nouveau : Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence*</p> </td> 
   <td> <p>Nouveau : Léger ou supérieur</p> 
   <p>Actuel : [!UICONTROL Révision] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td>Produit* </td> 
   <td> 
   <p>Pour les plans Workfront actuels : </p>
   <p>Vous devez acheter une licence supplémentaire pour le [!DNL Adobe Workfront Scenario Planner] afin d’accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’accès et les autorisations pour [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Accès nécessaire pour utiliser le [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Niveau d’accès </td> 
   <td> <p>[!UICONTROL Affichage] ou accès supérieur à [!UICONTROL Projects]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Autorisations [!UICONTROL View] pour un projet</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Exigences d’accès à la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Afficher l’attribution des rôles pour les projets et les initiatives dans l’ [!UICONTROL équilibreur de charge de travail]

Si votre entreprise a acheté une licence [!DNL Workfront Scenario Planner], vous pouvez réconcilier les allocations de ressources entre l’initiative et le projet qui y est lié dans l’ [!UICONTROL équilibreur de charge de travail] au niveau du projet.

1. (Conditionnel) Connectez un projet à une initiative à l’aide de l’une des méthodes décrites dans les articles suivants :

   * [Importez des projets dans des plans dans le  [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Mettez à jour ou créez des projets en publiant des initiatives dans le  [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Si vous apportez des modifications aux ressources de l’initiative, vous devez republier le scénario auquel appartient l’initiative pour que les dernières informations sur les ressources de l’initiative soient mises à jour sur le projet.

1. Accédez au projet dans lequel vous souhaitez examiner l’affectation des rôles de tâche pour le projet ainsi que pour l’initiative associée.
1. Cliquez sur [!UICONTROL équilibreur de charge de travail] dans le panneau de gauche.

   Vous devrez peut-être cliquer sur **[!UICONTROL Planification]**, puis sur **[!UICONTROL Basculer vers l’équilibreur de charge de travail]**.

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur **[!UICONTROL Month]** pour afficher l’équilibreur de charge de travail par mois, cliquez sur le menu déroulant en regard d’un mois dans la chronologie ![](assets/drop-down-next-to-month-month-view-wb.png), puis cliquez sur **[!UICONTROL Plus]**.
   * Cliquez sur l’icône **[!UICONTROL Afficher l’attribution des rôles]** ![](assets/show-role-allocation-icon.png) dans le coin supérieur droit de la barre d’outils.

   Le panneau [!UICONTROL Affectation de rôle] s’affiche.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Bien que vous puissiez afficher le panneau [!UICONTROL Affectation de rôle] même si votre entreprise n’a pas acheté de licence [!DNL Workfront Scenario Planner], vous ne pouvez pas afficher d’informations sur les rôles de tâche des initiatives.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Consultez les informations suivantes dans la zone **[!UICONTROL Totaux du projet]** du panneau Attribution des rôles :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Job Role]</td> 
      <td> <p>Les noms des rôles de tâche associés à l’un des éléments suivants :</p> 
       <ul> 
        <li> <p>tâches sur le projet</p> </li> 
        <li> <p>problèmes liés au projet</p> </li> 
        <li> <p>initiative liée au projet</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Heures de l’initiative]</td> 
      <td>Nombre d’heures requises associées à chaque rôle d’emploi de l’initiative pour la durée totale de l’initiative. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Heures planifiées]</td> 
      <td>Nombre d’heures planifiées associées à chaque rôle de tâche dans les tâches ou problèmes du projet pendant toute la durée du projet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>La différence entre les heures requises pour l’initiative et les heures prévues associées aux travaux sur le projet. [!DNL Workfront] calcule la [!UICONTROL Variance] à l’aide de cette formule :</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Lorsque les ressources sont planifiées pendant plus d’heures que nécessaire sur l’initiative, la [!UICONTROL Variance] est négative et s’affiche en rouge. Cela signifie que vos ressources sont surchargées. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Les heures planifiées du projet ne s’affichent pas dans les scénarios suivants :
   >
   >   
   >   
   >   * Lorsque des tâches ou des problèmes ne sont pas affectés à des rôles de tâche ou des utilisateurs auxquels un rôle de tâche est associé.
   >   * Lorsque les tâches ou les problèmes ont une [!UICONTROL durée] de zéro.
   >   
   >

1. (Facultatif) Si la colonne [!UICONTROL Variance] indique que vos ressources sont surchargées, ajustez l’une des options suivantes :

   * Réduisez le nombre d’heures planifiées pour un rôle de tâche qui indique une surallocation ou l’ajout de ressources aux tâches et distribuez davantage d’heures planifiées aux nouvelles ressources. Vous pouvez mettre à jour les affectations ou le nombre d’heures planifiées sur les tâches ou les problèmes lors de leur modification. Pour plus d’informations, voir les articles suivants :

      * [Modifier les tâches](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Modifier les problèmes](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >Vous devez disposer d’un accès et d’autorisations supplémentaires pour modifier les tâches et les problèmes.

   * Augmentez le nombre d’heures requises pour le rôle qui indique la suraffectation de l’initiative. Pour plus d’informations, voir [Création et modification d’initiatives dans  [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

     >[!NOTE]
     >
     >Vous devez disposer d’un accès et d’autorisations supplémentaires pour modifier les plans.

1. (Facultatif) Cliquez sur l’icône déroulante pour développer l’un des mois dans le panneau [!UICONTROL Affectation de rôle] ou dans la chronologie de l’ [!UICONTROL  équilibreur de charge de travail].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   Le même type d’informations s’affiche également dans la zone [!UICONTROL Totaux du projet] pour chaque mois.

   >[!TIP]
   >
   >Les mois répertoriés dans le panneau [!UICONTROL Affectation du rôle] sont les mois dans la chronologie affichée à l’écran dans l’ [!UICONTROL  équilibreur de charge de travail ]. Faites défiler la chronologie vers le bas pour afficher d’autres mois.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


