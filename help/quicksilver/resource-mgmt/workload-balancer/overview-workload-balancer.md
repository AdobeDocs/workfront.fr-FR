---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Vue d’ensemble de l’équilibreur de charge de travail
description: Une fois que les chefs de projet ont planifié le travail sur les projets en créant des tâches et une fois que les gestionnaires de ressources ont attribué des ressources de rôle aux projets dans le planificateur de ressources, les propriétaires de projet et les chefs d’équipe peuvent utiliser l’équilibreur de charge de travail pour affecter des tâches aux utilisateurs.
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 3%

---

# Vue d’ensemble de l’équilibreur de charge de travail

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Une fois que les chefs de projet ont planifié le travail sur les projets en créant des tâches et une fois que les gestionnaires de ressources ont attribué des ressources de rôle aux projets dans le planificateur de ressources, les propriétaires de projet et les chefs d’équipe peuvent utiliser l’équilibreur de charge de travail pour affecter des tâches aux utilisateurs.

>[!IMPORTANT]
>
>Vous pouvez utiliser l’équilibreur de charge de travail pour affecter le travail réel (tâches et problèmes) aux utilisateurs.
>
>Vous devez utiliser le planificateur de ressources et non l’équilibreur de charge de travail pour estimer, à un niveau élevé, la répartition des rôles de tâche pour vos projets. Pour plus d’informations sur le planificateur de ressources, consultez la [présentation du planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Cet article décrit l’objectif général de l’équilibreur de charge de travail et quelques-unes des bonnes pratiques pour configurer vos projets et ressources afin de l’utiliser correctement.

Pour consulter les tutoriels vidéo de l’équilibreur de charge de travail, accédez à la page [Workfront Tutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=fr) . Dans le menu de gauche, sélectionnez **Gérer les ressources** > **équilibreur de charge de travail** et choisissez un tutoriel.

## Localiser l’équilibreur de charge de travail

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

Nous vous recommandons d’utiliser l’équilibreur de charge de travail dans les zones suivantes pour planifier des ressources :

* Au niveau du système, dans la zone Ressource .
* Au niveau du projet, dans la section équilibreur de charge de travail d’un projet.
* Au niveau de l’équipe, dans la section équilibreur de charge de travail d’une équipe.

Pour plus d’informations sur la localisation de l’équilibreur de charge de travail, voir [Localisation de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Avantages de l’équilibreur de charge de travail

Tenez compte des avantages suivants lorsque vous utilisez l’équilibreur de charge de travail :

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Accédez à un mappage visuel clair de la suraffectation et de la sous-utilisation des ressources, qui est transparent pour toutes les parties prenantes.
* En tant que gestionnaire de personnes, vous pouvez protéger vos personnes de l&#39;épuisement et leur permettre de faire de leur mieux avec plus de concentration, de qualité et d&#39;engagement. Vous pouvez garantir leur pleine utilisation, rompre les silos et permettre l’alignement du travail entre les équipes.
* Lorsque vous affectez du travail au niveau de la tâche ou du problème, vous ne pouvez pas savoir à quel point un utilisateur est occupé. Lorsque vous utilisez l’équilibreur de charge de travail, vous pouvez voir quels utilisateurs sont disponibles dans leur charge de travail pour terminer la tâche ou le problème à temps. Cela inclut les détails des congés et des exceptions de planning.

  Pour plus d’informations, voir [Présentation de l’affectation du travail dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  Vous pouvez également attribuer des tâches en bloc, ce qui facilite la distribution simultanée de plusieurs tâches sur plusieurs projets. Pour plus d’informations, voir [Affecter du travail en masse à l’aide de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* Les cadres peuvent prendre des décisions opportunes en matière de recrutement en faisant preuve de transparence quant à la manière dont les membres de leur organisation sont utilisés.
* Les membres de l’équipe bénéficient d’une meilleure collaboration, car ils peuvent tous voir sur quoi travaillent leurs collègues à tout moment. Pour plus d’informations sur l’accès nécessaire pour afficher ou gérer les ressources dans l’équilibreur de charge de travail, voir [Accès nécessaire pour gérer les ressources dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Partagez-le avec toute personne qui n’a pas accès à la zone Ressource en y incorporant un lien dans un onglet personnalisé. Pour plus d’informations, voir [Partage de l’équilibreur de charge de travail avec un lien](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* Visualisez et gérez les charges de travail et la demande des personnes dans une vue unique au niveau global, du projet ou de l’équipe, selon votre rôle. Lors de la gestion de projets, cela inclut non seulement l’allocation de ressources pour le projet, mais également la visualisation de l’allocation de ressources à partir du planificateur de scénario Adobe Workfront. Les gestionnaires de personnes utilisent le planificateur de scénarios Workfront pour gérer les compétences professionnelles dans l’ensemble de l’entreprise. Le planificateur de scénario n’est disponible que dans la nouvelle expérience Adobe Workfront.

  >[!NOTE]
  >
  >  Le planificateur de scénario nécessite une licence supplémentaire. Pour plus d’informations sur le planificateur de scénarios Workfront, voir [Vue d’ensemble du planificateur de scénarios](../../scenario-planner/scenario-planner-overview.md).


## Bonnes pratiques relatives à l’utilisation de l’équilibreur de charge de travail

Nous recommandons les bonnes pratiques suivantes pour la planification de projets, la configuration des utilisateurs et l’utilisation de filtres avant de commencer à planifier vos ressources à l’aide de l’équilibreur de charge de travail.

* [ Bonnes pratiques pour l’affichage des informations dans l’équilibreur de charge de travail ](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Bonnes pratiques pour la configuration des utilisateurs](#best-practices-for-setting-up-users)
* [Bonnes pratiques relatives à la configuration des tâches et des problèmes](#best-practices-for-setting-up-tasks-and-issues)

### Bonnes pratiques pour l’affichage des informations dans l’équilibreur de charge de travail {#best-practices-for-displaying-information-in-the-workload-balancer}

Nous vous recommandons d’utiliser des filtres afin que vous puissiez afficher uniquement les informations pertinentes pour les tâches non affectées et affectées.

Pour plus d’informations sur la création et l’utilisation de filtres dans l’équilibreur de charge de travail, voir [Filtrage des informations dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Bonnes pratiques relatives à la configuration des utilisateurs

* En tant qu’utilisateur qui planifie le travail pour d’autres personnes, vous devez disposer des droits d’accès et des autorisations appropriés pour planifier des ressources pour le travail.

  Pour plus d’informations sur l’accès nécessaire pour gérer la charge de travail de vos ressources dans l’équilibreur de charge de travail, voir [Accès nécessaire pour gérer les ressources dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Les utilisateurs dont vous souhaitez gérer la charge de travail doivent respecter les critères suivants afin que les informations sur leur disponibilité et leurs compétences soient exactes :

   * Avoir des planifications et des rôles de tâche associés à leur profil.

     Pour plus d’informations sur l’association de planifications et de rôles de tâche avec les utilisateurs, voir [Ajout d’utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Si un utilisateur n’est pas associé à une planification, la planification par défaut de votre système Workfront est associée à l’utilisateur par défaut, à des fins de gestion des ressources.
   * Demandez que les exceptions de planification soient mises à jour dans leurs plannings.

     Pour plus d’informations sur la création de plannings, voir [Création d’un planning](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Faire mettre à jour leur calendrier de désactivation dans leur profil.

     Pour plus d’informations sur la mise à jour du calendrier de désactivation d’un utilisateur, voir [Configuration de l’heure de désactivation personnelle](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* L’administrateur de Workfront doit déterminer comment Workfront calcule la disponibilité de l’utilisateur. Ils peuvent décider si Workfront utilise la planification par défaut du système ou la planification de l’utilisateur pour calculer le temps de travail de l’utilisateur en ajustant les préférences de gestion des ressources dans la zone Configuration de Workfront.

  Pour plus d’informations, voir [Configurer les préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Bonnes pratiques relatives à la configuration des tâches et des problèmes {#best-practices-for-setting-up-tasks-and-issues}

Assurez-vous que la tâche et la configuration de problème suivantes existent avant de commencer à assigner du travail aux utilisateurs dans l’équilibreur de charge de travail :

* Les tâches parentes ne sont pas affectées aux utilisateurs ni aux rôles. Les tâches parentes ne s’affichent pas dans l’équilibreur de charge de travail.
* Les tâches et les problèmes ont une valeur pour les heures planifiées qui est supérieure à zéro.

* Les tâches et les problèmes ont une valeur pour leur durée supérieure à zéro.
* Les dates prévues des problèmes sont dans le calendrier du projet.

## Avant de commencer à utiliser l’équilibreur de charge de travail

* Consultez les articles suivants avant de commencer à utiliser l’équilibreur de charge de travail :

   * Cet article vous explique comment naviguer dans l’équilibreur de charge de travail pour effectuer ces actions : [Parcourez l’équilibreur de charge de travail](../workload-balancer/navigate-the-workload-balancer.md).

   * Les articles suivants vous expliquent comment affecter du travail et gérer les affectations d’utilisateurs :

      * [Présentation de l’affectation de travail dans l’équilibreur de charge de travail](../workload-balancer/assign-work-in-workload-balancer.md).
      * [Gérez les affectations utilisateur dans l’équilibreur de charge de travail](../workload-balancer/manage-user-allocations-workload-balancer.md).

* L’équilibreur de charge de travail se trouve dans différentes zones de Workfront. Pour plus d’informations sur l’emplacement de l’équilibreur de charge de travail, voir [Localisation de l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Accès nécessaire pour utiliser l’équilibreur de charge de travail

Pour pouvoir afficher et utiliser l’équilibreur de charge de travail dans Workfront, vous devez disposer des autorisations et de l’accès Workfront appropriés pour des projets spécifiques. Pour plus d’informations sur l’accès nécessaire à l’utilisation de l’équilibreur de charge de travail, consultez l’article [Accès nécessaire à la gestion des ressources dans l’équilibreur de charge de travail](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
