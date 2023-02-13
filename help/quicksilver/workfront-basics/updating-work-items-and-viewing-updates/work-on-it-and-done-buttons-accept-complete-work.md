---
content-type: o
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Bouton Travail dessus et bouton Terminé - Aperçu
description: Lorsque vous êtes affecté à une tâche ou à un problème, vous pouvez utiliser un bouton contextuel qui change de nom et de fonction en fonction de votre implication dans l’élément de travail.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: cfda6702-1a9a-4645-b031-8b2f201ac0af
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# Bouton Travail dessus et bouton Terminé - Aperçu

Lorsque vous êtes affecté à une tâche ou à un problème, vous pouvez utiliser un bouton contextuel qui change de nom et de fonction en fonction de votre implication dans l’élément de travail.

En utilisant le bouton contextuel pour accepter ou terminer des tâches, vous pouvez laisser Adobe Workfront mettre à jour plusieurs champs des éléments sans avoir à les mettre à jour manuellement.

## Utilisation et noms des boutons Terminer

Selon la zone de Workfront à partir de laquelle vous accédez à votre tâche ou à votre problème, le bouton Travailler dessus ou Terminé peut changer de nom, comme décrit dans les scénarios suivants : 

* Lorsque la tâche ou le problème vous est assigné pour la première fois et que l’état est Nouveau, le bouton s’affiche sous la forme Travail dessus.

   ![](assets/nwe-work-on-it-button.png)

   >[!TIP]
   >
   >Vous pouvez remplacer le bouton Travailler dessus par un bouton Démarrer . Pour plus d’informations sur le remplacement du bouton Travailler dessus par un bouton Démarrer , voir  [Remplacez le bouton Travailler dessus par un bouton Démarrer](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md) .

* Une fois que vous avez cliqué sur l’option Travailler dessus, le bouton devient Marquer comme terminé ou Terminé , en fonction de l’endroit où vous accédez à la tâche ou du problème dans Workfront. Pour plus d’informations sur l’emplacement où vous pouvez accéder au bouton Travailler dessus, reportez-vous à la section [Bouton Travailler dessus et Terminer](#locate-the-work-on-it-and-done-button) dans cet article.

   ![](assets/nwe-mark-as-done-button-350x122.png)

* Si vous n’êtes pas le seul à être affecté à la tâche ou au problème et que vous accédez à votre tâche à partir de la liste de tâches dans la zone Accueil, le bouton passe à Terminé avec ma partie.

   ![](assets/home-left-done-with-my-part-button-350x184.png)

## Bouton Travailler dessus et Terminer {#locate-the-work-on-it-and-done-button}

Vous pouvez localiser le bouton Travailler dessus et Terminé dans les zones suivantes de Workfront :

* La zone Accueil, à la fois dans la liste de travail et dans le panneau Détails

   Pour plus d’informations sur le marquage d’un élément comme terminé dans la zone Accueil, voir [Marquez un élément comme Terminé dans la zone Accueil](../../workfront-basics/using-home/using-the-home-area/mark-item-done-in-home.md).

* Dans l’en-tête de la tâche ou du problème

   Pour plus d’informations sur les en-têtes d’objet, voir [Nouveaux en-têtes d’objet](../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

* Dans le panneau Résumé de la tâche ou du problème dans une liste ou dans l’équilibreur de charge de travail

   Pour plus d’informations sur l’utilisation du panneau Résumé, voir [Aperçu du résumé](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

## Présentation des champs qui se mettent automatiquement à jour lorsque vous cliquez sur le bouton Travailler dessus et Terminé

L’utilisation des boutons Travail dessus et Terminé vous permet de permettre à Workfront de mettre à jour automatiquement les informations sur l’élément de travail qui vous a été attribué.

* [Bouton Travailler dessus](#work-on-it-button)
* [Bouton Démarrer](#start-button)
* [Bouton Terminé](#the-done-button)

### Bouton Travailler dessus {#work-on-it-button}

Lorsque vous cliquez sur Travailler dessus, les éléments suivants sont également mis à jour :

* Mises à jour de l’état d’affectation de la demande à l’état opérationnel

   >[!TIP]
   >
   >Le champ Statut de l’affectation n’est visible que dans les rapports et les listes. Pour plus d’informations sur le champ État d’affectation, voir [Glossaire de la terminologie Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

* Date de validation

   Pour plus d’informations sur la date de validation, voir [Présentation de la date de validation](../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

### Bouton Démarrer {#start-button}

Si vous avez accès aux équipes de modification, vous pouvez remplacer le bouton Travailler dessus par un bouton Démarrer pour une équipe. Lorsque les utilisateurs de cette équipe en tant qu’équipe d’accueil cliquent sur le bouton Démarrer sur les éléments auxquels ils sont affectés, les champs supplémentaires de leurs tâches sont automatiquement mis à jour. Pour plus d’informations sur le remplacement du bouton Travailler dessus par un bouton Démarrer , voir [Remplacez le bouton Travailler dessus par un bouton Démarrer](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Outre les champs qui se mettent à jour lorsque vous cliquez sur le bouton Travailler dessus, les champs suivants se mettent automatiquement à jour sur une tâche ou un problème lorsque vous cliquez sur le bouton Démarrer :

* Statut
* Date de début réelle

   Pour plus d’informations sur la date de début réelle, voir [Présentation de la date de début réelle du projet](../../manage-work/projects/planning-a-project/project-actual-start-date.md).

* Date de fin réelle si le bouton Début est associé à un état qui correspond à Terminé ou Fermé.

   Pour plus d’informations sur la date d’achèvement réelle, voir [Présentation du projet Date d’achèvement réelle](../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

>[!NOTE]
>
>Cliquez sur le bouton Annuler pour rétablir l’état d’origine de l’élément de travail et supprimer la date de début réelle.
>
>Le bouton Annuler n’est pas disponible dans les zones suivantes :
>
>* Requêtes d’équipe
>* En-tête de tâche
>


### Bouton Terminé {#the-done-button}

Si vous avez accès aux équipes de modification, vous pouvez configurer le bouton Terminé pour qu’une équipe mette à jour l’état de la tâche ou du problème lorsque vous marquez un élément comme terminé. Lorsque les utilisateurs de cette équipe en tant qu’équipe d’accueil cliquent sur le bouton Terminé sur leurs éléments, les champs suivants se mettent automatiquement à jour sur une tâche ou un problème :

* Statut
* Mises à jour de l’état d’affectation de l’état de travail à terminé
* Date d’achèvement réelle

Pour plus d’informations sur la configuration du bouton Terminé pour une équipe, voir les articles suivants :

* [Configuration du bouton Terminé pour les tâches](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
* [Configuration du bouton Terminé pour les problèmes](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)
