---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Désactivation des rôles de tâche
description: En tant que [!DNL Adobe Workfront] Pour un administrateur ou un utilisateur disposant d’un accès administratif aux rôles de tâche, vous pouvez désactiver les rôles de tâche qui deviennent obsolètes dans votre système. Lorsque vous désactivez un rôle de tâche au lieu de le supprimer, vous pouvez conserver toutes les informations historiques qui lui sont associées.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Désactivation des rôles de tâche

En tant que [!DNL Adobe Workfront] Pour un administrateur ou un utilisateur disposant d’un accès administratif aux rôles de tâche, vous pouvez désactiver les rôles de tâche qui deviennent obsolètes dans votre système. Lorsque vous désactivez un rôle de tâche au lieu de le supprimer, vous pouvez conserver toutes les informations historiques qui lui sont associées.

Vous pouvez également réactiver les rôles de tâche précédemment désactivés.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront]*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Accès administratif aux rôles de tâche</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Impact de la désactivation des rôles de tâche

Si vous désactivez un rôle de tâche, il ne s’affiche plus dans les zones suivantes :

* Le [!UICONTROL Affectations] Champ de saisie anticipée (pour les tâches, les tâches de modèle, les problèmes, les validations et les règles de routage)
* Le [!UICONTROL Affectations] champs dans les listes et les rapports
* Profils utilisateur

   >[!NOTE]
   >
   >Lorsque vous ajoutez un nouveau rôle à un utilisateur, un rôle de tâche désactivée ne s’affiche pas. Mais il continue de s’afficher dans la variable [!UICONTROL Rôle Principal] et [!UICONTROL Autres rôles] s’il était associé au rôle de tâche avant sa désactivation.

* Le [!UICONTROL Partage] boîte de dialogue pour les objets, y compris l’attribution du modèle de mise en page
* Champs de saisie anticipée dans les formulaires personnalisés
* Le [!UICONTROL Membres du pool] champ dans [!UICONTROL Groupes de ressources]
* Le [!UICONTROL Rôle de tâche] champ d’un [!UICONTROL Taux de facturation] écran de modification lorsqu’un utilisateur remplace les taux de facturation des projets
* Le [!UICONTROL Ajouter une affectation au panorama Kanban] boîte de dialogue d’un projet
* Le [!UICONTROL Rôle de tâche] champ d’un plan ou d’une initiative lorsqu’une personne utilise la variable [!DNL Adobe Workfront Scenario Planner].

   Le [!DNL Scenario Planner] n’est disponible que dans la nouvelle [!DNL Adobe Workfront] et nécessite une licence supplémentaire. Pour plus d’informations sur la variable [!DNL Workfront Scenario Planner], voir [Le [!DNL Scenario Planner] aperçu](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Les rôles désactivés s’affichent toujours dans les filtres des listes, des rapports et d’autres outils tels que le [!DNL Workload Balancer].

## Observations avant la désactivation d’un rôle de tâche

Il est préférable de désactiver plutôt que de supprimer les rôles de tâche devenus obsolètes afin de conserver toutes les informations historiques associées aux rôles que vous avez peut-être utilisés dans le passé.

>[!NOTE]
>
>Les tâches affectées au rôle de tâche avant la désactivation restent affectées.

Nous vous recommandons d’effectuer les opérations suivantes avant de désactiver un rôle de tâche inutilisé :

* Créez des rapports pour tous les objets affectés au rôle que vous prévoyez de désactiver et de les réaffecter à un rôle de tâche principal. Pour plus d’informations sur la création de rapports, voir [Créer un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

   >[!TIP]
   >
   >Vous pouvez créer un rapport afin de filtrer les tâches ou les problèmes pour lesquels le rôle désactivé est affecté. Utilisez ensuite le rapport pour réaffecter les tâches ou problèmes en suspens à un rôle principal.

* Faites l’inventaire de tous les processus d’approbation, chemins d’approbation actuels et règles de routage ou autres objets affectés au rôle de tâche que vous prévoyez de désactiver et de les réaffecter à un rôle principal.

   >[!TIP]
   >
   >Lors de l’utilisation des files d’attente de requête, si vous désactivez un rôle de tâche attribué comme cessionnaire par défaut dans une règle de routage, le rôle est conservé et les demandes sont toujours acheminées vers le rôle désactivé. Nous vous recommandons de mettre à jour les règles de routage avec des rôles principaux avant de désactiver l’équipe.

   Pour plus d’informations sur la création de processus de validation et de règles de routage, voir les articles suivants :

   * [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Création de règles de routage](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Désactivation d’un rôle de tâche

1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur &#x200B; **[!UICONTROL Rôles de tâche].**
1. (Facultatif) Dans le **[!UICONTROL Filtrer]** menu déroulant, sélectionnez **[!UICONTROL Principal]** pour afficher uniquement les rôles de tâche principaux.
1. Cliquez sur le nom du rôle de tâche à désactiver.
1. Dans le **[!UICONTROL Est Principal]** menu déroulant, sélectionnez **[!UICONTROL Non]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   Le rôle de tâche est désactivé et ne peut plus être attribué au travail, associé aux modèles de mise en page, etc. Pour plus d’informations sur toutes les utilisations des rôles de tâche dans [!DNL Workfront], voir [Présentation des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
