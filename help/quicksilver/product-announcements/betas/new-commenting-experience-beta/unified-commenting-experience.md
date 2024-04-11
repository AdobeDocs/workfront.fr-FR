---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: Nouvelle expérience de commentaire
description: Une mise à jour de l’expérience de commentaires dans Adobe Workfront est actuellement en cours de développement. Cette mise à jour inclut une nouvelle interface, de nouvelles fonctionnalités et une amélioration des performances dans la section Mises à jour de certains objets.
author: Alina
feature: Product Announcements
role: User
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: c6575c832fa21a17a1d20fa7e92798d970ca0f50
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 0%

---

# Nouvelle expérience de commentaire

<!--take out legacy, preview, prod references from below-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

-->

>[!IMPORTANT]
>
>Les informations de cet article font référence aux fonctionnalités qui ont été publiées dans le cadre de la nouvelle expérience de commentaires.
>
>Le programme bêta pour la nouvelle expérience de commentaires a commencé en avril 2023 et s&#39;est terminé en octobre 2023. Le programme bêta pour la nouvelle expérience de commentaires a été mis en place avec la version d’octobre 2023.
>
>À compter d’octobre 2023, toutes les nouvelles fonctionnalités relatives à la nouvelle expérience de commentaire seront publiées pour tous les clients. Pour plus d’informations, consultez la page d’aperçu de la version actuelle de chaque version.

<!--An update to the commenting experience in Adobe Workfront is currently in development. This update includes a new interface, new features, and improved performance in the Updates section of select objects. 

The new commenting experience will slowly become available for all the objects with an Updates section in Workfront, and later it will expand to other Adobe Experience Cloud applications.-->

<!--For additional resources for the new commenting experience, also see the following articles:

* [New commenting experience release activity](../new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md)
* [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md)
-->

## Fonctionnalités

La nouvelle expérience de commentaire comprend des améliorations et des modifications apportées à la section Mises à jour des objets Adobe Workfront.

Les améliorations suivantes ont été apportées à la nouvelle expérience de commentaires :

* Amélioration des performances et de l’expérience utilisateur
* Séparation des commentaires des utilisateurs des mises à jour de l’activité du système
* Indicateur en temps réel lorsque de nouveaux commentaires sont ajoutés à un objet
* Modification des commentaires après leur envoi

Les fonctionnalités suivantes ont été supprimées ou seront obsolètes de la nouvelle expérience :

* Commentaire sur une mise à jour du système. Les commentaires ajoutés aux mises à jour du système par le passé ont été importés en tant que commentaires en lecture seule dans le nouvel onglet Activité du système .
* Possibilité de modifier l’état, la condition, la date de validation et le pourcentage d’achèvement tout en commentant les tâches et les problèmes.

  Nous vous recommandons également d’ajouter ces champs dans le panneau Résumé des tâches et des problèmes afin de pouvoir y accéder facilement à partir des listes, de l’Accueil, de l’équilibreur Workfront ou d’une feuille de temps.
* Possibilité de modifier le formulaire personnalisé
* Les informations &quot;au nom de &lt; nom d’utilisateur >&quot; lorsqu’un administrateur Workfront ou de groupe se connecte en tant qu’autre utilisateur et ajoute un commentaire en leur nom ont été supprimées à l’origine. Il a été rétabli le 19 octobre 2023.
* L’option &quot;Demander l’approbation&quot; lorsque vous balisez des personnes en ajoutant un commentaire à un document.
* Le paramètre &quot;Afficher le pourcentage terminé à la mise à jour&quot; lors de la modification de la zone de profil d’un utilisateur est supprimé. La fonctionnalité de mise à jour du pourcentage d’achèvement d’une tâche ou d’un problème a été supprimée.


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

Le tableau suivant illustre les fonctionnalités qui seront disponibles dans la nouvelle expérience de commentaire, ainsi que leur disponibilité dans les zones où elles sont prises en charge :

<table>
  <tr>
   <td><strong>Fonctionnalité </strong>
   </td>
   <td><strong>Existe dans l’ancienne expérience de commentaire </strong>
   </td>
   <td><strong>Existe dans la nouvelle expérience de commentaire </strong>
   </td>
   <td><strong>Sera introduit dans la nouvelle expérience de commentaire </strong>
   </td>
   <td><strong>Quand sera introduit dans la nouvelle expérience de commentaire </strong>
   </td>
   <td><strong>En recherche </strong>
   </td>
  </tr>
  <tr>
   <td>Créer/lire/répondre/supprimer des commentaires 
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
   <td>Texte enrichi (hors guillemets et émoticônes)
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
   <td>Texte enrichi (guillemets anglais)
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 2e trimestre 2023
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
   <td> 2e trimestre 2023
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Réaction aux commentaires (j’aime) 
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
   <td>Ajout d’images aux commentaires 
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
   <td>Balisage des personnes dans les commentaires 
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
   <td>Suppression des participants de thread
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
   <td>Balisage automatique de tous les participants au thread
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
   <td>Commentaires privés à une entreprise 
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
   <td>Remplacé par le commentaire Modifier 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Désactivation des mises à jour système 
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
   <td>Enregistrement des brouillons de commentaires lors de la navigation en dehors de la page 
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
   <td>Voir les nouveaux commentaires en temps réel (notamment le moment où un commentaire est supprimé)
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
   <td> Remplacé par le lien Copier
   </td>
   <td> 
   </td>
   <td>2e trimestre 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Copier le lien du commentaire 
   </td>
   <td>✓ 
   </td>
   <td> Remplacé par le lien Copier
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Texte du commentaire de la citation 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td>2e trimestre 2023 
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
   <td>Recherche dans les commentaires 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>1er trimestre 2024 
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
   <td>1er trimestre 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Glisser-déposer des images dans un commentaire
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>1er trimestre 2024 
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
   <td>Possibilité de modifier l’état, la condition, la date de validation lors de l’ajout de commentaires 
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
   <td>Réponse aux mises à jour du système 
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
   <td>Afficher "au nom de" lors de l’ajout de commentaires connectés en tant qu’autre utilisateur
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
   <td>Possibilité pour le propriétaire du projet de modifier la date d’achèvement planifiée d’une tâche lorsque la date de validation est modifiée à partir de la section Mises à jour
   </td>
   <td> ✓
   </td>
   <td> Peut être publié à une date ultérieure
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
>Pour plus d’informations sur les fonctionnalités publiées dans la nouvelle expérience de commentaires au cours de la période bêta, voir [Nouvelle activité de commentaires sur la version bêta de l’expérience](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).
>
>Pour plus d’informations sur la gestion des mises à jour des objets Workfront, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


Vous trouverez ci-dessous une chronologie planifiée avec des jalons clés pour la publication de la nouvelle expérience de commentaire dans l’environnement de production. Outre les jalons ci-dessous, nous continuerons à améliorer l’expérience de commentaires grâce à des améliorations plus modestes.

Pour plus d’informations sur les fonctionnalités publiées pour la nouvelle expérience de commentaires après la fin de la période bêta, consultez la page de présentation de la version actuelle.

Voici un calendrier planifié de la publication de la nouvelle expérience de commentaires :

* Avec la version 23.2 (6 avril 2023) :
   * Lancement de l’expérience de commentaires bêta pour les problèmes
   * Publication de la nouvelle expérience de commentaire pour les objectifs (comme seule expérience)
* Avec la version 23.3 (20 juillet 2023) :
   * Lancez la version bêta des commentaires pour les projets, les tâches et les documents.
   * Publication de la nouvelle expérience de commentaires pour les cartes dans la zone Panoramas (comme seule expérience)
* Au cours de la version du quatrième trimestre 2023 (version limitée, disponible uniquement pour les clients qui choisissent la version rapide) :
   * Libérez la nouvelle expérience de commentaires pour les modèles, les tâches de modèle, les programmes, les portefeuilles, les équipes, les utilisateurs et les feuilles de temps (comme seule expérience).
   * Mettez à jour l’expérience de commentaire bêta pour que les projets, les tâches, les problèmes et les documents deviennent l’option par défaut. Le libellé &quot;Beta&quot; est supprimé.
* Avec la version du quatrième trimestre 2023 (23.10) (26 octobre 2023)
   * Libérez la nouvelle expérience de commentaires pour les modèles, les tâches de modèle, les programmes, les portefeuilles, les équipes, les utilisateurs et les feuilles de temps (la seule expérience) à tous les clients.
   * Faites de la nouvelle expérience de commentaire pour les projets, les tâches, les problèmes et les documents l’option par défaut.

  >[!IMPORTANT]
  >
  >    Cela mettra fin à l’étape bêta de la nouvelle expérience de commentaire.

   * Publiez toutes les fonctionnalités relatives à la nouvelle expérience de commentaires, à partir de cette date, dans les versions mensuelles et trimestrielles actuelles.
* Fin 2023 :
   * Conservez l’expérience héritée de commentaires comme option secondaire pour les objets suivants : projets, tâches, problèmes et documents. La nouvelle expérience de commentaire est l’option par défaut pour tous les utilisateurs de ces objets.
   * Faites de la nouvelle expérience de commentaire la seule expérience pour tous les autres objets.

  >[!NOTE]
  >
  >    Les itérations conserveront l’expérience héritée de commentaires. La nouvelle expérience de commentaire ne sera pas disponible pour les itérations.

* Avec la version du deuxième trimestre 2024 (11 avril 2024) :

   * Supprimez l’option permettant de revenir au flux de commentaires hérité et de faire du nouveau flux de commentaires la seule expérience pour tous les objets, à l’exception des itérations.

## Localisation de la nouvelle expérience de commentaire

<!--info for April 11: make this commented out text live and hide everything else underneath it, all the way to the end of the article:-->

>[!IMPORTANT]
>
>La nouvelle expérience de commentaire est disponible dans tous les environnements Workfront sur tous les objets, à l’exception des itérations.
>
>L’expérience héritée de commentaires a été supprimée de tous les environnements pour les projets, les tâches, les problèmes et les documents.

Pour plus d’informations sur l’accès à la section Mises à jour des objets Workfront, voir [Présentation de la section Mises à jour](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

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
