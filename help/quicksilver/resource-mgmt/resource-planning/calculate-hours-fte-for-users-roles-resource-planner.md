---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Présentation du calcul des heures et des équivalents temps plein pour les utilisateurs et les rôles dans le planificateur de ressources
description: Présentation du calcul des heures et des équivalents temps plein pour les utilisateurs et les rôles dans le planificateur de ressources.
author: Lisa
feature: Resource Management
exl-id: 10b0e507-658e-4d12-994a-e38da6111f5d
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '1323'
ht-degree: 67%

---

# Vue d’ensemble du calcul des heures et des ETP pour les utilisateurs et utilisatrices et les rôles dans le planificateur de ressources

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina:KEEP THIS:***Linked to: Configuring My Settings, Editing User Accounts, Planning in the Resource Planner -- *** Some of this documentation is also duplicated in this article (Scheduling): https://support.workfront.com/hc/en-us/articles/360000557174)</p>
-->

Vous pouvez afficher l’attribution et la disponibilité de vos ressources dans le planificateur de ressources par heure, ETP ou coût.\
Pour plus d’informations sur le calcul des coûts dans le planificateur de ressources, voir [Calculer les coûts dans le planificateur de ressources](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

L’équivalent temps plein (ETP) est une mesure du temps qui représente le nombre d’heures consacrées au travail réel au cours d’une journée ou d’une semaine pour un utilisateur ou une fonction.

Les ensembles d’informations sur les ressources suivants sont calculés différemment dans le planificateur de ressources :

* Les valeurs des heures disponibles ou ETP sont calculées selon la manière dont votre administrateur ou administratrice système configure les préférences de gestion des ressources dans votre système.\
  Pour plus d’informations sur le calcul des valeurs d’heures disponibles et d’ETP, voir [Calculer les heures disponibles ou d’ETP pour les personnes et les fonctions dans le planificateur de ressources](#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner).\
  Pour plus d’informations sur la définition des préférences de gestion des ressources pour le système Adobe Workfront, voir [Configurer les préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* Toutes les autres valeurs ETP sont calculées selon la planification par défaut du système.\
  Pour plus d’informations sur l’affichage de toutes les autres valeurs dans le planificateur de ressources lors de l’utilisation d’ETP, voir la section [Calculer toutes les autres valeurs d’heures et d’ETP pour les personnes et les fonctions dans le planificateur de ressources](#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner) dans cet article.

Il est important de comprendre ce qu’est ETP pour chacun de vos utilisateurs et utilisatrices et leurs fonctions afin de gérer précisément vos ressources au fur et à mesure que vous les affectez à un travail.

## Calculer les heures disponibles ou l’ETP pour les personnes et les fonctions dans le planificateur de ressources {#calculate-available-hours-or-fte-for-users-and-job-roles-in-the-resource-planner}

### Calculer les heures disponibles et l’ETP pour une personne dans le planificateur de ressources {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner}

L’administrateur Workfront détermine la manière dont le temps disponible pour un utilisateur est calculé en sélectionnant l’une des options suivantes dans la zone Gestion des ressources de la Configuration :

* Le planning par défaut du système et de l’ETP de la personne.
* Le planning de la personne.

![Paramètre du système pour les plannings des personnes](assets/setup-resource-mgmt.png)

>[!NOTE]
>
>Cela détermine comment calculer la disponibilité des ressources au niveau du système. Pour plus d’informations sur la définition des préférences de gestion des ressources pour le système, voir [Configurer les préférences de gestion des ressources](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Selon la configuration de ce paramètre, la disponibilité des personnes dans le planificateur de ressources (disponibilité en heures et ETP) est calculée à l’aide des méthodes suivantes :

* **Planning par défaut** : le planning par défaut du système et l’ETP de la personne sont utilisés pour déterminer les valeurs des heures disponibles et de l’ETP pour la personne dans le planificateur de ressources. Le planning de l’utilisateur est ignoré. Dans ce cas :

   * Les heures disponibles dans le planificateur de ressources sont calculées à l&#39;aide de la formule suivante :

     `User Available Hours = Default Schedule Hours * User FTE value`

     Par exemple, si le planning par défaut comporte 40 heures par semaine disponibles pour le travail et que l’ETP de la personne est 0,5, cette dernière peut travailler 20 heures par semaine dans le planificateur de ressources.

     Pour plus d’informations sur les planifications, y compris la planification par défaut, voir [Créer un planning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   * L’équivalent temps complet disponible pour l’utilisateur dans le planificateur de ressources est identique à l’équivalent temps complet de l’utilisateur spécifié dans les paramètres utilisateur.

     Par exemple, si l’ETP de la personne est 0,5 dans ses paramètres, l’ETP disponible de la personne est 0,5 dans le planificateur de ressources. Pour plus d’informations sur la valeur de l’ETP de la personne tel qu’il s’affiche dans les paramètres de l’utilisateur ou de l’utilisatrice, voir [Modifier le profil d’une personne](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* **Planning de l’utilisateur** : le planning de l’utilisateur est utilisé pour déterminer la disponibilité de l’utilisateur dans le planificateur de ressources. La valeur de l’ETP de la personne est ignorée. Dans ce cas :

   * Les heures disponibles dans le planificateur de ressources sont les mêmes que les heures du calendrier de l&#39;utilisateur.

     Par exemple, si l’horaire de l’utilisateur dispose de 40 heures de travail par semaine, l’utilisateur peut travailler 40 heures par semaine dans le Planificateur de ressources.

   * L&#39;équivalent temps complet disponible dans le planificateur de ressources est calculé par la formule suivante :

     `User Available FTE = Hours from the Schedule of the User/ Default Schedule Hours`

     Par exemple, si l’horaire de l’utilisateur dispose de 20 heures pour travailler et que l’horaire par défaut dans Workfront dispose de 40 heures pour travailler, l’équivalent temps complet de l’utilisateur est de 0,5.

     Pour plus d’informations sur les plannings, y compris le planning par défaut, voir [Créer un planning](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

>[!NOTE]
>
>Si la personne n’est pas associée à un planning, les heures disponibles pour elle sont calculées à l’aide du planning par défaut.

### Calculer les heures disponibles et l’ETP pour une fonction dans le planificateur de ressources {#calculate-the-available-hours-and-fte-for-a-job-role-in-the-resource-planner}

Vous devez d’abord calculer la disponibilité de la personne, puis la disponibilité de chacune de ses fonctions.

La disponibilité des fonctions dans le planificateur de ressources prend en compte la disponibilité totale de l&#39;utilisateur et le pourcentage de disponibilité d&#39;équivalent temps complet associé à chaque rôle de l&#39;utilisateur.\
![percent_of_fte_availlability_at_the_user_level.png](assets/percent-of-fte-availability-at-the-user-level-350x144.png)

Pour plus d&#39;informations sur l&#39;association d&#39;une valeur de pourcentage de disponibilité d&#39;équivalent temps complet à une fonction pour un utilisateur, voir [Modifier le profil d&#39;un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Par exemple, si la valeur des heures disponibles pour un utilisateur est de 40 et qu&#39;il peut remplir un rôle de Principal pendant 75 % de ce temps et un autre rôle pendant 25 % de ce temps, le planificateur de ressources indique que la valeur des heures disponibles pour le rôle de Principal pendant une semaine est de 30 heures et que la valeur des heures disponibles pour l&#39;autre rôle est de 10 heures. Dans ce cas, l’ETP rôle principal est 0,75 et l’ETP de l’autre rôle est 0,25.

>[!NOTE]
>
>Le temps total disponible de la personne est calculé par l’une des deux méthodes décrites dans la section [Calculer les heures disponibles et l’ETP pour une personne dans le planificateur de ressources](#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner) dans cet article.

Lorsque vous affichez le planificateur de ressources dans la vue Rôle, la disponibilité d’une fonction correspond à la disponibilité totale de tous les utilisateurs et utilisatrices pouvant remplir cette fonction.

Pour plus d’informations sur la disponibilité des ressources dans le planificateur de ressources, voir [Vue d’ensemble du planificateur de ressources](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Calculer les heures disponibles et l’ETP pour une personne dans le planificateur de ressources (exemple) {#calculate-the-available-hours-and-fte-for-a-user-in-the-resource-planner-example}

Le tableau suivant illustre la manière dont les heures disponibles et l&#39;équivalent temps complet disponible sont calculés pour l&#39;utilisateur dans le planificateur de ressources en fonction de la méthode utilisée par l&#39;administrateur système pour le calcul de l&#39;équivalent temps complet dans les préférences de gestion des ressources.

Pour cet exemple, nous utilisons les chiffres suivants :

* Planning système par défaut de 40 heures
* Planning de l’utilisateur ou de l’utilisatrice de 20 heures
* Équivalent temps complet de l’utilisateur ou de l’utilisatrice de 0,8

| Méthode de calcul de l’équivalent temps complet (paramètre système) | **Heures du planning de l’utilisateur ou de l’utilisatrice** | **Heures du planning par défaut** | **Champ Équivalent temps complet de l’utilisateur ou de l’utilisatrice** | **Heures disponibles dans le planificateur de ressources** | **Équivalent temps complet disponible dans le planificateur de ressources** |
|---|---|---|---|---|---|
| **Planning par défaut** | Ignoré | 40 | 0,8 | **32** (calculé) | **0,8** |
| **Planning de l’utilisateur ou de l’utilisatrice** | 20 | 40 | Ignoré | **20** | **0,5** (calculé) |

Les exceptions de planning et les congés peuvent avoir une incidence sur le nombre d’heures prévues ou sur l’équivalent temps complet. Pour plus d’informations, voir [Configurer les préférences de gestion des ressources](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Exemple d’affichage du planificateur de ressource par utilisateur ou utilisatrice et par heures :

![Affichage du planificateur de ressources par utilisateur ou utilisatrice et par heures](assets/resource-planner-by-user-by-hours.png)

Exemple d’affichage du planificateur de ressources par utilisateur ou utilisatrice et par équivalent temps complet :

![Affichage du planificateur de ressources par utilisateur ou utilisatrice et par équivalent temps complet](assets/resource-planner-by-user-by-fte.png)

## Calculer toutes les autres valeurs d’heure et d’équivalent temps complet pour les utilisateurs et utilisatrices et les fonctions dans le planificateur de ressources {#calculate-all-other-hour-and-fte-values-for-users-and-job-roles-in-the-resource-planner}

Outre les heures disponibles ou l’équivalent temps complet, les informations temporelles suivantes s’affichent également dans le planificateur de ressources :

* Heures prévues
* Heures budgétées
* Écart d’heures
* Heures nettes\
  Pour plus d’informations, voir [Vue d’ensemble des informations sur les heures, les équivalents temps complet et les coûts dans les vues de Projet et Rôle du planificateur de ressources](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

* Différence d’heure\
  Pour plus d’informations, voir [Vue d’ensemble des informations sur les heures, les équivalents temps complet et les coûts dans les vues de Projet et Rôle du planificateur de ressources](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

Vous pouvez afficher dans le Planificateur de ressources les mêmes informations que l&#39;équivalent temps complet ou les heures.

Workfront utilise la formule suivante pour afficher toutes les autres valeurs sous forme d’équivalent temps complet dans le planificateur de ressources :

`FTE = Resource Planner Hours/ Default Schedule Hours`

>[!NOTE]
>
>Le planning de l&#39;utilisateur est ignoré lors du calcul de l&#39;équivalent temps complet pour toutes les valeurs, à l&#39;exception des valeurs d&#39;équivalent temps complet disponibles (AVL) dans le planificateur de ressources. Seul le planning par défaut est pris en compte pour le calcul.

Ce calcul s’applique aux valeurs suivantes :

* Équivalent temps complet prévu (PLN)
* Équivalent temps complet budgété (BDG)
* Variance de l’équivalent temps complet (VAR)
* Équivalent temps complet NET
* Différence d’équivalent temps complet (DIF)
