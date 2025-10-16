---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Supprimer des initiatives dans le planificateur de scénarios
description: Vous pouvez supprimer des initiatives d’un plan que vous avez créé ou d’un plan que quelqu’un a partagé avec vous. Vous ne pouvez pas récupérer les initiatives que vous avez supprimées.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 84%

---

# Supprimer des initiatives dans le [!DNL Scenario Planner]

Vous pouvez supprimer des initiatives d’un plan que vous avez créé ou d’un plan que quelqu’un a partagé avec vous. Vous ne pouvez pas récupérer les initiatives que vous avez supprimées.

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
   <td> <p>Accès [!UICONTROL Edit] à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autorisations d’objet </p> </td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour un plan</p> </td> 
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
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Supprimer des initiatives

Tenez compte des points suivants lors de la suppression d’initiatives :

* La suppression d’une initiative supprime du plan le nombre requis de fonctions et les informations de coûts associées à l’initiative.
* La suppression d’une initiative créée par import d’un projet ne supprime pas le projet associé à l’initiative.
* La suppression d’une initiative qui a été publiée sur un projet au moins une fois entraîne les résultats suivants :

   * L’initiative est supprimée du scénario, mais la zone [!DNL Scenario Planner] reste dans la section [!UICONTROL Détails du projet].
   * Si l’initiative que vous supprimez est la seule initiative publiée sur le scénario, l’indicateur signalant que le plan a été publié est également supprimé.

     Pour plus d’informations sur la publication d’initiatives dans des projets, consultez [Mettre à jour ou créer des projets en publiant des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

     Pour plus d’informations sur la création d’initiatives par import de projets, consultez [Importer des projets dans des plans dans le  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

Vous pouvez supprimer une initiative à la fois ou supprimer plusieurs initiatives en bloc.

* [Supprimer une seule initiative](#delete-one-initiative)
* [Supprimer des initiatives en bloc](#delete-initiatives-in-bulk)

### Supprimer une seule initiative {#delete-one-initiative}

{{step1-to-scenario-planner}}

Une liste des plans s’affiche.

1. Cliquez sur le nom d’un plan pour l’ouvrir, puis localisez l’initiative que vous souhaitez supprimer.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur le **[!UICONTROL menu Plus]** ![menu Plus](assets/more-menu.png) à droite du nom de l’initiative, puis cliquez sur **[!UICONTROL Supprimer]** > **[!UICONTROL Oui, supprimer]**.

   * Sélectionnez la zone située à gauche de l’initiative, puis cliquez sur **[!UICONTROL Supprimer]** dans le menu flottant qui apparaît au bas du plan, et sur **[!UICONTROL Oui, supprimer]**.

   L’initiative, sa fonction et ses informations de coût sont supprimées du plan.

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.

### Supprimer des initiatives en bloc {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

Une liste des plans s’affiche.

1. Cliquez sur le nom d’un plan pour l’ouvrir, puis localisez l’initiative que vous souhaitez supprimer.
1. Sélectionnez les cases à gauche des initiatives que vous souhaitez supprimer, puis cliquez sur **[!UICONTROL Supprimer]** dans le menu qui apparaît au bas du plan, puis sur **[!UICONTROL Oui, supprimer]**.

   ![Menu Gérer l’initiative](assets/bottom-manage-initiative-menu-350x45.png)

   Les initiatives, leur fonction et leurs informations sur les coûts sont supprimées du plan.

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.
