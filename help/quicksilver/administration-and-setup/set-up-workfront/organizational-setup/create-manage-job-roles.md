---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Créer et gérer des fonctions
description: En tant qu’administrateur  [!DNL Adobe Workfront] ou utilisateur disposant d’un accès administratif aux rôles de tâche, vous pouvez créer des rôles de tâche qui peuvent être attribués à des utilisateurs et supprimer les rôles de tâche par défaut qui ne sont pas pertinents pour votre organisation.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 5%

---

# Créer et gérer des fonctions

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

En tant qu’administrateur [!DNL Adobe Workfront] ou utilisateur disposant d’un accès administratif aux rôles de tâche, vous pouvez créer des rôles de tâche qui peuvent être attribués à des utilisateurs et supprimer les rôles de tâche par défaut qui ne sont pas pertinents pour votre organisation. Pour plus d&#39;informations sur l&#39;accès administratif dans [!DNL Workfront], voir [Octroi aux utilisateurs de l&#39;accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>
   <p>Nouvelle : standard</p>
   <p>Actuelle : [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Accès administratif aux rôles de tâche</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

+++

## Création d’un rôle de tâche

Pour créer un rôle de tâche :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur &#x200B; **[!UICONTROL Rôles de tâche].**
1. Cliquez sur **[!UICONTROL Nouveau rôle de tâche].**
1. Configurez les éléments suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indiquez un nom pour le rôle de tâche. Il s’agit du nom qui s’affiche partout dans [!DNL Workfront] où s’affiche le champ [!UICONTROL Rôle de la tâche]. </p> <p>Conseil : Le nom d’un rôle de tâche peut contenir jusqu’à 255 caractères. Cependant, les noms plus longs peuvent être tronqués dans certaines zones de [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Saisissez une description pour le rôle qui indique ce qui est unique à son sujet. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Sélectionnez <b>[!UICONTROL Oui]</b> si vous souhaitez que le rôle soit actif et disponible partout dans [!DNL Workfront] pour être associé aux utilisateurs, aux tâches, etc. </p> </li> 
        <li> <p>Sélectionnez <b>[!UICONTROL Non]</b> si vous souhaitez que le rôle soit désactivé et qu’il ne soit pas disponible pour être attribué aux utilisateurs, aux tâches, etc. </p> </li> 
       </ul> <p><span>Pour plus d’informations sur la désactivation des rôles de tâche, voir </span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Désactivation des rôles de tâche</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Devise de base]</span> </td> 
      <td> <p><span>Il s’agit de la [!UICONTROL Devise de base], telle que définie dans la zone [!UICONTROL Configuration] par votre administrateur Workfront. Pour plus d'informations, voir </span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configuration des taux d'exchange</a> .</p> <p>Conseil : <span>Vous ne pouvez pas modifier la [!UICONTROL Devise de base] au niveau du rôle de tâche. Ce champ est grisé et sert de rappel de la devise de base de votre système.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>Il s’agit du taux de coût par heure du rôle de tâche. Cette valeur calcule les coûts prévus et les coûts réels des tâches et des problèmes associés au rôle, ainsi que, en fin de compte, les coûts prévus et les coûts réels des projets. Saisissez le taux à l’aide de la [!UICONTROL Devise de base].</p> 
      <p>Pour les taux de coût en vigueur à la date, cliquez sur <strong>[!UICONTROL Ajouter le taux]</strong>. Saisissez la valeur du coût/de l’heure pour la période, puis attribuez une [!UICONTROL Date de début] et une [!UICONTROL Date de fin] si nécessaire. Le premier taux de coût ne comporte pas de date de début et le dernier taux de coût ne comporte pas de date de fin.</p> <p>Certaines dates sont ajoutées automatiquement. Par exemple, si le premier taux de coût n’a pas de date de fin et que vous ajoutez un second taux de coût avec une date de début le 1er mai 2023, une date de fin le 30 avril 2023 est ajoutée au premier taux de coût afin qu’il n’y ait pas d’écart.</p> <p>Conseil : Lors de la modification d’un rôle de tâche existant, vous pouvez sélectionner <strong>Trier par date de début</strong> pour afficher la date de début la plus récente en haut de la liste des taux.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Taux de facturation] </td> 
      <td><p>Il s’agit du taux de facturation par heure du rôle de tâche. Cette valeur calcule les revenus prévus et réels des tâches et des problèmes associés au rôle, ainsi que, en fin de compte, les revenus prévus et réels des projets. Saisissez le taux à l’aide de la [!UICONTROL Devise de base].</p> <p>Pour connaître les taux de facturation en vigueur à la date, cliquez sur <strong>[!UICONTROL Ajouter le taux]</strong>. Saisissez la valeur de la facturation/heure pour la période, puis attribuez une [!UICONTROL Date de début] et une [!UICONTROL Date de fin], le cas échéant. Le premier taux de facturation n'a pas de date de début et le dernier taux de facturation n'a pas de date de fin.</p> <p>Certaines dates sont ajoutées automatiquement. Par exemple, si le premier taux de facturation ne comporte pas de date de fin et que vous ajoutez une seconde avec une date de début le 1er mai 2023, une date de fin du 30 avril 2023 est ajoutée au premier taux de facturation afin qu’il n’y ait pas d’écart.</p> <p>Conseil : Lors de la modification d’un rôle de tâche existant, vous pouvez sélectionner <strong>Trier par date de début</strong> pour afficher la date de début la plus récente en haut de la liste des taux.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Remplacer la devise]</span> </td> 
      <td>
        <p>Sélectionnez une devise associée à ce rôle de tâche. Il s’agit de la devise utilisée par [!DNL Workfront] pour calculer les coûts et les recettes associés à ce rôle de tâche. </p> 
        <p><span>Ceci est différent de la [!UICONTROL Base Currency] configurée par votre administrateur [!DNL Workfront] dans la zone [!UICONTROL Setup] et peut être différente de la devise associée à un projet.</span> </p> 
        <p>Conseil : Seules les devises disponibles dans la zone [!UICONTROL Taux d’Exchange] de votre système sont disponibles dans ce champ. Si une seule devise est configurée, ce champ n’apparaît pas.</p> 
       <p><span> Pour plus d’informations sur la configuration de la [!UICONTROL Devise de base] dans [!DNL Workfront], voir </span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref"> </a> Configuration des taux d’exchange.</p> <p><span>Pour plus d’informations sur la modification de la devise d’un projet, voir </span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Modification de la devise du projet</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Remplacer le taux de coût de la devise]</span> </td> 
      <td>
        <p>Il s’agit du taux de coût par heure du rôle de tâche à l’aide de la [!UICONTROL Devise de remplacement] sélectionnée. [!DNL Workfront] utilise cette valeur pour calculer les coûts prévus et les coûts réels des tâches et des problèmes associés au rôle de tâche. </p> 
        <p><span>Saisissez le taux dans la devise de remplacement [!UICONTROL] spécifiée ci-dessus. Cela met également à jour le taux de coût de ce rôle de tâche lors de l’utilisation de la [!UICONTROL Devise de base].</span> </p> 
        <p>Pour plus d'informations sur la façon dont [!DNL Workfront] calcule le coût, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Tracker les coûts</a>.</p> 
       <p>Conseil : Lors de la mise à jour d’un rôle de tâche existant auquel est déjà associé un taux de coût, [!DNL Workfront] calcule le taux de [!UICONTROL Override Currency] (devise de remplacement) en fonction du taux de conversion de votre système. Si vous mettez à jour le [!UICONTROL Override Currency Cost Rate] (Taux de coût de la devise de remplacement), le taux de coût du rôle de tâche est également mis à jour automatiquement.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Remplacement du taux de facturation de la devise]</span> </td> 
      <td>
        <p>Il s’agit du taux de facturation par heure du rôle de tâche à l’aide de la [!UICONTROL Devise de remplacement] sélectionnée. [!DNL Workfront] utilise cette valeur pour calculer les recettes prévues et réelles des tâches et des problèmes associés au rôle de tâche. </p>
        <p><span>Saisissez le taux dans la devise de remplacement [!UICONTROL] spécifiée ci-dessus. Cela met également à jour le taux de facturation pour ce rôle de tâche lors de l’utilisation de la [!UICONTROL Devise de base].</span> </p>
        <p>Pour plus d’informations sur la façon dont [!DNL Workfront] calcule les recettes, voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Présentation de la facturation et des recettes</a>.</p>
        <p>Conseil : Lors de la mise à jour d’un rôle de tâche existant auquel est déjà associé un taux de facturation, [!DNL Workfront] calcule le taux de change de remplacement en fonction du taux de conversion de votre système. Si vous mettez à jour le taux de facturation de la devise de remplacement, le taux de facturation du rôle de tâche est également mis à jour automatiquement. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Les rôles de tâche font partie intégrante de la gestion des ressources. Pour utiliser les outils de planification des ressources, les rôles de tâche doivent comporter un coût et un taux de facturation. Pour plus d’informations, voir [Prise en main de la gestion des ressources](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Cliquez sur **[!UICONTROL Créer un rôle de tâche]**. Le rôle de tâche peut désormais être attribué à des tâches, des problèmes, des validations ou vous pouvez partager des modèles de mise en page ou d’autres objets avec lui. Pour plus d’informations sur toutes les utilisations des rôles de tâche dans [!DNL Workfront], voir [Présentation des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Pour plus d’informations sur la suppression d’un rôle de tâche, voir [Suppression de rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
