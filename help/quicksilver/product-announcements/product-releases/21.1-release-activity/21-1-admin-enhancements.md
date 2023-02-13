---
content-type: release-notes
keywords: notes,trimestriel,mise à jour
navigation-topic: product-releases
title: 21.1 Améliorations apportées aux administrateurs
description: Cette page décrit toutes les améliorations apportées par l’administrateur à la version 21.1 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.
author: Luke
feature: Product Announcements, System Setup and Administration
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# 21.1 Améliorations apportées aux administrateurs

Cette page décrit toutes les améliorations apportées par l’administrateur à la version 21.1 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.

Pour obtenir la liste de toutes les modifications disponibles avec la version 21.1, voir [Présentation de la version 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Ajout d’un nouveau paramètre Niveau d’accès pour la copie de projets

Pour vous donner plus de contrôle, en tant qu’administrateur système, sur ce que les planificateurs peuvent faire d’un projet, nous avons rendu l’accès Modifier aux projets du niveau d’accès plus granulaire, en introduisant un nouveau paramètre qui vous permet d’activer ou de désactiver leur capacité à copier des projets. Avant cette modification, lorsque vous avez activé l’accès des utilisateurs à l’option Modifier des projets, ils avaient automatiquement accès à la copie. Grâce à la nouvelle fonctionnalité, vous pouvez donner à une personne l’accès pour modifier des projets sans nécessairement avoir accès à les copier en désactivant le nouveau paramètre Copier.

Si vos utilisateurs avaient accès à l’option Modifier des projets dans leur niveau d’accès avant cette modification, ce paramètre sera automatiquement activé lorsqu’elle sera publiée.

Pour plus d’informations sur le niveau d’accès au plan, voir [Accorder l’accès aux projets](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Pour plus d’informations sur la copie d’un projet, voir [Copier un projet](../../../manage-work/projects/manage-projects/copy-project.md).

Cette fonctionnalité est désormais incluse dans la variable [Principes fondamentaux de l’administrateur dans la nouvelle expérience Workfront, partie 1 : Organisation des utilisateurs](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) parcours d’apprentissage sur Workfront One.

## Dans un formulaire personnalisé sur un objet, sélectionnez tous les éléments d’un champ déroulant à sélection multiple.

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible lorsque vous envoyez une nouvelle requête.

Sur la page Détails d’un objet, lorsque vous remplissez un champ déroulant à sélection multiple sur un formulaire personnalisé, vous pouvez cliquer sur Sélectionner tout si vous devez sélectionner toutes les options disponibles.

Pour plus d’informations sur la modification des données dans un formulaire personnalisé, voir [Modifier les informations dans les champs de formulaire personnalisés](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Recalculer tous les champs de formulaire personnalisés d’un objet

Il est désormais plus facile de s’assurer que toutes les données des champs personnalisés calculés sont à jour pour un objet. Une nouvelle option de menu Recalculer les expressions permet de recalculer rapidement toutes les données de ces champs.

Cela s’avère particulièrement utile lorsqu’une personne modifie des données dans un autre objet référencé par un champ personnalisé calculé de votre objet.

Auparavant, les utilisateurs devaient utiliser des solutions pour s’assurer que toutes les données des champs personnalisés calculés étaient à jour. Par exemple, ils ont modifié l’objet avec d’autres objets pour utiliser l’option de recalcul disponible pour la modification en masse.

Pour plus d’informations, voir [Modifier les informations dans les champs de formulaire personnalisés](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Déverrouiller les préférences de tâche et de problème pour les administrateurs de groupe

>[!NOTE]
>
>Jusqu’au 24 juin 2021, cette option était disponible dans le cadre d’un déploiement échelonné uniquement pour les clients qui ont la possibilité de déverrouiller les préférences de projet pour les groupes. Il est maintenant disponible pour tous les clients.

Les administrateurs d’Adobe Workfront peuvent désormais accorder aux administrateurs de groupe une plus grande autonomie en déverrouillant les tâches individuelles et les préférences d’émission. Lorsqu’une préférence est déverrouillée, les administrateurs de groupe peuvent la configurer pour que leurs groupes répondent aux besoins uniques et aux processus internes de chaque groupe.

Pour plus d’informations, voir [Configuration des préférences de tâche et de problème pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

Cette fonctionnalité est désormais incluse dans la variable [Principes fondamentaux de l’administrateur dans la nouvelle expérience Workfront, Partie 2 : Configuration du projet](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) parcours d’apprentissage sur Workfront One.

## Configurer séparément les paramètres de niveau d’accès pour les portefeuilles et les programmes

Il est désormais plus facile de gérer l’accès des utilisateurs aux portefeuilles et aux programmes, car vous pouvez configurer leurs paramètres de niveau d’accès séparément.

Auparavant, les paramètres de niveau d’accès pour les portefeuilles et les programmes étaient combinés. Cela signifie que vous ne pouviez pas configurer les paramètres d’accès pour les programmes sans les configurer de la même manière pour les portefeuilles, et c’était également le cas en sens inverse.

Pour plus d’informations sur la configuration d’un niveau d’accès, voir [Création ou modification de niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Pour plus d’informations sur les paramètres d’accès que vous pouvez configurer pour les programmes et les portefeuilles, voir [Accès configurable à la fonctionnalité pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Cette fonctionnalité est désormais incluse dans la variable [Principes fondamentaux de l’administrateur dans la nouvelle expérience Workfront, partie 1 : Organisation des utilisateurs](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) parcours d’apprentissage sur Workfront One.

## Cochez toutes les cases d’une série lors de la modification d’informations dans un formulaire personnalisé.

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible lorsque vous envoyez une nouvelle requête.

Sur la page Détails d’un objet, lorsque vous renseignez un champ Formulaire personnalisé contenant des cases à cocher, vous pouvez cliquer sur Sélectionner tout si vous devez cocher toutes les cases disponibles.

Cette option s’affiche uniquement si le champ contient plus de 2 cases à cocher.

Pour plus d’informations, voir [Modifier les informations dans les champs de formulaire personnalisés](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Configuration de votre liste autorisée de messagerie Workfront

Pour mieux sécuriser vos données, vous pouvez désormais utiliser une liste autorisée de domaine de courriel pour :

* Contrôle de l’emplacement où se rendent les emails Workfront s’ils contiennent des rapports ou des documents stockés dans Workfront
* Les domaines de contrôle des courriers électroniques peuvent se trouver dans l’adresse électronique que les utilisateurs peuvent spécifier dans leur profil d’utilisateur.

Par exemple, si vous souhaitez protéger des données sensibles, telles qu’un rapport répertoriant vos clients à risque, vous pouvez inclure uniquement votre domaine de courriel interne ou vos domaines dans la liste autorisée de courriel. De cette manière, les utilisateurs ne peuvent pas envoyer ce rapport (ni aucun autre rapport Workfront) à une adresse électronique externe.

Pour plus d’informations, voir la section [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) dans l’article [Configuration de la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Affectation d’un administrateur de groupe à un sous-groupe

Pour faciliter le fonctionnement indépendant des niveaux de votre organisation, nous avons ajouté la possibilité d’affecter un administrateur de groupe à un sous-groupe. Vous pouvez désormais vous assurer que vous déléguez la gestion des sous-groupes aux personnes appropriées.

Auparavant, seul un groupe de niveau supérieur pouvait avoir des administrateurs de groupe, et ces administrateurs géraient tous les sous-groupes sous le groupe de niveau supérieur.

Pour plus d’informations, voir la section [Administrateurs de groupe pour les sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) dans l’article [Présentation des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

Cette fonctionnalité est désormais incluse dans la variable [Principes fondamentaux de l’administrateur dans la nouvelle expérience Workfront, partie 1 : Organisation des utilisateurs](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) parcours d’apprentissage sur Workfront One.

## Configuration des notifications d’événement pour les groupes

>[!NOTE]
>
>Disponible dans le cadre d’un déploiement par étapes uniquement pour les clients qui ont la possibilité de déverrouiller les préférences de projet pour les groupes. Cela inclut tous les clients des clusters 4 et 6 et un petit nombre de clients des autres clusters. Cette note sera mise à jour au fur et à mesure que les fonctionnalités seront disponibles pour d’autres grappes.

Les administrateurs Workfront peuvent désormais accorder aux administrateurs de groupe une plus grande autonomie en leur permettant de configurer des notifications d’événement pour leurs groupes de niveau supérieur. Les sous-groupes héritent des configurations de notification d’événement de leur groupe parent supérieur.

Auparavant, les notifications d’événement n’étaient configurables que par un administrateur Workfront au niveau du système, ce qui signifie que tous les groupes devaient utiliser le même ensemble de notifications d’événement.

Pour plus d’informations, voir les articles suivants :

* [Déverrouiller ou verrouiller la configuration des notifications d’événement pour tous les groupes](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [Affichage et configuration des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

Cette fonctionnalité est désormais incluse dans la variable [Principes fondamentaux de l’administrateur dans la nouvelle expérience Workfront, partie 1 : Organisation des utilisateurs](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) parcours d’apprentissage sur Workfront One.

Cette fonctionnalité est désormais incluse dans la variable [Notifications par e-mail et In-App dans la nouvelle expérience Workfront](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) parcours d’apprentissage sur Workfront One.

## Utilisation de projets de groupe et processus de validation dans la zone Groupes

Si vous êtes administrateur de groupe, il est facile d’afficher et de travailler avec les projets de votre groupe et les processus d’approbation maintenant qu’ils sont répertoriés dans la zone Groupes . La page principale d’un groupe vous permet d’effectuer les opérations suivantes :

* Cliquez sur Projets dans le menu de gauche pour afficher les projets du groupe et en créer de nouveaux pour le groupe. Si un projet sélectionné a été partagé avec vous, vous pouvez utiliser les boutons de la barre d’outils pour le modifier, l’exporter, le copier ou le supprimer.

   Pour plus d’informations, voir [Création et modification des projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* Cliquez sur Validations dans le menu de gauche pour visualiser et gérer tous les processus de validation associés au groupe.

   Pour plus d’informations, voir [Processus de validation au niveau du groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Cette fonctionnalité est également disponible pour les administrateurs de Workfront.

## Afficher le nombre de licences utilisées et allouées dans un groupe

Pour déterminer la distribution de vos licences, vous pouvez désormais afficher le nombre de licences utilisées dans un groupe et les sous-groupes situés en dessous.

Si vous gérez un groupe de niveau supérieur, vous pouvez afficher à la fois le nombre de licences utilisées dans un groupe (et ses sous-groupes) et le nombre maximal de licences attribuées au groupe.

Pour plus d’informations, voir [Afficher le nombre de licences attribuées et utilisées dans un groupe dans la nouvelle expérience Adobe Workfront](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

