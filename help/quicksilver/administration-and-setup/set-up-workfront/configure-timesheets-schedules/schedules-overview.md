---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: user,schedule
navigation-topic: configure-timesheets-and-schedules
title: Présentation des planifications
description: Vous pouvez définir votre semaine de travail à l’aide de plannings. Vous pouvez associer un planning à un utilisateur ou à un projet. Cela permet [!DNL Adobe Workfront] pour calculer les chronologies et la disponibilité de l’utilisateur. Pour plus d’informations, voir Création d’un planning.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# Présentation des planifications

Vous pouvez définir votre semaine de travail à l’aide de plannings et associer un planning à un utilisateur ou à un projet. Cela permet [!DNL Adobe Workfront] pour calculer les chronologies et la disponibilité de l’utilisateur. Pour obtenir des instructions, voir [Création d’un planning](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Tenez compte des points suivants lorsque vous utilisez des plannings dans Workfront :

* Le [!DNL Workfront] L’administrateur identifie les heures d’opération pour l’organisation dans un planning.

   De même, un administrateur de groupe peut identifier les heures de fonctionnement d’un planning géré par un groupe qu’il gère.

   Pour plus d’informations sur les administrateurs de groupe, voir [Administrateurs de groupe](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

   Par exemple, un planning peut être défini comme suit : Du lundi au vendredi, de 8 h à 17 h, avec une pause d&#39;une heure pour le déjeuner.

* [!DNL Workfront] utilise le planning pour déterminer quand la journée de travail commence et se termine.

   Cela n’empêche pas un utilisateur de travailler ou d’effectuer un travail dans [!DNL Workfront] en dehors des heures de bureau normales. En règle générale, il n’est pas nécessaire de créer un nouveau planning ou une exception de planning pour se concentrer sur les travaux prévus le soir.

   De même, votre entreprise peut avoir des horaires d’arrivée flexibles pour votre journée de travail. Vous pouvez avoir un groupe d’employés qui arrive à 8 heures et un autre groupe qui arrive à 9 heures. Il n’est pas nécessaire de créer des plannings uniques pour chaque groupe, si les groupes ont des plannings similaires ou identiques. Mais si les groupes ont des plannings radicalement différents, leurs utilisateurs doivent être associés à des plannings uniques. Un employé comprend si une tâche doit être terminée à 17 heures, cela signifie que le travail doit être effectué avant la fin de la journée de travail, quelle que soit l’heure à laquelle il entre au travail.

* Nous vous recommandons de créer des plannings distincts pour chaque fuseau horaire associé à l’organisation.

   Vous pouvez affecter un fuseau horaire spécifique à chaque planification afin de vous assurer que le travail est planifié de manière appropriée pour les utilisateurs qui travaillent dans différents fuseaux horaires.

* Le [!DNL Workfront] La planification par défaut est utilisée dans les calculs de chronologie lorsque les utilisateurs ou les projets ne sont pas associés à une planification.

   La planification par défaut est fournie avec votre [!DNL Workfront] et ne peuvent pas être supprimés à moins qu’il ne soit remplacé par un nouveau planning que vous créez.

* En plus du calcul des chronologies, [!DNL Workfront] utilise des plannings pour calculer la disponibilité des utilisateurs.

   >[!IMPORTANT]
   >
   >[!DNL Workfront] utilise l’utilisateur ou le planning du projet pour déterminer la disponibilité des ressources dans le planificateur de ressources. La planification utilisée dépend de ce que la variable [!DNL Workfront] l’administrateur sélectionné pour le [!UICONTROL Calcul de la disponibilité des ressources à l’aide de] . Pour plus d’informations sur les paramètres de gestion des ressources, voir [Configuration des préférences de gestion des ressources](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Hiérarchie des plannings

Si une tâche est assignée à un utilisateur associé à un planning et réside sur un projet associé à un second planning, au moins deux plannings peuvent éventuellement être appliqués à vos calculs de frise chronologique.

>[!IMPORTANT]
>
>[!DNL Workfront] utilise le planning d’un utilisateur uniquement lorsque la variable [!UICONTROL Calcul de la disponibilité des ressources à l’aide de] est défini sur [!UICONTROL Planification de l’utilisateur] dans le [!UICONTROL Gestion des ressources] area of [!UICONTROL Configuration]. Pour plus d’informations sur la manière dont la variable [!UICONTROL Calcul de la disponibilité des ressources à l’aide de] affecte le planning utilisé pour la gestion des ressources, voir [Configuration des préférences de gestion des ressources](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

L’ordre dans lequel les planifications sont utilisées par le système lorsqu’il en existe plusieurs est le suivant :

* Lorsqu’un utilisateur est affecté à une tâche, [!DNL Workfront] utilise le planning de l’utilisateur pour calculer la chronologie de la tâche. Cela inclut également l’heure personnelle de l’utilisateur. Le planning du projet est ignoré.

   Pour plus d’informations sur le temps personnel, voir [Configuration du temps de connexion personnel [!DNL Adobe Workfront]](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Lorsque plusieurs utilisateurs sont affectés à une tâche et que les utilisateurs ont des plannings différents pendant la période de la tâche, [!DNL Workfront] utilise l’un des plannings suivants, comme défini dans la variable [!UICONTROL Préférences du projet] area of [!UICONTROL Configuration]:

   * Planification de l’utilisateur désigné comme cessionnaire Principal
   * Planning associé au projet.

      Pour plus d’informations sur les préférences du projet, voir [Configuration des préférences de projet à l’échelle du système](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si l’utilisateur affecté à la tâche n’a pas de planning, ou si la tâche n’est affectée qu’à un rôle de tâche, à une équipe ou est non affectée, [!DNL Workfront] utilise le planning du projet pour les calculs de la chronologie.
* Si l’utilisateur affecté à la tâche n’a pas de planning, ou si la tâche est affectée uniquement à un rôle de tâche, à une équipe ou est non affectée et que le projet n’a pas de planning, alors [!DNL Workfront] utilise la planification dans le système désigné comme planification par défaut pour les calculs de chronologie.

   ![](assets/default-schedule.png)

## Collaboration dans [!DNL Workfront] à travers les fuseaux horaires

Pour plus d’informations sur l’utilisation des plannings pour aider les utilisateurs à collaborer dans [!DNL Workfront] à travers les fuseaux horaires, voir [Utilisation des fuseaux horaires](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
