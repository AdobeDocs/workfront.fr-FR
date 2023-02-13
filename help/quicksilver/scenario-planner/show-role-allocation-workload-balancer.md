---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Afficher l’affectation des rôles pour les projets et les initiatives dans l’équilibreur de charge de travail
description: Une fois que vous avez connecté les projets et les initiatives, vous pouvez gérer leur allocation de ressources côte à côte afin de vous assurer qu’elles
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# Afficher l’affectation des rôles pour les projets et les initiatives dans le [!DNL Workload Balancer]

>[!IMPORTANT]
>
>Votre entreprise doit acheter une licence supplémentaire pour la variable [!DNL Adobe Workfront Scenario Planner] afin que vous puissiez afficher les informations d’initiative sur un projet. Pour plus d’informations sur l’obtention de [!DNL Workfront Scenario Planner], voir [Accès nécessaire pour utiliser la variable [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Une fois que vous avez connecté les projets et les initiatives, vous pouvez gérer leur allocation de ressources côte à côte afin de vous assurer qu’elles correspondent. Cela permet d’éviter de les surestimer ou de les sous-utiliser.

Cet article décrit comment réconcilier des ressources à l’aide de la variable [!UICONTROL Attribution des rôles] dans [!UICONTROL Équilibreur de charge de travail] d’un projet.

Pour obtenir des informations générales sur la réconciliation des ressources entre les projets et les initiatives, y compris les conditions préalables, voir [Présentation de la réconciliation des allocations de ressources entre les projets et les initiatives](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Exigences d’accès

Vous devez :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> license*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produit</b> </td> 
   <td> <p>Vous devez acheter une licence supplémentaire pour la variable [!DNL Adobe Workfront Scenario Planner] pour accéder aux fonctionnalités décrites dans cet article.</p> <p>Pour plus d’informations sur l’obtention de [!DNL Workfront Scenario Planner], voir <a href="../scenario-planner/access-needed-to-use-sp.md">Accès nécessaire pour utiliser la variable [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Paramétrages du niveau d'accès*</strong> </td> 
   <td> <p>[!UICONTROL Affichage] ou accès supérieur à Projets </p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Autorisations d’objet</strong> </p> </td> 
   <td> <p>Autorisations [!UICONTROL View] ou supérieures pour le projet</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un plan, voir <a href="../scenario-planner/request-access-to-plan.md">[!UICONTROL Demander] l’accès à un plan dans la variable [!DNL Workfront Scenario Planner]</a>.</p> <p>Pour plus d’informations sur la demande d’un accès supplémentaire à un projet, voir <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Afficher l’affectation des rôles pour les projets et les initiatives dans le [!DNL Workload Balancer]

Si votre société a acheté une [!DNL Workfront Scenario Planner] , vous pouvez réconcilier les allocations de ressources entre l’initiative et le projet qui y est lié au niveau du projet. [!DNL Workload Balancer].

1. (Conditionnel) Connectez un projet à une initiative à l’aide de l’une des méthodes décrites dans les articles suivants :

   * [Importation de projets dans des plans dans [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Mettez à jour ou créez des projets en publiant des initiatives dans le [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Si vous apportez des modifications aux ressources de l’initiative, vous devez republier le scénario auquel appartient l’initiative pour que les dernières informations sur les ressources de l’initiative soient mises à jour sur le projet.

1. Accédez au projet dans lequel vous souhaitez examiner l’affectation des rôles de tâche pour le projet ainsi que pour l’initiative associée.
1. Cliquez sur [!DNL Workload Balancer] dans le panneau de gauche.

   Vous devrez peut-être cliquer sur **[!UICONTROL Planification]**, puis **[!UICONTROL Basculer vers l’équilibreur de charge de travail]**.

1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur **[!UICONTROL Mois]** pour afficher l’équilibreur de charge de travail par mois, cliquez sur le menu déroulant en regard d’un mois dans la chronologie. ![](assets/drop-down-next-to-month-month-view-wb.png), puis cliquez sur **[!UICONTROL Plus]**.
   * Cliquez sur le bouton **[!UICONTROL Afficher l’affectation des rôles]** icon ![](assets/show-role-allocation-icon.png) dans le coin supérieur droit de la barre d’outils.

   Le [!UICONTROL Attribution des rôles] s’affiche.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Bien que vous puissiez afficher la variable [!UICONTROL Attribution des rôles] même si votre entreprise n’a pas acheté un [!DNL Workfront Scenario Planner] licence, vous ne pouvez pas afficher d’informations sur les rôles de travail des initiatives.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Consultez les informations suivantes dans la section **[!UICONTROL Totaux du projet]** zone du panneau Attribution des rôles :

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
      <td> <p>La différence entre les heures requises pour l’initiative et les heures planifiées associées aux travaux sur le projet. [!DNL Workfront] calcule la [!UICONTROL Variance] à l’aide de cette formule :</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Lorsque les ressources sont planifiées pendant plus d’heures que nécessaire sur l’initiative, la [!UICONTROL Variance] est négative et s’affiche en rouge. Cela signifie que vos ressources sont surchargées. </p> </td> 
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
   >   * Lorsque des tâches ou des problèmes ont une propriété [!UICONTROL Durée] de zéro.




1. (Facultatif) Si la variable [!UICONTROL Variance] indique que vos ressources sont surchargées, ajustez l’une des options suivantes :

   * Réduisez le nombre d’heures planifiées pour un rôle de tâche qui indique une surallocation ou l’ajout de ressources aux tâches et distribuez davantage d’heures planifiées aux nouvelles ressources. Vous pouvez mettre à jour les affectations ou le nombre d’heures planifiées sur les tâches ou les problèmes lors de leur modification. Pour plus d’informations, voir les articles suivants :

      * [Modifier les tâches](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Modification des problèmes](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >Vous devez disposer d’un accès et d’autorisations supplémentaires pour modifier les tâches et les problèmes.

   * Augmentez le nombre d’heures requises pour le rôle qui indique la suraffectation de l’initiative. Pour plus d’informations, voir [Créez et modifiez des initiatives dans le [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >Vous devez disposer d’un accès et d’autorisations supplémentaires pour modifier les plans.


1. (Facultatif) Cliquez sur l’icône déroulante pour développer l’un des mois du [!UICONTROL Attribution des rôles] ou dans la chronologie de la [!UICONTROL Équilibreur de charge de travail].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   Le même type d’informations affichées dans la variable [!UICONTROL Totaux du projet] s’affiche également pour chaque mois.

   >[!TIP]
   >
   >Les mois répertoriés dans la variable [!UICONTROL Attribution des rôles] sont les mois de la chronologie affichée à l’écran dans le [!UICONTROL Équilibreur de charge de travail]. Faites défiler la chronologie pour afficher d’autres mois.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


