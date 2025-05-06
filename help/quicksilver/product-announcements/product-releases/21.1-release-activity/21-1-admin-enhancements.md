---
content-type: release-notes
keywords: notes,trimestrielle,mise à jour
navigation-topic: product-releases
title: Améliorations apportées à l’administration (version 21.1)
description: Cette page décrit toutes les améliorations apportées à l’administration pour la version 21.1 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: 6fe1a2c71f53d6b314c2b1402a547f9c934bfbea
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 99%

---

# Améliorations apportées à l’administration (version 21.1)

Cette page décrit toutes les améliorations apportées à l’administration pour la version 21.1 de l’environnement de prévisualisation. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 15 février 2021.

Pour obtenir une liste de tous les changements disponibles avec la version 21.1, voir [Vue d’ensemble de la version 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Ajout d’un nouveau paramètre Niveau d’accès pour la copie de projets

Pour vous donner plus de contrôle, en tant qu’administrateur ou administratrice système, sur ce que les planificateurs et planificatrices peuvent faire avec un projet, nous avons rendu plus granulaire l’accès Modifier aux projets du niveau d’accès, en introduisant un nouveau paramètre qui vous permet d’activer ou de désactiver leur capacité à copier des projets. Avant cette modification, lorsque vous avez activé l’accès des utilisateurs et utilisatrices à l’option Modifier des projets, l’accès à la copie était automatique. Grâce à la nouvelle fonctionnalité, vous pouvez donner à une personne l’accès pour modifier des projets sans nécessairement lui accorder l’accès à les copier en désactivant le nouveau paramètre Copier.

Si vos utilisateurs et utilisatrices avaient accès à l’option Modifier des projets dans leur niveau d’accès avant cette modification, ce paramètre sera automatiquement activé lorsqu’elle sera publiée.

Pour plus d’informations sur le niveau d’accès au plan, voir [Accorder l’accès aux projets](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Pour plus d’informations sur la copie d’un projet, voir [Copier un projet](../../../manage-work/projects/manage-projects/copy-project.md).

Cette fonctionnalité est désormais incluse dans le parcours d’apprentissage [Principes fondamentaux de l’administrateur ou administratrice dans la nouvelle expérience Workfront, Partie 1 : organisation de l’utilisateur ou utilisatrice](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) sur Workfront One.

## Dans un formulaire personnalisé sur un objet, sélectionnez tous les éléments d’un champ déroulant à sélection multiple.

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible lorsque vous envoyez une nouvelle requête.

Sur la page Détails d’un objet, lorsque vous remplissez un champ déroulant à sélection multiple sur un formulaire personnalisé, vous pouvez cliquer sur Sélectionner tout si vous devez sélectionner toutes les options disponibles.

Pour plus d’informations sur la modification des données dans un formulaire personnalisé, voir [Modifier les informations dans les champs des formulaires personnalisés](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Recalculer tous les champs de formulaire personnalisés d’un objet

Il est désormais plus facile de s’assurer que toutes les données des champs personnalisés calculés sont à jour pour un objet. Une nouvelle option de menu Recalculer les expressions permet de recalculer rapidement toutes les données de ces champs.

Cela s’avère particulièrement utile lorsqu’une personne modifie des données dans un autre objet référencé par un champ personnalisé calculé de votre objet.

Auparavant, les utilisateurs et utilisatrices devaient utiliser des solutions de contournement pour s’assurer que toutes les données des champs personnalisés calculés étaient à jour. Par exemple, il fallait modifié l’objet avec d’autres objets pour utiliser l’option de recalcul disponible pour la modification en masse.

Pour plus d’informations, voir [Modifier les informations dans les champs des formulaires personnalisés](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Déverrouiller les préférences de tâche et de problème pour les administrateurs et administratrices de groupes

>[!NOTE]
>
>Jusqu’au 24 juin 2021, cette option était disponible dans le cadre d’un déploiement échelonné uniquement pour les clientes et clients qui ont la possibilité de déverrouiller les préférences de projet pour les groupes. Elle est maintenant disponible à toute la clientèle.

Désormais, les administrateurs et administratrices Adobe Workfront peuvent accorder aux administrateurs et administatrices de groupes une plus grande autonomie en déverrouillant les préférences de tâche et de problème individuelles. Lorsqu’une préférence est déverrouillée, les administrateurs et administratrices de groupes peuvent la configurer pour répondre aux besoins uniques et aux processus internes de chaque groupe.

Pour plus d’informations, consultez [Configurer les préférences en matière de tâches et de problèmes pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

Cette fonctionnalité est désormais incluse dans le parcours d’apprentissage [Principes fondamentaux de l’administrateur ou administratrice dans la nouvelle expérience Workfront, Partie 2 : configuration du projet](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) sur Workfront One.

## Configurer séparément les paramètres de niveau d’accès pour les portefeuilles et les programmes

Il est désormais plus facile de gérer l’accès des utilisateurs et utilisatrices aux portefeuilles et aux programmes, car vous pouvez configurer leurs paramètres de niveau d’accès séparément.

Auparavant, les paramètres de niveau d’accès pour les portefeuilles et les programmes étaient combinés. Cela signifie que vous ne pouviez pas configurer les paramètres d’accès pour les programmes sans les configurer de la même manière pour les portefeuilles, et vice versa.

Pour plus d’informations sur la configuration d’un niveau d’accès, voir [Créer ou modifier des niveaux d’accès personnalisés](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Pour plus d’informations sur les paramètres d’accès que vous pouvez configurer pour les programmes et les portefeuilles, voir [Accès configurable aux fonctionnalités pour chaque type d’objet](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Cette fonctionnalité est désormais incluse dans le parcours d’apprentissage [Principes fondamentaux de l’administrateur ou administratrice dans la nouvelle expérience Workfront, Partie 1 : organisation de l’utilisateur ou utilisatrice](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) sur Workfront One.

## Cocher toutes les cases d’une série lors de la modification d’informations dans un formulaire personnalisé

>[!NOTE]
>
>Cette fonctionnalité n’est actuellement pas disponible lorsque vous envoyez une nouvelle requête.

Sur la page Détails d’un objet, lorsque vous renseignez un champ Formulaire personnalisé contenant des cases à cocher, vous pouvez cliquer sur Sélectionner tout si vous devez cocher toutes les cases disponibles.

Cette option s’affiche uniquement si le champ contient plus de 2 cases à cocher.

Pour plus d’informations, voir [Modifier les informations dans les champs de formulaire personnalisés](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Configurer la liste autorisée d’e-mails Workfront

Pour mieux sécuriser vos données, vous pouvez désormais utiliser une liste autorisée de domaines d’e-mail pour :

* Contrôler la destination des e-mails de Workfront s’ils contiennent des rapports ou des documents stockés dans Workfront
* Le contrôle des domaines de messagerie peut se faire dans l’adresse e-mail que les utilisateurs et les utilisatrices spécifient dans leurs profils.

Si, par exemple, vous souhaitez protéger des données sensibles, telles qu’un rapport répertoriant votre clientèle à risque, vous pouvez n’inclure que votre ou vos domaines de messagerie interne dans la liste autorisée d’e-mails. De cette manière, les utilisateurs et les utilisatrices ne peuvent pas envoyer ce rapport (ni aucun autre rapport Workfront) à une adresse e-mail externe.

Pour plus d’informations, consultez la section [Configurer la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) dans l’article [Configurer la liste autorisée de votre pare-feu](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Affecter un administrateur ou une administratrice de groupes à un sous-groupe

Pour faciliter le fonctionnement indépendant des niveaux de votre organisation, nous avons ajouté la possibilité d’affecter un administrateur ou une administratrice de groupes à un sous-groupe. Vous pouvez désormais vous assurer que vous déléguez la gestion des sous-groupes aux personnes appropriées.

Auparavant, seul un groupe de niveau supérieur pouvait avoir des administrateurs et des administratrices de groupes qui géraient tous les sous-groupes sous le groupe de niveau supérieur.

Pour plus d’informations, consultez la section [Administrateurs et administratrices de groupes pour les sous-groupes ](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) dans l’article [Vue d’ensemble des sous-groupes](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

Cette fonctionnalité est désormais incluse dans le parcours de formation [Principes d’administration pour la nouvelle expérience Workfront, Partie 1 : organisation des utilisateurs et des utilisatrices](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) de Workfront One.

## Configurer les notifications d’événement pour les groupes

>[!NOTE]
>
>Disponible dans le cadre d’un déploiement par étapes uniquement pour la clientèle qui a la possibilité de déverrouiller les préférences de projet pour les groupes. Il s’agit de toutes les clientes et de tous les clients des clusters 4 et 6 et d’un petit nombre des autres clusters. Cette note sera mise à jour au fur et à mesure que la fonctionnalité deviendra disponible pour d’autres clusters.

Désormais, l’équipe d’administration de Workfront peut accorder une plus grande autonomie à celle des groupes en leur permettant de configurer des notifications d’événement pour leurs groupes de niveau supérieur. Les sous-groupes héritent des configurations de notification d’événement de leur groupe parent.

Auparavant, les notifications d’événement n’étaient configurables que par un administrateur ou un administratrice Workfront au niveau du système, ce qui signifiait que tous les groupes devaient utiliser le même jeu de notifications d’événement.

Pour plus d’informations, consultez les articles suivants :

* [Déverrouiller ou verrouiller la configuration des notifications d’événement pour tous les groupes](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [Afficher et configurer des notifications d’événement pour un groupe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

<!--This feature is now included in the [Administrator Fundamentals in the new Workfront experience, Part 1: User Organization](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) learning path on Workfront One.

This feature is now included in the [Email and In-App Notifications in the new Workfront experience](https://experienceleague.adobe.com/en/docs/workfront/using/home://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) learning path on Workfront One.-->

## Travailler avec des projets de groupe et des processus d’approbation dans la zone des groupes

En tant qu’administrateur ou administratrice de groupes, il est désormais facile d’afficher et de travailler sur les projets et les processus d’approbation de votre groupe, car ils sont maintenant répertoriés dans la zone des groupes. La page principale d’un groupe vous permet d’effectuer les opérations suivantes :

* Cliquer sur Projets dans le menu de gauche pour afficher les projets du groupe et en créer de nouveaux pour le groupe. Si un projet sélectionné a été partagé avec vous, vous pouvez utiliser les boutons de la barre d’outils pour le modifier, l’exporter, le copier ou le supprimer.

  Pour plus d’informations, voir [Créer et modifier les projets d’un groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* Cliquez sur Approbations dans le menu de gauche pour afficher et gérer tous les processus d’approbation associés au groupe.

  Pour plus d’informations, voir [Processus d’approbation au niveau du groupe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Cette fonctionnalité est également disponible pour les administrateurs et les administratrices de Workfront.

## Afficher le nombre de licences utilisées et affectées dans un groupe

Pour déterminer la pertinence de la distribution de vos licences, vous pouvez désormais afficher le nombre de licences utilisées dans un groupe et dans les sous-groupes qui lui sont subordonnés.

Si vous gérez un groupe de niveau supérieur, vous pouvez afficher le nombre de licences utilisées dans un groupe (et ses sous-groupes) et le nombre maximum de licences affectées au groupe.

Pour plus d’informations, voir [Afficher le nombre de licences affectées et utilisées dans un groupe dans la nouvelle expérience Adobe Workfront](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

