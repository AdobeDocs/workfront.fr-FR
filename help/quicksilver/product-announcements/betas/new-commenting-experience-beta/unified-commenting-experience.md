---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: Nouvelle expérience de commentaire
description: Une mise à jour de l’expérience de commentaires dans Adobe Workfront est actuellement en cours de développement. Cette mise à jour comprend une nouvelle interface, de nouvelles fonctionnalités et des performances améliorées dans la section Mises à jour de certains objets.
author: Alina
feature: Product Announcements
role: User
hide: true
hidefromtoc: true
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 98%

---

# Nouvelle expérience de commentaire

<!--take out legacy, preview, prod references from below-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

-->

>[!IMPORTANT]
>
>Les informations de cet article font référence aux fonctionnalités publiées dans le cadre de la nouvelle expérience de commentaires.
>
>Le programme beta pour la nouvelle expérience de commentaires a commencé en avril 2023 et s’est terminé en octobre 2023, avec la version d’octobre 2023.
>
>Depuis le 11 avril 2024, toutes les fonctionnalités relatives à la nouvelle expérience de commentaire sont disponibles dans l’environnement de production pour l’ensemble de la clientèle.

## Fonctionnalités

La nouvelle expérience de commentaire comprend des améliorations et des modifications de la section Mises à jour des objets Adobe Workfront.

Parmi les améliorations apportées à la nouvelle expérience de commentaire, on peut citer les suivantes :

* Amélioration des performances et de l’expérience client
* Séparation des commentaires des utilisateurs et utilisatrices des mises à jour de l’activité du système
* Indicateur en temps réel lors de l’ajout de nouveaux commentaires à un objet
* Modification des commentaires après leur soumission

Les fonctionnalités suivantes ont été supprimées ou seront obsolètes dans la nouvelle expérience :

* Commentaire sur une mise à jour système. Les commentaires ajoutés aux mises à jour système par le passé ont été importés en tant que commentaires en lecture seule dans le nouvel onglet Activité du système.
* Possibilité de modifier le statut, la condition, la date d’engagement et le pourcentage terminé tout en commentant les tâches et les problèmes.

  Nous vous recommandons également d’ajouter ces champs dans le panneau Résumé des tâches et des problèmes afin de pouvoir y accéder facilement à partir des listes, de la page d’accueil, de l’équilibreur Workfront ou d’une feuille de temps.
* Possibilité de modifier le formulaire personnalisé
* L’information « au nom de &lt; nom d’utilisateur ou d’utilisatrice > », lorsqu’un administrateur ou une administratrice Workfront ou de groupe se connecte en tant qu’autre utilisateur ou utilisatrice et ajoute un commentaire en son nom, avait été supprimée. Elle a été rétablie le 19 octobre 2023.
* Option « Demander l’approbation » lorsque vous taguez des personnes en ajoutant un commentaire à un document.
* Le paramètre « Afficher le pourcentage terminé pour le statut de la mise à jour » lors de la modification de la zone de profil d’un utilisateur ou d’une utilisatrice sera supprimé. La fonctionnalité de mise à jour du pourcentage terminé d’une tâche ou d’un problème a été supprimée.


<!--removed this note on November 28, 2023, when this limitation was removed: 

>[!NOTE]
>
>The objects listed below have only the comments and system updates starting with January 1, 2019 available in the new commenting experience.  
>
>You can view comments and system updates on these objects prior to January 1, 2019 when viewing the Updates section in the current experience:
>
>* Issues
>* Projects
>* Tasks
>* Documents

For more information, see the [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md). 
-->

Le tableau suivant illustre les fonctionnalités qui seront disponibles dans la nouvelle expérience de commentaire, ainsi que leur disponibilité dans les zones où elles sont prises en charge :

<table>
  <tr>
   <td><strong>Fonctionnalité</strong>
   </td>
   <td><strong>Existe dans l’ancienne expérience de commentaire.</strong>
   </td>
   <td><strong>Existe dans la nouvelle expérience de commentaire.</strong>
   </td>
   <td><strong>Sera introduite dans la nouvelle expérience de commentaire.</strong>
   </td>
   <td><strong>Date d’introduction dans la nouvelle expérience de commentaire</strong>
   </td>
   <td><strong>Dans la recherche</strong>
   </td>
  </tr>
  <tr>
   <td>Créer/lire/répondre à/supprimer des commentaires 
   </td>
   <td>✓ 
  </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Texte enrichi (à l’exclusion des citations et des emojis)
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Texte enrichi (emojis)
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Texte enrichi (citations)
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 2e trimestre 2023
   </td>
   <td> 
   </td>
  </tr>
  <tr>
<tr>
   <td> Commentaires sur les citations
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 2e trimestre 2023
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Réagir aux commentaires (J’aime) 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Joindre des images aux commentaires 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Taguer des personnes dans les commentaires 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Supprimer des participantes et participants au thread
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>


<tr>
   <td>Taguer automatiquement tous les participantes et participants au thread
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Commentaires privés d’une entreprise 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Annuler la publication d’un commentaire 
   </td>
   <td>✓ 
   </td>
   <td>Remplacé par un commentaire modifié 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Désactiver les mises à jour du système 
   </td>
   <td>✓ 
   </td>
   <td>Remplacé par l’onglet Activité 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Modifier les commentaires 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Sauvegarde des brouillons de commentaires lors de la navigation hors de la page 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Voir les nouveaux commentaires en temps réel (y compris lors de la suppression d’un commentaire)
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Enregistrer des heures 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>Copier le lien du thread 
   </td>
   <td>✓ 
   </td>
   <td> Remplacé par Copier le lien
   </td>
   <td> 
   </td>
   <td>2e trimestre 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Copier le lien du commentaire 
   </td>
   <td>✓ 
   </td>
   <td> Remplacé par Copier le lien
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Citer le texte du commentaire 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td>2e trimestre 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Copier le texte du message 
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>Rechercher dans les commentaires 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>1er trimestre 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Copier et coller des images dans un commentaire
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>1er trimestre 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Faire glisser et déposer des images dans un commentaire
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>1er trimestre 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Modifier le formulaire personnalisé 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Possibilité de modifier le statut, la condition, la date d’engagement lors de l’ajout de commentaires 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
  </tr>
<tr>
   <td>Répondre aux mises à jour du système 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
<tr>
   <td>Afficher « pour le compte de » lors de l’ajout de commentaires avec une connexion au nom d’une autre personne
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Possibilité pour la personne propriétaire du projet de modifier la date d’achèvement prévue d’une tâche lorsque la date d’engagement est modifiée à partir de la section Mises à jour
   </td>
   <td> ✓
   </td>
   <td> Peut être lancé à une date ultérieure
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> ✓
   </td>
  </tr>
</table>

## Calendrier des versions

>[!IMPORTANT]
>
>Pour plus d’informations sur les fonctionnalités ajoutées à la nouvelle expérience de commentaire pendant la période de version bêta, voir [Activité de version bêta de la nouvelle expérience de commentaire](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).
>
>Pour plus d’informations sur la gestion des mises à jour des objets Workfront, voir [Mettre à jour le travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


Voici une chronologie prévisionnel avec des étapes clés pour le lancement de la nouvelle expérience de commentaire dans l’environnement de production. En plus des étapes ci-dessous, nous continuerons à améliorer l’expérience de commentaire en y apportant de petites améliorations.

Pour plus d’informations sur les fonctionnalités de la nouvelle expérience de commentaire après la clôture de la période de version bêta, voir la page de vue d’ensemble de la version actuelle.

Voici le calendrier prévisionnel pour le lancement de la nouvelle expérience de commentaire :

* Avec la version 23.2 (6 avril 2023) :
   * Lancer la version bêta de l’expérience de commentaire pour les problèmes
   * Lancer la nouvelle expérience de commentaire pour les objectifs (comme expérience unique)
* Avec la version 23.3 (20 juillet 2023) :
   * Lancer la version bêta de l’expérience de commentaire pour les projets, les tâches et les documents.
   * Lancer la nouvelle expérience de commentaire pour les cartes dans la zone des panoramas (comme expérience unique)
* Lors de la version du quatrième trimestre 2023 (version limitée, uniquement pour les clientes et clients ayant choisi la version rapide) :
   * Lancer la nouvelle expérience de commentaire pour les modèles, les tâches des modèles, les programmes, les portfolios, les équipes, les utilisateurs et utilisatrices et les feuilles de temps (comme expérience unique)
   * Mettre à jour la version bêta de l’expérience de commentaire pour les projets, les tâches, les problèmes et les documents afin qu’elle devienne l’option par défaut. Le libellé « Version bêta » est supprimé.
* Avec la version du quatrième trimestre 2023 (23.10) (26 octobre 2023)
   * Lancer la nouvelle expérience de commentaire pour les modèles, les tâches des modèles, les programmes, les portfolios, les équipes, les utilisateurs et utilisatrices et les feuilles de temps (comme expérience unique) pour tous les clientes et clients.
   * Faire de la nouvelle expérience de commentaire pour les projets, les tâches, les problèmes et les documents l’option par défaut.

  >[!IMPORTANT]
  >
  >    Cette étape clôturera la phase de version bêta de la nouvelle expérience de commentaire.

   * Incluez toutes les fonctionnalités publiées pour la nouvelle expérience de commentaire à partir de cette date dans les versions mensuelles et trimestrielles normales actuelles.
* Fin de l’année 2023 :
   * Conserver l’expérience de commentaire héritée comme option secondaire pour les objets suivants : projets, tâches, problèmes et documents. La nouvelle expérience de commentaire est l’option par défaut pour tous les utilisateurs et utilisatrices de ces objets.
   * Faire de la nouvelle expérience de commentaire la seule expérience pour tous les autres objets.

  >[!NOTE]
  >
  >    Les itérations continueront à utiliser l’expérience de commentaire héritée. La nouvelle expérience de commentaire ne sera pas disponible pour les itérations.

* Avec la version du deuxième trimestre 2024 (11 avril 2024) :

  Supprimer l’option permettant de revenir au flux de commentaires hérité et définissez le nouveau flux de commentaires comme la seule expérience pour tous les objets.

## Localiser la nouvelle expérience de commentaire

La nouvelle expérience de commentaire est disponible dans les zones suivantes de Workfront :

* Dans la section Mises à jour de tous les objets.

  Pour plus d’informations sur l’accès à la section Mises à jour des objets Workfront, voir [Vue d’ensemble de la section Mises à jour](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

* Dans le panneau Résumé de tâches, de problèmes et de documents dans toutes les zones où cela est disponible (listes, feuilles de temps, Équilibreur de charge de travail et Accueil).
* Dans la zone Accueil pour les tâches et les problèmes.



<!--

The new commenting experience is currently available for all customers and for all environments.

Depending on what objects you access the commenting experience for, you might see the following functionality for the Updates section:

* Both the new and legacy commenting experience for the following objects: 

    * Project
    * Task (this includes Stories)
    * Issue
    * Document

      >[!NOTE]
      >
      ><span class="preview">The legacy commenting experience has been removed from the Preview environment since April 1, 2024. </span>

* Only the new commenting experience for the objects listed below. There is no option to enable the legacy commenting experience for these objects:   

    * Goal

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
  * Card on a board
  * Team
  * Template
  * Template Task
  * Timesheet
  * Program
  * Portfolio
  * User

* Only the legacy commenting experience for the following objects:

  * Iterations
    
    There is no option to enable the new commenting experience for iterations. Only the legacy commenting experience is available for iterations. 

-->


<!--before August 17: 

The new commenting experience is currently supported for the following objects:


* When enabling the Beta experience in the Updates section for 

    * Issues, projects, tasks, and documents

    For more information about managing updates for Workfront objects, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

* By default, as the only commenting experience for

    * Goals, cards on a board

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

-->

<!--Depending on the environment you access the commenting experience you can do one of the following: 

* Enable the commenting experience Beta in the Production environment
* <span class="preview">Enable the legacy commenting experience in the Preview  environment </span>
-->

<!--

To enable the commenting experience option for projects, tasks, issues, and documents: 

1. (Conditional) In the Production environment, go to an object that you want to activate the new commenting experience for, then click **Updates** in the left panel.
1. (Conditional) If it is disabled, enable the **New commenting** option in the upper-right corner of the Updates area to enable it. This should be enabled by default. 
<span class="preview">The New commenting option has been removed from the Preview environment.</span> 

    ![](assets/new-commenting-toggle-off-highlighted.png)

1. Start typing an update in the **Comments** tab. The Comments tab is the default tab when the new experience opens

    Or

    Click the  **System Activity** tab to view the activity updates generated by Workfront. 

1. (Optional) To disable the new commenting experience and return to legacy commenting, deselect the **New commenting** option. 

-->
