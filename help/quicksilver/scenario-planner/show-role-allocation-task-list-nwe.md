---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Afficher l'allocation des rôles pour les projets et initiatives dans la liste des tâches
description: Une fois que vous avez connecté les projets et les initiatives, vous pouvez gérer l’affectation de leurs ressources en parallèle pour vous assurer qu’elles correspondent. Cela permet d’éviter de les suraffecter ou de les sous-utiliser.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 82%

---

# Afficher l’attribution des rôles pour les projets et les initiatives dans la liste des tâches

<!--Audited: 07/2024-->

Une fois que vous avez connecté les projets et les initiatives, vous pouvez gérer l’affectation de leurs ressources en parallèle pour vous assurer qu’elles correspondent. Cela permet d’éviter de les suraffecter ou de les sous-utiliser.

Cet article décrit comment réconcilier des ressources à l’aide du panneau [!UICONTROL Affectation des rôles] dans la liste des tâches d’un projet.

Pour obtenir des informations générales sur la réconciliation des ressources entre les projets et les initiatives, y compris les conditions préalables, voir [Vue d’ensemble de la réconciliation des affectations de ressources entre les projets et les initiatives](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] paquet</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTE</b></p>
<p>Contactez votre représentant Workfront si vous disposez d’un autre package Workfront.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licence</p> </td> 
   <td> <p>[!UICONTROL Light] ou version ultérieure</p> 
   <p>[!UICONTROL Review] ou niveau supérieur</p> </td> 
  </tr> 
    <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td> <p>Accès en affichage ou supérieur aux projets.</p></td> 
  </tr> 
  <tr> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p> Autorisation Afficher ou supérieur pour un projet.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur l’accès au planificateur de scénarios, voir [&#x200B; Accès nécessaire pour utiliser le  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Pour plus d’informations sur les exigences d’accès à Workfront, voir [Documentation sur les exigences d’accès à Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>View or higher access to Projects.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p> View or higher permission to a project.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Afficher l’attribution des rôles pour les projets et les initiatives dans la liste des tâches

Si votre société a acheté une licence [!DNL Workfront Scenario Planner], vous pouvez réconcilier les allocations de ressources entre l’initiative et le projet qui y est lié dans la section [!UICONTROL Tâche] du projet.

1. (Conditionnel) Un projet doit être associé à une initiative en utilisant l’une des méthodes décrites dans la section [Afficher l’affectation de rôle pour les projets et initiatives dans la liste des tâches](#show-role-allocation-for-projects-and-initiatives-in-the-task-list) de cet article.

   >[!IMPORTANT]
   >
   >Si vous modifiez les ressources de l’initiative, vous devez republier le scénario auquel elle appartient pour que les dernières informations sur les ressources de l’initiative soient mises à jour dans le projet.

1. Accédez au projet pour lequel vous souhaitez revoir l’affectation des fonctions pour le projet et l’initiative associée.
1. Cliquez sur **[!UICONTROL Tâches]** dans le panneau de gauche.
1. Cliquez sur l’icône **[!UICONTROL Afficher l’affectation des rôles]** ![Afficher l’affectation des rôles](assets/show-role-allocation-icon.png) dans le coin supérieur droit de la barre d’outils.

   Le panneau [!UICONTROL Affectation des rôles] s’affiche.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Consultez les informations suivantes dans la zone **[!UICONTROL Totaux du projet]** du panneau [!UICONTROL Affectation des rôles] :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Job Role]</td> 
      <td> <p>Les noms des fonctions associées à l’un des éléments suivants :</p> 
       <ul> 
        <li> <p>tâches du projet</p> </li> 
        <li> <p>problèmes du projet</p> </li> 
        <li> <p>initiative liée au projet</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>Le nombre d’heures requises associées à chaque fonction dans le cadre de l’initiative pour la durée totale de l’initiative. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Planned Hours]</td> 
      <td>Nombre d’heures prévues associées à chaque fonction dans les tâches ou les problèmes du projet pour la durée totale du projet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>Différence entre les heures nécessaires à l’initiative et le nombre d’heures prévues associées au travail sur le projet. [!DNL Workfront] calcule la [!UICONTROL Variance] à l’aide de cette formule :</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Lorsque les ressources sont prévues pour un nombre d’heures supérieur à celui requis par l’initiative, la [!UICONTROL Variance] est négative et s’affiche en rouge. Cela signifie que vos ressources sont surallouées. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Les heures prévues du projet ne s’affichent pas dans les scénarios suivants :
   >
   >   
   >   
   >   * Lorsque des tâches ou des problèmes ne sont pas affectés à des fonctions ou à des utilisateurs et utilisatrices auxquels une fonction est associée.
   >   * Lorsque la durée des tâches ou des problèmes est nulle.
   >   
   >



1. (Facultatif) Si la colonne [!UICONTROL Écart] indique que vos ressources sont en suraffectation, ajustez l’une des options suivantes :

   * Diminuez le nombre d’heures prévues pour une fonction présentant trop d’affectations ou ajoutez plus de ressources aux tâches et distribuez plus d’heures prévues aux nouvelles ressources. Vous pouvez mettre à jour les affectations ou le nombre d’heures prévues sur les tâches ou les problèmes lors de leur modification. Pour plus d’informations, voir les articles suivants :

      * [Modifier des tâches](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Modifier des problèmes](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >Vous devez disposer d’un accès et d’autorisations supplémentaires pour modifier les tâches et les problèmes.

   * Augmentez le nombre d’heures requises pour le rôle qui indique la suraffectation de l’initiative. Pour plus d’informations, voir [Créer et modifier des initiatives dans le  [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

     >[!NOTE]
     >
     >Vous devez disposer d’un accès et d’autorisations supplémentaires pour modifier les plans.


