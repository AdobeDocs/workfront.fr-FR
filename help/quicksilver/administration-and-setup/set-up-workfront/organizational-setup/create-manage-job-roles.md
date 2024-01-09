---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Création et gestion des rôles de tâche
description: Comme [!DNL Adobe Workfront] administrateur ou utilisateur disposant d’un accès administratif aux rôles de tâche, vous pouvez créer des rôles de tâche qui peuvent être attribués à des utilisateurs et supprimer les rôles de tâche par défaut qui ne sont pas pertinents pour votre organisation.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 3af289f9aeecee417d1e82f9c66551360185b85c
workflow-type: tm+mt
source-wordcount: '1163'
ht-degree: 0%

---

# Création et gestion des rôles de tâche

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Comme [!DNL Adobe Workfront] administrateur ou utilisateur disposant d’un accès administratif aux rôles de tâche, vous pouvez créer des rôles de tâche qui peuvent être attribués à des utilisateurs et supprimer les rôles de tâche par défaut qui ne sont pas pertinents pour votre organisation. Pour plus d’informations sur l’accès administrateur dans [!DNL Workfront], voir [Octroi aux utilisateurs un accès administratif à certaines zones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Quelconque </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>Actuel : formule [!UICONTROL]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux rôles de tâche</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

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
      <td> <p>Indiquez un nom pour le rôle de tâche. Nom qui s’affiche partout dans [!DNL Workfront] où le champ [!UICONTROL Rôle de la tâche] s’affiche. </p> <p>Conseil : Le nom d’un rôle de tâche peut contenir jusqu’à 255 caractères. Toutefois, les noms plus longs peuvent être tronqués dans certaines zones de [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Saisissez une description pour le rôle qui indique ce qui est unique à son sujet. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Est Actif]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Sélectionner <b>[!UICONTROL Oui]</b> si vous souhaitez que le rôle soit actif et disponible partout dans [!DNL Workfront] à être associés aux utilisateurs, aux tâches, etc. </p> </li> 
        <li> <p>Sélectionner <b>[!UICONTROL No]</b>, si vous souhaitez que le rôle soit désactivé et qu’il ne soit pas disponible pour être affecté aux utilisateurs, aux tâches, etc. </p> </li> 
       </ul> <p><span>Pour plus d’informations sur la désactivation des rôles de tâche, voir</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Désactivation des rôles de tâche</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Devise de base]</span> </td> 
      <td> <p><span>Il s’agit de la [!UICONTROL Devise de base], telle que définie dans la zone [!UICONTROL Configuration] par votre administrateur Workfront. Pour plus d’informations, voir</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurer les taux de change</a> .</p> <p>Conseil : <span>Vous ne pouvez pas modifier la [!UICONTROL Devise de base] au niveau du rôle de tâche. Ce champ est grisé et sert de rappel de la devise de base de votre système.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>Il s’agit du taux de coût par heure du rôle de tâche. Cette valeur calcule les coûts prévus et les coûts réels des tâches et des problèmes associés au rôle, ainsi que, en fin de compte, les coûts prévus et les coûts réels des projets. Saisissez le taux à l’aide de la [!UICONTROL Devise de base].</p> 
      <p>Pour consulter les taux de coût en vigueur à la date, cliquez sur <strong>[!UICONTROL Taux d’ajout]</strong>. Saisissez la valeur du coût/de l’heure pour la période, puis attribuez une [!UICONTROL Date de début] et une [!UICONTROL Date de fin] si nécessaire. Le premier taux de coût ne comporte pas de date de début et le dernier taux de coût ne comporte pas de date de fin.</p> <p>Certaines dates sont ajoutées automatiquement. Par exemple, si le premier taux de coût n’a pas de date de fin et que vous ajoutez un second taux de coût avec une date de début le 1er mai 2023, une date de fin le 30 avril 2023 est ajoutée au premier taux de coût afin qu’il n’y ait pas d’écart.</p> <p>Conseil : Lorsque vous modifiez un rôle de tâche existant, vous pouvez sélectionner <strong>Tri par date de début</strong> pour afficher la date de début la plus récente en haut de la liste des taux.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Taux de facturation] </td> 
      <td><p>Il s’agit du taux de facturation par heure du rôle de tâche. Cette valeur calcule les revenus prévus et réels des tâches et des problèmes associés au rôle, ainsi que, en fin de compte, les revenus prévus et réels des projets. Saisissez le taux à l’aide de la [!UICONTROL Devise de base].</p> <p>Pour connaître les taux de facturation en vigueur à la date, cliquez sur <strong>[!UICONTROL Taux d’ajout]</strong>. Saisissez la valeur de la facturation/heure pour la période, puis attribuez une [!UICONTROL Date de début] et une [!UICONTROL Date de fin], le cas échéant. Le premier taux de facturation n'a pas de date de début et le dernier taux de facturation n'a pas de date de fin.</p> <p>Certaines dates sont ajoutées automatiquement. Par exemple, si le premier taux de facturation ne comporte pas de date de fin et que vous ajoutez une seconde avec une date de début le 1er mai 2023, une date de fin du 30 avril 2023 est ajoutée au premier taux de facturation afin qu’il n’y ait pas d’écart.</p> <p>Conseil : Lorsque vous modifiez un rôle de tâche existant, vous pouvez sélectionner <strong>Tri par date de début</strong> pour afficher la date de début la plus récente en haut de la liste des taux.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Remplacer la devise]</span> </td> 
      <td>
        <p>Sélectionnez une devise associée à ce rôle de tâche. Il s’agit de la devise qui [!DNL Workfront] utilise pour calculer les coûts et les recettes associés à ce rôle de tâche. </p> 
        <p><span>Différent de la [!UICONTROL Devise de base] configurée par votre [!DNL Workfront] dans la zone [!UICONTROL Configuration] et peut être différent de la devise associée à un projet.</span> </p> 
        <p>Conseil : Seules les devises disponibles dans la zone [!UICONTROL Taux de change] de votre système sont disponibles dans ce champ.</p> 
       <p><span>Pour plus d’informations sur la configuration de la [!UICONTROL Devise de base] dans [!DNL Workfront], voir</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurer les taux de change</a>.</p> <p><span>Pour plus d’informations sur la modification de la devise d’un projet, voir</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Modification de la devise du projet</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Remplacement du taux de coût de la devise]</span> </td> 
      <td>
        <p>Il s’agit du taux de coût par heure du rôle de tâche à l’aide de la [!UICONTROL Devise de remplacement] sélectionnée. [!DNL Workfront] utilise cette valeur pour calculer les coûts prévus et les coûts réels des tâches et des problèmes associés au rôle de tâche. </p> 
        <p><span>Saisissez le taux dans la devise de remplacement [!UICONTROL] spécifiée ci-dessus. Cela met également à jour le taux de coût de ce rôle de tâche lors de l’utilisation de la [!UICONTROL Devise de base].</span> </p> 
        <p>Pour plus d’informations sur la manière dont [!DNL Workfront] calcule le coût, voir <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Suivi des coûts</a>.</p> 
       <p>Conseil : lors de la mise à jour d’un rôle de tâche existant auquel est déjà associé un taux de coût, [!DNL Workfront] calcule le taux de remplacement de la devise [!UICONTROL] en fonction du taux de conversion de votre système. Si vous mettez à jour le [!UICONTROL Override Currency Cost Rate] (Taux de coût de la devise de remplacement), le taux de coût du rôle de tâche est également mis à jour automatiquement.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Remplacement du taux de facturation de la devise]</span> </td> 
      <td>
        <p>Il s’agit du taux de facturation par heure du rôle de tâche à l’aide de la [!UICONTROL Devise de remplacement] sélectionnée. [!DNL Workfront] utilise cette valeur pour calculer les recettes prévues et réelles des tâches et des problèmes associés au rôle de tâche. </p>
        <p><span>Saisissez le taux dans la devise de remplacement [!UICONTROL] spécifiée ci-dessus. Cela met également à jour le taux de facturation pour ce rôle de tâche lors de l’utilisation de la [!UICONTROL Devise de base].</span> </p>
        <p>Pour plus d’informations sur la manière dont [!DNL Workfront] calcule les recettes, voir <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Présentation de la facturation et des recettes</a>.</p>
        <p>Conseil : lors de la mise à jour d’un rôle de tâche existant auquel est déjà associé un taux de facturation, [!DNL Workfront] calcule le taux de change de remplacement en fonction du taux de conversion de votre système. Si vous mettez à jour le taux de facturation de la devise de remplacement, le taux de facturation du rôle de tâche est également mis à jour automatiquement. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Les rôles de tâche font partie intégrante de la gestion des ressources. Pour utiliser les outils de planification des ressources, les rôles de tâche doivent comporter un coût et un taux de facturation. Pour plus d’informations, voir [Prise en main de la gestion des ressources](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Cliquez sur **[!UICONTROL Création d’un rôle de tâche]**. Le rôle de tâche peut désormais être attribué à des tâches, des problèmes, des validations ou vous pouvez partager des modèles de mise en page ou d’autres objets avec lui. Pour plus d’informations sur toutes les utilisations des rôles de tâche dans [!DNL Workfront], voir [Présentation des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Pour plus d’informations sur la suppression d’un rôle de tâche, voir [Suppression de rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
