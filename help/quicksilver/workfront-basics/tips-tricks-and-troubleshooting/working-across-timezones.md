---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Utilisation des fuseaux horaires
description: 'Il peut s’avérer utile de comprendre comment [!DNL Adobe Workfront] utilise les fuseaux horaires pour calculer ce qui suit : EDIT ME.'
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: ecb6928c946203b03a93cf5687fd53abf8e6a8f3
workflow-type: tm+mt
source-wordcount: '1086'
ht-degree: 0%

---

# Utilisation des fuseaux horaires

Il peut s’avérer utile de comprendre comment [!DNL Adobe Workfront] utilise les fuseaux horaires pour calculer les éléments suivants :

* Champs temporels des objets
* Temps passé dans d&#39;autres [!DNL Workfront] zones, telles que les courriers électroniques Workfront automatisés

## Fuseaux horaires dans [!DNL Workfront]

Temps que vous voyez dans [!DNL Workfront] sont basés sur les configurations de fuseau horaire de votre entreprise. [!DNL Workfront] et pour votre profil utilisateur. Si ces deux fuseaux horaires sont différents, il se peut que vous constatiez des incohérences entre les heures dans les différentes zones et fonctionnalités que vous utilisez dans [!DNL Workfront].

>[!NOTE]
>
><div class="preview">Dans un formulaire personnalisé joint à un objet, les instructions de date et d’heure dans les champs personnalisés calculés sont calculées et enregistrées selon l’heure universelle coordonnée (UTC), et non selon les configurations de fuseau horaire définies pour l’instance de votre organisation et votre profil utilisateur. Les calculs dans un formulaire personnalisé sont générés et affichés en fonction des fuseaux horaires individuels de chaque utilisateur.</div>




* [Votre entreprise [!DNL Workfront] instance](#your-organization-s-workfront-instance)
* [Votre profil utilisateur](#your-user-profile)

### Votre entreprise [!DNL Workfront] instance {#your-organization-s-workfront-instance}

Le fuseau horaire de l’événement [!DNL Workfront] est généralement définie pour l’emplacement du bureau principal. Cela détermine les éléments suivants :

* L’heure affichée dans les emails générés par [!DNL Workfront]
* Le fuseau horaire des utilisateurs nouvellement ajoutés (avant le [!DNL Workfront] L’administrateur configure un fuseau horaire différent pour eux en fonction de l’endroit où ils travaillent)

   Pour plus d’informations sur ces deux exemples, voir [Configuration des informations de base pour votre système](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Début ou fin d’un taux de facturation remplacé pour un projet. Pour plus d’informations, voir [Remplacer les taux de facturation des rôles de tâche au niveau du projet](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Votre profil utilisateur {#your-user-profile}

Le fuseau horaire de votre profil utilisateur doit être configuré pour l’emplacement où vous travaillez. Cela détermine les éléments suivants :

* L’heure indiquée dans votre [!DNL Workfront] messages électroniques
* Heures pour un objet sur lequel vous travaillez, telles que les heures de début et de fin

   Si les utilisateurs de plusieurs fuseaux horaires sont affectés à un objet, [!DNL Workfront] convertit les heures de l’objet pour toutes les personnes impliquées, à l’aide du fuseau horaire configuré dans chaque profil utilisateur.

   **Exemple :** Dans le fuseau horaire de l’heure normale de l’Est (EST) où vous travaillez, vous définissez une tâche qui commencera à 16h00 et l’affectez aux utilisateurs du fuseau horaire de l’heure normale du Pacifique (PST). Pour ces utilisateurs, l’heure de début s’affiche à 13h00. S&#39;il devait l&#39;afficher à 16h00, il commencerait à travailler avec trois heures de retard.

   Si le créateur d’objets ne remarque pas la différence entre les fuseaux horaires des personnes désignées et effectue les ajustements nécessaires lors de la définition des heures de l’objet, ou si les personnes désignées ne remarquent pas cette différence, il peut être difficile d’obtenir le bon timing pendant que chacun collabore sur l’objet.

   **Exemple :** Vous configurez une tâche d’une journée pour qu’elle démarre à 9 heures HNE, en oubliant que certains utilisateurs de la tâche travaillent dans la zone PST. Pour eux, heure de début : 6h00. Comme ils ne commenceront pas à travailler dessus avant 9 heures (heure de midi), la tâche commence et se termine avec trois heures de retard.

Pour plus d’informations sur la configuration de votre fuseau horaire dans votre profil utilisateur, voir [Configurer mes paramètres](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Pour plus d’informations sur la manière dont une [!DNL Workfront] administrateur (ou une personne avec [!UICONTROL Modifier] l’accès aux utilisateurs) peut configurer le fuseau horaire dans un profil utilisateur, voir [Modification du profil d’un utilisateur](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Comment faciliter le travail des utilisateurs dans les fuseaux horaires

Vous pouvez aider les utilisateurs qui travaillent plus facilement dans plusieurs fuseaux horaires de différentes manières :

* [Utilisation des plannings](#use-schedules)
* [Utilisation de champs d’heure calculée dans un formulaire personnalisé](#use-calculated-time-fields-in-a-custom-form)
* [Utiliser des champs de texte au lieu de champs de date dans un formulaire personnalisé](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Utilisation des plannings {#use-schedules}

[!DNL Workfront] Les administrateurs créent des calendriers distincts pour chaque fuseau horaire de votre entreprise afin de s’assurer que le travail est planifié de manière appropriée pour tous, où qu’ils se trouvent. Une fois les planifications créées par l’administrateur, elles peuvent être associées à certains projets et utilisateurs :

* **[!UICONTROL Projets]**: Un créateur de projet peut sélectionner une planification pour un projet individuel. Cela détermine la planification des tâches dans le projet, en fonction des heures de travail définies pour les fuseaux horaires des personnes désignées.
* **[!UICONTROL Utilisateurs]**: A [!DNL Workfront] administrateur (ou une personne avec [!UICONTROL Modifier] l’accès aux utilisateurs) peut sélectionner un planning pour chaque utilisateur dans son profil.

   Ce planning peut différer de celui d’un projet. Par exemple, lorsqu’une personne crée une tâche dans le projet et qu’elle n’y a encore affecté personne, la tâche utilise le planning du projet. Lorsqu’un utilisateur est affecté à la tâche, la tâche utilise le planning de cet utilisateur.

   Si plusieurs utilisateurs sont affectés à une tâche, le système utilise l’un des éléments suivants, tel que configuré dans les préférences de projet à l’échelle du système :

   * Fuseau horaire du planning de l’Principal propriétaire de la tâche
   * Fuseau horaire du planning du projet.

   Cela peut entraîner la modification des dates des tâches.

   **Exemple :** Un utilisateur EST affecté à une tâche d’une journée planifiée pour commencer à 9 h 00 PST, qui est midi HNE. Comme il ne reste que 2 heures de travail pour l’utilisateur EST, la date d’achèvement de la tâche s’étend d’environ 6 heures au jour de travail suivant.

   Pour plus d’informations sur la variable [!UICONTROL Préférences du projet] area of [!UICONTROL Configuration], voir [Configuration des préférences de projet à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   Pour obtenir des instructions sur l’affectation d’une planification à un projet ou à un utilisateur, voir [Création d’un planning](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   Pour plus d’informations sur l’impact du fuseau horaire configuré dans votre planning sur la distribution de [!UICONTROL Heures planifiées] dans le [!UICONTROL Planification] et dans les [!DNL Workload Balancer], voir ce qui suit :

   * [Gestion des affectations d’utilisateurs dans [!UICONTROL Planification] area](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md)
   * [Gestion des affectations d’utilisateurs dans [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)



### Utilisation de champs d’heure calculée dans un formulaire personnalisé {#use-calculated-time-fields-in-a-custom-form}

Vous pouvez utiliser une série de champs personnalisés calculés sur un formulaire personnalisé pour afficher l’heure actuelle pour les utilisateurs de votre entreprise, comme une ligne d’horloges d’aéroport affichant l’heure dans plusieurs villes. Vous pouvez créer un champ pour chacun des fuseaux horaires dans lesquels travaillent vos utilisateurs, chacun calculant l’heure de son fuseau horaire.

Pour plus d’informations, voir [Ajout de données calculées à un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md), ainsi que la section [Champs personnalisés calculés par date et heure](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) dans l’article [Expressions de données calculées](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Utiliser des champs de texte au lieu de champs de date dans un formulaire personnalisé {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Si tu ne veux pas [!DNL Workfront] pour convertir les heures configurées dans un objet pour les utilisateurs de différents fuseaux horaires, vous pouvez utiliser un champ de texte dans un formulaire personnalisé que vous joignez à un objet, plutôt qu’un champ de date. Ainsi, l’heure affiche l’heure que vous tapez pour tous les membres du projet.

Dans ce cas, nous vous recommandons de rappeler aux utilisateurs du formulaire de calculer la différence entre leur fuseau horaire et le vôtre afin qu’ils puissent déterminer quand le travail doit commencer et se terminer. Vous pouvez l’inclure dans les instructions que vous saisissez pour le formulaire personnalisé ou dans une info-bulle pour ce champ. Pour plus d’informations, voir [Ajouter un champ personnalisé à un formulaire personnalisé](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
