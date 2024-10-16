---
title: Personnalisation du panneau de gauche à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Dans un modèle de mise en page, vous pouvez personnaliser ce que les personne voient dans la zone du panneau de gauche dans Adobe Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 66%

---

# Personnaliser le panneau de gauche à l’aide d’un modèle de mise en page

<!--Audited: 10/2024-->

Dans un modèle de mise en page, vous pouvez personnaliser ce que les personnes voient dans la zone du panneau de gauche dans l’ensemble d’[!DNL Adobe Workfront].

Par exemple, vous pouvez déterminer les éléments suivants que les personnes voient dans le panneau de gauche lorsqu’elles affichent une tâche :

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>Les modifications apportées à l’ordre et à la visibilité sont répercutées dans l’application mobile.

Pour plus d’informations sur la création de modèles de mise en page, voir [Créer et gérer des modèles de mise en page](../use-layout-templates/create-and-manage-layout-templates.md).

Pour plus d’informations sur les modèles de disposition pour les groupes, voir [Créer et modifier des modèles de disposition d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Après avoir configuré un modèle de mise en page, vous devez l’affecter aux utilisateurs et utilisatrices pour que les modifications que vous avez apportées soient visibles par d’autres personnes. Pour plus d’informations sur l’attribution d’un modèle de disposition aux utilisateurs et utilisatrices, voir [Affecter des utilisateurs et utilisatrices à un modèle de disposition](../use-layout-templates/assign-users-to-layout-template.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td><p>Nouveau : Standard</p>
  <p> Actuel : formule</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès Administrateur ou administratrice système.
Pour les exécuter pour un groupe, vous devez être une personne responsable de ce groupe.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personnaliser le panneau de gauche d’une zone dans [!DNL Workfront] :

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans [Créer et gérer des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Cliquez sur la flèche vers le bas ![](assets/dropdown-arrow.png) sous **[!UICONTROL Personnaliser ce que les utilisateurs voient]**, puis cliquez sur le nom d’un type d’objet ou d’une zone [!DNL Workfront] dont vous souhaitez personnaliser le panneau de gauche.

   Les types d’objet et les zones [!DNL Workfront] dont vous pouvez personnaliser le panneau de gauche sont répertoriés dans le tableau suivant :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Type d’objet ou zone [!DNL Workfront]</th> 
      <th>Lorsque les personnes cliquent sur ce qui suit...</th> 
      <th>Sections du panneau de gauche que les utilisateurs voient après leur affichage dans le modèle de mise en page :</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Project]</td> 
      <td>Nom d’un projet</td> 
      <td>[!UICONTROL Tâches], [!UICONTROL Détails Du Projet], [!UICONTROL Business Case], [!UICONTROL Mises À Jour], [!UICONTROL Documents], [!UICONTROL Problèmes], [!UICONTROL Risques], [!UICONTROL Approbations], [!UICONTROL Principes], [!UICONTROL], Rates!UICONTROL Enregistrements De Facturation], [!UICONTROL Dépenses], [!UICONTROL Hours], [!UICONTROL équilibreur De Charge De Travail], [!UICONTROL People], [!UICONTROL Utilization], [!UICONTROL Queue Details], [!UICONTROL Règles De Routage], [!UICONTROL Queue Groupe de rubriques L], [!UICONTROL Mesures], [!UICONTROL Planification]*</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Task]</td> 
      <td>Nom d’une tâche</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Task Details], [!UICONTROL Subtask], [!UICONTROL Issues], [!UICONTROL Hours], [!UICONTROL Approvals], [!UICONTROL Expenses], [!UICONTROL Predecessors]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Issue]</td> 
      <td>Nom d’un problème</td> 
      <td> [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Issue Details], [!UICONTROL Hours], [!UICONTROL Approvals]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>Nom d’un portfolio</td> 
      <td>[!UICONTROL Projets], [!UICONTROL Programmes], [!UICONTROL Détails du Portfolio], [!UICONTROL Portfolio] [!UICONTROL Optimisation], [!UICONTROL Documents], [!UICONTROL Mises à jour], [!UICONTROL Planification]*</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>Nom d’un programme</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Program Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Planning]*</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template]</td> 
      <td>Nom d’un modèle de projet</td> 
      <td>[!UICONTROL Template Tasks], [!UICONTROL Template Details], [!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Risks], [!UICONTROL Expenses], [!UICONTROL People], [!UICONTROL Approvals], [!UICONTROL Billing Rates], [!UICONTROL Queue Details], [!UICONTROL Routing Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template Task]</td> 
      <td>Nom d’une tâche de modèle</td> 
      <td>[!UICONTROL Updates], [!UICONTROL Documents], [!UICONTROL Template Task Details], [!UICONTROL Subtasks], [!UICONTROL Expenses], [!UICONTROL Approvals], [!UICONTROL Predecessors]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Billing Record]</td> 
      <td>Nom d’un enregistrement de facturation d’un projet</td> 
      <td>[!UICONTROL Billing Record Details], [!UICONTROL Billable Hours], [!UICONTROL Billable Expenses], [!UICONTROL Fixed Revenues]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Projects]</td> 
      <td>Projets <img src="assets/projects-in-main-menu.png"> dans le [!UICONTROL Main menu] <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projects]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Requests]</td> 
      <td>Nom d’une demande</td> 
      <td>[!UICONTROL New Request], [!UICONTROL Submitted requests], [!UICONTROL All Requests], [!UICONTROL Drafts]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Dashboards]</td> 
      <td>Nom d’un tableau de bord</td> 
      <td>[!UICONTROL My Dashboards], [!UICONTROL Shared Dashboards], [!UICONTROL All Dashboards]<p><b>NOTE</b> : si vous avez créé des onglets personnalisés pour la zone [!UICONTROL Reports] à l’aide d’un modèle de mise en page dans [!DNL Adobe Workfront Classic], ils s’affichent au bas de cette liste. Pour les utilisateurs et utilisatrices, ils s’affichent au bas du panneau de gauche dans la zone [!UICONTROL Dashboards].</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum Team]</td> 
      <td>Nom d’une équipe Scrum</td> 
      <td><p>[!UICONTROL Iterations], [!UICONTROL Current iteration], [!UICONTROL Backlog], [!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Settings]</p> <p><strong>NOTE :</strong> l’élément <strong>[!UICONTROL Current iteration]</strong> s’affiche uniquement dans le panneau de gauche lorsqu’il y a au moins une tâche ou un problème sur l’itération.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban Team]</td> 
      <td>Nom d’une équipe Kanban</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Kanban board], [!UICONTROL Backlog], [!UICONTROL Updates], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfall Team]</td> 
      <td>Nom d’une équipe Waterfall</td> 
      <td>[!UICONTROL Workload Balancer], [!UICONTROL Updates], [!UICONTROL Team Requests], [!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteration]</td> 
      <td>Nom d’une itération</td> 
      <td>[!UICONTROL Stories], [!UICONTROL Issues], [!UICONTROL Story Board], [!UICONTROL Overview], [!UICONTROL Custom Forms], [!UICONTROL Updates] </td> 
     </tr> 
     <!--
      <tr> 
       <td>Company</td> 
       <td>The name of the company</td> 
       <td> <p>People (cannot be hidden), Billing Rates, Custom Forms </p> </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Timesheets</td> 
       <td>The name of the timesheet</td> 
       <td>My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden) </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Resourcing</td> 
       <td>The name of the resource</td> 
       <td>Planner (cannot be hidden), Workload Balancer, Utilization, Resource Pools </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>User Details</td> 
       <td>____________</td> 
       <td>Details (cannot be hidden), Org Chart, Time Off, Custom Forms </td> 
      </tr>
     --> 
    </tbody> 
   </table>

   *Votre entreprise doit acquérir une licence supplémentaire pour Workfront Planning afin de pouvoir ajouter cette zone au panneau de gauche des projets, portefeuilles et programmes. Pour plus d’informations, voir [Présentation de la planification Adobe Workfront](/help/quicksilver/planning/general/planning-overview.md)


1. Dans la liste **[!UICONTROL Panneau de gauche]**, effectuez l’une des opérations suivantes pour déterminer ce que les utilisateurs verront dans le panneau de gauche pour la zone [!DNL Workfront] ou le type d’objet sélectionné :

   * Cliquez sur les icônes **Afficher** ![](assets/add-secondary-nav-item.png) ou **Masquer** ![](assets/delete-secondary-nav-item.png) pour afficher ou masquer les sections dans le panneau de gauche. Vous ne pouvez pas masquer les éléments qui n’ont pas d’icône **Afficher** ou **Masquer** .

   * Faites glisser des éléments ![](assets/move-icon---dots.png) pour modifier leur ordre dans le panneau de gauche.

   >[!NOTE]
   >
   >Les éléments suivants de la liste déroulante **[!UICONTROL Personnaliser ce que les utilisateurs voient]** se rapportent à des zones autres que le panneau de gauche :
   >* [!UICONTROL Listes]
   >* [!UICONTROL Panneau Résumé]
   >* [!UICONTROL Accueil]
   >* [!UICONTROL Branding]
   > 
   >Pour plus d’informations sur la personnalisation des zones supplémentaires, consultez les articles suivants :
   >
   >* [Personnaliser des filtres, des vues et des regroupements à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >* [Personnaliser le [!UICONTROL panneau de résumé] à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   >* [Personnaliser l’accueil à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   >* [Personnaliser le branding Adobe  [!DNL Workfront]  à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. (Facultatif) Si vous souhaitez ajouter un élément du panneau de gauche lié à l’un des tableaux de bord de votre entreprise, cliquez sur **[!UICONTROL Ajouter une section personnalisée]**, saisissez un **[!UICONTROL titre de la section personnalisée]** pour l’élément, puis ajoutez le tableau de bord.

   Les éléments du tableau de bord s’affichent au bas du panneau de gauche. Les utilisateurs voient le titre de la section personnalisée que vous tapez en regard de l’élément du tableau de bord lorsqu’ils le survolent avec la souris dans le panneau de gauche.

   >[!NOTE]
   >
   >Les utilisateurs et utilisatrices peuvent ajouter des éléments de tableau de bord personnalisés à leur propre panneau de gauche. Lorsque vous ajoutez des éléments de tableau de bord personnalisés dans un modèle de mise en page, les éléments s’affichent en plus de ceux qu’ils ajoutent, sans les remplacer ni les réinitialiser. Cela est également vrai si vous affectez des utilisateurs et utilisatrices à un nouveau modèle de mise en page avec des éléments de tableau de bord personnalisés. Pour plus d’informations sur la personnalisation du panneau de gauche par les utilisateurs et utilisatrices, voir [Créer des onglets ou sections personnalisés](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
   >
   >Pour plus d’informations sur les tableaux de bord, voir [Tableaux de bord](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Poursuivez la personnalisation du modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **[!UICONTROL Enregistrer]**.

   >[!TIP]
   >
   >Vous pouvez cliquer à tout moment sur [!UICONTROL **Enregistrer**] pour enregistrer votre progression, ce qui ferme l’éditeur de modèles de mise en page, puis continuer à modifier le modèle ultérieurement.
