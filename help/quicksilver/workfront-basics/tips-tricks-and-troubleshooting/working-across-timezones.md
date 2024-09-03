---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Travailler sur plusieurs fuseaux horaires
description: Il peut être utile de comprendre comment  [!DNL Adobe Workfront]  utilise les fuseaux horaires pour calculer les champs horaires des objets et les heures dans d’autres domaines tels que les e-mails.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 97%

---

# Travailler sur plusieurs fuseaux horaires

<!-- Audited: 2/2024 -->

Il peut être utile de comprendre comment [!DNL Adobe Workfront] utilise les fuseaux horaires pour calculer les éléments suivants :

* Champs horaires pour les objets
* Délais dans d’autres zones [!DNL Workfront], tels que les e-mails automatisés Workfront

>[!WARNING]
>
>Si vous ne trouvez pas votre fuseau horaire exact dans la liste que nous proposons, recherchez le fuseau horaire le plus proche du vôtre et mettez-le à jour pour votre instance.
>
>Sachez également qu’un fuseau horaire similaire peut ne pas correspondre parfaitement au vôtre.
>
>Par exemple, certains pays ou territoires peuvent observer l’heure d’été, mais pas votre pays. Si nécessaire, vous devrez peut-être ajuster les fuseaux horaires de votre système en fonction de ces modifications.


## Fuseaux horaires dans [!DNL Workfront]

Les heures affichées sur [!DNL Workfront] sont basées sur les configurations des fuseaux horaires de l’instance [!DNL Workfront] de votre organisation et de votre profil d’utilisateur ou d’utilisatrice. Si ces deux fuseaux horaires sont différents, il se peut que vous constatiez des décalages horaires dans différentes zones et fonctions que vous utilisez sur [!DNL Workfront].

>[!NOTE]
>
>Dans un formulaire personnalisé joint à un objet, les instructions de date et d’heure dans les champs personnalisés calculés sont traitées et enregistrées en fonction du temps universel coordonné (UTC), et non en fonction des configurations de fuseau horaire définies pour l’instance de votre organisation et votre profil d’utilisateur ou d’utilisatrice. Les calculs d’un formulaire personnalisé sont générés et affichés en fonction des fuseaux horaires de chaque utilisateur ou utilisatrice.

* [Instance  [!DNL Workfront]  de votre organisation](#your-organization-s-workfront-instance)
* [Votre profil d’utilisateur ou d’utilisatrice](#your-user-profile)

### Instance [!DNL Workfront] de votre organisation {#your-organization-s-workfront-instance}

Le fuseau horaire de l’instance [!DNL Workfront] de votre organisation est généralement défini en fonction de l’emplacement du bureau principal. Cette fonctionnalité permet de déterminer les éléments suivants :

* L’heure indiquée dans les e-mails générés par [!DNL Workfront]
* Le fuseau horaire des utilisateurs et utilisatrices nouvellement ajoutés (avant que l’administration de [!DNL Workfront] ne configure un fuseau horaire différent pour eux en fonction de leur lieu de travail).

  Pour plus d’informations sur ces deux exemples, voir [Configurer les informations de base de votre système](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Le début ou la fin d’un taux de facturation dérogatoire pour un projet. Pour plus d’informations, voir [Remplacer les taux de facturation des fonctions à l’échelle d’un projet](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Votre profil d’utilisateur ou d’utilisatrice {#your-user-profile}

Le fuseau horaire de votre profil d’utilisateur ou d’utilisatrice doit être configuré en fonction de votre lieu de travail. Cette fonctionnalité permet de déterminer les éléments suivants :

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Horaires d’un objet sur lequel vous travaillez, tels que les heures de début et de fin.

  Si des utilisateurs et utilisatrices situés dans plusieurs fuseaux horaires sont affectés à un objet, [!DNL Workfront] convertit les heures de l’objet pour toutes les personnes concernées grâce au fuseau horaire configuré dans chaque profil d’utilisateur ou d’utilisatrice.

  **Exemple :** dans la zone d’heure normale de l’Est (EST) où vous travaillez, vous définissez une tâche qui doit commencer à 16 h 00 et l’assignez aux utilisateurs et utilisatrices travaillant dans la zone d’heure normale du Pacifique (PST). Pour ces utilisateurs et utilisatrices, l’heure de début s’affiche à 13 h 00. Si elle affichait 16 h 00, ils commenceraient à travailler avec trois heures de retard.

  Si la personne qui a créé l’objet ne remarque pas la différence entre les fuseaux horaires des personnes cessionnaires et n’effectue pas les ajustements nécessaires lors de la définition des heures de l’objet, ou si les personnes cessionnaires ne relèvent pas cette différence, il peut être difficile d’obtenir le bon timing alors que tout le monde collabore sur l’objet.

  **Exemple :** vous configurez une tâche d’une journée pour qu’elle commence à 9 h 00 EST, mais oubliez que certains utilisateurs et utilisatrices de la tâche travaillent dans la zone PST. Pour eux, l’heure de début est 6 h 00. Comme ils ne commenceront pas à travailler avant 9 h 00 dans leur fuseau horaire (midi dans le vôtre), la tâche commence et se termine avec trois heures de retard.

Pour plus d’informations sur la configuration de votre fuseau horaire dans votre profil d’utilisateur ou d’utilisatrice, voir [Configurer mes paramètres](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Pour plus d’informations sur la manière dont un administrateur ou une administratrice de [!DNL Workfront] (ou une personne ayant un accès [!UICONTROL Modifier] aux utilisateurs et utilisatrices) peut configurer le fuseau horaire dans le profil d’une personne, voir [Modifier le profil d’un utilisateur ou d’une utilisatrice](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Comment faciliter le travail des utilisateurs et utilisatrices sur les différents fuseaux horaires ?

Vous pouvez aider les utilisateurs et utilisatrices à travailler plus facilement sur plusieurs fuseaux horaires de différentes manières :

* [Utiliser les plannings](#use-schedules)
* [Utiliser des champs d’heure calculés dans un formulaire personnalisé](#use-calculated-time-fields-in-a-custom-form)
* [Utiliser des champs de texte au lieu de champs de date dans un formulaire personnalisé](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Utiliser les plannings {#use-schedules}

Les administrateurs et administratrices de [!DNL Workfront] créent des plannings distincts pour chaque fuseau horaire au sein de votre organisation afin de garantir que le travail est planifié de manière appropriée pour toutes les personnes concernées, où qu’elles se trouvent. Une fois que l’administrateur ou l’administratrice a créé les plannings, ceux-ci peuvent être associés à certains projets ainsi qu’aux utilisateurs et utilisatrices :

* **[!UICONTROL Projets]** : un créateur ou une créatrice de projet peut sélectionner un calendrier pour un projet individuel. Cette fonctionnalité détermine la planification des tâches dans le projet, en fonction des heures de travail définies pour les fuseaux horaires des personnes cessionnaires.
* **[!UICONTROL Utilisateurs et utilisatrices]** : un administrateur ou une administratrice de [!DNL Workfront] (ou une personne ayant un accès [!UICONTROL Modifier] aux utilisateurs et utilisatrices) peut sélectionner un planning pour une personne dans le profil de l’utilisateur ou de l’utilisatrice.

  Ce planning peut être différent de celui d’un projet. Par exemple, lorsqu’une personne crée une tâche dans le projet, mais n’y a encore affecté personne, la tâche utilise le planning du projet. Lorsqu’une personne est affectée à la tâche, celle-ci utilise le planning de cette personne.

  Si plusieurs utilisateurs et utilisatrices sont affectés à une tâche, le système utilise l’une des options suivantes, conformément à la configuration des préférences du projet à l’échelle du système :

   * Le fuseau horaire pour le planning de la personne propriétaire principale de la tâche.
   * Le fuseau horaire pour le planning du projet.

  Cela peut entraîner une modification des dates des tâches.

  **Exemple :** une personne EST est affectée à une tâche d’une journée dont le début est prévu à 9 h 00 PST, soit midi EST. Comme il ne reste à la personne EST que deux heures de travail pour la journée, la date d’achèvement de la tâche est reportée d’environ six heures au jour ouvrable suivant.

  Pour plus d’informations sur la zone [!UICONTROL Préférences du projet] dans [!UICONTROL Configuration], consultez [Configurer les préférences de projet à l’échelle du système](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  Pour plus d’informations sur l’affectation d’un planning à un projet ou à une personne, consultez [Créer un planning](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  Pour plus d’informations sur la façon dont le fuseau horaire configuré dans votre planning affecte la distribution du [!UICONTROL nombre d’heures prévues] dans l’[!UICONTROL équilibreur de charge de travail], consultez [Gérer les affectations des personnes dans l’[!UICONTROL équilibreur de charge de travail]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Utiliser des champs d’heure calculés dans un formulaire personnalisé {#use-calculated-time-fields-in-a-custom-form}

Vous pouvez utiliser une série de champs personnalisés calculés dans un formulaire personnalisé pour afficher l’heure pour les personnes de votre organisation, comme une rangée d’horloges d’aéroport affichant l’heure dans plusieurs villes. Vous pouvez créer un champ pour chacun des fuseaux horaires dans lesquels travaillent vos personnes, chacun calculant l’heure pour son fuseau horaire.

Pour plus d’informations, voir [Ajout de champs calculés à un formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md), ainsi que la section [ Champs personnalisés calculés par date et heure](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) de l’article [Présentation des expressions de données calculées](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Utiliser des champs de texte au lieu de champs de date dans un formulaire personnalisé {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Si vous ne souhaitez pas que [!DNL Workfront] convertisse les heures configurées dans un objet pour des personnes situées dans des fuseaux horaires différents, vous pouvez utiliser un champ de texte dans un formulaire personnalisé que vous attachez à un objet, plutôt qu’un champ de date. De cette façon, l’heure affiche l’heure que vous saisissez pour toutes les personnes qui participent au projet.

Dans ce cas, nous vous recommandons de rappeler aux utilisateurs et utilisatrices du formulaire de calculer la différence entre leur fuseau horaire et le vôtre afin qu’ils puissent déterminer les heures de début et de fin du travail. Vous pouvez l’inclure dans les instructions que vous saisissez pour le formulaire personnalisé ou dans une info-bulle pour ce champ. Pour plus d’informations, voir [Concevoir un formulaire avec le créateur de formulaire](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
