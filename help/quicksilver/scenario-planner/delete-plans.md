---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Supprimer des plans dans le planificateur de scénarios
description: Vous pouvez supprimer les plans que vous avez créés. Vous ne pouvez pas supprimer les plans qui sont partagés avec vous.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 81%

---

# Supprimer des plans dans le [!DNL Scenario Planner]

Vous pouvez supprimer les plans que vous avez créés. Vous ne pouvez pas supprimer les plans qui sont partagés avec vous.

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

Pour plus d’informations sur l’accès au planificateur de scénarios, voir [ Accès nécessaire pour utiliser le  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

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
</table>-->

## Supprimer les plans

>[!IMPORTANT]
>
>Vous ne pouvez pas récupérer les plans supprimés.

Vous pouvez supprimer un plan ou supprimer un scénario dans un plan.

* [Supprimer des plans](#delete-plans)
* [Supprimer des scénarios](#delete-scenarios)

### Supprimer les plans

>[!IMPORTANT]
>
>Tenez compte des points suivants lors de la suppression de plans :
>
>* Toutes les informations relatives au plan sont également supprimées. Cela inclut tous les scénarios et toutes les initiatives associés au plan, y compris des informations sur les fonctions et les coûts. Ces informations ne peuvent pas être récupérées.
>* Si le plan contient un scénario publié, les projets liés aux initiatives supprimées sont préservés et la zone [!DNL Scenario Planner] reste dans la section [!UICONTROL Détails du projet].
>
>  Pour plus d’informations sur la publication d’initiatives dans des projets, consultez [Mettre à jour ou créer des projets en publiant des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Pour supprimer un plan :

{{step1-to-scenario-planner}}

Une liste des plans s’affiche.

1. Cliquez sur le nom d’un plan pour l’ouvrir.
1. Cliquez sur le **[!UICONTROL menu Plus]** ![menu Plus](assets/more-menu.png) à droite du nom du plan, puis cliquez sur **[!UICONTROL Supprimer]** > **[!UICONTROL Oui, supprimer]**.

   Le plan est supprimé et vous revenez à la liste des plans.

### Supprimer des scénarios {#delete-scenarios}

>[!IMPORTANT]
>
>Tenez compte des points suivants lors de la suppression d’un scénario :
>
>* La suppression d’un scénario supprime toutes les initiatives et leurs informations du scénario. Si elles sont copiées vers d’autres scénarios, les initiatives restent dans les autres scénarios.
>* Lors de la suppression d’un scénario, le scénario suivant reprend le numéro du scénario supprimé et l’ordre de comptage est conservé. Par exemple, si vous supprimez le scénario 4, le scénario 5 devient le scénario 4.
>* Si certaines initiatives du scénario sont publiées, le projet lié à l’initiative est conservé et la zone du planificateur de scénarios reste sur les projets liés.
>* Si les initiatives publiées existent dans un autre scénario, elles restent sur ce scénario, y compris leur lien vers le projet. La publication de ces initiatives à partir des autres scénarios met à jour les projets liés avec de nouvelles informations issues de ces scénarios.
>
>  Pour plus d’informations sur la publication d’initiatives dans des projets, consultez [Mettre à jour ou créer des projets en publiant des initiatives dans le  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Pour supprimer un scénario :

1. Accédez au plan pour lequel vous souhaitez supprimer un scénario.

   Par défaut, c’est le scénario initial qui s’affiche.

1. Cliquez sur **[!UICONTROL Comparer les scénarios]**.
1. Dans le coin supérieur droit de la carte de scénario, cliquez sur le menu **[!UICONTROL Plus]** ![Plus](assets/more-menu.png), puis sur **[!UICONTROL Supprimer]**.

   Le scénario est supprimé.

1. Cliquez sur **[!UICONTROL Enregistrer le plan]** pour enregistrer vos modifications.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives) </p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->


