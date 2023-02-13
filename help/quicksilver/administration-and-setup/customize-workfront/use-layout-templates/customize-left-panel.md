---
title: Personnalisation du panneau de gauche à l’aide d’un modèle de mise en page
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Dans un modèle de mise en page, vous pouvez personnaliser ce que les utilisateurs voient dans la zone de panneau de gauche dans Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: c0b0102eb1e1f45e794f962f7e905349f9e241eb
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---

# Personnalisation du panneau de gauche à l’aide d’un modèle de mise en page

Dans un modèle de mise en page, vous pouvez personnaliser ce que les utilisateurs voient dans la zone de panneau de gauche dans tout le [!DNL Adobe Workfront].

Par exemple, vous pouvez déterminer les éléments suivants que les utilisateurs voient dans le panneau de gauche lorsqu’ils visualisent une tâche :

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>Les modifications apportées à l’ordre et à la visibilité sont répercutées dans l’application mobile.

Pour plus d’informations sur les modèles de mise en page pour les groupes, voir [Création et modification des modèles de mise en page d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> Pour effectuer ces étapes au niveau du système, vous devez disposer du niveau d’accès [!UICONTROL Administrateur système].<p>Pour les exécuter pour un groupe, vous devez être un responsable de ce groupe.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personnalisation du panneau de gauche d’une zone dans [!DNL Workfront]:

1. Commencez à travailler sur un modèle de mise en page, comme décrit dans la section [Création et gestion des modèles de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Cliquez sur la flèche vers le bas ![](assets/dropdown-arrow.png) under **[!UICONTROL Personnalisation des éléments affichés par les utilisateurs]**, puis cliquez sur le panneau de gauche que vous souhaitez personnaliser.

   >[!NOTE]
   >
   >Pour plus d’informations sur la variable [!UICONTROL Accueil] dans cette liste déroulante, voir [Personnaliser [!UICONTROL Accueil] et [!UICONTROL Résumé] utilisation d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). Pour plus d’informations sur l’option Listes, voir [Personnalisation des filtres, des vues et des groupes à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Dans le **[!UICONTROL Panneau gauche]** effectuez l’une des opérations suivantes pour déterminer ce que verront les utilisateurs dans le panneau de gauche pour l’option ([!DNL Workfront] zone ou type d’objet) que vous avez sélectionné :

   * Afficher ![](assets/add-secondary-nav-item.png) ou masquer ![](assets/delete-secondary-nav-item.png) éléments. Tout élément sans ![](assets/add-secondary-nav-item.png) ou ![](assets/delete-secondary-nav-item.png) ne peut pas être masqué.

   * Faire glisser des éléments ![](assets/move-icon---dots.png) pour modifier leur ordre dans le panneau de gauche.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Option</th> 
      <th>Lorsque les utilisateurs cliquent sur ce qui suit...</th> 
      <th>Ils affichent les éléments du panneau de gauche que vous choisissez parmi les suivants :</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Project]</td> 
      <td>Nom d’un projet</td> 
      <td>[!UICONTROL Tâches], [!UICONTROL Détails Du Projet], [!UICONTROL Business Case], [!UICONTROL Mises À Jour], [!UICONTROL Documents], [!UICONTROL Problèmes], [!UICONTROL Risques], [!UICONTROL Approbations], [!UICONTROL Principes], [!UICONTROL], Rates!UICONTROL Enregistrements De Facturation], [!UICONTROL Dépenses], [!UICONTROL Hours], [!UICONTROL équilibreur De Charge De Travail], [!UICONTROL People], [!UICONTROL Utilization], [!UICONTROL Queue Details], [!UICONTROL Règles De Routage], [!UICONTROL Queue Groupe de rubriques L], [!UICONTROL Mesures]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Task]</td> 
      <td>Nom d’une tâche</td> 
      <td> [!UICONTROL Mises À Jour], [!UICONTROL Documents], [!UICONTROL Task Details], [!UICONTROL Subtask], [!UICONTROL Issues], [!UICONTROL Hours], [!UICONTROL Approvals], [!UICONTROL Expenses], [!UICONTROL Predecessors]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Problème]</td> 
      <td>Nom d’un problème</td> 
      <td> [!UICONTROL Mises À Jour], [!UICONTROL Documents], [!UICONTROL Détails Du Problème], [!UICONTROL Hours], [!UICONTROL Approbations]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>Nom d’un portfolio</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Programmes], [!UICONTROL Portfolio Details], [!UICONTROL Portfolio] [!UICONTROL Optimization], [!UICONTROL Documents], [!UICONTROL Updates]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>Nom d’un programme</td> 
      <td>[!UICONTROL Projects], [!UICONTROL Program Details], [!UICONTROL Updates], [!UICONTROL Documents]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template]</td> 
      <td>Nom d’un modèle de projet</td> 
      <td>[!UICONTROL Tâches De Modèle], [!UICONTROL Détails Du Modèle], [!UICONTROL Mises À Jour], [!UICONTROL Documents], [!UICONTROL Risques], [!UICONTROL Dépenses], [!UICONTROL Personnes], [!UICONTROL Approbations], [!UICONTROL Taux De Facturation], [!UICONTROL [!UICONTROL Routage Rules], [!UICONTROL Queue Topic], [!UICONTROL Topic Group]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tâche Modèle]</td> 
      <td>Nom d’une tâche de modèle</td> 
      <td>[!UICONTROL Mises À Jour], [!UICONTROL Documents], [!UICONTROL Template Task Details], [!UICONTROL Subtasks], [!UICONTROL Expenses], [!UICONTROL Approvals], [!UICONTROL Predecessors]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Enregistrement de facturation]</td> 
      <td>Nom d’un enregistrement de facturation pour un projet</td> 
      <td>[!UICONTROL Détails de l’enregistrement de facturation], [!UICONTROL Heures facturables], [!UICONTROL Dépenses facturables], [!UICONTROL Recettes fixes]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Projects]</td> 
      <td>Projets <img src="assets/projects-in-main-menu.png"> dans le menu principal [!UICONTROL] <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projects]</td> 
     </tr> 
     <tr> 
      <td>Demandes [!UICONTROL]</td> 
      <td>Nom d’une requête</td> 
      <td>[!UICONTROL Nouvelle requête], [!UICONTROL Demandes envoyées], [!UICONTROL Toutes les requêtes], [!UICONTROL Brouillons]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Tableaux de bord]</td> 
      <td>Nom d’un tableau de bord</td> 
      <td>[!UICONTROL Mes tableaux de bord], [!UICONTROL Tableaux de bord partagés], [!UICONTROL Tous les tableaux de bord]<p><b>REMARQUE</b>: Si vous avez créé des onglets personnalisés pour la zone [!UICONTROL Rapports] à l’aide d’un modèle de mise en page dans [!DNL Adobe Workfront Classic], ils s’affichent au bas de cette liste. Pour les utilisateurs, ils s’affichent au bas du panneau de gauche dans la zone [!UICONTROL Tableaux de bord] .</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum Team]</td> 
      <td>Nom d’une équipe Scrum</td> 
      <td><p>[!UICONTROL Itérations], [!UICONTROL Actuelle itération], [!UICONTROL Backlog], [!UICONTROL équilibreur de charge de travail], [!UICONTROL Mises à jour], [!UICONTROL Paramètres de l’équipe]</p> <p><strong>REMARQUE :</strong> Le <strong>[!UICONTROL itération actuelle]</strong> s’affiche uniquement dans le panneau de gauche lorsqu’il y a au moins une tâche ou un problème sur l’itération.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Équipe Kanban]</td> 
      <td>Le nom d'une équipe de Kanban</td> 
      <td>[!UICONTROL équilibreur de charge de travail], [!UICONTROL panorama Kanban], [!UICONTROL Backlog], [!UICONTROL Mises à jour], [!UICONTROL Paramètres de l’équipe]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Equipe des cascades]</td> 
      <td>Nom d’une équipe de cascade</td> 
      <td>[!UICONTROL équilibreur de charge de travail], [!UICONTROL Mises à jour], [!UICONTROL Demandes d’équipe], [!UICONTROL Paramètres de l’équipe]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Itération]</td> 
      <td>Nom d’une itération</td> 
      <td>[!UICONTROL Stories], [!UICONTROL Issues], [!UICONTROL Story Board], [!UICONTROL Story Board], [!UICONTROL Overview], [!UICONTROL Custom Forms], [!UICONTROL Updates] </td> 
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

   >[!NOTE]
   >
   >Les 3 derniers éléments de la variable **[!UICONTROL Personnalisation des éléments affichés par les utilisateurs]** liste déroulante ([!UICONTROL Listes], [!UICONTROL Accueil et résumé], et [!UICONTROL Marques]) sont destinés à la configuration de zones autres que le panneau de gauche. Pour plus d’informations à leur sujet, voir ces articles :
>   * [Personnalisation des filtres, des vues et des groupes à l’aide d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [Personnaliser [!UICONTROL Accueil] et [!UICONTROL Résumé] utilisation d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [Adobe de marque [!DNL Workfront] utilisation d’un modèle de mise en page](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)



1. (Facultatif) Si vous souhaitez ajouter un élément de panneau de gauche lié à l’un des tableaux de bord de votre entreprise, cliquez sur **[!UICONTROL Ajout d’une section personnalisée]**, saisissez une **[!UICONTROL Titre de la section personnalisée]** pour l’élément , puis ajoutez le tableau de bord.

   Les éléments du tableau de bord s’affichent au bas du panneau de gauche. Les utilisateurs voient le titre de la section personnalisée que vous tapez en regard de l’élément du tableau de bord lorsqu’ils passent leur curseur sur le panneau de gauche.

   >[!NOTE]
   Les utilisateurs peuvent ajouter des éléments de tableau de bord personnalisés à leur propre panneau de gauche. Lorsque vous ajoutez des éléments de tableau de bord personnalisés dans un modèle de mise en page, vos éléments fusionnent avec les leurs, sans les remplacer ni les réinitialiser. Cela est également vrai si vous affectez des utilisateurs à un nouveau modèle de mise en page avec des éléments de tableau de bord personnalisés. Pour plus d’informations sur la personnalisation du panneau de gauche par les utilisateurs, voir [Création d’onglets ou de sections personnalisés](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

   Pour plus d’informations sur les tableaux de bord, voir [Tableaux de bord](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. Continuez à personnaliser le modèle de mise en page.

   Ou

   Si vous avez terminé de personnaliser, cliquez sur **[!UICONTROL Enregistrer]**.

   >[!TIP]
   Vous pouvez cliquer sur [!UICONTROL Enregistrer] à tout moment pour enregistrer votre progression, puis continuez à modifier le modèle ultérieurement.
