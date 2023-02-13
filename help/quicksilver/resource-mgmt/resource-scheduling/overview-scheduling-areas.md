---
content-type: overview
product-area: resource-management
navigation-topic: resource-scheduling
title: Présentation des zones de planification
description: Les sections suivantes décrivent où vous pouvez accéder à la zone de planification dans Adobe Workfront, ainsi que les fonctionnalités disponibles dans la zone de planification.
author: Alina
feature: Resource Management
exl-id: ed6f1db9-917d-4a19-9fd4-1ed5d2ca95fb
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1790'
ht-degree: 0%

---

# Présentation des zones de planification

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


Les sections suivantes décrivent où vous pouvez accéder à la zone de planification dans Adobe Workfront, ainsi que les fonctionnalités disponibles dans la zone de planification.

## Zones Workfront qui vous permettent de planifier des ressources

Vous pouvez planifier des ressources dans les zones suivantes de Workfront :

* **Pour les projets pour lesquels vous êtes le responsable des ressources** (de la fonction **Planification** ) La zone Planification de Workfront permet aux gestionnaires de ressources d’effectuer des affectations de ressources sur plusieurs projets.

* **Pour un projet individuel lorsque vous êtes membre de l’équipe de projet** (de la fonction **Planification** zone d’un projet) :

   La zone Planification d’un projet permet aux membres de l’équipe du projet d’affecter la tâche du projet aux utilisateurs de l’équipe du projet.

* **Pour une équipe individuelle, vous êtes membre de** (de la fonction **Planification** de l’équipe) La section Planification d’une équipe permet aux membres de l’équipe d’affecter aux membres de l’équipe le travail déjà affecté à l’équipe à partir de plusieurs projets à des membres individuels de l’équipe.

## Fonctionnalités disponibles dans la zone Planification

La zone de planification affiche les tâches, les problèmes et les affectations de ressources actuelles.\
![resource_schedule_overview.png](assets/resource-scheduling-overview-350x237.png)

* [Outils de filtrage et de permutation](#filter-and-swap-tools)
* [Sélection de date](#date-selection)
* [Zone non attribuée](#unassigned-area)
* [Utilisateurs et rôles](#users-and-roles)
* [Planification de la chronologie](#scheduling-timeline)

### Outils de filtrage et de permutation {#filter-and-swap-tools}

* **Outil de filtrage :** Permet de filtrer le contenu affiché dans la chronologie de planification. Pour plus d’informations sur l’utilisation de l’outil Filtre, voir [Filtrage des informations dans la zone Planification](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).
* **Outil de permutation :** (Disponible uniquement lors de la planification de ressources pour des projets à partir de l’onglet Planification ou Affectation de personnel) Permet d’affecter, d’échanger ou de supprimer rapidement des utilisateurs à des tâches sur plusieurs projets. Pour plus d’informations, voir [Affectez manuellement des tâches et des problèmes non attribués dans les zones Planification .](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Sélection de date {#date-selection}

Vous pouvez ajuster la période pour laquelle les données sont affichées dans la chronologie de planification. Par défaut, la période est de 2 semaines (14 jours consécutifs, week-ends compris) à partir du jour en cours.

### Zone non attribuée {#unassigned-area}

* [Lors de la planification des ressources en tant que gestionnaire des ressources (pour plusieurs projets dans la zone Planification )](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Lors de la planification de ressources en tant que membre de l’équipe de projet (à partir d’un projet)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Lors de la planification de ressources en tant que membre de l’équipe (à partir d’une équipe)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Lors de la planification des ressources en tant que gestionnaire des ressources (pour plusieurs projets dans la zone Planification ) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area}

Le **Non attribué** sur la chronologie de la planification, affiche uniquement les tâches et problèmes qui répondent à tous les critères suivants :

* Non attribué à un utilisateur.
* Non affecté à une équipe.\
   Si la tâche ou le problème est assigné à une équipe, il est toujours affiché dans la **Non attribué** zone si la tâche ou le problème est également affecté à un rôle en plus de l’affectation de l’équipe.\
   Si des tâches ou des problèmes ont des affectations de rôles de tâche supplémentaires qui ne sont pas remplies par un utilisateur, elles s’affichent également.\
   Par exemple, une tâche est affectée à 3 rôles de tâche : Designer, gestionnaire de produits et développeur. Vous affectez cette tâche à l’utilisateur A qui a un rôle de tâche Designer et à l’utilisateur B qui a un rôle de gestionnaire de produits. Dans ce scénario, la tâche est toujours visible dans la zone Non affecté de la chronologie de la planification, car le rôle de tâche Développeur n’est pas attribué à un utilisateur.

#### Lors de la planification de ressources en tant que membre de l’équipe de projet (à partir d’un projet) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project}

Le **Non attribué** dans la partie supérieure de la chronologie de la planification, la section affiche les tâches et les problèmes qui répondent aux critères suivants :

* Associé au projet, mais n’étant attribué à aucun utilisateur de l’équipe de projet.\
   Les tâches associées au projet et affectées à un utilisateur de l’équipe du projet s’affichent dans la ligne de l’utilisateur auquel les tâches sont affectées.
* Associé au projet, mais affecté à un membre qui ne fait pas partie de l’équipe du projet.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! Is it even possible to have the task assigned to a member who is not part of the project team? If so, then would this end up in the Unassigned area?])</p>
  -->

#### **Lors de la planification de ressources en tant que membre de l’équipe (à partir d’une équipe)** {#when-scheduling-resources-as-a-team-member-from-a-team}

Le **Non attribué** dans la partie supérieure de la chronologie de la planification, la section affiche les tâches et les problèmes qui répondent aux critères suivants :

* Affecté à l’équipe et à aucun autre utilisateur de l’équipe.\
   Les tâches qui sont affectées à la fois à l’équipe et à un utilisateur de l’équipe s’affichent dans la ligne de l’utilisateur auquel les tâches sont affectées.
* Affecté à l’équipe et à un utilisateur qui n’est pas membre de l’équipe.

### Utilisateurs et rôles {#users-and-roles}

* [Lors de la planification des ressources en tant que gestionnaire des ressources (pour plusieurs projets dans la zone Planification )](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Lors de la planification de ressources en tant que membre de l’équipe de projet (à partir d’un projet)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Lors de la planification de ressources en tant que membre de l’équipe (à partir d’une équipe)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Lors de la planification des ressources en tant que gestionnaire des ressources (pour plusieurs projets dans la zone Planification ) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area-1}

Tous les utilisateurs qui peuvent se voir attribuer l’une des tâches non affectées se trouvent sous le **Non attribué** zone. Les utilisateurs peuvent, dans la chronologie de planification, se voir attribuer une tâche ou un problème dans les cas suivants :

* Par défaut, les utilisateurs ne s’affichent sur la chronologie de la planification que lorsqu’un rôle de tâche est défini dans le système (rôle de tâche Principal ou rôle de tâche secondaire), et que ce rôle correspond au rôle de tâche affecté à une tâche ou à un problème actuellement visible dans la fonction **Non attribué** sur la chronologie de la planification. Vous pouvez désactiver cette fonctionnalité afin de permettre l’affectation de tâches et de problèmes à un utilisateur, que ce dernier ait ou non un rôle défini dans son profil utilisateur correspondant à l’attribution du rôle de la tâche ou au problème qui lui est assigné. Pour plus d’informations, voir [Autorisation des affectations d’utilisateurs, quel que soit le rôle et l’appartenance à un groupe dans les zones de planification](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md).\
   Un utilisateur et les tâches qui lui sont assignées peuvent apparaître plusieurs fois dans la chronologie de planification s’il dispose de plusieurs rôles de tâche désignés dans le système Workfront.\
   Les utilisateurs restent dans la chronologie de la planification une fois qu’une tâche ou un problème leur a été assigné, même s’il n’y a plus aucune tâche ou problème ayant une affectation de rôle correspondante. Cela vous permet d’apporter les modifications nécessaires une fois qu’elles ont été affectées.\
   Si la tâche n’est pas affectée à un rôle de tâche, tous les utilisateurs qui répondent aux exigences de filtrage s’affichent. Pour plus d’informations sur le filtre, voir [Filtrage des informations dans la zone Planification](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

* Ils ont été désignés dans la variable **Utilisateurs** dans le champ **Filtrer** .\
   Pour plus d’informations sur le filtre, voir [Filtrage des informations dans la zone Planification](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).\
   Lors de la planification de ressources pour une équipe (dans l’onglet Travail sur ), l’affectation de l’équipe s’affiche également.

Toutes les autres tâches ou problèmes affectés à ces utilisateurs sont également affichés dans la chronologie.

Vous pouvez voir le niveau d’allocation des utilisateurs un jour donné, comme décrit dans la section [Gestion des affectations d’utilisateurs dans les zones de planification](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Les tâches dont vous ne disposez pas au moins des autorisations de contribution s’affichent sous forme de barre grise dans la chronologie de la planification.

#### Lors de la planification de ressources en tant que membre de l’équipe de projet (à partir d’un projet) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project-1}

Chaque membre de l’équipe est toujours affiché dans la chronologie de la planification, quelles que soient les affectations de rôles des utilisateurs et les affectations de rôles des tâches dans la zone Non affecté.

Si un utilisateur possède plusieurs rôles de tâche définis dans le système, il apparaît plusieurs fois dans la chronologie de planification lorsque l’un des critères suivants est satisfait :

* Des tâches ou des problèmes s’affichent dans la variable **Non attribué** zone affectée aux rôles de tâche associés à l’utilisateur.
* Il existe des tâches ou des problèmes sur le projet qui ont des rôles de tâche attribués, et ces tâches ou ces problèmes sont affectés à un utilisateur qui a ce rôle de tâche défini dans le système.

#### Lors de la planification de ressources en tant que membre de l’équipe (à partir d’une équipe) {#when-scheduling-resources-as-a-team-member-from-a-team-1}

Chaque membre de l’équipe est toujours affiché dans la chronologie de la planification, quelles que soient les affectations de rôles des utilisateurs et les affectations de rôles des tâches dans la zone Non affecté.

Vous pouvez voir le niveau d’allocation des utilisateurs un jour donné, comme décrit dans la section [Gestion des affectations d’utilisateurs dans les zones de planification](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Tâches dont vous ne disposez pas au moins des autorisations de contribution pour s’afficher sous forme de barre grise dans la chronologie de planification.

### Planification de la chronologie {#scheduling-timeline}

* **Contenu par défaut :** Par défaut, toutes les tâches répondant aux exigences définies dans la section [Tâche et problèmes préalables](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#task-and-issue-prerequisites) dans le [Prise en main de la planification des ressources](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md) Les articles sur tous les projets dont l’état est Actuel s’affichent dans la chronologie de planification.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: [! true for teams? - Yes, but really we're focusing on tasks, and the team assignment.])
  </MadCap:conditionalText>
  -->

   Pour personnaliser les éléments affichés dans la chronologie de la planification, y compris l’affichage des problèmes et des projets avec un état différent, utilisez le filtre, comme décrit dans la section [Filtrage des informations dans la zone Planification](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

   Un maximum de 10 tâches par jour s’affiche pour un utilisateur donné. Vous pouvez développer la liste pour afficher toutes les tâches actuellement affectées à cet utilisateur.

* **Tâches parentes :** L’affichage ou non des tâches parentes dans la chronologie dépend de plusieurs paramètres. Pour plus d’informations, voir la section &quot;Configurer l’affichage des tâches parentes dans la chronologie de planification&quot; dans la section [Configuration des paramètres dans les zones Planification](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) article.

* **Color coding:** Les tâches et les problèmes de la chronologie de la planification sont codés par couleur en fonction du projet auquel ils appartiennent. Vous ne pouvez pas personnaliser la couleur associée à un projet spécifique.

   Lors de la planification du travail en équipe (dans l’onglet Personnel ), les couleurs ne sont utilisées que si la variable **Afficher toutes les tâches de l’utilisateur** est activée. Pour plus d’informations, voir la section &quot;Configurer l’affichage des tâches parentes dans la chronologie de planification&quot; dans la section [Configuration des paramètres dans les zones Planification](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) article.

* **Durée des tâches :** Les durées de tâche sont représentées dans la chronologie de chaque tâche (la tâche s’étend physiquement sur le nombre de jours égal à la durée). Vous ne pouvez pas ajuster la durée de la tâche à partir de la chronologie de planification.

* **Time off :** Le décalage est représenté sur la chronologie de la planification par un indicateur gris clair dans la colonne le jour où le décalage est planifié pour un utilisateur donné.\
   Le délai d’expiration est configuré pour chaque utilisateur en fonction des informations suivantes :

   Le calendrier de désactivation personnel de l’utilisateur. Pour plus d’informations sur le calendrier de désactivation personnel, voir [Configuration du temps de pause personnel dans Adobe Workfront](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

   Planification affectée à l’utilisateur. Il peut s’agir du planning par défaut ou d’un planning personnalisé. Pour plus d’informations sur les plannings, voir [Création d’un planning](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Week-ends :** Les week-ends sont représentés sur la chronologie de planification sous forme d’ombrage gris clair les samedis et dimanches. Les jours de la semaine définis comme week-ends dans la chronologie de planification ne peuvent pas être configurés. Vous pouvez planifier le travail des utilisateurs le week-end.
