---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Désactiver les fonctions
description: En tant qu’administrateur et administratrice d’ [!DNL Adobe Workfront]  ou utilisateur et utilisatrice disposant d’un accès administratif aux fonctions, vous pouvez désactiver les fonctions qui deviennent obsolètes dans votre système. Lorsque vous désactivez une fonction au lieu de la supprimer, vous pouvez conserver toutes les informations historiques qui lui sont associées.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 934cef1a-8157-45db-b000-24a08a94dd18
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 98%

---

# Désactiver des fonctions

En tant qu’administrateur et administratrice d’[!DNL Adobe Workfront] ou utilisateur et utilisatrice disposant d’un accès administratif aux fonctions, vous pouvez désactiver les fonctions qui deviennent obsolètes dans votre système. Lorsque vous désactivez une fonction au lieu de la supprimer, vous pouvez conserver toutes les informations historiques qui lui sont associées.

Vous pouvez également réactiver les fonctions précédemment désactivées.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Tous </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>
   <p>Nouvelle : [!UICONTROL Standard]</p>
   <p>Ou</p>
   <p>Actuelle : [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Accès administratif aux fonctions</td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

  Le [!DNL Scenario Planner] n’est disponible que dans la nouvelle expérience d’[!DNL Adobe Workfront] et nécessite une licence supplémentaire. Pour plus d’informations sur le [!DNL Workfront Scenario Planner], voir [Vue d’ensemble du  [!DNL Scenario Planner] &#x200B;](../../../scenario-planner/scenario-planner-overview.md).

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

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **[!UICONTROL Fonctions].**
1. (Facultatif) Dans le menu déroulant **[!UICONTROL Filtrer]**, sélectionnez **[!UICONTROL Actif]** pour afficher uniquement les fonctions actives.
1. Cliquez sur le nom de la fonction à désactiver.
1. Dans le menu déroulant **[!UICONTROL Est actif]**, sélectionnez **[!UICONTROL Non]**.

   ![Désactiver la fonction](assets/deactivate-job-role-edit-role-box-nwe.png)

1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

   La fonction est désactivée et ne peut plus être attribuée au travail, associée aux modèles de disposition, etc. Pour plus d’informations sur toutes les utilisations des fonctions dans [!DNL Workfront], voir [Vue d’ensemble des fonctions](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).
