---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Désactiver des fonctions
description: En tant qu’administrateur et administratrice d’ [!DNL Adobe Workfront]  ou utilisateur et utilisatrice disposant d’un accès administratif aux fonctions, vous pouvez désactiver les fonctions qui deviennent obsolètes dans votre système. Lorsque vous désactivez une fonction au lieu de la supprimer, vous pouvez conserver toutes les informations historiques qui lui sont associées.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 100%

---

# Désactiver des fonctions

En tant qu’administrateur et administratrice d’[!DNL Adobe Workfront] ou utilisateur et utilisatrice disposant d’un accès administratif aux fonctions, vous pouvez désactiver les fonctions qui deviennent obsolètes dans votre système. Lorsque vous désactivez une fonction au lieu de la supprimer, vous pouvez conserver toutes les informations historiques qui lui sont associées.

Vous pouvez également réactiver les fonctions précédemment désactivées.

## Conditions d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan [!UICONTROL Adobe Workfront]*</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence [!UICONTROL Adobe Workfront]*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Accès administratif aux fonctions</p> <p><b>NOTE</b> : si votre accès n’est toujours pas activé, demandez à votre administrateur ou à votre administratrice [!DNL Workfront] si des restrictions supplémentaires au niveau de votre accès ont été définies. Pour plus d’informations sur la manière dont une équipe d’administration [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Impact de la désactivation des fonctions

Si vous désactivez une fonction, elle ne s’affiche plus dans les zones suivantes :

* Le champ de saisie semi-automatique [!UICONTROL Affectations] (pour les tâches, les tâches de modèle, les problèmes, les approbations et les règles de routage)
* Les champs [!UICONTROL Affectations] dans les listes et les rapports
* Profils d’utilisateur et d’utilisatrice

  >[!NOTE]
  >
  >Lorsque vous ajoutez un nouveau rôle à une personne, les fonctions désactivées ne s’affichent pas. Mais elles continuent de s’afficher dans les champs [!UICONTROL Rôle principal] et [!UICONTROL Autres rôles], si la personne était associée à ces fonctions avant leur désactivation

* La boîte de dialogue [!UICONTROL Partage] pour les objets, y compris l’attribution du modèle de mise en page
* Champs de saisie semi-automatique dans les formulaires personnalisés
* La variable [!UICONTROL Membres du pool] champ dans [!UICONTROL Pools de ressources]
* Le champ [!UICONTROL Fonction] d’un écran de modification [!UICONTROL Taux de facturation] lorsqu’une personne remplace les taux de facturation des projets
* La boîte de dialogue [!UICONTROL Ajouter une affectation au panorama Kanban] d’un projet
* Le champ [!UICONTROL Fonction] d’un plan ou d’une initiative lorsqu’une personne utilise [!DNL Adobe Workfront Scenario Planner]

  Le [!DNL Scenario Planner] n’est disponible que dans la nouvelle expérience d’[!DNL Adobe Workfront] et nécessite une licence supplémentaire. Pour plus d’informations sur le [!DNL Workfront Scenario Planner], voir [Vue d’ensemble du  [!DNL Scenario Planner] ](../../../scenario-planner/scenario-planner-overview.md).

>[!TIP]
>
>Les rôles désactivés s’affichent toujours dans les filtres des listes, des rapports et d’autres outils tels que l’[!UICONTROL Équilibreur de charge de travail].

## Éléments à prendre en compte avant la désactivation d’une fonction

Il est préférable de désactiver plutôt que de supprimer les fonctions devenues obsolètes afin de conserver toutes les informations historiques associées aux rôles que vous avez peut-être utilisés dans le passé.

>[!NOTE]
>
>Les travaux affectés à la fonction avant la désactivation restent affectées.

Nous vous recommandons d’effectuer les opérations suivantes avant de désactiver une fonction inutilisée :

* Créez des rapports pour tous les objets affectés au rôle que vous prévoyez de désactiver et réaffectez-les à une fonction active. Pour plus d’informations sur la création de rapports, voir [Créer un rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

  >[!TIP]
  >
  >Vous pouvez créer un rapport afin de filtrer les tâches ou les problèmes pour lesquels le rôle désactivé est affecté. Utilisez ensuite le rapport pour réaffecter les tâches ou problèmes en suspens à un rôle actif.

* Faites l’inventaire de tous les processus d’approbation, parcours d’approbation actuels et règles de routage ou autres objets affectés à la fonction que vous prévoyez de désactiver et réaffectez-les à un rôle actif.

  >[!TIP]
  >
  >Lors de l’utilisation des files d’attente des demandes, si vous désactivez une fonction attribuée comme cessionnaire par défaut dans une règle de routage, le rôle est conservé et les demandes sont toujours acheminées vers le rôle désactivé. Nous vous recommandons de mettre à jour les règles de routage avec les rôles actifs avant de désactiver l’équipe.

  Pour plus d’informations sur la création de processus de validation et de règles de routage, voir les articles suivants :

   * [Créer un processus d’approbation pour les éléments de travail](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)
   * [Créer des règles de routage](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)

## Désactiver une fonction

1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Fonctions].**
1. (Facultatif) Dans le menu déroulant **[!UICONTROL Filtrer]**, sélectionnez **[!UICONTROL Actif]** pour afficher uniquement les fonctions actives.
1. Cliquez sur le nom de la fonction à désactiver.
1. Dans le menu déroulant **[!UICONTROL Est actif]**, sélectionnez **[!UICONTROL Non]**.

   ![](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   La fonction est désactivée et ne peut plus être attribuée au travail, associée aux modèles de disposition, etc. Pour plus d’informations sur toutes les utilisations des fonctions dans [!DNL Workfront], voir [Vue d’ensemble des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
