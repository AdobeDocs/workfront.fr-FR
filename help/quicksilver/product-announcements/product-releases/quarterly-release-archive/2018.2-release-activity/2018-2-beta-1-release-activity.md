---
content-type: release-notes
navigation-topic: product-releases-archive
title: Activité Version 2018.2, version bêta 1
description: Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation avec la version 2018.2, version bêta 1. Cette fonctionnalité a été mise à disposition dans l’environnement de prévisualisation le 22 mars 2018. Elle a été rendue disponible dans l’environnement de production en juin 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: cbe98ee2-f155-4d31-88c4-7f41b6f91eb2
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 100%

---

# Activité Version 2018.2, version bêta 1

Cette page décrit toutes les modifications les plus récentes disponibles dans l’environnement de prévisualisation avec la version 2018.2, version bêta 1. Cette fonctionnalité a été mise à disposition dans l’environnement de prévisualisation le 22 mars 2018. Elle a été rendue disponible dans l’environnement de production en juin 2018.

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2018.2, voir [Vue d’ensemble de l’activité Version 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

La version 2018.2, version bêta 1 contient les améliorations suivantes :

* [Modification des dates de tâches dans le graphique de Gantt](#modify-task-dates-in-the-gantt-chart)
* [Accès au graphique de Gantt du projet à partir de l’onglet Mises à jour](#access-the-project-gantt-chart-from-the-updates-tab) (temporairement supprimé)

* [Réintroduction de divers liens dans les documents de la liste de documents](#various-links-re-introduced-to-documents-on-the-document-list)
* [Améliorations de la vue utilisateur dans le planificateur de ressources](#user-view-improvements-in-the-resource-planner)
* [Nouvelle expérience de liste de projets](#new-project-list-experience)
* [Nouvel aspect de l’onglet Mises à jour](#new-look-for-updates-tab)
* [Améliorations apportées à l’application mobile](#mobile-improvements)

## Modifier des dates de tâches dans le graphique de Gantt {#modify-task-dates-in-the-gantt-chart}

Vous pouvez maintenant faire glisser la bulle de tâche pour modifier les dates de début et d’achèvement prévues dans le graphique de Gantt. Grâce à cette modification, vous pouvez appliquer des scénarios d’hypothèses à votre projet sans affecter la chronologie.

Avant cette modification, vous ne pouviez modifier les dates de tâches que dans la liste des tâches ou au niveau de la tâche.

Pour plus d’informations, voir [Mettre à jour des informations du graphique de Gantt de la liste de tâches](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Accéder au graphique de Gantt du projet à partir de l’onglet Mises à jour {#access-the-project-gantt-chart-from-the-updates-tab}

>[!NOTE]
>
>Cette fonctionnalité a été temporairement supprimée de l’environnement de prévisualisation.

Vous pouvez maintenant accéder au nouveau graphique de Gantt du projet à partir de l’onglet Mises à jour. Lorsqu’un utilisateur ou une utilisatrice modifie la date d’engagement d’une tâche d’une manière qui affecte la chronologie du projet, vous pouvez afficher l’impact dans le graphique de Gantt du projet.

Avant cette modification, le lien de la chronologie du projet ouvrait le graphique de Gantt hérité.

Pour plus d’informations, voir [Vue d’ensemble de la date d’engagement](../../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

Pour plus d’informations, voir [Vue d’ensemble de l’optimisateur de portfolio](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

## Réintroduction de divers liens vers les documents de la liste de documents {#various-links-re-introduced-to-documents-on-the-document-list}

Dans la version 18.1, divers liens ont été supprimés des documents de la liste de documents et déplacés vers d’autres zones de l’interface (certains sous forme de bouton en regard du nom du document, d’autres dans un menu déroulant sur le bouton). Avec cette version, les liens suivants sont réintroduits sous le nom du document et sont désormais disponibles dans des documents individuels de la liste de documents :

* Créer une épreuve (disponible lorsqu’une épreuve n’est pas encore générée)
* Ouvrir l’épreuve (disponible lorsqu’une épreuve est générée)
* Détails du document (disponible lorsqu’une épreuve n’est pas encore générée)
* Détails de l’épreuve (disponible lorsqu’une épreuve est générée)
* Imprimer le résumé

Les actions suivantes ne sont pas réintroduites sous forme de liens sur le document dans la liste de documents :

* Partager (toujours disponible sous forme de bouton dans le menu)
* Extraire/Archiver (toujours disponible dans le menu déroulant Plus du menu)

Pour plus d’informations, consultez les sections suivantes :

* dans

## Améliorations de la vue utilisateur dans le planificateur de ressources {#user-view-improvements-in-the-resource-planner}

La vue utilisateur du planificateur de ressources contient désormais les améliorations suivantes :

* La vue utilisateur est désormais la vue par défaut, remplaçant la vue projet.
* Amélioration des filtres qui extraient les informations de l’ensemble de la base de données, plutôt que les informations à l’écran seulement.
* Mode Plein écran.
* Les performances sont désormais plus rapides et plus efficaces.

   * Nouvelles limites d’affichage pour le nombre d’utilisateurs et d’utilisatrices, de projets, de rôles et de tâches.
   * Chargement différé (lazy loading), pour un chargement plus rapide des utilisateurs et des utilisatrices.

La fonctionnalité suivante a été temporairement désactivée dans le planificateur de ressources :

* export des données à partir du planificateur de ressources en vue utilisateur

Avant ces améliorations, vous avez signalé que le planificateur de ressources était lent à charger et que les données affichées présentaient des incohérences. Ces problèmes sont à présent résolus grâce à ces améliorations.

Pour plus d’informations sur les zones du planificateur de ressources, consultez la section [Vue d’ensemble de la navigation du planificateur de ressources](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a></p>
-->

## Nouvelle expérience de liste de projets {#new-project-list-experience}

L’affichage des listes de projets fait peau neuve. Vous bénéficiez de meilleures performances et d’une navigation par liste plus fluide et rapide. Cette mise à jour ne concerne que les listes de l’onglet Projets de la zone Projets de Workfront.

Ces améliorations portent essentiellement sur la rapidité et l’efficacité de la liste. Les modifications suivantes ont été ajoutées :

* Affichage de jusqu’à 2 000 éléments par défaut.

  (Avant cette amélioration, la liste affichait 100 éléments.)

* Réduction des regroupements par défaut.

  (Avant cette modification, les regroupements étaient développés par défaut.)

* Extension de la zone de sélection d’une ligne à la ligne entière.

Les fonctionnalités suivantes ont été temporairement désactivées dans les listes de projets spécifiées :

* Redimensionnement des colonnes (cette fonctionnalité a été réintroduite dans la version 2018.2, version bêta 5).
* Réorganisation des colonnes.
* Les champs d’icône de statut s’affichent comme vides (cette fonctionnalité a été réintroduite dans la version 2018.2, version bêta 5).
* Le diagramme de Gantt n’est pas accessible (cette fonctionnalité a été réintroduite dans la version 2018.2, version bêta 3).

Pour plus d’informations sur l’utilisation des listes, consultez la section [Commencer avec les listes dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Nouvel aspect de l’onglet Mises à jour {#new-look-for-updates-tab}

>[!NOTE]
>
>Pour certaines personnes, le nouvel onglet Mises à jour peut ne pas s’afficher dans l’environnement de prévisualisation. Notre équipe de développement travaille à résoudre le problème le plus rapidement possible.

L’aspect de l’onglet Mises à jour est désormais harmonisé avec les autres zones de l’interface. Cette modification s’applique aux projets, aux tâches, aux problèmes et aux documents.

Le tableau suivant répertorie les mises à jour apportées à l’onglet Mises à jour :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tâche</strong> </p> </th> 
   <th> <p><strong>Action utilisateur précédente</strong> </p> </th> 
   <th> <p><strong>Nouvelle action utilisateur</strong> </p> </th> 
   <th> <p><strong>Pour plus d’informations, voir...</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Consigner les heures sur une feuille de temps</p> </td> 
   <td> <p>Cliquer sur le lien Consigner les heures</p> </td> 
   <td> <p>Cliquer sur le bouton Consigner les heures</p> </td> 
   <td> <p><a href="../../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Consigner les heures</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Filtrer les mises à jour système dans l’onglet Mises à jour</p> </td> 
   <td> <p>Cliquer sur le lien Filtrer les mises à jour système</p> </td> 
   <td> <p>Désactiver le bouton (bascule) Afficher le journal d’activité</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mettre à jour le travail</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Afficher les mises à jour système dans l’onglet Mises à jour</p> </td> 
   <td> <p>Cliquer sur Afficher toutes les mises à jour</p> </td> 
   <td> <p>Activer le bouton (bascule) Afficher le journal d’activité</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mettre à jour le travail</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Taguer d’autres utilisateurs et utilisatrices lors d’une mise à jour ou d’un commentaire</p> </td> 
   <td> <p>Cliquer sur l’icône Inclure d’autres utilisateurs et utilisatrices pour cette mise à jour</p> </td> 
   <td> <p>Ajouter des utilisateurs, des utilisatrices et des équipes dans le champ Notifier</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mettre à jour le travail</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autoriser les utilisateurs et utilisatrices de votre entreprise à afficher un objet uniquement</p> </td> 
   <td> <p>Cliquer sur l’icône de verrouillage</p> </td> 
   <td> <p>Activer le bouton (bascule) Réservé à mon entreprise.</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Taguer d’autres personnes sur les mises à jour</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Autoriser les utilisateurs et utilisatrices en dehors de votre entreprise à afficher un objet</p> </td> 
   <td> <p>Cliquer sur l’icône de verrouillage</p> </td> 
   <td> <p>Désactiver le bouton (bascule) Réservé à mon entreprise</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md" class="MCXref xref">Taguer d’autres personnes sur les mises à jour</a> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ajouter une réponse ou mettre à jour un commentaire ou une mise à jour</p> </td> 
   <td> <p>Cliquer sur le bouton Commenter</p> </td> 
   <td> <p>Cliquer sur le bouton Répondre ou Mettre à jour</p> </td> 
   <td> <p><a href="../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Mettre à jour le travail</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-task-status.md" class="MCXref xref">Mettre à jour le statut de la tâche</a> </p> <p><a href="../../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md" class="MCXref xref">Mettre à jour la condition pour les tâches et les problèmes</a> </p> <p> </p> <p><a href="../../../../documents/managing-documents/add-update-documents.md" class="MCXref xref">Ajouter une mise à jour à un document</a> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Améliorations apportées à l’application mobile {#mobile-improvements}

L’application mobile contient les améliorations suivantes :

* Les liens partagés avec vous dans d’autres applications mobiles s’ouvrent désormais dans l’application mobile Workfront.

  Pour plus d’informations sur le partage de liens, voir .

  Cette mise à jour sera publiée sur iOS cette semaine et la mise à jour d’Android devrait suivre rapidement.

* Nous avons mis à jour nos conditions de support de la plateforme iOS pour prendre en charge iPhone X.

  Pour plus d’informations sur les appareils mobiles et les systèmes d’exploitation pris en charge, voir .
