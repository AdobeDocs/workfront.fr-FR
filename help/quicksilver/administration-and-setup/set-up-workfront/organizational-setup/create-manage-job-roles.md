---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Créer et gérer des fonctions
description: En tant qu’administrateur ou administratrice  [!DNL Adobe Workfront]  ou en tant que personne disposant d’un accès administratif aux fonctions, vous pouvez créer des fonctions qui peuvent être affectées à des personnes et supprimer les fonctions par défaut qui ne concernent pas votre organisation.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 99%

---

# Créer et gérer des fonctions

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

En tant qu’administrateur ou administratrice [!DNL Adobe Workfront] ou en tant que personne disposant d’un accès administratif aux fonctions, vous pouvez créer des fonctions qui peuvent être affectées à des personnes et supprimer les fonctions par défaut qui ne concernent pas votre organisation. Pour plus d’informations sur l’accès administratif dans [!DNL Workfront], voir [Accorder aux utilisateurs et aux utilisatrices un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>Accès administratif aux fonctions</td>
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Créer une fonction

Pour créer une fonction, procédez comme suit :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Fonctions].**
1. Cliquez sur **[!UICONTROL Nouvelle fonction].**
1. Configurez les éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indiquez le nom de la fonction. Il s’agit du nom qui s’affiche partout dans [!DNL Workfront], là où apparaît le champ [!UICONTROL Job Role]. </p> <p>Conseil : le nom d’une fonction peut contenir jusqu’à 255 caractères. Toutefois, les noms plus longs peuvent être tronqués dans certaines zones de [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Saisissez une description pour le rôle, précisant ses spécificités. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Sélectionnez <b>[!UICONTROL Yes]</b> pour que le rôle soit actif et disponible partout dans [!DNL Workfront], et associé à des personnes, des éléments de travail, etc. </p> </li> 
        <li> <p>Sélectionnez <b>[!UICONTROL No]</b> pour que le rôle soit désactivé et ne puisse pas être affecté aux personnes, éléments de travail, etc. </p> </li> 
       </ul> <p><span>Pour plus d’informations sur la désactivation des fonctions, voir la section</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Désactiver des fonctions</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>Il s’agit de la [!UICONTROL Base Currency], telle que définie dans la zone [!UICONTROL Setup] par votre équipe d’administration Workfront. Pour plus d’informations, voir</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurer les taux de change</a>.</p> <p>Conseil : <span>vous ne pouvez pas modifier la [!UICONTROL Base Currency] au niveau de la fonction. Ce champ est grisé et permet de rappeler quelle est la devise de base de votre système.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>Il s’agit du coût horaire de la fonction. Cette valeur calcule les coûts prévus et réels des tâches et des problèmes associés au rôle et, par conséquent, les coûts prévus et réels des projets. Saisissez le taux à l’aide de la [!UICONTROL Base Currency].</p> 
      <p>Pour consulter les coûts applicables à une date donnée, cliquez sur <strong>[!UICONTROL Add Rate]</strong>. Saisissez la valeur du coût/heure pour la période, puis affectez une [!UICONTROL Start Date] et une [!UICONTROL End Date] en fonction des besoins. Le premier taux de coût ne comporte pas de date de début et le dernier taux de coût ne comporte pas de date de fin.</p> <p>Certaines dates sont ajoutées automatiquement. Par exemple, si le premier taux de coût ne comporte pas de date de fin et que vous en ajoutez un second avec une date de début au 1er mai 2023, une date de fin au 30 avril 2023 est ajoutée au premier taux de coût afin d’éviter tout écart.</p> <p>Conseil : lorsque vous modifiez une fonction existante, vous pouvez sélectionner <strong>Trier par date de début</strong> pour afficher la date de début la plus récente en haut de la liste des taux.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>Il s’agit du taux horaire de facturation de la fonction. Cette valeur calcule les revenus prévus et réels des tâches et des problèmes associés au rôle et, par conséquent, les revenus prévus et réels des projets. Saisissez le taux à l’aide de la [!UICONTROL Base Currency].</p> <p>Pour connaître les taux de facturation en vigueur à une date donnée, cliquez sur <strong>[!UICONTROL Add Rate]</strong>. Saisissez la valeur de la facturation/heure pour la période, puis affectez une [!UICONTROL Start Date] et une [!UICONTROL End Date] en fonction des besoins. Le premier taux de facturation ne comporte pas de date de début et le dernier taux de facturation ne comporte pas de date de fin.</p> <p>Certaines dates sont ajoutées automatiquement. Par exemple, si le premier taux de facturation ne comporte pas de date de fin et que vous en ajoutez un second avec une date de début au 1er mai 2023, une date de fin au 30 avril 2023 est ajoutée au premier taux de facturation pour éviter tout écart.</p> <p>Conseil : lorsque vous modifiez une fonction existante, vous pouvez sélectionner <strong>Trier par date de début</strong> pour afficher la date de début la plus récente en haut de la liste des taux.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Sélectionnez une devise associée à cette fonction. Il s’agit de la devise utilisée par [!DNL Workfront] pour calculer les coûts et les revenus associés à cette fonction. </p> 
        <p><span>Cette devise est différente de la [!UICONTROL Base Currency] configurée par votre administrateur ou administratrice [!DNL Workfront] dans la zone [!UICONTROL Setup] et peut être différente de la devise associée à un projet.</span> </p> 
        <p>Conseil : seules les devises disponibles dans la zone [!UICONTROL Exchange Rates] de votre système sont disponibles dans ce champ. Si une seule devise est configurée, ce champ n’apparaît pas.</p> 
       <p><span>Pour plus d’informations sur la configuration de la [!UICONTROL Base Currency] dans [!DNL Workfront], voir</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurer les taux de change</a>.</p> <p><span>Pour plus d’informations sur la modification de la devise d’un projet, voir</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Modifier la devise d’un projet</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>Il s’agit du coût horaire de la fonction selon la [!UICONTROL Override Currency] sélectionnée. [!DNL Workfront] utilise cette valeur pour calculer les coûts prévus et réels des tâches et des problèmes associés à la fonction. </p> 
        <p><span>Saisissez le taux dans la [!UICONTROL Override Currency] spécifiée ci-dessus. Cela met également à jour le taux de coût de cette fonction lors de l’utilisation de la [!UICONTROL Base Currency].</span> </p> 
        <p>Pour plus d’informations sur la manière dont [!DNL Workfront] calcule le coût, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivre les coûts</a>.</p> 
       <p>Conseil : lors de la mise à jour d’une fonction existante à laquelle est déjà associée un taux de coût, [!DNL Workfront] calcule le taux de la [!UICONTROL Override Currency] selon le taux de conversion de votre système. Si vous mettez à jour le [!UICONTROL Override Currency Cost Rate], le taux de coût de la fonction est également mis à jour automatiquement.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>Il s’agit du taux horaire de facturation de la fonction selon la [!UICONTROL Override Currency] sélectionnée. [!DNL Workfront] utilise cette valeur pour calculer les revenus prévus et réels des tâches et des problèmes associés à la fonction. </p>
        <p><span>Saisissez le taux dans la [!UICONTROL Override Currency] spécifiée ci-dessus. Cela met également à jour le taux de facturation pour cette fonction lors de l’utilisation de la [!UICONTROL Base Currency].</span> </p>
        <p>Pour plus d’informations sur la manière dont [!DNL Workfront] calcule les revenus, voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Vue d’ensemble de la facturation et des revenus</a>.</p>
        <p>Conseil : lors de la mise à jour d’une fonction existante à laquelle est déjà associée un taux de facturation, [!DNL Workfront] calcule le taux de la devise de remplacement selon le taux de conversion de votre système. Si vous mettez à jour le taux de facturation de la devise de remplacement, le taux de facturation de la fonction est également mis à jour automatiquement. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Les fonctions font partie intégrante de la gestion des ressources. Pour utiliser les outils de planification des ressources, les fonctions doivent comporter un coût et un taux de facturation qui leurs sont associés. Pour plus d’informations, voir [Commencer avec la gestion des ressources](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Cliquez sur **[!UICONTROL Créer une fonction]**. La fonction peut désormais être affectée à des tâches, des problèmes et des approbations. Vous pouvez aussi partager avec elle des modèles de mise en page ou d’autres objets. Pour plus d’informations sur tous les usages des fonctions dans [!DNL Workfront], voir [Vue d’ensemble des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Pour plus d’informations sur la suppression d’une fonction, voir [Supprimer des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
