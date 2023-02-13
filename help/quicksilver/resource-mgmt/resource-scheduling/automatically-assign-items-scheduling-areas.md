---
product-area: resource-management
navigation-topic: resource-scheduling
title: Affecter automatiquement des tâches et des problèmes non attribués dans les zones Planification
description: Lorsque vous utilisez les outils de planification, vous pouvez permettre à Adobe Workfront d’analyser les affectations de travail actuelles parmi vos utilisateurs disponibles et de proposer des affectations logiques et intelligentes pour toutes les tâches ou problèmes qui ne sont pas encore affectés. Vous pouvez modifier toutes les affectations proposées avant de les finaliser.
author: Alina
feature: Resource Management
exl-id: 087fe3ef-9b85-491b-9fdc-436a01822ede
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 0%

---

# Affecter automatiquement des tâches et des problèmes non attribués dans les zones Planification

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Lorsque vous utilisez les outils de planification, vous pouvez permettre à Adobe Workfront d’analyser les affectations de travail actuelles parmi vos utilisateurs disponibles et de proposer des affectations logiques et intelligentes pour toutes les tâches ou problèmes qui ne sont pas encore affectés. Vous pouvez modifier toutes les affectations proposées avant de les finaliser.

Workfront examine les tâches et les problèmes disponibles dans la zone Non affecté de la période actuellement sélectionnée et propose des affectations pour chaque élément à la fois. Vous pouvez créer un filtre pour limiter le nombre d’éléments disponibles dans la zone Non affecté .

Votre administrateur système détermine la manière dont Workfront calcule la disponibilité des ressources au niveau du système (en tenant compte des heures ainsi que de la disponibilité de l’éditeur de texte enrichi). Selon ce paramètre à l’échelle du système, la disponibilité de la ressource est calculée en utilisant le planning par défaut ou le planning de l’utilisateur. Pour plus d’informations, voir [Configuration de la manière dont Workfront calcule l’heure de la ressource et la disponibilité de l’éditeur de texte enrichi pour la zone de planification](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td> <p>Affichage ou accès supérieur à Projets, tâches et problèmes</p> <p><strong>NOTE</strong>

Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Attribuez des autorisations ou des autorisations supérieures aux projets, tâches et problèmes pour lesquels vous mettez à jour les affectations.</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables {#prerequisites}

Workfront utilise un algorithme propriétaire pour déterminer les propositions d’attribution. Pour optimiser les résultats, assurez-vous que les informations suivantes sont exactes dans Workfront :

* Tâche et informations sur les problèmes, notamment :

   * Affectations de rôles\
      Aucune proposition n’est faite pour les tâches et les problèmes qui ne sont pas affectés à un rôle.
   * Heures prévues\
      Si une tâche ou un problème ne comporte actuellement aucune heure planifiée, Workfront suppose 4 heures planifiées par jour de travail lors de l’affectation automatique du travail. Ces heures ne sont pas automatiquement affectées à l’élément de travail ; elles ne sont utilisées que pour garantir des distributions d’affectation plus réalistes.
   * Dates de début planifiées et dates de fin planifiées

* Informations sur l’utilisateur, notamment :

   * Affectations de rôles Principal et secondaires sur le profil utilisateur
   * Informations sur l’équipe de projet

## Configuration des limites de rôle

Les limites de rôle contrôlent le nombre d’utilisateurs, avec un rôle spécifique, qui peuvent se voir attribuer du travail automatiquement. Les limites de rôle fonctionnent par projet pour garantir que les tâches basées sur les rôles ne sont pas réparties entre un grand nombre d’utilisateurs.

Les scénarios suivants décrivent comment les limites de rôle s’appliquent aux projets :

* **Scénario 1**: Si aucun utilisateur n’est affecté à l’équipe de projet, le système utilise la limite de rôles pour affecter des tâches.\
   Par exemple, vous avez un projet auquel aucun utilisateur n’est affecté à l’équipe du projet. Ce projet comporte 10 tâches de gestion de projet qui doivent être affectées et vous avez défini une limite de rôle de 1 pour le rôle de chef de projet. Le système attribue les 10 tâches à 1 chef de projet, car la limite de rôle est définie sur 1.

* **Scénario 2**: Si la limite de rôle est supérieure au nombre d’utilisateurs affectés à l’équipe de projet, des tâches sont affectées à d’autres utilisateurs.\
   Par exemple, un projet avec un auteur est assigné à l’équipe de projet. Ce projet comporte 12 tâches de rédaction qui doivent être affectées et vous avez une limite de rôle de 2 définie pour le rôle d’auteur. Le système attribue les 12 tâches entre l’auteur de l’équipe de projet et un auteur supplémentaire, car la limite de rôle est définie sur 2.

* **Scénario 3**: Si la limite de rôle est inférieure au nombre d’utilisateurs affectés à l’équipe de projet, elle est remplacée.\
   Par exemple, vous avez un projet auquel 4 concepteurs sont affectés à l’équipe de projet. Ce projet comporte 8 tâches de concepteur qui doivent être affectées et vous avez défini une limite de rôle de 2 pour le rôle de concepteur. Le système attribue les 8 tâches entre chacun des quatre concepteurs de l’équipe de projet, même si la limite de rôle est définie sur 2.

Pour définir des limites pour les affectations de rôles de tâche :

1. Accédez à la chronologie de planification pour plusieurs projets ou pour un projet individuel :

   * **Pour plusieurs projets**:  Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, cliquez sur **Ressource > Équilibreur de charge de travail**, puis sélectionnez **Planification** dans le menu déroulant supérieur gauche.
   * **Pour un projet individuel**: Accédez à un projet, cliquez sur le bouton **Équilibreur de charge de travail** dans le panneau de gauche, puis sélectionnez **Planification** dans le menu déroulant supérieur gauche.

1. Cliquez sur le bouton **Paramètres** icône .\
   ![Automode_settings.png](assets/automode-settings.png)

1. Dans la section Planification automatisée des ressources , cliquez sur dans le **Limite** en ligne avec l’élément dans la variable **Rôle** et saisissez un nombre positif.\
   Workfront enregistre automatiquement vos modifications.

   >[!NOTE]
   >
   >Tous les membres actuels de l’équipe de projet sont automatiquement éligibles pour tous les travaux recommandés, quelle que soit la limite de rôle définie.

   ![Set_Role_Limits.png](assets/set-role-limits-350x341.png)

1. (Facultatif) Cliquez sur le **Affichage** dans la partie supérieure de la colonne Limiter et sélectionnez les options d’affichage de votre choix.
1. Pour revenir à la zone de planification des ressources, cliquez sur **Revenir à la planification**.

## Affecter automatiquement des tâches et des problèmes

Vous pouvez affecter des tâches et des problèmes aux utilisateurs dans la chronologie de planification, que vous vous trouviez dans l’onglet Planification (lors de la planification de ressources pour plusieurs projets) ou dans l’onglet Personnel (lors de la planification de ressources pour un projet individuel).

Pour permettre à Workfront de proposer automatiquement des affectations pour les tâches et les problèmes dans la zone Non affecté :

1. Accédez à la chronologie de planification pour plusieurs projets ou pour un projet individuel :

   * **Pour plusieurs projets**:  Cliquez sur le bouton **Menu Principal** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de Workfront, cliquez sur **Ressource > Équilibreur de charge de travail**, puis sélectionnez **Planification** dans le menu déroulant supérieur gauche.
   * **Pour un projet individuel**: Accédez à un projet, cliquez sur le bouton **Équilibreur de charge de travail** dans le panneau de gauche, puis sélectionnez **Planification** dans le menu déroulant supérieur gauche.

1. (Facultatif) Créez un filtre pour personnaliser le contenu affiché dans la zone Non affecté de la chronologie de planification.\
   Pour plus d’informations sur la création d’un filtre, voir [Filtrage des informations dans la zone Planification](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md#creating-and-modifying-filters-on-the-scheduling-tab-for-projects) in [Filtrage des informations dans la zone Planification](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) [Filtrage des informations dans la zone Planification](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md)

   >[!TIP]
   >
   >Pour vous assurer que Workfront affecte du travail aux utilisateurs les plus éligibles :
   >
   >* Filtrez uniquement les informations qui affectent les tâches affichées dans la zone Non affecté (par exemple, Portfolios, Programmes et Projets).
   >* Nous vous recommandons de ne pas filtrer les informations qui affectent les utilisateurs disponibles à affecter dans la chronologie de planification. Cela limite Workfront à l’affichage de toutes les personnes désignées potentielles, ce qui peut entraîner des affectations moins satisfaisantes.


1. (Facultatif) Modifiez la plage de dates affichée dans la chronologie de planification, comme décrit dans la section [Ajuster la plage de dates des zones de planification](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [Prise en main de la planification des ressources](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md). Workfront effectue des affectations uniquement pour les tâches et les problèmes au cours de la période visible dans la chronologie de planification.

1. Cliquez sur le bouton **Auto** dans le coin supérieur droit de la chronologie de planification.\
   ![schedule_auto.png](assets/scheduling-auto-350x221.png)\
   Workfront propose des affectations pour chaque tâche ou problème dans **Non attribué** zone.

   >[!TIP]
   >
   >Les tâches et les problèmes doivent déjà être affectés à un rôle pour qu’une affectation soit proposée. Pour optimiser les résultats, les tâches et les problèmes doivent contenir les informations décrites dans la section [Conditions préalables](#prerequisites).

   Les affectations proposées se différencient par un contour en pointillés autour de chaque tâche ou problème, comme suit :\
   **Assignation de la tâche proposée :**

   **Affectation de tâche existante :**

1. (Facultatif) Vous pouvez modifier les affectations proposées ou existantes avant de finaliser les affectations :

   >[!NOTE]
   >
   >Si vous modifiez une affectation existante, elle passe à l’état proposé.

   * Pour affecter un élément à un autre utilisateur :

      * Faites glisser la tâche ou le problème de l’utilisateur proposé vers la ligne d’un autre utilisateur que vous souhaitez affecter.

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE: lists in this article need to be reformatted and maybe split - too many levels in)      
        </MadCap:conditionalText>      
        -->

         Un maximum de 10 tâches par jour s’affiche pour un utilisateur donné. Vous pouvez développer la liste pour afficher toutes les tâches actuellement affectées à cet utilisateur. (Après avoir effectué des affectations dans la chronologie de planification, plus de 10 tâches peuvent être temporairement affichées.)\
         Lorsque vous faites glisser un élément, les informations suivantes s’affichent avant de publier la tâche ou le problème et de terminer l’affectation :

         * Un indicateur de dépôt s’affiche dans la ligne de l’utilisateur. Cela vous permet de voir où un élément est affecté avant d’effectuer l’affectation.
         * Si les affectations de l’utilisateur sont activées dans la chronologie de planification, les indicateurs de suraffectation rouges s’affichent si l’exécution de l’affectation entraîne une surallocation de l’utilisateur.\
            Pour plus d’informations sur les indicateurs de suraffectation, voir [Indicateurs d’affectation](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators).

         * Les utilisateurs qui ne peuvent pas recevoir l’affectation sont grisés.
      * Développez la tâche ou le problème que vous souhaitez affecter, cliquez sur la flèche de liste déroulante dans le **Affectations** , commencez à saisir le nom de l’utilisateur à affecter, puis cliquez sur son nom dans la liste déroulante.\
         ![schedule_task_expand.png](assets/schedule-task-expanded-350x170.png)
   * Pour reporter l’attribution, faites glisser une tâche ou un problème que vous n’êtes pas encore prêt à réaffecter à la fonction **Non attribué** zone.



1. Cliquez sur le bouton **Effectuer des affectations** en haut de la chronologie de planification pour finaliser les affectations proposées.\
   Ou\
   Cliquez sur **Annuler** pour renvoyer toutes les affectations proposées à leurs anciens postes.
