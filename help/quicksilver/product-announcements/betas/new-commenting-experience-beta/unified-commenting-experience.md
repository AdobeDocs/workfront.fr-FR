---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: Nouvelle expérience de commentaire
description: Une mise à jour de l’expérience de commentaires dans Adobe Workfront est actuellement en cours de développement. Cette mise à jour inclut une nouvelle interface, de nouvelles fonctionnalités et une amélioration des performances dans la section Mises à jour de certains objets.
author: Alina
feature: Product Announcements
role: User
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: c3abb5dce14c0b19ab2e5b82f159cd29f80f79e4
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 3%

---

# Nouvelle expérience de commentaire


<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Il est disponible uniquement dans l’environnement Aperçu pour tous les clients.  </span>

<span class="preview">Pour plus d’informations sur le calendrier de publication actuel, voir [Présentation de la version du premier trimestre 2024](../../product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

<!--

After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases.

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  -->

>[!IMPORTANT]
>
>Les informations de cet article font référence aux fonctionnalités qui ont été publiées dans le cadre de la nouvelle expérience de commentaires.
>
>Le programme bêta pour la nouvelle expérience de commentaires a commencé en avril 2023 et s&#39;est terminé en octobre 2023. Le programme bêta pour la nouvelle expérience de commentaires a été mis en place avec la version d’octobre 2023.
>
>Les fonctionnalités décrites dans cet article ont été publiées pour tous les clients en octobre 2023, sauf indication contraire.

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

Les fonctionnalités suivantes ont été supprimées de la nouvelle expérience :

* Commentaire sur une mise à jour du système
* Possibilité de modifier l’état, la condition, la date de validation tout en commentant
* Modifier le formulaire personnalisé
* Les informations &quot;au nom de &lt; nom d’utilisateur >&quot; lorsqu’un administrateur Workfront ou de groupe se connecte en tant qu’autre utilisateur et ajoute un commentaire en leur nom ont été supprimées à l’origine. Il a été rétabli le 19 octobre 2023.
* L’option &quot;Demander l’approbation&quot; lorsque vous balisez des personnes en ajoutant un commentaire à un document.

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
   <td> <span class="preview">✓</span>
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
   <td> <span class="preview">✓</span>
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
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>1er trimestre 2024 
   </td>
   <td>✓ 
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
   <td>Possibilité de modifier l’état, la condition, la date de validation tout en commentant 
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
</table>

## Calendrier des versions

Pour plus d’informations sur les fonctionnalités récemment publiées dans le cadre de la nouvelle expérience de commentaires, ainsi que sur la chronologie de la mise à jour, voir [Nouvelle activité de commentaires sur la version bêta de l’expérience](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).

Pour plus d’informations sur la gestion des mises à jour des objets Workfront, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

## Localisation de la nouvelle expérience de commentaire

&lt;!—IMPORTANT : lorsque nous supprimons l’expérience héritée, déplacez une version de celle-ci vers l’article de travail Mise à jour ou la présentation de la section Mise à jour — pour dire que l’expérience est différente pour tous, à l’exception des itérations —>

La nouvelle expérience de commentaire est actuellement disponible pour tous les clients et pour tous les environnements.

Selon les objets pour lesquels vous accédez à l’expérience de commentaire, les fonctionnalités suivantes peuvent s’afficher dans la section Mises à jour :

* L’expérience de commentaire nouvelle et héritée pour les objets suivants :

   * Projet
   * Tâche (y compris les articles)
   * Problème
   * Document

  >[!TIP]
  >
  >Utilisez l’option Nouveau commentaire pour afficher la nouvelle expérience de commentaire (lorsque vous l’activez) ou l’expérience de commentaire héritée (lorsque vous la désactivez), comme décrit dans cette section. La nouvelle expérience de commentaire est la valeur par défaut.

   * Seule la nouvelle expérience de commentaire pour les objets répertoriés ci-dessous. Il n’existe pas d’option permettant d’activer l’expérience héritée de commentaires pour ces objets :

      * Objectif

     >[!NOTE]
     >
     >Pour pouvoir accéder à cette zone de Workfront, vous devez disposer d’une licence supplémentaire pour les objectifs Adobe Workfront. Pour plus d’informations, voir [Conditions requises pour utiliser les objectifs Workfront](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
      * Carte sur un panorama
      * Équipe
      * Modèle
      * Tâche de modèle
      * Feuille de temps
      * Programme
      * Portfolio
      * l’utilisateur ou de l’utilisatrice

* Seule l’expérience de commentaire héritée pour les objets suivants :

   * Itérations

     Il n’existe pas d’option permettant d’activer la nouvelle expérience de commentaire pour les itérations. Seule l’expérience de commentaire héritée est disponible pour les itérations.


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

Pour activer l’option d’expérience de commentaire pour les projets, les tâches, les problèmes et les documents, procédez comme suit :

1. Accédez à un objet pour lequel vous souhaitez activer la nouvelle expérience de commentaire, puis cliquez sur **Mises à jour** dans le panneau de gauche.
1. (Conditionnel) Si elle est désactivée, activez la variable **Nouveaux commentaires** dans le coin supérieur droit de la zone Mises à jour pour l’activer. Cette option doit être activée par défaut.

   ![](assets/new-commenting-toggle-off-highlighted.png)

1. Commencez à saisir une mise à jour dans la variable **Commentaires** . L’onglet Commentaires est l’onglet par défaut à l’ouverture de la nouvelle expérience.

   Ou

   Cliquez sur le bouton  **Activité du système** pour afficher les mises à jour d’activité générées par Workfront.

1. (Facultatif) Pour désactiver la nouvelle expérience de commentaire et revenir à la création de commentaires hérités, désélectionnez l’option **Nouveaux commentaires** .

