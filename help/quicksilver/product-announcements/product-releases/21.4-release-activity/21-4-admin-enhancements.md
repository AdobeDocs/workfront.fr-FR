---
title: Améliorations apportées aux administrateurs et administratrices (version 21.4)
description: Améliorations apportées aux administrateurs et administratrices (version 21.4)
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 100%

---

# Améliorations apportées aux administrateurs et administratrices (version 21.4)

Cette page décrit toutes les améliorations pour les administrateurs et administratrices apportées à l’environnement de prévisualisation dans la version 21.4. Ces améliorations sont disponibles dans l’environnement de production à partir de la semaine du 4 octobre 2021.

Pour obtenir la liste de toutes les modifications introduites par la version 21.4, consultez la section [Vue d’ensemble de la version 21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Pour les administrateurs et administratrices : voir les groupes associés à un processus d’approbation

Pour vous aider à déterminer les groupes qui sont associés aux processus d’approbation de votre système, nous avons ajouté une colonne Nom de groupe à la vue Standard sur la page Approbations dans Configuration. Vous pouvez désormais afficher ces informations sans avoir à créer une vue personnalisée.

Pour plus d’informations sur les processus d’approbation, voir [Vue d’ensemble du processus d’approbation](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Pour plus d’informations sur la gestion des processus d’approbation de groupe, voir [Processus de validation au niveau du groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Nouveau pour les administrateurs et administratrices : les groupes peuvent configurer leurs propres préférences de feuille de temps et d’heure.

>[!NOTE]
>
>Au départ, en production, cette fonctionnalité sera disponible dans le cadre d’un déploiement échelonné uniquement pour la clientèle sur le cluster 4. Cette note sera mise à jour au fur et à mesure que les fonctionnalités seront disponibles pour d’autres clusters.

Dans une grande organisation, certains groupes peuvent avoir besoin de configurer les préférences des feuilles de temps et des heures de manière indépendante pour les adapter à leurs workflows uniques, plutôt que d’hériter des préférences configurées par une équipe d’administration au niveau du système. Désormais, l’équipe d’administration de Workfront peut déverrouiller les préférences en matière de feuilles de temps et d’heures pour tous les groupes du système afin qu’ils puissent les configurer.

Cette possibilité a également été ajoutée récemment pour les préférences de projet et pour celles de tâches et de problèmes.

Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront déverrouille une préférence de feuille de temps et d’heure, consultez la section [Déverrouiller les préférences des feuilles de temps et des heures pour les groupes](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) dans l’article [Configuration des préférences de feuilles de temps et des heures](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Pour plus d’informations sur la façon dont un administrateur ou une administratrice de groupe configure les préférences de tâche déverrouillée et de problème pour un groupe, voir [Configurer les préférence de feuilles de temps et d’heures pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Nouveau pour les administrateurs et administratrices de Workfront : Configurer des modèles de mise en page pour les personnes auto-allouées dans la nouvelle expérience Workfront

Vous pouvez maintenant configurer des modèles de mise en page dans la nouvelle expérience Workfront pour les personnes auto-allouées. Dans le menu déroulant Attribut utilisateur Workfront, dans lequel vous mappez les attributs utilisateur (Configuration > Système > Authentification unique), un nouvel élément de menu « Modèle de mise en page NWE » est désormais disponible pour effectuer cette configuration. Auparavant, vous pouviez configurer des modèles de mise en page pour les personnes auto-allouées uniquement dans Workfront Classic.

Pour plus d’informations sur le mappage des attributs, voir [Mapper les attributs de l’utilisateur ou de l’utilisatrice et auto-allouer de nouvelles personnes](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## Le nouveau champ affiche les groupes auxquels vos utilisateurs et utilisatrices appartiennent.

Il est maintenant facile de déterminer à quels groupes vos utilisateurs et utilisatrices appartiennent. Dans un rapport ou une vue qui répertorie les utilisateurs et utilisatrices, vous pouvez créer une colonne à l’aide du nouveau champ Autres groupes. Ce champ répertorie les groupes dont chaque personne est membre.

Pour plus d’informations sur l’utilisation des rapports et des vues, voir [Créer un rapport personnalisé](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) et [Vue d’ensemble des vues dans Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## La page de détails des plans directeurs affiche désormais une image.

La page de détails de chaque plan directeur affiche désormais une image du modèle de projet installé avec le plan directeur. L’image fournit un aperçu du contenu du plan directeur afin que vous sachiez ce que vous êtes sur le point d’installer. Vous pouvez éventuellement prévisualiser l’image complète dans le navigateur ou télécharger l’image.

Pour plus d’informations, consultez [Vue d’ensemble des plans directeurs](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## Préférences des plans directeurs pour les nouveaux problèmes

De nouvelles préférences de problème sont désormais disponibles pour certains plans directeurs. Elles sont installées par défaut, mais vous pouvez choisir de ne pas les installer lorsque vous configurez les détails de l’installation.

Les préférences incluent les groupes de rubriques de file d’attente, les rubriques de file d’attente et les règles de routage pour collecter les informations correctes lorsqu’un problème ou une demande est soumis, et envoyer le problème ou la demande à la fonction ou à l’équipe appropriée. L’utilisation des préférences permet de créer une cohérence dans la manière dont les nouveaux problèmes ou demandes sont capturés sur vos projets.

Notez que l’utilisation de ces préférences ne transforme pas les projets créés à partir du modèle en files d’attente des demandes.

Pour plus d’informations, voir [Configurer un plan directeur](../../../administration-and-setup/blueprints/configure-template-package.md).

## Nouveau pour les administrateurs et administratrices de groupe : afficher et gérer les éléments récemment supprimés et restaurés d’un groupe

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Nous continuons à simplifier la gestion de vos groupes et de leurs objets associés en un seul endroit. Vous pouvez désormais afficher et utiliser les éléments récemment supprimés et restaurés d’un groupe dans la zone Groupes. Cela vous évite d’avoir à accéder à la zone Récemment supprimés ou Récemment restaurés dans Configuration pour gérer ces éléments. Et la liste des éléments de groupe avec lesquels vous travaillez est conservée séparément des autres éléments supprimés et restaurés dans le système.

Pour plus d’informations, voir [Afficher et gérer les éléments récemment supprimés d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) et [Afficher et gérer les éléments récemment restaurés d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## Nouveauté pour les administrateurs et administratrices de groupe : les préférences de groupe affectent désormais les modèles de groupe.

Il est désormais plus facile de vous assurer que les modèles de projet de votre groupe répondent aux besoins de votre groupe. Lorsque vous attribuez un nouveau modèle de projet à un groupe au moment de sa création, celui-ci hérite des paramètres suivants des préférences de projet et de tâche du groupe :

* Méthode d&#39;indice de performances
* Type de condition
* Planifier à partir de
* Congés de l’utilisateur ou de l’utilisatrice
* Type de mise à jour
* Paramètres de la section Accès

Lorsque vous créez une tâche de modèle dans un modèle de projet associé à un groupe, la tâche de modèle hérite des paramètres suivants des préférences de tâche du groupe :

* Type de durée
* Type de revenus
* Type de coût

Auparavant, les modèles de projet et les tâches de modèle de projet héritaient de ces paramètres des préférences de projet et de tâche définies au niveau du système.

Si vous créez un modèle ou une tâche de modèle sans groupe (par exemple, à partir de la page Modèles principale), les paramètres ci-dessus sont hérités des préférences de projet et de tâche au niveau du système. Cependant, si vous attribuez par la suite un groupe au modèle ou à la tâche de modèle, les préférences du groupe ne l’affectent pas.

Pour plus d’informations, voir la section Comment les préférences s’appliquent aux modèles et aux tâches de modèle dans l’article [Créer et modifier des modèles de projet d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Nouveauté pour les administrateurs et administratrices : découvrir quels formulaires personnalisés utilisent un champ personnalisé

Il est désormais plus facile de modifier un champ personnalisé dans un formulaire personnalisé. En un seul clic dans le formulaire personnalisé, vous pouvez découvrir d’autres formulaires personnalisés qui utilisent également le champ. Il est important d’évaluer si ces formulaires devront être ajustés afin de continuer à fonctionner correctement après avoir apporté la modification.

Pour plus d’informations, voir [Afficher tous les formulaires personnalisés qui utilisent un champ personnalisé ou un widget particulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## Nouveauté pour les administrateurs et administratrices de groupe : verrouillage et déverrouillage des préférences de projet, de tâche et de problème pour un groupe

Vous pouvez maintenant vous assurer que tous les membres des sous-groupes situés sous votre groupe utilisent les mêmes paramètres de préférence ou vous pouvez leur permettre de configurer un paramètre de préférence pour leurs workflows uniques.

* Une fois qu’un administrateur ou une administratrice Workfront a déverrouillé une préférence au niveau du système, vous pouvez la configurer, puis la verrouiller pour tous les sous-groupes situés sous votre groupe. Bien que vous puissiez toujours reconfigurer la préférence verrouillée, les administrateurs et administratrices des sous-groupes inférieurs ne peuvent pas le faire pour leurs groupes.

  Inversement, vous pouvez déverrouiller une préférence pour votre groupe. Cela permet aux administrateurs et administratrices de sous-groupes de la configurer pour répondre aux besoins uniques de leurs utilisateurs et utilisatrices en termes de workflows de projet, de tâche ou de problème.

  Pour plus d’informations, voir [Verrouiller ou déverrouiller une préférence de projet, de tâche ou de problème pour les sous-groupes](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* Si vous êtes administrateur ou administratrice Workfront, vous n’avez pas besoin d’accéder à la zone Groupes pour configurer les préférences d’un sous-groupe. Dans la zone principale Préférences du projet, Préférences des tâches et des problèmes ou Préférences des feuilles de temps et des heures, vous pouvez utiliser la zone de recherche située en haut de la page pour trouver le sous-groupe et configurer ses préférences.

  Pour plus d’informations, voir [Configurer les préférences de projet pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) et [Configurer les préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Nouveauté pour les administrateurs et administratrices de groupe  : créer et modifier des modèles à partir de la zone Groupes

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Workfront.

Nous continuons à faciliter la gestion de vos groupes et de leurs objets associés au même endroit. Vous pouvez désormais afficher et utiliser les modèles d’un groupe à partir de la zone Groupes dans la configuration. Cela vous évite d’avoir à accéder à la zone Modèles pour gérer les modèles d’un groupe. Et cela permet de conserver la liste des modèles de groupe sur lesquels vous travaillez séparément des autres dans le système.

Pour plus d’informations, voir [Créer et modifier des modèles de projet d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Saisir et enregistrer des informations dans un seul formulaire personnalisé joint à la fois

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Il est désormais plus facile de fournir des informations dans la section Détails d’un objet : saisissez et enregistrez les informations dans un champ personnalisé unique ou une zone extensible (comme Vue d’ensemble et Finance), même si les champs requis dans d’autres formulaires personnalisés de l’objet ne sont pas encore remplis.

Auparavant, lorsque vous saisissiez des informations dans un formulaire personnalisé ou une zone extensible pour un objet, tous les formulaires personnalisés joints à l’objet passaient en mode de modification et tous leurs champs obligatoires devaient être renseignés avant que vous puissiez enregistrer vos modifications. Il s’agissait d’un problème si vous ne pouviez pas remplir un champ obligatoire, car il était destiné à un autre utilisateur ou une autre utilisatrice.

Si vous souhaitez modifier tous les formulaires personnalisés et toutes les zones déroulantes de la section Détails d’un objet, vous pouvez cliquer sur Modifier tout dans le nouveau menu Modifier que nous avons ajouté à l’icône Modifier. Ou, dans le même menu, vous pouvez cliquer sur un nom pour accéder au formulaire personnalisé ou à la section que vous souhaitez modifier.

>[!NOTE]
>
>Cette fonctionnalité a été initialement lancée en prévisualisation avec la version 21.3.

Afin de faciliter la gestion et le contrôle indépendants des workflows pour tous les niveaux d’une organisation, nous avons introduit la possibilité de créer et de gérer des statuts pour les sous-groupes. Désormais, la section Groupes de la Configuration permet d’effectuer les opérations suivantes pour les groupes que vous administrez, quel que soit le niveau :

* Créer, modifier, supprimer et masquer le statut d’un groupe.
* Verrouiller le statut d’un groupe afin que tous les sous-groupes inférieurs puissent l’utiliser de la même manière.
* Déverrouiller un statut pour n’importe quel groupe afin que les administrateurs et administratrices des sous-groupes inférieurs puissent le personnaliser en fonction de leurs besoins uniques.
* Définir le statut d’un groupe comme statut par défaut.
* Réorganiser et masquer l’affichage des statuts de groupe sur les objets.

Les administrateurs et administratrices de Workfront peuvent également effectuer ces opérations (pour tous les groupes).

Auparavant, cette fonctionnalité n’était disponible que pour les groupes de niveau supérieur.

Pour plus d’informations, voir [Gérer les statuts de groupe](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Nouveau pour les administrateurs et administratrices Workfront : migrez vous-même les modèles de mise en page de Workfront Classic vers la nouvelle expérience Workfront

>[!NOTE]
>
>Cette fonctionnalité a été ajoutée à l’environnement de prévisualisation le 1er juillet 2021. Elle sera publiée dans l’environnement de production le 15 juillet 2021.

Pour vous aider à gérer les modèles de mise en page pendant que vos utilisateurs et utilisatrices passent à l’utilisation de la nouvelle expérience Workfront, nous avons créé un bouton que vous pouvez utiliser pour migrer les modèles de mise en page de Workfront Classic vers la nouvelle expérience sans faire appel au service de support client de Workfront.

Auparavant, seul le service de support client de Workfront pouvait migrer vos modèles de mise en page de Workfront Classic vers la nouvelle expérience Workfront.

## Lorsque vous associez un modèle à un groupe, sélectionnez un processus d’approbation de groupe dans Détails de la file d’attente et Rubriques de la file d’attente.

Nous avons ajouté une nouvelle option au processus d’association d’un modèle à un groupe. Vous pouvez désormais sélectionner des processus d’approbation spécifiques à un groupe pour les problèmes dans les détails de file d’attente du modèle ou dans l’une de ses rubriques de file d’attente.

Dans la version 21.3, lorsque nous avons ajouté la possibilité d’associer un modèle de groupe à un groupe, vous pouviez sélectionner un processus d’approbation spécifique au groupe dans le modèle, mais vous ne pouviez pas le faire dans les détails de file d’attente ou dans les rubriques de file d’attente du modèle.

Pour plus d’informations, voir [Associer un processus d’approbation nouveau ou existant au travail](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
