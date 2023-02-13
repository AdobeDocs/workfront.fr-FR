---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Affectez manuellement des tâches et des problèmes non attribués dans les zones Planification .
description: À l’aide de la chronologie de planification, vous pouvez gérer les affectations d’utilisateurs, en plus de spécifier le temps alloué à chaque utilisateur pour une tâche.
author: Alina
feature: Resource Management
exl-id: 627e4442-767a-41a2-9700-76f2ad2dc9cf
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Affectez manuellement des tâches et des problèmes non attribués dans les zones Planification .

>[!IMPORTANT]
>  
><span class="preview">La fonctionnalité de planification décrite dans cet article a été abandonnée et supprimée d’Adobe Workfront à compter de la version 23.1 de janvier 2023.   </span>
>  
> <span class="preview"> Cet article sera également supprimé peu de temps après la version 23.1, début 2023. Pour l’instant, nous vous recommandons de mettre à jour les signets en conséquence. </span>
> 
><span class="preview"> Vous pouvez désormais utiliser l’équilibreur de charge de travail pour planifier le travail de vos ressources. </span>
>  
> <span class="preview">Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir la section [L’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

À l’aide de la chronologie de planification, vous pouvez gérer les affectations d’utilisateurs, en plus de spécifier le temps alloué à chaque utilisateur pour une tâche.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Travail ou plus élevé</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Niveau d’accès*</td> 
   <td> <p>Affichage ou accès supérieur à Projets, tâches et problèmes</p> <p><b>NOTE</b>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Contribution des autorisations aux projets, tâches et problèmes</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables avant d’affecter des tâches et des problèmes dans la chronologie de planification

Avant de commencer à gérer les affectations d’utilisateurs comme décrit dans cette section, familiarisez-vous avec le fonctionnement de la planification des ressources dans Workfront, comme décrit dans la section [Prise en main de la planification des ressources](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Pour gérer correctement les affectations d’utilisateurs comme décrit dans cette section, vous devez d’abord vous assurer que vous, vos projets, ainsi que vos tâches et problèmes, remplissez les conditions préalables décrites dans la section [Conditions préalables à l’utilisation des outils de planification dans Workfront](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#prerequisites) dans l’article [Prise en main de la planification des ressources](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Les sections suivantes décrivent comment modifier les affectations d’utilisateurs manuellement, automatiquement ou en permutant les affectations par utilisateur ou rôle.

## Affectez manuellement aux utilisateurs des tâches ou des problèmes non attribués

La chronologie de planification fournit la visibilité nécessaire sur laquelle les utilisateurs sont capables d’exécuter la tâche ou le problème.\
Pour plus d’informations sur la planification de la chronologie, voir [Prise en main de la planification des ressources](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Vous pouvez affecter des tâches et des problèmes individuels aux utilisateurs de la chronologie de planification à partir des zones suivantes de Workfront :

* La section Planification sous Ressources (lors de la planification des ressources pour plusieurs projets).
* La section Planification sous un projet (lors de la planification de ressources pour un seul projet).
* La section Planifier sous une équipe (lors de la planification des ressources pour une équipe).

Les informations affichées dans la zone Non affecté en haut de la chronologie de la planification varient en fonction de la zone de Workfront dans laquelle vous utilisez la planification des ressources (soit dans la section Planification (lors de la planification des ressources pour plusieurs projets), la section Planification (lors de la planification des ressources pour un seul projet), soit dans la section Planification (lors de la planification des ressources pour une équipe). Pour plus d’informations, voir la section [Fonctionnalités disponibles dans la zone Planification](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md#functionality-available-in-the-scheduling-area) dans l’article [Présentation des zones de planification](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

En fonction de la zone de Workfront dans laquelle vous visualisez la chronologie de la planification, seuls certains utilisateurs peuvent être éligibles à un travail. Pour plus d’informations, voir [Présentation des zones de planification](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

Pour affecter des tâches ou des problèmes non attribués aux utilisateurs dans la chronologie de planification :

1. Accédez à la chronologie de planification pour plusieurs projets, pour un projet individuel ou pour une équipe :

   * **Pour plusieurs projets**:  Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, cliquez sur **Ressource > Équilibreur de charge de travail**, puis sélectionnez **Planification** dans le menu déroulant supérieur gauche.
   * **Pour un projet individuel**: Accédez à un projet, cliquez sur le bouton **Équilibreur de charge de travail** dans le panneau de gauche, puis sélectionnez **Planification** dans le menu déroulant supérieur gauche.
   * **Pour une équipe**: Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, puis cliquez sur **Équipes**, sélectionnez une équipe, puis cliquez sur **Équilibreur de charge de travail** dans le panneau de gauche, puis sélectionnez **Planification** dans le menu déroulant supérieur gauche.

   ![schedule_contours.png](assets/scheduling-contours-350x139.png)

1. (Facultatif) Créez un filtre pour personnaliser le contenu affiché dans la chronologie de planification, comme décrit dans la section [Filtrage des informations dans la zone Planification](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) . [Filtrage des informations dans la zone Planification](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md). Par exemple, pour les problèmes à afficher dans la chronologie de la planification, vous devez créer un filtre.

1. (Facultatif) Modifiez la plage de dates affichée dans la chronologie de planification, comme décrit dans la section [Ajuster la plage de dates des zones de planification](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [Prise en main de la planification des ressources](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

1. Procédez comme suit pour affecter une tâche ou un problème non assigné :

   * Faites glisser la tâche ou le problème sur la ligne de l’utilisateur que vous souhaitez affecter.\
      Un maximum de 10 tâches par jour s’affiche pour un utilisateur donné. Vous pouvez développer la liste pour afficher toutes les tâches actuellement affectées à cet utilisateur. (Après avoir effectué des affectations dans la chronologie de planification, plus de 10 tâches peuvent être temporairement affichées.)\
      Lorsque vous faites glisser un élément, les informations suivantes s’affichent avant de publier la tâche ou le problème et de terminer l’affectation :

   * Si les affectations utilisateur sont activées dans la chronologie de planification, les indicateurs de suraffectation rouges s’affichent si l’exécution de l’affectation entraîne la surallocation de l’utilisateur.\
      Pour plus d’informations sur les indicateurs de surallocation, voir la section [Indicateurs d’affectation](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators) dans l’article [Gestion des affectations d’utilisateurs dans les zones de planification](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

      Si la variable **Limiter les affectations aux utilisateurs ayant un rôle correspondant** est activée dans la zone Paramètres , les utilisateurs qui ne sont pas éligibles pour recevoir l’affectation sont grisés. Si cette option est désactivée, tous les utilisateurs peuvent recevoir l’affectation. L’option est activée par défaut.\
      Pour plus d’informations sur cette option, voir [](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md#allowing-assignmennts-to-users-regardless-of-role) in [Autorisation des affectations d’utilisateurs, quel que soit le rôle et l’appartenance à un groupe dans les zones de planification](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md)

      Un indicateur de dépôt s’affiche sur la ligne de l’utilisateur. Cela vous permet de voir où un élément est affecté avant d’effectuer l’affectation.

      Développez la tâche ou le problème que vous souhaitez affecter, cliquez sur la flèche de liste déroulante dans le **Affectations** , commencez à saisir le nom de l’utilisateur à affecter, puis cliquez sur son nom dans la liste déroulante.\
      ![schedule_task_expand.png](assets/schedule-task-expanded-350x170.png)

1. (Conditionnel) Après avoir affecté une tâche ou un problème non assigné à un utilisateur, vous pouvez modifier les affectations existantes pour les tâches et les problèmes parmi les utilisateurs de la chronologie de planification. Lors de la planification de ressources pour des projets (dans l’onglet Planification ou l’onglet Personnel ), seuls les utilisateurs qui ont le même rôle de tâche peuvent recevoir l’affectation.\
   Pour réaffecter une tâche ou un problème à un autre utilisateur, faites glisser la tâche de la ligne d’un utilisateur vers la ligne d’un autre utilisateur.
1. (Facultatif) Configurez le nombre d’heures pendant lesquelles chaque utilisateur affecté est affecté à la tâche ou au problème, comme décrit dans la section [Gestion des affectations d’utilisateurs dans les zones de planification](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md) .
