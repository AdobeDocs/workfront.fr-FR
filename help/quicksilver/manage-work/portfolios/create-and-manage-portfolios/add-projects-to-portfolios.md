---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Add Projects to a Portfolio
description: Nous vous recommandons d’ajouter des projets aux portfolios lorsque vous les lancez. Cependant, vous pouvez les ajouter à un portfolio à tout moment de leur durée de vie.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 97f36c18-3ac8-45ac-b5bc-dfe8b1363faf
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: fee6b71eeb0ca79703a2a9e29a14040b91cb7387
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 54%

---

# Ajouter des projets à un portfolio

<!--Audited: 08/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

Nous vous recommandons d’ajouter des projets aux portfolios lorsque vous les lancez. Cependant, vous pouvez les ajouter à un portfolio à tout moment de leur durée de vie.

Tenez compte des éléments suivants lorsque vous ajoutez des projets aux portfolios :

* You can associate only one portfolio with a project.
* Un projet reste dans un portfolio jusqu’à ce qu’il soit supprimé ou associé à un autre portfolio.
* A portfolio may contain an unlimited number of projects.

>[!CAUTION]
>
>   Inherited permissions may not be applied correctly when used across a large number of child objects.
>   
>   To help avoid inherited permissions issues, we recommend the following:
>
>   * Limit the number of child objects (projects) under a single parent (portfolio or program). We recommend no more than 10,000 projects per portfolio or program.
>   * Reduce inheritance depth by applying permissions at a lower-level object.
>
>     For example, apply permissions directly at the project level rather than rely on the permissions inherited from the portfolio to the program, and then to the project.
>   * Split programs to contain fewer projects, which reduces permission complexity.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Tous</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Standard</p> 
   <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>[!UICONTROL Edit] access Portfolios</p> <p>[!UICONTROL Edit] l’accès aux Projets</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Autorisations [!UICONTROL Manage] pour le portfolio</p> <p>[!UICONTROL Manage] les permissions des projets</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>[!UICONTROL Edit] access Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Ajouter un projet à un portfolio

1. Accédez à un portfolio, puis cliquez sur **[!UICONTROL Projets]** dans le panneau de gauche.

   ![Portfolio with projects](assets/qs-portfolio-with-projects-350x90.png)

1. Cliquez sur **[!UICONTROL Nouveau projet]** et sélectionnez une méthode pour ajouter un projet.

   >[!TIP]
   >
   >You cannot add a project when you view the list of projects in the [!UICONTROL Milestone] view.

   Sélectionnez l’une des options suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Existing Project]</td> 
      <td> <p>Ajoutez un projet déjà créé.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New Project]</td> 
      <td> <p>Ajoutez un nouveau projet. </p> <p>Pour plus d’informations sur la création d’un nouveau projet, consultez la section <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Créer un projet</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Import a Project from [!DNL MS Project]] </td> 
      <td> <p>Ajoutez un projet que vous avez précédemment exporté depuis [!DNL MS Project] et que vous avez enregistré sur votre ordinateur. </p> <p>Pour plus d’informations sur la création d’un nouveau projet en l’important à partir de [!DNL Microsoft Project], consultez la section <a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">Importer un projet à partir de [!DNL Microsoft Project]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Project]</td> 
      <td> <p>Demander l’approbation d’un projet.</p> <p>Pour plus d’informations sur la requête de projets, consultez la section <a href="../../../manage-work/projects/create-projects/request-project.md">Demander un projet</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL New from Template]</td> 
      <td> <p>Ajouter un nouveau projet en utilisant un modèle existant. </p> <p>Pour plus d’informations sur la création d’un projet à partir d’un modèle, consultez la section <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Créer un projet à l’aide d’un modèle</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![New project dropdown](assets/new-project-dropdown-expanded-from-portfolio-nwe-350x376.png)

1. (Conditional) If you selected to add an existing project, the **Add Projects** box opens. <!--check this after UI changes-->

   ![Add existing project](assets/add-existing-projects-to-portfolios-box.png) <!--check this after UI changes-->

1. Start typing the name of a project in the **[!UICONTROL Add Projects to this Portfolio]** field, then click them when they appear in the list.  <!--check this after UI changes-->

   You can add more than one project.

1. (Optional) Click the **X** icon to the right of the project name to remove it from the list, if you decide not to add it to the portfolio.

   <!--replace last step with this, for unshim: 1. (Optional) Click the **Delete** icon ![Delete icon](assets/delete-icon.png) next to the name of a project if you decide not to add it to the portfolio.-->

1. Click **[!UICONTROL Add Projects]**. <!--check this after UI changes-->

   Le ou les projets sélectionnés sont désormais associés au portfolio.
