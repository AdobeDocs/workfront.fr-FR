---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.2, version bêta 1
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.2 de Beta 1. Cette fonctionnalité a été rendue disponible dans l’environnement Aperçu le 22 mars 2018. Il sera disponible dans l'environnement de production en juin 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 1%

---

# Activité Version 2018.2, version bêta 1

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement Aperçu avec la version 2018.2 de Beta 1. Cette fonctionnalité a été rendue disponible dans l’environnement Aperçu le 22 mars 2018. Il sera disponible dans l&#39;environnement de production en juin 2018.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées en 2018.2, consultez la [présentation de l’activité de version 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La version 2018.2 de Beta 1 contient les améliorations suivantes :

* [ Modifier les dates des tâches dans le diagramme de Gantt ](#modify-task-dates-in-the-gantt-chart)
* [Accédez au diagramme de Gantt du projet à partir de l’onglet Mises à jour](#access-the-project-gantt-chart-from-the-updates-tab) (temporairement supprimé)

* [Divers liens réintroduits dans les documents de la liste de documents](#various-links-re-introduced-to-documents-on-the-document-list)
* [Améliorations de l’affichage des utilisateurs dans le planificateur de ressources](#user-view-improvements-in-the-resource-planner)
* [Nouvelle expérience de liste de projets](#new-project-list-experience)
* [Nouvel onglet Recherche de mises à jour](#new-look-for-updates-tab)
* [Améliorations des périphériques mobiles](#mobile-improvements)

## Modification des dates de tâche dans le diagramme de Gantt {#modify-task-dates-in-the-gantt-chart}

Vous pouvez maintenant faire glisser la bulle de tâche pour modifier les dates de début et de fin planifiées dans le diagramme de Gantt. Grâce à cette modification, vous pouvez appliquer des scénarios d’exécution à votre projet sans affecter la chronologie.

Avant cette modification, vous ne pouviez modifier les dates des tâches qu’au niveau de la liste des tâches ou de la tâche.

Pour plus d’informations, voir [Mise à jour d’informations dans la liste de tâches Graphique de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Accès au diagramme de Gantt du projet à partir de l’onglet Mises à jour {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>Cette fonctionnalité a été temporairement supprimée de l’environnement Aperçu.

Vous pouvez maintenant accéder au nouveau diagramme Gantt du projet à partir de l’onglet Mises à jour . Lorsqu’un utilisateur modifie la date de validation d’une tâche d’une manière qui affecte la chronologie du projet, vous pouvez afficher l’impact dans le diagramme de Gantt du projet.

Avant cette modification, le lien Chronologie du projet ouvrait le diagramme de Gantt hérité.

Pour plus d’informations, voir [Présentation de la date de validation](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

Pour plus d’informations, voir [Présentation de Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Divers liens réintroduits dans les documents de la liste de documents {#various-links-re-introduced-to-documents-on-the-document-list}

Dans la version 18.1, divers liens ont été supprimés des documents de la liste de documents et déplacés vers d’autres zones de l’interface (certains sous forme de bouton en regard du nom du document, d’autres dans un menu déroulant sur le bouton). Les liens suivants sont réintroduits sous le nom du document avec cette version et sont désormais disponibles dans les documents individuels de la liste des documents :

* Générer un bon à tirer (disponible lorsqu’un bon à tirer n’est pas encore généré)
* Bon à tirer ouvert (disponible lorsqu’un BAT est généré)
* Détails du document (disponibles lorsqu’un BAT n’est pas encore généré)
* Détails du BAT (disponibles lorsqu’un BAT est généré)
* Imprimer le résumé

Les actions suivantes ne sont pas réintroduites en tant que liens dans le document dans la liste de documents :

* Partager (toujours disponible sous forme de bouton dans le menu)
* Extraire / Archiver (toujours disponible dans le menu déroulant Plus du menu)

Pour plus d’informations, voir les sections suivantes :

*  in 

## Améliorations de la vue utilisateur dans le planificateur de ressources {#user-view-improvements-in-the-resource-planner}

L’affichage utilisateur du planificateur de ressources contient désormais les améliorations suivantes :

* La vue Utilisateur est désormais la vue par défaut, remplaçant la vue Projet.
* Amélioration des filtres qui extraient les informations de l’ensemble de la base de données, plutôt que simplement des informations à l’écran.
* Mode Plein écran.
* Les performances sont désormais plus rapides et plus efficaces.

   * Nouvelles limites pour le nombre d’utilisateurs, de projets, de rôles et de tâches que vous pouvez afficher.
   * Chargement différé, pour un chargement plus rapide des utilisateurs.

La fonctionnalité suivante a été temporairement désactivée dans le planificateur de ressources :

* Exportation des données à partir du planificateur de ressources lors de l’utilisation de la vue utilisateur.

Avant ces améliorations, vous avez signalé que le planificateur de ressources était lent à charger et que vous aviez remarqué des incohérences dans les données affichées. Ces améliorations devraient maintenant être éliminées.

Pour plus d’informations sur les zones du planificateur de ressources, consultez la [présentation de la navigation du planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## Nouvelle expérience de liste de projets {#new-project-list-experience}

Une nouvelle expérience est désormais disponible lors de l’affichage d’une liste de projets. Cette expérience inclut des performances accrues et une navigation par liste plus fluide et plus rapide. Seules les listes de l’onglet Projets de la zone Projets de Workfront ont été mises à jour pour cette nouvelle expérience.

La plupart du temps, les changements concernent la vitesse et l’efficacité de la liste. Les modifications visibles suivantes ont également été introduites :

* La liste affiche jusqu’à 2 000 éléments par défaut.

  Avant cette amélioration, la liste affichait 100 éléments.

* Les groupes sont réduits par défaut.

  Avant cette modification, les regroupements étaient développés par défaut.

* La zone de sélection d’une ligne a été étendue à la ligne entière.

Les fonctionnalités suivantes ont été temporairement désactivées dans les listes de projets spécifiées :

* Redimensionnement des colonnes (cette fonctionnalité a été réintroduite dans la version 2018.2 de Beta 5)
* Réorganisation des colonnes
* Les champs d’icône d’état s’affichent comme vides (cette fonctionnalité a été réintroduite dans la version 2018.2 de Beta 5)
* Le graphique Gantt n’est pas accessible (cette fonctionnalité a été réintroduite dans la version 2018.2 de Beta 3.)

Pour plus d’informations sur l’utilisation des listes, voir [Prise en main des listes dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Nouvel onglet Recherche des mises à jour {#new-look-for-updates-tab}

>[!NOTE]
>
>Pour certains utilisateurs, le nouvel onglet Mises à jour peut ne pas s’afficher dans l’environnement Aperçu . Notre équipe de développement est en train de résoudre le problème et de travailler à le résoudre le plus tôt possible.

L’aspect de l’onglet Mises à jour a été modifié afin d’être plus aligné sur les autres zones de l’interface. Cette modification s’applique aux projets, aux tâches, aux problèmes et aux documents.

Le tableau suivant répertorie les mises à jour apportées à l’onglet Mises à jour :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tâche</strong> </p> </th> 
   <th> <p><strong>Action de l’utilisateur précédent</strong> </p> </th> 
   <th> <p><strong>Nouvelle action utilisateur</strong> </p> </th> 
   <th> <p><strong>Pour plus d’informations, voir..</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Temps de journalisation sur une feuille de temps</p> </td> 
   <td> <p>Cliquez sur le lien Heure de journal</p> </td> 
   <td> <p>Cliquez sur le bouton Temps journal</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Consigner le temps</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Filtrage des mises à jour système dans l’onglet Mises à jour</p> </td> 
   <td> <p>Cliquez sur le lien Filtrer les mises à jour du système .</p> </td> 
   <td> <p>Désactivation du bouton activer/désactiver Afficher le journal d’activité</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mise à jour du travail</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Affichage des mises à jour du système dans l’onglet Mises à jour</p> </td> 
   <td> <p>Cliquez sur Afficher toutes les mises à jour .</p> </td> 
   <td> <p>Activez le bouton bascule Afficher le journal d’activité .</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mise à jour du travail</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Balisage d’autres utilisateurs sur une mise à jour ou un commentaire</p> </td> 
   <td> <p>Cliquez sur l’icône Inclure les autres dans cette mise à jour</p> </td> 
   <td> <p>Ajouter des utilisateurs et des équipes dans le champ Notifier</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mise à jour du travail</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autoriser uniquement les utilisateurs de votre entreprise à afficher un objet</p> </td> 
   <td> <p>Cliquez sur l’icône Verrouiller</p> </td> 
   <td> <p>Activez le bouton bascule Privé à ma société .</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Baliser d'autres mises à jour</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autoriser les utilisateurs en dehors de votre entreprise à afficher un objet</p> </td> 
   <td> <p>Cliquez sur l’icône Verrouiller</p> </td> 
   <td> <p>Désactiver le bouton activer/désactiver de Privé à ma société</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Baliser d'autres mises à jour</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ajouter une réponse ou mettre à jour un commentaire ou mettre à jour</p> </td> 
   <td> <p>Cliquez sur le bouton Commenter .</p> </td> 
   <td> <p>Cliquez sur le bouton Répondre ou Mettre à jour .</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mise à jour du travail</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Mettre à jour l’état de la tâche</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Mettre à jour la condition pour les tâches et les problèmes</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">Ajouter une mise à jour à un document</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Améliorations des périphériques mobiles {#mobile-improvements}

L’application mobile contient les améliorations suivantes :

* Les liens partagés avec vous dans d’autres applications mobiles s’ouvrent désormais dans l’application mobile Workfront.

  Pour plus d’informations sur le partage de liens, voir .

  Cette mise à jour sera publiée sur iOS parfois cette semaine et la mise à jour d’Android devrait suivre peu de temps après.

* Nous avons mis à jour nos exigences de prise en charge de la plateforme iOS pour prendre en charge iPhone X.

  Pour plus d’informations sur les périphériques mobiles et les systèmes d’exploitation pris en charge, voir .
