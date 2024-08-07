---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Vue d’ensemble du calcul des heures et des ETP pour les utilisateurs et utilisatrices et les rôles dans le planificateur de ressources
description: Vue d’ensemble du calcul des heures et des ETP pour les utilisateurs et utilisatrices et les rôles dans le planificateur de ressources
author: Alina
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: de015496d4cb960b10368e4dfa0f7abec1b7d989
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 4%

---

# Vue d’ensemble du calcul des heures et des ETP pour les utilisateurs et utilisatrices et les rôles dans le planificateur de ressources

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

Vous pouvez afficher l’allocation et la disponibilité de vos ressources dans le planificateur de ressources par heure, ETR ou Coût.\
Pour plus d’informations sur le calcul des coûts dans le planificateur de ressources, voir [Calculer les coûts dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

&quot;FTE&quot; signifie &quot;équivalent temps plein&quot;. Il s’agit d’une mesure du temps qui représente le nombre d’heures consacrées au travail réel au cours d’une journée ou d’une semaine pour un utilisateur ou un rôle de tâche.

Les ensembles d’informations sur les ressources suivants sont calculés différemment dans le planificateur de ressources :

* Les valeurs des heures disponibles ou de l’éditeur de texte enrichi sont calculées selon la manière dont votre administrateur système configure les préférences de gestion des ressources dans votre système.\
  Pour plus d’informations sur le mode de calcul des valeurs des heures disponibles et de l’éditeur de texte enrichi, voir [Calculer les heures disponibles ou l’éditeur de texte enrichi pour les utilisateurs et les rôles de tâche dans le planificateur de ressources](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  Pour plus d’informations sur la définition des préférences de gestion des ressources pour le système Adobe Workfront, voir [Configuration des préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* Toutes les autres valeurs de l’éditeur de texte enrichi sont calculées selon la planification par défaut du système.\
  Pour plus d’informations sur l’affichage de toutes les autres valeurs dans le planificateur de ressources lors de l’utilisation de l’éditeur de texte enrichi, voir la section [ Calculer toutes les autres valeurs d’heure et d’éditeur de texte enrichi pour les utilisateurs et les rôles de tâche dans le planificateur de ressources ](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) de cet article.

Il est important de comprendre ce qu’est l’éditeur de texte enrichi pour chacun de vos utilisateurs et leurs rôles professionnels afin de gérer précisément vos ressources au fur et à mesure que vous les affectez pour qu’elles fonctionnent.

## Calcul des heures disponibles ou de l’éditeur de texte enrichi pour les utilisateurs et les rôles de tâche dans le planificateur de ressources {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

* [Calcul des heures disponibles et de l’éditeur de texte enrichi pour un utilisateur dans le planificateur de ressources](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner)
* [Calcul des heures disponibles et de l’éditeur de texte enrichi pour un rôle de tâche dans le planificateur de ressources](#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner)
* [Calcul des heures disponibles et de l’éditeur de texte enrichi pour un utilisateur dans le planificateur de ressources (exemple)](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example)

### Calcul des heures disponibles et de l’éditeur de texte enrichi pour un utilisateur dans le planificateur de ressources {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

L’administrateur de Workfront détermine le mode de calcul de l’heure disponible pour un utilisateur en sélectionnant d’utiliser l’une des options suivantes dans la zone Resource Management de la section Configuration :

* Planification par défaut du système et de l’éditeur de texte enrichi de l’utilisateur.
* Planification de l’utilisateur.

![Paramètre système pour les plannings utilisateur](assets/setup-resource-mgmt.png)

>[!NOTE]
>
>Cela détermine comment calculer la disponibilité des ressources au niveau du système. Pour plus d’informations sur la définition des préférences de gestion des ressources pour le système, voir [Configuration des préférences de gestion des ressources](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Selon la configuration de ce paramètre, la disponibilité des utilisateurs dans le planificateur de ressources (heures et disponibilité de l’éditeur de texte enrichi) est calculée à l’aide des méthodes suivantes :

* **The Default Schedule** : la planification par défaut du système et de l’utilisateur FTE sont utilisées pour déterminer les valeurs Hours disponibles et FTE pour l’utilisateur dans le planificateur de ressources. Le planning de l’utilisateur est ignoré. Dans ce cas :

   * Les **Heures disponibles** du planificateur de ressources sont calculées à l’aide de la formule suivante :

     `User Available Hours = Default Schedule Hours * User FTE value`

     Par exemple, si la planification par défaut comporte 40 heures par semaine disponibles pour le travail et que l’utilisateur est 0,5, l’utilisateur peut travailler 20 heures par semaine dans le planificateur de ressources.

     Pour plus d’informations sur les plannings, y compris la planification par défaut, voir [Créer une planification](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * L’ **éditeur de texte enrichi disponible** pour l’utilisateur dans le planificateur de ressources est identique à l’éditeur de texte enrichi spécifié dans les paramètres utilisateur.

     Par exemple, si l’éditeur de texte enrichi de l’utilisateur est 0.5 dans les paramètres utilisateur, l’éditeur de texte enrichi disponible de l’utilisateur est 0.5 dans le planificateur de ressources. Pour plus d’informations sur la valeur de l’éditeur de texte enrichi tel qu’il s’affiche dans les paramètres utilisateur, voir [Modification du profil d’un utilisateur](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* **Planification de l’utilisateur** : la planification de l’utilisateur est utilisée pour déterminer la disponibilité de l’utilisateur dans le planificateur de ressources. La valeur de l’utilisateur FTE est ignorée. Dans ce cas :

   * Les **Heures disponibles** du planificateur de ressources sont identiques à celles du planning de l’utilisateur.

     Par exemple, si le planning de l’utilisateur dispose de 40 heures de travail par semaine, l’utilisateur peut travailler 40 heures par semaine dans le planificateur de ressources.

   * Le **FTE disponible** dans le planificateur de ressources est calculé à l’aide de la formule suivante :

     `User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours`

     Par exemple, si le planning de l’utilisateur dispose de 20 heures de travail et que le planning par défaut dans Workfront dispose de 40 heures de travail, l’éditeur de texte enrichi de l’utilisateur est de 0,5.

     Pour plus d’informations sur les plannings, y compris la planification par défaut, voir [Créer une planification](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

>[!NOTE]
>
>Si l’utilisateur n’est pas associé à une planification, les Heures disponibles pour l’utilisateur sont calculées à l’aide de la Planification par défaut.

### Calcul des heures disponibles et de l’éditeur de texte enrichi pour un rôle de tâche dans le planificateur de ressources {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

Vous devez d’abord calculer la disponibilité de l’utilisateur, puis la disponibilité de chacun de ses rôles de travail.

La disponibilité des rôles de tâche dans le planificateur de ressources prend en compte la disponibilité totale de l’utilisateur et le **pourcentage de disponibilité de l’éditeur de texte enrichi** associé à chaque rôle de l’utilisateur.\
![percent_of_fte_disponibilité_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

Pour plus d’informations sur l’association d’une valeur **Pourcentage de disponibilité de l’éditeur de texte enrichi** à un rôle de tâche pour un utilisateur, voir [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Par exemple, si la valeur des heures disponibles pour un utilisateur est de 40 et qu’il peut remplir un rôle de Principal pendant 75 % de ce temps, et un autre rôle pendant 25 % de ce temps, le planificateur de ressources indique que la valeur **Hours disponibles** pour le rôle de Principal pendant une semaine est de 30 heures et que la valeur **Heures disponibles** pour l’autre rôle est de 10 heures . Dans ce cas, l’éditeur de texte enrichi pour le rôle de Principal est 0,75 et l’éditeur de texte enrichi pour l’autre rôle est 0,25.

>[!NOTE]
>
>Le temps total disponible pour l’utilisateur est calculé par l’une des deux méthodes décrites dans la section [Calcul des heures disponibles et de l’éditeur de texte enrichi pour un utilisateur dans la planification des ressources](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) de cet article.

Lorsque vous affichez le planificateur de ressources dans la vue Rôle, la disponibilité d’un rôle de tâche correspond à la disponibilité totale de tous les utilisateurs pouvant remplir ce rôle de tâche.\
Pour plus d’informations sur la disponibilité des ressources dans le planificateur de ressources, consultez la [présentation du planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Calcul des heures disponibles et de l’éditeur de texte enrichi pour un utilisateur dans le planificateur de ressources (exemple) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

Le tableau suivant illustre le mode de calcul des heures disponibles et de l’éditeur de texte enrichi disponibles pour l’utilisateur dans le planificateur de ressources, selon la méthode utilisée par l’administrateur système pour le calcul de l’éditeur de texte enrichi dans les préférences de gestion des ressources.

Pour cet exemple, nous utilisons les chiffres suivants :

* Une planification système par défaut de 40 heures
* Planification de 20 heures pour l’utilisateur
* Un éditeur de texte enrichi de 0.8

| Méthode de calcul de l’éditeur de texte enrichi (paramètre système) | **Heures à partir de la planification de l’utilisateur** | **Heures à partir de la planification par défaut** | **Champ d’éditeur de texte enrichi de l’utilisateur** | **Heures disponibles dans le planificateur de ressources** | **Éditeur de texte enrichi disponible dans le planificateur de ressources** |
|---|---|---|---|---|---|
| **La Planification Par Défaut** | Ignoré | 40 | 0,8 | **32** (calculé) | **0.8** |
| **Planification de l’utilisateur** | 20 | 40 | Ignoré | **20** | **0.5** (calculé) |

Les exceptions de planification et les congés peuvent avoir une incidence sur le nombre d’heures planifiées ou sur l’éditeur de texte enrichi. Pour plus d’informations, voir [Configurer les préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Exemple d’affichage du planificateur de ressource par utilisateur et heures :

![Affichage du planificateur de ressources par utilisateur et heures](assets/resource-planner-by-user-by-hours.png)

Exemple d’affichage du planificateur de ressources par utilisateur et éditeur de texte enrichi :

![Affichage du planificateur de ressources par utilisateur et FTE](assets/resource-planner-by-user-by-fte.png)

## Calcul de toutes les autres valeurs d’heure et d’éditeur de texte enrichi pour les utilisateurs et les rôles de tâche dans le planificateur de ressources {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

Outre les heures disponibles ou l’éditeur de texte enrichi, les informations temporelles suivantes s’affichent également dans le planificateur de ressources :

* Heures prévues
* Heures budgétées
* Variance horaire
* Heures nettes\
  Pour plus d’informations sur ces valeurs, voir [Aperçu des heures, de l’ETR et des informations de coût dans les vues Projet et Rôle du planificateur de ressources](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

* Différence horaire\
  Pour plus d’informations sur ce que représente cette valeur, voir [Aperçu des heures, de l’EPT et des informations de coût dans les vues Projet et Rôle du planificateur de ressources](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

Vous pouvez afficher les mêmes informations dans le planificateur de ressources sous forme d’éditeur de texte enrichi ou d’heures.

Workfront utilise la formule suivante pour afficher toutes les autres valeurs sous forme d’éditeur de texte enrichi dans le planificateur de ressources :

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>Le planning de l’utilisateur est ignoré lors du calcul de l’éditeur de texte enrichi pour toutes les valeurs, à l’exception des valeurs d’AVL disponibles dans le planificateur de ressources. Seul le Planning par défaut est pris en compte pour le calcul.

Ce calcul s&#39;applique aux valeurs suivantes :

* ETR planifié (PLN)
* ETR (BDG) budgété
* Variance de l’éditeur de texte enrichi (VAR)
* NET FTE
* Différence FTE (DIF)
