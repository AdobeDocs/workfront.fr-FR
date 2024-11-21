---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: utilisateur ou utilisatrice,planning
navigation-topic: configure-timesheets-and-schedules
title: Présentation des planifications
description: Vous pouvez définir votre semaine de travail en utilisant des plannings. Vous pouvez associer un planning à une personne ou à un projet. Cela permet à  [!DNL Adobe Workfront]  de calculer les chronologies et la disponibilité des personnes. Pour savoir obtenir des instructions, voir Créer un planning.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 99%

---

# Vue d’ensemble des plannings

<!-- Audited: 1/2024 -->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  

-->

Vous pouvez définir votre semaine de travail à l’aide de plannings et associer un planning à une personne ou à un projet. Cela permet à [!DNL Adobe Workfront] de calculer les chronologies et la disponibilité des utilisateurs et utilisatrices. Pour obtenir des instructions, voir [Créer un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Tenez compte des points suivants lorsque vous travaillez avec des plannings dans Workfront :

* L’équipe d’administration [!DNL Workfront] définit les heures d’ouverture de l’entreprise dans un planning.

  De même, une équipe d’administration de groupes peut identifier les heures d’ouverture d’un planning administré par un groupe qu’elle gère. Pour plus d’informations sur les administrateurs et administratrices de groupes, voir [Équipes d’administration de groupes](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Par exemple, un planning peut être défini comme suit : du lundi au vendredi, de 8 heures à 17 heures, avec une heure de pause pour le déjeuner.

* [!DNL Workfront] utilise le planning pour déterminer le début et la fin de la journée de travail.

  Cela n’empêche pas une personne de travailler ou de terminer son travail sur [!DNL Workfront] en dehors des heures normales de travail. En général, il n’est pas nécessaire de créer un planning ou une exception de planning pour se concentrer sur le travail prévu le soir.

  De même, votre entreprise peut prévoir des heures d’arrivée flexibles pour votre journée de travail. Vous pouvez avoir un groupe de personnes membres du personnel qui arrive à 8 heures et un autre qui arrive à 9 heures. Il n’est pas nécessaire de créer des plannings uniques pour chaque groupe si les groupes ont des horaires similaires ou identiques. Mais si les groupes ont des horaires radicalement différents, les personnes doivent être associées à des plannings uniques. Une personne membre du personnel comprend que si une affectation doit être terminée à 17 heures, cela signifie que le travail doit être effectué avant la fin de la journée de travail, quelle que soit l’heure d’arrivée au travail.

* Nous vous recommandons de créer des plannings distincts pour chaque fuseau horaire associé à l’entreprise.

  Vous pouvez attribuer un fuseau horaire spécifique à chaque planning afin de vous assurer que le travail est planifié de manière appropriée pour les personnes qui travaillent dans des fuseaux horaires différents.

* Le planning par défaut [!DNL Workfront] est utilisé dans les calculs de chronologies lorsque les personnes ou les projets ne sont pas associés à un planning.

  Le planning par défaut est fourni avec votre système [!DNL Workfront] et ne peut pas être supprimé à moins d’être remplacé par un nouveau planning que vous créez.

* Outre le calcul des chronologies, [!DNL Workfront] utilise les plannings pour calculer la disponibilité des personnes.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] utilise le planning de la personne ou le planning du projet pour déterminer la disponibilité des ressources dans le planificateur de ressources. Le planning utilisé dépend de ce que l’équipe d’administration [!DNL Workfront] a sélectionné pour le paramètre [!UICONTROL Calculer la disponibilité des ressources avec]. Pour plus d’informations sur les paramètres de la gestion des ressources, voir [Configurer les préférences de la gestion des ressources](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Hiérarchie des plannings

Si une tâche est affectée à une personne associée à un planning et qu’elle se trouve sur un projet associé à un deuxième planning, vous avez au moins deux plannings qui peuvent potentiellement être appliqués à vos calculs de chronologies.

>[!IMPORTANT]
>
>[!DNL Workfront] utilise le planning d’une personne uniquement lorsque le paramètre [!UICONTROL Calculer la disponibilité des ressources avec] est défini sur [!UICONTROL Planning de la personne] dans la zone [!UICONTROL Gestion des ressources] de la [!UICONTROL Configuration]. Pour plus d’informations sur la manière dont le paramètre [!UICONTROL Calculer la disponibilité des ressources avec] affecte le planning utilisé pour la gestion des ressources, voir [Configurer les préférences pour la gestion des ressources](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

L’ordre dans lequel les plannings sont utilisés par le système lorsqu’il en existe plusieurs est le suivant :

<!--Replace the first bullet below with this when the setting releases: 
* When one user is assigned to a task, the following scenarios exist, depending on what environment you use: 

   * In the Production environment, [!DNL Workfront] uses the user's schedule for calculating the timeline of the task. This also includes the personal time of the user. The schedule of the project is ignored.

      For more information about personal time, see [Configure personal time off](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

   * <span class="preview">In the Preview environment, [!DNL Workfront] uses either one of the following schedules, as defined in the [!UICONTROL Project Preferences] area of [!UICONTROL Setup]:</span>

      * <span class="preview">The schedule of the user who is assigned to the task </span>
      * <span class="preview">The schedule associated with the project.</span>

-->

* Lorsqu’une personne est affectée à une tâche, [!DNL Workfront] utilise le planning de la personne pour calculer la chronologie de la tâche. Cela comprend également le temps personnel de la personne. Le planning du projet n’est pas pris en compte.

  Pour plus d’informations sur le temps libre, voir [Configurer les congés personnels](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Lorsque plusieurs personnes sont affectées à une tâche et ont des horaires différents pendant la durée de la tâche, [!DNL Workfront] utilise l’un des plannings suivants, tels que définis dans la zone [!UICONTROL Préférences du projet] de la [!UICONTROL Configuration] :

   * Planning de la personne désignée comme personne cessionnaire principale.
   * Planning associé au projet.

     Pour plus d’informations sur les préférences de projet, voir [Configurer les préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si la personne affectée à la tâche n’a pas de planning, ou si la tâche est affectée uniquement à une fonction, à une équipe ou n’est pas assignée, alors [!DNL Workfront] utilise le planning du projet désigné comme le planning par défaut pour les calculs des chronologies.
* Si la personne affectée à la tâche n’a pas de planning, ou si la tâche est affectée uniquement à une fonction, à une équipe ou n’est pas assignée, et que le projet n’a pas de planning, alors [!DNL Workfront] utilise le planning du système désigné comme le planning par défaut pour les calculs des chronologies.

  ![](assets/default-schedule.png)

## Collaboration dans [!DNL Workfront] avec les fuseaux horaires

Pour plus d’informations sur l’utilisation des plannings pour aider les personnes à collaborer dans [!DNL Workfront] avec des fuseaux horaires, voir [Travailler avec des fuseaux horaires](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
