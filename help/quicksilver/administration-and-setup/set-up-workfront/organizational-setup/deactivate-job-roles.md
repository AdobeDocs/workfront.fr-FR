---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Désactiver des fonctions
description: En tant qu’administrateur  [!DNL Adobe Workfront] ou utilisateur disposant d’un accès administratif aux rôles de tâche, vous pouvez désactiver les rôles de tâche qui deviennent obsolètes dans votre système. Lorsque vous désactivez un rôle de tâche au lieu de le supprimer, vous pouvez conserver toutes les informations historiques qui lui sont associées.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 12%

---

# Désactiver des fonctions

En tant qu’administrateur [!DNL Adobe Workfront] ou utilisateur disposant d’un accès administratif aux rôles de tâche, vous pouvez désactiver les rôles de tâche qui deviennent obsolètes dans votre système. Lorsque vous désactivez un rôle de tâche au lieu de le supprimer, vous pouvez conserver toutes les informations historiques qui lui sont associées.

Vous pouvez également réactiver les rôles de tâche précédemment désactivés.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront]*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès administratif aux rôles de tâche</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Impact de la désactivation des rôles de tâche

Si vous désactivez un rôle de tâche, il ne s’affiche plus dans les zones suivantes :

* Champ de type [!UICONTROL  Affectations] (pour les tâches, les tâches de modèle, les problèmes, les approbations et les règles de routage)
* Champs [!UICONTROL Affectations] dans les listes et les rapports
* Profils d’utilisateur

  >[!NOTE]
  >
  >Lorsque vous ajoutez un nouveau rôle à un utilisateur, un rôle de tâche désactivée ne s’affiche pas. Cependant, il continue à s’afficher dans les champs [!UICONTROL Rôle Principal] et [!UICONTROL Autres rôles] si l’utilisateur était associé au rôle de tâche avant qu’il ne soit désactivé.

* Boîte de dialogue [!UICONTROL Partage] pour les objets, y compris l’affectation de modèle de mise en page
* Champs de saisie anticipée dans les formulaires personnalisés
* Le champ [!UICONTROL Pool Members] dans les [!UICONTROL  pools de ressources]
* Le champ [!UICONTROL Rôle de tâche] d’un écran de modification [!UICONTROL Taux de facturation] lorsqu’un utilisateur remplace les taux de facturation des projets
* Boîte de dialogue [!UICONTROL Ajouter une affectation à la carte Kanban] dans un projet
* Le champ [!UICONTROL Rôle de tâche] d’un plan ou d’une initiative lorsqu’une personne utilise [!DNL Adobe Workfront Scenario Planner].

  [!DNL Scenario Planner] est disponible uniquement dans la nouvelle expérience [!DNL Adobe Workfront] et nécessite une licence supplémentaire. Pour plus d’informations sur [!DNL Workfront Scenario Planner], voir [The [!DNL Scenario Planner] overview](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Les rôles désactivés s’affichent toujours dans les filtres des listes, des rapports et d’autres outils tels que l’ [!UICONTROL équilibreur de charge de travail].

## Observations avant la désactivation d’un rôle de tâche

Il est préférable de désactiver plutôt que de supprimer les rôles de tâche devenus obsolètes afin de conserver toutes les informations historiques associées aux rôles que vous avez peut-être utilisés dans le passé.

>[!NOTE]
>
>Les tâches affectées au rôle de tâche avant la désactivation restent affectées.

Nous vous recommandons d’effectuer les opérations suivantes avant de désactiver un rôle de tâche inutilisé :

* Créez des rapports pour tous les objets affectés au rôle que vous prévoyez de désactiver et de les réaffecter à un rôle de tâche actif. Pour plus d’informations sur la création de rapports, voir [Création d’un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

  >[!TIP]
  >
  >Vous pouvez créer un rapport afin de filtrer les tâches ou les problèmes pour lesquels le rôle désactivé est affecté. Utilisez ensuite le rapport pour réaffecter les tâches ou problèmes en suspens à un rôle actif.

* Faites l’inventaire de tous les processus d’approbation, chemins d’approbation actuels et règles de routage ou autres objets affectés au rôle de tâche que vous prévoyez de désactiver et de les réaffecter à un rôle actif.

  >[!TIP]
  >
  >Lors de l’utilisation des files d’attente de requête, si vous désactivez un rôle de tâche attribué comme cessionnaire par défaut dans une règle de routage, le rôle est conservé et les demandes sont toujours acheminées vers le rôle désactivé. Nous vous recommandons de mettre à jour les règles de routage avec les rôles actifs avant de désactiver l’équipe.

  Pour plus d’informations sur la création de processus de validation et de règles de routage, voir les articles suivants :

   * [Créer un processus d’approbation pour les tâches](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Créer des règles de routage](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Désactivation d’un rôle de tâche

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur &#x200B; **[!UICONTROL Rôles de tâche].**
1. (Facultatif) Dans le menu déroulant **[!UICONTROL Filtre]**, sélectionnez **[!UICONTROL Actif]** pour afficher uniquement les rôles de tâche actifs.
1. Cliquez sur le nom du rôle de tâche à désactiver.
1. Dans le menu déroulant **[!UICONTROL Est actif]**, sélectionnez **[!UICONTROL Non]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   Le rôle de tâche est désactivé et ne peut plus être attribué au travail, associé aux modèles de mise en page, etc. Pour plus d’informations sur toutes les utilisations des rôles de tâche dans [!DNL Workfront], voir [Présentation des rôles de tâche](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
