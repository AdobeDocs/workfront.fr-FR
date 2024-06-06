---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Gérer les affectations des utilisateurs et utilisatrices dans l’équilibreur de charge de travail
description: En tant que gestionnaire de ressources, vous pouvez affecter du travail aux utilisateurs et gérer leurs allocations quotidiennes, hebdomadaires ou mensuelles à partir de l’équilibreur de charge de travail.
author: Lisa
feature: Resource Management
exl-id: 9649e482-af24-4516-9a69-ef12b2f1d579
source-git-commit: 1ce89f7e680f11a11c8646853652f9f24ee89b14
workflow-type: tm+mt
source-wordcount: '2887'
ht-degree: 1%

---

# Gérer les affectations des utilisateurs et utilisatrices dans l’équilibreur de charge de travail

<!-- Audited: 01/2024 -->

{{highlighted-preview}}

En tant que gestionnaire de ressources, vous pouvez affecter du travail aux utilisateurs et gérer leurs allocations quotidiennes, hebdomadaires ou mensuelles à partir de l’équilibreur de charge de travail afin de vous assurer qu’un nombre d’heures adapté à leurs plannings disponibles leur est alloué.

## Conditions d’accès {#access-requirements}

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td> <p>N’importe quelle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>
   <p>Lors de l’utilisation de l’équilibreur de charge de travail dans la zone Ressource , vous avez besoin des éléments suivants :</p>
   <p>Nouveau : Standard</p>
   <p>Ou</p>
   <p>Actuel : formule</p>
   <p>Lorsque vous utilisez l’équilibreur de charge de travail d’une équipe ou d’un projet, vous avez besoin des éléments suivants :</p>
   <p>Nouveau : Standard</p>
   <p>Ou</p>
   <p>Actuel : travail</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuration du niveau d’accès</td> 
   <td> <p>Modifiez l’accès aux éléments suivants :</p> 
    <ul> 
     <li> <p>Gestion des ressources</p> </li> 
     <li> <p>Projets</p> </li> 
     <li> <p>Tâches</p> </li> 
     <li> <p>Problèmes</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Contribuez à des autorisations ou des autorisations supérieures qui incluent l’attribution aux tâches et problèmes pour lesquels vous souhaitez gérer les affectations. </p> <p>Ou </p> <p>Gérez les autorisations pour les tâches pour lesquelles vous souhaitez mettre à jour les Heures planifiées, en plus de mettre à jour les affectations. Pour plus d’informations sur la mise à jour des heures planifiées dans l’équilibreur de charge de travail, voir la section <a href="#update-task-planned-hours-when-managing-user-allocations">Mettre à jour les heures planifiées de la tâche lors de la gestion des affectations utilisateur</a> dans cet article.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Présentation des affectations utilisateur

Les affectations utilisateur sont des quantités d’heures qui indiquent le temps qu’un utilisateur doit consacrer à un jour, un jour de semaine, une semaine ou un mois donné pour terminer l’élément de travail. Elles sont incluses dans les heures planifiées de l’élément de travail.

Cet article décrit comment mettre à jour les affectations horaires quotidiennes, hebdomadaires ou mensuelles pour les utilisateurs affectés à des tâches ou des problèmes. Pour plus d’informations sur la gestion des affectations globales pour les utilisateurs et les rôles de tâche pour les tâches, voir [Gestion des heures d’affectation des utilisateurs et des rôles pour les tâches](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md).

### Présentation de l’affectation des utilisateurs {#user-allocation-overview}

Vous pouvez afficher l’affectation des utilisateurs sous forme d’heures ou de pourcentage dans l’équilibreur de charge de travail. Vous pouvez ajuster les heures ou les pourcentages.

Les affectations d’utilisateurs sont incluses dans le nombre d’heures planifiées d’un élément de travail. Pour plus d’informations sur les heures planifiées, voir [Présentation des heures planifiées](../../manage-work/tasks/task-information/planned-hours.md).

La tâche Heures planifiées est répartie uniformément entre tous les jours compris dans la Durée de la tâche pour l’utilisateur affecté à la tâche. Par exemple, si une tâche a une durée de 5 jours et un total de 10 heures planifiées, le nombre d’affectations quotidiennes de la tâche est de 2 heures. L’allocation hebdomadaire est de 10 heures. Cela signifie qu’un utilisateur est affecté à la tâche pendant 2 heures par jour. Vous pouvez toutefois modifier manuellement l’allocation quotidienne de l’utilisateur à l’aide de l’équilibreur de charge de travail.

>[!CAUTION]
>
>L’équilibreur de charge de travail affiche uniquement 1 000 heures planifiées par élément de travail et jusqu’à 1 000 jours de la durée d’un élément. Les affectations dans l’équilibreur de charge de travail s’affichent sous la forme de zéro après la limite de 1 000 heures ou de 1 000 jours. Nous vous recommandons de diviser les tâches en sous-tâches plus petites afin de tenir compte d’un plus grand nombre d’heures planifiées ou d’une durée supérieure à 1 000 jours.

Tenez compte des points suivants lorsque vous localisez des allocations quotidiennes, hebdomadaires ou mensuelles pour des tâches ou des problèmes dans l’équilibreur de charge de travail :

* Vous pouvez afficher les allocations quotidiennes, hebdomadaires et mensuelles des utilisateurs à leurs tâches. Activez la vue Semaine ou Mois pour afficher les allocations hebdomadaires ou mensuelles.
* Vous pouvez utiliser l’équilibreur de charge de travail pour modifier l’allocation quotidienne, hebdomadaire ou mensuelle des utilisateurs aux tâches ou problèmes. Pour plus d’informations sur l’ajustement de l’affichage de l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  >[!NOTE]
  >
  >Nous vous recommandons de choisir la période (quotidienne, hebdomadaire ou mensuelle) que vous souhaitez toujours utiliser lors de la gestion des affectations utilisateur et de ne pas basculer entre ces périodes pour les mêmes tâches. La mise à jour des allocations hebdomadaires pour le même utilisateur pour lequel vous avez précédemment mis à jour les allocations quotidiennes modifie l’allocation quotidienne pour l’utilisateur.

* Vous pouvez mettre à jour les allocations pour les jours ouvrés et non ouvrés.
* Les horodatages des dates de début et de fin planifiées des tâches, ainsi que le planning du projet, sont importants lorsque Workfront calcule automatiquement l’allocation quotidienne de la tâche.

  >[!INFO]
  >
  > Par exemple, une tâche peut avoir une durée de 2 jours et 2 heures planifiées et une heure de début planifiée de 12h00 le premier jour de la durée avec un utilisateur et une planification de projet qui se termine à 17h. La capacité de l’utilisateur pour le premier jour est de 5 heures. La capacité de l’utilisateur pour le deuxième jour est de 8 heures (si la planification commence à 9 heures).
  >
  >Workfront calcule l&#39;allocation des 2 heures sur les 2 jours de la durée à l&#39;aide de la formule suivante :
  >
  >`Daily allocation hours = (Total Planned Hours / Total of available hours) * Daily available hours`
  >
  >Dans notre exemple, les heures d’affectation quotidiennes pour chaque jour sont les suivantes :
  >   
  >(2 / 13) * 5 = 0,77 heures d’affectation pour le premier jour
  >
  >(2 / 13) * 8 = 1,23 heures d’affectation pour le deuxième jour
  >
  >Dans les calculs ci-dessus, 13 est le total des heures disponibles pour la tâche : 5 + 8 = 13

* Deux utilisateurs dans des fuseaux horaires ou des plannings différents de ceux des utilisateurs affectés peuvent faire apparaître les quantités d’allocation différemment à deux utilisateurs affichant les mêmes tâches.

* Lorsqu’un utilisateur a planifié un congé, le jour ou la partie de la journée s’affiche en arrière-plan gris, <span class="preview">et une icône d’avion indique le temps de pause</span>. Si l’administrateur de Workfront a activé le paramètre de désactivation de l’heure de l’utilisateur dans la zone Configuration afin de prendre en compte l’heure de désactivation de l’utilisateur, les heures allouées sont déplacées vers le jour disponible suivant dans la chronologie. Si le paramètre est désactivé, les heures allouées restent le jour désigné pour le congé et l’utilisateur s’affiche comme suralloué. Pour plus d’informations, voir [Configuration des préférences de projet à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!TIP]
  >
  >Si le temps de pause a été marqué après l’affectation de l’utilisateur à une tâche, vous devez recalculer la chronologie du projet pour afficher l’allocation déplacée. Pour plus d’informations, voir [Recalculer les calendriers du projet](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

   * <span class="preview">Lorsque plusieurs utilisateurs sont affectés à une tâche et que le cessionnaire principal a programmé un congé, la chronologie est décalée (si les dates ne sont pas fixes) et les heures planifiées de tous les cessionnaires sont redistribuées sur la nouvelle durée de la tâche. Si la tâche comporte des dates fixes, la chronologie n’est pas modifiée en raison d’un temps de congé et les heures sont réaffectées parmi les jours restants.</span>
   * <span class="preview">Si les affectations sont effectuées manuellement, les heures planifiées ne sont pas redistribuées après le congé.</span>

* Si plusieurs utilisateurs sont affectés à la tâche, le montant des heures planifiées est réparti uniformément entre chaque utilisateur en premier, puis uniformément sur chaque jour au cours de la durée de la tâche. Cette répartition devient l’affectation de chaque utilisateur à la tâche.

  Par exemple, les scénarios suivants peuvent exister :

   * Pour une tâche avec une durée de 2 jours et 10 heures planifiées affectées à un utilisateur, l’allocation quotidienne à l’utilisateur est de 5 heures pour chaque jour par défaut.
   * Pour une tâche avec une durée de 2 jours et 10 heures planifiées affectées à deux utilisateurs, l’allocation quotidienne par défaut à chaque utilisateur est de 2,5 heures pour chaque jour.

* Si une tâche ou un problème s’est terminé avant la date d’achèvement planifiée, le nombre d’heures allouées pour les jours restants est écoulé et ne compte pas dans l’allocation globale de l’utilisateur. Cette option s’affiche uniquement lorsque l’icône Afficher les allocations et le paramètre Afficher les dates prévues sont activés. Pour plus d’informations sur l’activation des paramètres dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  ![Heures affectées traversées](assets/allocations-struck-through-highlighted.png)

* Lorsqu’un utilisateur est surchargé, ses heures allouées s’affichent avec un arrière-plan rouge dans le champ utilisateur.
* Lorsque l’utilisateur est sous-alloué ou alloué un nombre égal d’heures à l’heure disponible planifiée, les heures s’affichent avec un arrière-plan bleu.
* Vous pouvez afficher l’allocation des utilisateurs dans une vue graphique dans la ligne de l’utilisateur. Pour plus d’informations sur l’activation de la vue graphique pour les affectations utilisateur, reportez-vous à la section &quot;Navigation dans l’équilibreur de charge de travail&quot; de l’article . [Navigation dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

  ![Graphique d’affectation des utilisateurs](assets/user-allocation-chart.png)

### Critères qui réinitialisent les attributions d’utilisateurs {#criteria-that-reset-user-allocations}

Toutes les modifications de tâche ne déclenchent pas les affectations modifiées à redistribuer. Cependant, certaines actions peuvent réinitialiser les allocations déjà ajustées de vos ressources et les redistribuer uniformément à tous les jours pendant la durée de l’élément de travail pour chacun des cessionnaires.

>[!NOTE]
>
>Si vous n’avez pas modifié la distribution automatique des allocations sur les éléments de travail, les heures sont redistribuées uniformément entre tous les cessionnaires en cas de changement du nombre de cessionnaires, de la durée d’une tâche ou du montant des heures planifiées sur l’élément de travail.

#### Actions qui réinitialisent les allocations ajustées {#actions-that-reset-adjusted-allocations}

Les actions suivantes réinitialisent ou modifient les allocations quotidiennes, hebdomadaires ou mensuelles pour les utilisateurs après les avoir manuellement ajustées, comme décrit dans la section [Modification des attributions d’utilisateurs](#modify-user-allocations) dans cet article :

* Lorsque vous raccourcissez la durée d’un élément de travail qui raccourcit le nombre de jours dans sa durée, les heures allouées ajustées des jours perdus sont ajoutées au montant d’allocation du dernier jour de l’élément de travail.
* Lorsque vous modifiez le nombre d’heures planifiées sur une affectation ou sur l’élément de travail, le nouveau nombre d’heures planifiées est uniformément redistribué pour toute la durée de l’élément de travail.
* Lorsque vous ajoutez ou supprimez une personne désignée pour un élément de travail, ce qui entraîne la modification des Heures planifiées de la tâche, les valeurs ajustées sont redistribuées uniformément.

#### Actions qui ne réinitialisent pas les allocations ajustées {#actions-that-do-not-reset-adjusted-allocations}

Les modifications suivantes apportées à un élément de travail ne déclenchent pas les affectations ajustées à réinitialiser ou à modifier :

* Lorsque vous déplacez les jours d’un élément de travail mais que le nombre de jours dans la Durée ne change pas, les valeurs allouées ajustées restent identiques et passent aux nouvelles dates.
* Lorsque vous augmentez la durée d’un élément de travail qui augmente le nombre de jours dans sa durée, les heures allouées ajustées restent identiques pour les jours ajustés. Des jours supplémentaires sont ajoutés à la tâche avec 0 heure allouée.
* Lorsque vous ajoutez ou supprimez une personne désignée pour un élément de travail, ce qui n’entraîne pas la modification des Heures planifiées de l’élément, les valeurs ajustées restent les mêmes.

## Localisation des heures planifiées dans l’équilibreur de charge

Vous pouvez modifier les affectations d’utilisateurs à des tâches ou des problèmes à l’aide de l’équilibreur de charge de travail en recherchant les Heures planifiées des tâches ou des problèmes affectés aux utilisateurs.

Tenez compte des points suivants lors de l’affichage des heures planifiées dans l’équilibreur de charge de travail :

* Le nombre total d’heures planifiées pour une tâche ou un problème s’affiche en regard du nom de la tâche ou du problème à gauche de l’équilibreur de charge de travail.

* Le total des heures planifiées d’un projet s’affiche en regard du nom du projet à gauche de l’équilibreur de charge de travail. Ceci représente le total des heures planifiées pour toutes les tâches et problèmes répertoriés sous le projet dans l’équilibreur de charge de travail et non pas toutes les heures planifiées du projet.
* Le temps alloué quotidiennement ou hebdomadaire pour toutes les tâches et tous les projets s’affiche uniquement lorsque vous activez manuellement le paramètre Afficher les affectations . Pour plus d’informations sur l’activation des paramètres dans l’équilibreur de charge de travail, voir [Navigation dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Modification des attributions d’utilisateurs {#modify-user-allocations}

Dans le cadre de l’affectation de travail aux utilisateurs, vous pouvez modifier les affectations des utilisateurs dans l’équilibreur de charge de travail afin de vous assurer qu’ils ne sont jamais surchargés ou de garantir un équilibre précis des heures entre vos ressources. Pour plus d’informations sur l’identification d’un utilisateur surchargé, voir la section [Présentation de l’affectation des utilisateurs](#user-allocation-overview) dans cet article.

1. Assurez-vous que des tâches et des problèmes sont affectés aux utilisateurs. Pour plus d’informations sur l’affectation de travail aux utilisateurs dans l’équilibreur de charge de travail, voir [Présentation de l’affectation de travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).
1. Accédez à l’équilibreur de charge de travail.
1. (Facultatif) Cliquez sur **Semaine** ou **Mois** pour gérer les affectations hebdomadaires ou mensuelles pour les utilisateurs.

   ![Sélectionnez Semaine ou Mois .](assets/month-icon-on-toolbar-selected-wb-350x226.png)

1. Dans le **Travail assigné** recherchez l’utilisateur pour lequel vous souhaitez modifier manuellement l’allocation, puis cliquez sur la flèche pointant vers la droite située à gauche du nom d’utilisateur pour développer l’utilisateur.

   ![Développer l’utilisateur](assets/wb-highlight-on-name-caret2.png)

1. Cliquez sur la flèche pointant vers la droite située à gauche du nom du projet pour développer le projet et afficher les tâches auxquelles l’utilisateur est affecté.

   >[!TIP]
   >
   >Vous pouvez modifier les affectations utilisateur uniquement pour les tâches et les problèmes. Vous ne pouvez pas modifier les affectations utilisateur pour les projets.

1. (Facultatif) Cliquez sur le **Afficher les attributions** icon ![](assets/show-allocations-icon-small.png) pour afficher les affectations pour tous les éléments de travail.

   Le nom des tâches et des projets est remplacé par l’allocation de l’utilisateur pour la tâche ou le projet.

1. (Facultatif) Cliquez sur le **Paramètres** icon ![](assets/gear-icon-settings.png) et sélectionnez l’une des options suivantes :

   1. **Inclure les heures des problèmes**. Cela vous permet de gérer les affectations de problèmes en plus des affectations de tâches.
   1. **Afficher le travail terminé**. Cette option affiche les éléments qui ont été terminés et qui sont programmés pendant la chronologie pour laquelle vous gérez les affectations.
   1. **Afficher le temps restant**. Le nombre total d’heures pour chaque utilisateur (dans la ligne de l’utilisateur) change. Lorsque ce paramètre est activé, l’équilibreur de charge de travail affiche les heures disponibles pour chaque utilisateur au lieu du nombre d’heures qui lui sont allouées.

      >[!TIP]
      >
      >Lorsque ce paramètre est activé, la modification des attributions réduit le nombre total dans la ligne utilisateur.

   1. **Projet** dans le **Sélectionner le thème de couleur** . Cela permet d’afficher chaque projet et ses tâches respectives dans des couleurs uniques et facilite la compréhension des éléments appartenant au projet.
   1. **Pourcentage** dans le **Afficher l’affectation des utilisateurs dans** . Cette valeur affiche les allocations sous la forme d’une valeur en pourcentage. La capacité de l’utilisateur selon le planning est considérée comme étant de 100 %. Par exemple, si un utilisateur est associé à un planning de 8 heures par jour, 8 heures équivaut à une capacité de 100 %. Si vous souhaitez affecter l’utilisateur au travail 4 heures par jour, vous devez mettre à jour son allocation à 50 %.

      >[!NOTE]
      >
      >L’administrateur de Workfront décide de la planification à utiliser sur l’ensemble de votre système pour calculer la capacité de l’utilisateur dans la zone Gestion des ressources de la configuration. Pour plus d’informations, voir [Configuration des préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

1. Cliquez sur le bouton **Plus** menu ![](assets/qs-more-menu.png) pour une tâche, puis cliquez sur **Modifier les attributions**.

   ![Plus de menu pour l’élément de travail](assets/more-menu-on-task-wb-nwe.png)

   Ou

   Double-cliquez sur le jour, la semaine ou le mois dans la barre d’une tâche ou d’un problème.

   Les boîtes d’attribution deviennent modifiables.

1. Cliquez dans la zone de chaque attribution quotidienne, hebdomadaire ou mensuelle pour mettre à jour manuellement le nombre d’heures ou le pourcentage pour lequel vous souhaitez que l’utilisateur soit affecté chaque jour, semaine ou mois, puis cliquez sur le bouton **Enregistrer** icon ![](assets/checkmark-icon.png).

   >[!TIP]
   >
   >Cliquez sur le bouton **Annuler** icon ![](assets/cancel-allocations-wb.png) pour supprimer les allocations que vous avez ajustées.

   ![Enregistrer ou annuler des affectations ajustées](assets/wb-contouring-with-check-and-x-boxes-350x63.png)

   Les affectations pour la mise à jour de l’utilisateur.

   >[!TIP]
   >
   >Si une tâche ou un problème s’est terminé avant la date d’achèvement planifiée, le nombre d’heures allouées pour les jours restants est écoulé et ne compte pas dans l’allocation globale de l’utilisateur. Cette variable s’affiche uniquement lorsque la variable **Afficher les attributions** et le **Afficher les dates prévues** sont activés.

   Les scénarios suivants existent :

   * Pour les tâches dont les types de durée ne sont pas simples ou pour des problèmes, le total des affectations doit correspondre à la tâche Heures planifiées avant de pouvoir cliquer sur l’icône en forme de coche.
   * Pour les tâches avec un type de durée simple , le total des affectations peut être supérieur ou inférieur aux heures planifiées et vous pouvez cliquer sur l’icône en forme de coche même si elles ne correspondent pas. Cela met également à jour le nombre d’heures planifiées pour la tâche. Vous devez disposer des autorisations et de l’accès appropriés pour mettre à jour les heures planifiées sur les tâches à partir de l’équilibreur de charge de travail.

     >[!TIP]
     >
     >Une icône représentant un verrou s’affiche à droite du nom de la tâche lorsque vous commencez à ajuster vos affectations pour indiquer que la tâche a un type de durée simple.

     ![Icône Verrouiller](assets/lock-icon-on-simple-task-in-the-balancer.png)

   Pour plus d’informations sur les conditions qui doivent être remplies pour mettre à jour les heures planifiées dans l’équilibreur de charge de travail, voir la section [Mettre à jour les heures planifiées de la tâche lors de la gestion des affectations utilisateur](#update-task-planned-hours-when-managing-user-allocations) dans cet article. Pour plus d’informations sur les types de durée de tâche, voir [Présentation de la durée et du type de durée de la tâche](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Conditionnel) Si la tâche est affectée à plusieurs utilisateurs, répétez ces étapes pour chaque utilisateur affecté à la tâche afin de mettre à jour les affectations pour chaque utilisateur.

   Toute personne ayant accès à l’équilibreur de charge de travail et qui affiche les mêmes utilisateurs et les mêmes projets que ceux que vous avez gérés affiche désormais l’allocation mise à jour pour les utilisateurs que vous avez gérés.

>[!TIP]
>
>Une icône représentant un crayon s’affiche à droite du nom de l’élément de travail pour indiquer qu’il a été modifié manuellement.

![Icône Heures ajustées manuellement](assets/icon-for-manually-adjusted-hours.png)

## Mettre à jour les heures planifiées de la tâche lors de la gestion des affectations utilisateur {#update-task-planned-hours-when-managing-user-allocations}

Vous pouvez mettre à jour les Heures planifiées d’une tâche lors de la gestion des affectations utilisateur dans l’équilibreur de charge de travail pour la tâche. Cela se produit lorsque le total des heures allouées mises à jour ne correspond pas au total initial des heures planifiées pour une tâche.

>[!IMPORTANT]
>
>* La mise à jour des heures planifiées pour les tâches peut avoir un impact sur la progression de votre projet.
>* La mise à jour manuelle des heures planifiées en modifiant les affectations quotidiennes peut avoir un impact sur les heures planifiées lors de la suppression ultérieure des affectations des tâches. Pour plus d’informations, voir [Présentation des heures planifiées](../../manage-work/tasks/task-information/planned-hours.md).
>
>* Il n’est pas possible de mettre à jour les heures planifiées pour les problèmes en mettant à jour les affectations dans l’équilibreur de charge de travail.

Cela est possible lorsque les conditions suivantes existent :

* Vous disposez des autorisations et de l’accès appropriés pour gérer les heures planifiées à partir de l’équilibreur de charge de travail. Il s’agit notamment des éléments suivants :

   * Gérer les autorisations pour les tâches.
   * Mettez à jour les heures planifiées dans l’accès de l’équilibreur de charge de travail dans la zone Gestion des ressources de votre niveau d’accès.

  Pour plus d’informations sur l’accès nécessaire à l’utilisation de l’équilibreur de charge de travail, voir la section [Exigences d’accès](#access-requirements) dans cet article.

* La tâche a un type de durée simple.

