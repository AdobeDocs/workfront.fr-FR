---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Vue d’ensemble des boutons Travailler sur ce projet et Terminé
description: Lorsqu’une tâche ou un problème vous a été affecté, vous pouvez utiliser un bouton contextuel qui change les noms et les fonctions selon votre implication dans l’élément de travail.
author: Lisa and Alina
feature: Get Started with Workfront
role: User
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
source-git-commit: ecafbd693237427d727b15dd22afd485b4e59c72
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 65%

---

# Vue d’ensemble des boutons Travailler sur ce projet et Terminé

Lorsqu’une tâche ou un problème vous a été affecté, vous pouvez utiliser un bouton contextuel qui change les noms et les fonctions selon votre implication dans l’élément de travail.

Le bouton contextuel vous permet d’accepter ou de compléter les éléments de travail, autorisant Adobe Workfront à mettre à jour automatiquement plusieurs champs sans que vous ayez à les mettre à jour vous-même.

Les boutons Travail dessus et Terminé sont visibles par les utilisateurs disposant des éléments suivants :

* Une licence standard (nouvelle) ou une licence Plan ou Travail (en cours)
* Accès à des modifications limité ou supérieur à la tâche ou au problème

>[!NOTE]
>
>Le bouton Terminé s’affiche sous la forme Marquer comme prévu dans toutes les zones de Workfront.

## Boutons Travailler sur ce projet et Terminé

Selon la zone de Workfront à partir de laquelle vous accédez à votre tâche ou à votre problème, le bouton Travailler dessus ou Terminé peut changer de nom, comme décrit dans les scénarios suivants :

* Lorsque la tâche ou le problème vous est affecté pour la première fois et que le statut est Nouveau, le bouton indique Travailler sur ce projet.

  ![](assets/nwe-work-on-it-button.png)

  >[!TIP]
  >
  >Vous pouvez remplacer le bouton Travailler sur ce projet par un bouton Démarrer. Pour plus d’informations sur le remplacement du bouton Travailler sur ce projet par un bouton Démarrer, consultez la section [Remplacer le bouton Travailler sur ce projet par un bouton Démarrer](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

* Une fois que vous avez cliqué sur l’option Travailler sur l’acceptation, le bouton passe à Marquer comme prévu. Pour savoir où vous pouvez accéder au bouton Travailler sur ce projet, consultez dans cet article la section [Trouver les boutons Travailler sur ce projet et Terminé](#locate-the-work-on-it-and-done-button).

  ![](assets/nwe-mark-as-done-button-350x122.png)


<!--If you are not the only one assigned to the task or issue and you are accessing your work item from the My Work widget in the Home area, the button changes to Done with my part.

  ![](assets/home-left-done-with-my-part-button-350x184.png)-->

## Bouton Travailler dessus et Terminer {#locate-the-work-on-it-and-done-button}

Vous pouvez localiser le bouton Travailler dessus et Terminé dans les zones suivantes de Workfront :

* La zone Accueil du widget Mon travail

  Pour plus d’informations sur la façon d’indiquer qu’un élément est Terminé dans la zone d’accueil, consultez la section [Marquer un élément comme Terminé dans la zone d’accueil](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md).

* dans l’en-tête de la tâche ou du problème.

  Pour plus d’informations sur les en-têtes d’objets, consultez la section [Nouveaux en-têtes d’objets](../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

* Dans le panneau Résumé de la tâche ou du problème

  Pour plus d’informations sur l’utilisation du panneau de résumé, consultez la section [Vue d’ensemble du résumé](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

## Présentation des champs qui se mettent automatiquement à jour lorsque vous cliquez sur le bouton Travailler dessus ou Terminé

L’avantage d’utiliser les boutons Travailler sur ce projet et Terminé est que vous pouvez permettre à Workfront de mettre à jour automatiquement les informations sur l’élément de travail qui vous a été affecté.

* [Bouton Travailler sur ce projet](#work-on-it-button)
* [Bouton Démarrer](#start-button)
* [Bouton Terminé](#the-done-button)

### Bouton Travailler sur ce projet {#work-on-it-button}

Lorsque vous cliquez sur Travailler sur ce projet, les éléments suivants sont également mis à jour :

* Le statut de l’affectation passe de Demandé à Travail en cours.

  >[!TIP]
  >
  >Le champ Statut de l’affectation n’est visible que dans les rapports et les listes. Pour plus d’informations sur le champ Statut de l’affectation, consultez la section [Glossaire de la terminologie Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Date d’engagement

  Pour plus d’informations sur la date d’engagement, consultez la section [Vue d’ensemble de la date d’engagement](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

### Bouton Démarrer {#start-button}

Si vous avez accès aux équipes de modification, vous pouvez remplacer le bouton Travailler dessus par un bouton Démarrer pour une équipe. Lorsque les utilisateurs et les utilisatrices ayant cette équipe comme équipe d’accueil cliquent sur le bouton Démarrer pour les éléments qui leur sont affectés, les champs supplémentaires de leurs éléments de travail sont automatiquement mis à jour. Pour plus d’informations sur le remplacement du bouton Travailler sur ce projet par un bouton Démarrer, consultez la section [Remplacer le bouton Travailler sur ce projet par un bouton Démarrer](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Outre les champs qui se mettent à jour lorsque vous cliquez sur le bouton Travailler dessus, les champs suivants se mettent automatiquement à jour sur une tâche ou un problème lorsque vous cliquez sur le bouton Démarrer :

* Statut
* Date de début effective

  Pour plus d’informations sur la date de début effective, consultez la section [Vue d’ensemble de la date de début effective du projet](../../manage-work/projects/planning-a-project/project-actual-start-date.md).

* Date d’achèvement effective si le bouton Démarrer est associé à un statut qui équivaut à Terminé ou Fermé.

  Pour plus d’informations sur la date d’achèvement effective, consultez la section [Vue d’ensemble de la date d’achèvement effective du projet](../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

>[!NOTE]
>
>Cliquer sur le bouton Annuler rétablit le statut d’origine de l’élément de travail et supprime la date de début effective.
>
>Le bouton Annuler n’est pas disponible dans les zones suivantes :
>
>* Demandes de l’équipe
>* En-tête de tâche
>

### Bouton Terminé {#the-done-button}

Si vous avez accès aux équipes de modification, vous pouvez configurer le bouton Terminé pour qu’une équipe mette à jour l’état de la tâche ou du problème lorsque vous marquez un élément comme terminé. Lorsque les utilisateurs de cette équipe en tant qu’équipe d’accueil cliquent sur le bouton Marquer comme effectué sur leurs éléments, les champs suivants se mettent automatiquement à jour sur une tâche ou un problème :

* Statut
* Mises à jour de l’état d’affectation de l’état de travail à terminé
* Date d&#39;achèvement effective

Pour plus d’informations sur la configuration du bouton Terminé pour une équipe, voir les articles suivants :

* [Configurer le bouton Terminé pour les tâches](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
* [Configurer le bouton Terminé pour les problèmes](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)
