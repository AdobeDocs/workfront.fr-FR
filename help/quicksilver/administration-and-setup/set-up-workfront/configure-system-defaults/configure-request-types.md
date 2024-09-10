---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configuration des types de requête
description: Lorsque vous travaillez sur un projet, des événements inattendus peuvent survenir. Vous pouvez enregistrer ces événements inattendus en tant que problèmes pour un projet ou une tâche spécifique. Vous pouvez également soumettre des requêtes, qui sont enregistrées en tant que problèmes sur un projet désigné comme file d’attente des demandes. Les problèmes et les requêtes sont considérés comme interchangeables dans Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 99%

---

# Configurer les types de demandes

Lorsque vous travaillez sur un projet, des événements inattendus peuvent survenir. Vous pouvez enregistrer ces événements inattendus en tant que problèmes pour un projet ou une tâche spécifique. Vous pouvez également soumettre des requêtes, qui sont enregistrées en tant que problèmes sur un projet désigné comme file d’attente des demandes. Les problèmes et les requêtes sont considérés comme interchangeables dans Adobe Workfront.

Pour plus d’informations sur la création de problèmes dans [!DNL Workfront], consultez la section [Créer des problèmes](../../../manage-work/issues/manage-issues/create-issues.md). Pour plus d’informations sur la création de requêtes dans [!DNL Workfront], consultez la section [Créer et soumettre des requêtes  [!DNL Adobe Workfront] ](../../../manage-work/requests/create-requests/create-submit-requests.md). Pour plus d’informations sur l’association de types de requêtes à des projets, consultez la section [Définir des types de requêtes pour un projet](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td><p>Nouvelle : [!UICONTROL Standard]</p>
   Ou
   <p>Actuelle : [!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## Personnaliser les noms des types de requête

En tant que personne membre de l’équipe d’administration de [!DNL Workfront], vous pouvez configurer les noms des types de requêtes dans votre système. Les nouveaux noms sont visibles dans toutes les zones de [!DNL Workfront] où les champs **[!UICONTROL Type de problème]** ou **[!UICONTROL Type de requête]** s’affichent :

* Dans la zone **[!UICONTROL Détails de la file d’attente]** d’un projet qui recevra les problèmes ou les requêtes.
* Lorsque vous créez un problème ou soumettez une nouvelle requête, plusieurs types de requêtes sont sélectionnés pour une file d’attente des demandes, dans le champ **[!UICONTROL Type de problème]** du **[!UICONTROL formulaire Nouveau problème]**.

  Pour plus d’informations sur la création de problèmes dans [!DNL Workfront], consultez la section [Créer des problèmes](../../../manage-work/issues/manage-issues/create-issues.md).

  Pour plus d’informations sur la création de requêtes dans [!DNL Workfront], consultez la section [Créer et soumettre des requêtes  [!DNL Adobe Workfront] ](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Sur le formulaire **[!UICONTROL Détails de la rubrique de file d’attente]**, lorsque vous configurez la rubrique de file d’attente.\
   Pour plus d’informations sur la création de rubriques de file d’attente, consultez la section [Créer des rubriques de file d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Pour personnaliser les noms des types de requête, procédez comme suit :

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL Statuts]**.

1. Sélectionnez l’onglet **[!UICONTROL Problèmes]**.
1. En haut de l’onglet **[!UICONTROL Problèmes]**, pointez sur le nom d’un type de requête, puis cliquez sur l’icône **[!UICONTROL Modifier]** qui apparaît.

   ![](assets/edit-request-type-name-nwe.png)

1. Dans la zone qui apparaît, saisissez un nouveau nom, puis appuyez sur **[!UICONTROL Entrée]**.

## Configurer les statuts des problèmes dans les différents types de requêtes

Vous pouvez affecter différents statuts de problème à chaque type de requête. Vous pouvez également modifier l’ordre dans lequel les statuts s’affichent sur un problème, en fonction du type de problème.

Pour plus d’informations sur la modification de l’ordre par défaut des statuts d’un problème et la configuration des statuts d’un problème, consultez la section [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) dans l’article [Créer ou modifier un statut](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
