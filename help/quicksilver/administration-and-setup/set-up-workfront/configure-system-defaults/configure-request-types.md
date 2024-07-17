---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurer les types de requêtes
description: Lorsque vous travaillez sur un projet, vous pouvez découvrir que des événements inattendus se produisent. Vous pouvez consigner ces événements inattendus comme des problèmes pour un projet ou une tâche spécifique. Vous pouvez également envoyer des requêtes, qui sont enregistrées en tant que problèmes sur un projet désigné comme file d’attente de requêtes. Les problèmes et les requêtes sont considérés comme interchangeables dans Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 19%

---

# Configurer les types de requêtes

Lorsque vous travaillez sur un projet, vous pouvez découvrir que des événements inattendus se produisent. Vous pouvez consigner ces événements inattendus comme des problèmes pour un projet ou une tâche spécifique. Vous pouvez également envoyer des requêtes, qui sont enregistrées en tant que problèmes sur un projet désigné comme file d’attente de requêtes. Les problèmes et les requêtes sont considérés comme interchangeables dans Adobe Workfront.

Pour plus d’informations sur la création de problèmes dans [!DNL Workfront], voir [Création de problèmes](../../../manage-work/issues/manage-issues/create-issues.md). Pour plus d’informations sur la création de requêtes dans [!DNL Workfront], voir [Créer et envoyer [!DNL Adobe Workfront] requêtes](../../../manage-work/requests/create-requests/create-submit-requests.md). Pour plus d’informations sur l’association des types de requête aux projets, voir [Définition des types de requête pour un projet](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront].</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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

## Personnalisation des noms des types de requêtes

En tant qu’administrateur [!DNL Workfront], vous pouvez configurer les noms des types de requêtes de votre système. Les nouveaux noms sont visibles dans n’importe quelle zone de [!DNL Workfront] où s’affichent les champs **[!UICONTROL Type de problème]** ou **[!UICONTROL Type de demande]** :

* Dans la zone **[!UICONTROL Détails de la file d’attente]** d’un projet qui recevra les problèmes ou les requêtes.
* Si plusieurs types de requêtes sont sélectionnés pour une file d’attente des requêtes, dans le formulaire **[!UICONTROL New Issue] Form** du champ **[!UICONTROL Issue Type]** , lorsque vous créez un problème ou envoyez une nouvelle requête.

  Pour plus d’informations sur la création de problèmes dans [!DNL Workfront], voir [Création de problèmes](../../../manage-work/issues/manage-issues/create-issues.md)

  Pour plus d’informations sur la création de requêtes dans [!DNL Workfront], voir [Créer et envoyer [!DNL Adobe Workfront] requêtes](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Sur le formulaire **[!UICONTROL Queue Topic Detail]**, lorsque vous configurez la rubrique de la file d’attente.\
   Pour plus d’informations sur la création de rubriques de files d’attente, consultez la section [Créer des rubriques de files d’attente](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Pour personnaliser les noms des types de requêtes :

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Préférences du projet]** > **[!UICONTROL États]**.

1. Cliquez sur l’onglet **[!UICONTROL Problèmes]** .
1. Dans la partie supérieure de l’onglet **[!UICONTROL Problèmes]**, passez la souris sur le nom d’un type de requête, puis cliquez sur l’icône **[!UICONTROL Modifier]** qui s’affiche.

   ![](assets/edit-request-type-name-nwe.png)

1. Dans la zone qui s’affiche, saisissez un nouveau nom, puis appuyez sur **[!UICONTROL Entrée]**.

## Configuration des statuts des problèmes dans différents types de requêtes

Vous pouvez associer chaque type de requête à différents statuts de problème. Vous pouvez également modifier l’ordre dans lequel les états s’affichent sur un problème, selon le type de problème.

Pour plus d’informations sur la modification de l’ordre par défaut des statuts des problèmes et la configuration des statuts des problèmes, consultez la section [Créer ou modifier un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) dans [Créer ou modifier un état](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
