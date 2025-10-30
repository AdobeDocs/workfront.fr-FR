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
source-git-commit: d342df9949eb1434acbb53c29b7e329dd91c9b28
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 32%

---

# Créer et gérer des fonctions

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>Avec la version 25.11, la devise de remplacement pour les fonctions sera abandonnée dans la production. (L’obsolescence a lieu le 30 octobre dans l’environnement de prévisualisation.) Au lieu d’avoir une devise de base et des devises de remplacement, une devise sera disponible pour les fonctions, et les taux de coût et de facturation seront définis à l’aide de cette devise.

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
1. Configurez les champs suivants :

   * **Nom** : indiquez un nom pour la fonction. Il s’agit du nom qui s’affiche partout dans Workfront où s’affiche le champ Fonction .

     >[!TIP]
     >
     >Le nom d’une fonction peut contenir jusqu’à 255 caractères. Toutefois, les noms plus longs peuvent être tronqués dans certaines zones de Workfront.

   * **Description** : saisissez une description du rôle qui indique ce qui est unique à son sujet.
   * **Est actif** : sélectionnez **Oui** si vous souhaitez que le rôle soit actif et disponible partout dans Workfront pour être associé aux utilisateurs et utilisatrices, aux tâches, etc. Sélectionnez **Non** si vous souhaitez que le rôle soit désactivé et qu’il ne soit pas disponible pour être affecté aux utilisateurs, aux éléments de travail, etc.

     Pour plus d’informations sur la désactivation des fonctions, voir la section [Désactiver des fonctions](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

   * **Devise de base** : il s’agit de la devise de base, telle que définie dans la zone Configuration par votre administrateur Workfront. Pour plus d’informations, voir [Configurer les taux de change](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     >[!TIP]
     >
     >Vous ne pouvez pas modifier la devise de base au niveau de la fonction. Ce champ est grisé et sert de rappel de la devise de base de votre système.

   * **Taux de coût** : il s’agit du taux de coût horaire de la fonction. Cette valeur calcule les coûts prévus et réels des tâches et des problèmes associés au rôle et, par conséquent, les coûts prévus et réels des projets. Entrez le taux en utilisant la devise de base.

     Pour connaitre les taux de dépenses effectifs par date, cliquez sur **Ajouter un taux**. Saisissez la valeur du coût/heure pour la période, puis affectez une Date de début et une Date de fin, le cas échéant. Le premier taux de coût ne comporte pas de date de début et le dernier taux de coût ne comporte pas de date de fin.

     Certaines dates sont ajoutées automatiquement. Par exemple, si le premier taux de coût n’a pas de date de fin et que vous ajoutez un second taux de coût avec une date de début fixée au 1er mai 2025, une date de fin fixée au 30 avril 2025 est ajoutée au premier taux de coût afin qu’il n’y ait aucun écart.

     >[!TIP]
     >
     >Lors de la modification d’une fonction existante, vous pouvez sélectionner **Trier par date de début** pour afficher la date de début la plus récente en haut de la liste des taux.

   * **Taux de facturation** : il s’agit du taux de facturation horaire de la fonction. Cette valeur calcule les revenus prévus et réels des tâches et des problèmes associés au rôle et, par conséquent, les revenus prévus et réels des projets. Entrez le taux en utilisant la devise de base.

     Pour connaître les taux de facturation effectifs par date, cliquez sur **Ajouter un taux**. Saisissez la valeur de la facturation/heure pour la période, puis affectez une date de début et une date de fin, si nécessaire. Le premier taux de facturation ne comporte pas de date de début et le dernier taux de facturation ne comporte pas de date de fin.

     Certaines dates sont ajoutées automatiquement. Par exemple, si le premier taux de facturation n’a pas de date de fin et que vous ajoutez un second avec une date de début fixée au 1er mai 2025, une date de fin fixée au 30 avril 2025 est ajoutée au premier taux de facturation afin qu’il n’y ait aucun écart.

     >[!TIP]
     >
     >Lors de la modification d’une fonction existante, vous pouvez sélectionner **Trier par date de début** pour afficher la date de début la plus récente en haut de la liste des taux.

   * **Remplacer la devise** : sélectionnez une devise associée à cette fonction. Il s’agit de la devise utilisée par Workfront pour calculer les coûts et les revenus associés à cette fonction.

     Cette devise est différente de la devise de base configurée par votre administrateur Workfront dans la zone Configuration et peut être différente de la devise associée à un projet.

     >[!TIP]
     >
     >Seules les devises disponibles dans la zone Taux de change de votre système sont disponibles dans ce champ. Si une seule devise est configurée, ce champ n’apparaît pas.

     Pour plus d’informations sur la configuration de la devise de base dans Workfront, voir [Configurer des taux de change](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     Pour plus d’informations sur la modification de la devise d’un projet, voir [Modifier la devise du projet](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

   * **Taux de remplacement de devise** : Il s&#39;agit du taux horaire du coût de la fonction utilisant la devise de remplacement sélectionnée. Workfront utilise cette valeur pour calculer les coûts prévus et réels des tâches et des événements associés à la fonction.

     Entrez le taux dans la devise de remplacement spécifiée ci-dessus. Cette option met également à jour le taux de coût pour cette fonction lors de l&#39;utilisation de la devise de base.

     Pour plus d’informations sur la façon dont Workfront calcule les coûts, voir [Suivre les coûts](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >Lors de la mise à jour d’une fonction existante à laquelle un taux de coût est déjà associé, Workfront calcule le taux de change de remplacement en fonction du taux de conversion de votre système. Si vous mettez à jour le taux de remplacement de devise, le taux de coût de la fonction est également mis à jour automatiquement.

   * **Taux de facturation de la devise de remplacement** : il s’agit du taux de facturation par heure de la fonction utilisant la devise de remplacement sélectionnée. Workfront utilise cette valeur pour calculer le revenu prévu et le revenu réel des tâches et des événements associés à la fonction.

     Entrez le taux dans la devise de remplacement spécifiée ci-dessus. Cette action met également à jour le taux de facturation de cette fonction lors de l’utilisation de la devise de base.

     Pour plus d’informations sur le calcul du chiffre d’affaires par Workfront, voir [Présentation de la facturation et du chiffre d’affaires](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >Lors de la mise à jour d’une fonction existante à laquelle un taux de facturation est déjà associé, Workfront calcule le taux de remplacement de la devise en fonction du taux de conversion de votre système. Si vous mettez à jour le taux de facturation de la devise de remplacement, le taux de facturation de la fonction est également mis à jour automatiquement.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicate a name for the job role. This is the name that displays everywhere in [!DNL Workfront] where the [!UICONTROL Job Role] field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Enter a description for the role that indicates what is unique about it. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <b>[!UICONTROL Yes]</b> if you want the role to be active and available everywhere in [!DNL Workfront] to be associated with users, work items, etc. </p> </li> 
        <li> <p>Select <b>[!UICONTROL No]</b>, if you want the role to be deactivated and not available to assign to users, work items, etc. </p> </li> 
       </ul> <p><span>For information about deactivating job roles, see</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>This is the [!UICONTROL Base Currency], as set in the [!UICONTROL Setup] area by your Workfront administrator. For information, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span>You cannot edit the [!UICONTROL Base Currency] at the job role level. This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> 
      <p>For date effective cost rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the cost/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first cost rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> <p>For date effective billing rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the billing/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first billing rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Select a currency associated with this job role. This is the currency that [!DNL Workfront] uses for calculating costs and revenue associated with this job role. </p> 
        <p><span>This is different than the [!UICONTROL Base Currency] set up by your [!DNL Workfront] administrator in the [!UICONTROL Setup] area, and can be different than the currency associated with a project.</span> </p> 
        <p>Tip: Only currencies available in the [!UICONTROL Exchange Rates] area in your system are available in this field. If you only have one currency set up, this field is does not appear.</p> 
       <p><span>For information about setting up the [!UICONTROL Base Currency] in [!DNL Workfront], see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span>For information about changing the currency of a project, see</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>This is the cost per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Cost Rate for this job role when using the [!UICONTROL Base Currency].</span> </p> 
        <p>For information about how [!DNL Workfront] calculates cost, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> 
       <p>Tip: When updating an existing job role that already has a Cost Rate associated with it, [!DNL Workfront] calculates the [!UICONTROL Override Currency] rate based on the conversion rate in your system. If you update the [!UICONTROL Override Currency Cost Rate], the Cost Rate of the job role also updates automatically.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>This is the billing per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p>
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Billing Rateate for this job role when using the [!UICONTROL Base Currency].</span> </p>
        <p>For information about how [!DNL Workfront] calculates revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p>
        <p>Tip: When updating an existing job role that already has a Billing Rate associated with it, [!DNL Workfront] calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the Billing Rate of the job role also updates automatically. </p>
       </td>
     </tr> 
    </tbody> 
   </table>
-->

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
