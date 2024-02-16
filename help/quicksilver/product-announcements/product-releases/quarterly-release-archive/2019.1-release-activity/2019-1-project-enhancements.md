---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: Améliorations du projet 2019.1
description: Cette page décrit toutes les améliorations de projet incluses dans la version 2019.1. Cette fonctionnalité est actuellement disponible dans l’environnement Aperçu . Elle sera mise à disposition dans l’environnement de production de .
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7b39082a-ab96-4e54-8f28-96629760715a
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 1%

---

# Améliorations du projet 2019.1

Cette page décrit toutes les améliorations de projet incluses dans la version 2019.1. Cette fonctionnalité est actuellement disponible dans l’environnement Aperçu . Elle sera mise à disposition dans l’environnement de production de .

>[!IMPORTANT]
>
>Les fonctionnalités décrites sur cette page peuvent être modifiées avant leur disponibilité dans l’environnement de production.

Pour obtenir la liste de toutes les modifications apportées à la version 2019.1, reportez-vous à la section &quot;Aperçu de l’activité de version 2019.1&quot;.

**Pour les administrateurs**

* [Restaurer des modèles à partir de la corbeille](#restore-templates-from-the-recycle-bin)
* [Afficher les horodatages des champs de date à l’accueil](#show-timestamps-for-date-fields-in-home)
* [Tous les types de durée disponibles sous Préférences de projet](#all-duration-types-available-under-project-preferences)

**Pour tous les utilisateurs**

* [Améliorations rapides](#agile-improvements)
* [Ajout de tâches et de problèmes d’une liste à une itération](#add-tasks-and-issues-from-a-list-to-an-iteration)
* [Nouvelles tailles de papier pour l’exportation du graphique Gantt](#new-paper-sizes-for-gantt-chart-export)
* [Suppression de l’accès aux boîtes de dialogue dans le diagramme de Gantt en mode d’édition](#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode)
* [Affichage des informations sur les tâches dans le diagramme de Gantt de liste de projets dans un programme ou un Portfolio](#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio)
* [Accès au diagramme de Gantt de la liste des tâches sur les modèles](#access-the-task-list-gantt-chart-on-templates)
* [Modification du nom de la vue Projet sur le diagramme de Gantt](#renamed-the-project-view-on-the-gantt-chart)
* [Scénarios d’hypothèses dans le diagramme de Gantt de la liste des tâches](#what-if-scenarios-in-the-task-list-gantt-chart)
* [Améliorations de la liste des tâches](#task-list-improvements)
* [Afficher les listes en plein écran](#display-lists-in-full-screen)
* [Nouvelles listes dans d’autres zones](#new-lists-in-additional-areas)
* [Envoyer un rapport distribué au format XLSX](#send-a-delivered-report-in-xlsx-format)
* [Exporter les journaux d’audit](#export-audit-logs)

## Restaurer des modèles à partir de la corbeille {#restore-templates-from-the-recycle-bin}

Les administrateurs de Workfront peuvent désormais restaurer des modèles à partir de la Corbeille. Comme pour les autres éléments supprimés, vous pouvez restaurer un modèle jusqu’à 30 jours à compter de sa suppression.

Pour plus d’informations, voir &quot;Restauration des éléments supprimés&quot;.

## Afficher les horodatages des champs de date à l’accueil {#show-timestamps-for-date-fields-in-home}

En tant qu’administrateur Workfront, vous pouvez désormais choisir d’afficher ou de masquer les horodatages des dates d’échéance dans la liste de travail et le calendrier à l’aide des modèles de mise en page. Par défaut, les horodatages sont visibles pour les utilisateurs de modèles et non de modèles.

Pour plus d’informations, voir &quot;Personnalisation de la zone d’accueil&quot; dans l’article &quot;Création et gestion des modèles de mise en page&quot;.

## Tous les types de durée disponibles sous Préférences de projet {#all-duration-types-available-under-project-preferences}

Lorsque vous définissez la tâche par défaut et le type de durée de publication dans Configuration > Préférences du projet, vous pouvez utiliser l’une des options suivantes :

Simple

Piloté par l&#39;effort

Calcul d&#39;affectation

Travail calculé

Auparavant, si vous définissiez Simple ou Effort Driven comme type de durée par défaut, vous ne pouviez pas choisir Affectation calculée et Travail calculé.

Pour plus d’informations sur la définition des valeurs par défaut des types de tâche et de durée de publication, voir &quot;Préférences des tâches et des problèmes&quot;.

## Améliorations rapides {#agile-improvements}

Les améliorations suivantes sont désormais disponibles dans l’outil Agile :

Kanban

Ajoutez des tâches et des problèmes à un panorama Kanban à partir de n’importe quelle liste de tâches ou de rapport.

Auparavant, vous pouviez ajouter des tâches au panorama Kanban à partir du journal uniquement. Vous ne pouviez pas ajouter de problèmes.

Filtrez le panorama Kanban par utilisateurs individuels de l’équipe.

Pour plus d’informations, voir &quot;Utilisation de la planche Kanban&quot;.

Affichez et gérez les problèmes sur le journal de Kanban.

Pour plus d’informations, voir &quot;Utilisation de la planche Kanban&quot;.

Auparavant, vous ne pouviez pas ajouter ni gérer des problèmes sur un panorama Kanban.

Scrum

Vous pouvez filtrer le panorama des narrations d’itération par utilisateurs individuels de l’équipe.

Pour plus d’informations, reportez-vous à la section &quot;Utilisation du panorama d’articles agiles de Scrum&quot;.

Auparavant, vous ne pouviez pas filtrer par utilisateur sur les panoramas Kanban ou scrum.

## Ajout de tâches et de problèmes d’une liste à une itération {#add-tasks-and-issues-from-a-list-to-an-iteration}

Vous pouvez désormais utiliser une tâche ou une liste de problèmes, un rapport ou un tableau de bord pour ajouter des articles à une itération. Plusieurs équipes peuvent également se voir attribuer des articles dans une même itération.

Auparavant, vous pouviez ajouter un article à une itération uniquement à partir de la page Détails de la tâche ou des problèmes, et vous pouviez ajouter des articles uniquement aux itérations créées par votre équipe.

Pour plus d’informations, voir &quot;Création et gestion des itérations agiles&quot;.

## Envoyer un rapport distribué au format XLSX {#send-a-delivered-report-in-xlsx-format}

Vous pouvez désormais planifier la remise d’un rapport au format MS Excel (.xlsx), en plus de tous les autres formats actuels.

Auparavant, vous pouviez uniquement envoyer un rapport aux formats suivants :

HTML

PDF

MS Excel (.xls)

TSV

Pour plus d’informations sur la planification des rapports pour la remise, voir Configuration des diffusions de rapports.

## Améliorations de la liste des tâches {#task-list-improvements}

[mettre à jour la version 18.3 bêta 4 où elle a été supprimée de]

Les listes de tâches nouvellement repensées ont été réactivées, après une brève suppression au cours de la version 18.3 bêta 4. Nous avons également ajouté les fonctionnalités supplémentaires suivantes aux listes de tâches qui ne faisaient pas partie de la version d’origine :

Remplacement du menu contextuel par une icône Plus lors de la modification en ligne d’une tâche.

Les options disponibles dans le menu contextuel lors de l&#39;édition en ligne de plusieurs tâches ont désormais été déplacées vers les icônes affichées en haut de la liste des tâches.

Par défaut, les listes de tâches affichent 2 000 tâches.

Lorsque Workfront recalcule les chronologies, les points d’interrogation en regard des tâches dont les dates sont mises à jour ont été remplacés par des zones grises.

Pour plus d’informations sur la modification des tâches en ligne, voir &quot;Copie et duplication de tâches&quot; et &quot;Création de relations de prédécesseur par chaînement de tâches&quot;.

Pour plus d’informations sur le nouveau calcul des calendriers de projet, voir &quot;Recalcul des calendriers de projet&quot;.

## Afficher les listes en plein écran {#display-lists-in-full-screen}

Lorsqu’une liste de projets ou de tâches dépasse la taille de votre écran, la liste s’affiche désormais automatiquement dans toute la fenêtre du navigateur lorsque vous faites défiler l’écran. Cela augmente la quantité d’informations affichées simultanément et vous permet de faciliter la gestion des listes.

Vous pouvez afficher les listes suivantes en plein écran :

Liste des projets dans les onglets et sous-onglets suivants :

Projets auxquels je participe

Projets dont je suis propriétaire

Tous les projets

Onglet Projets dans un Portfolio

Onglet Projets dans un programme

Liste des tâches dans les onglets suivants :

Onglet Tâches dans un projet

Onglet Sous-tâches dans une tâche

Pour plus d’informations sur l’affichage des objets dans les listes, voir &quot;Affichage des éléments dans une liste&quot;.

## Nouvelles listes dans d’autres zones {#new-lists-in-additional-areas}

Nous avons amélioré les performances et l’aspect des listes de projets et de tâches dans les domaines suivants :

Onglets Portfolio et programmes dans la zone Projets

Onglet Sous-tâches au niveau de la tâche

Avant cette amélioration, les nouvelles listes n’étaient disponibles que dans les zones suivantes :

Onglet Projets de la zone Projets

Onglet Tâches au niveau du projet

Pour plus d’informations sur l’affichage des objets dans les listes, voir &quot;Affichage des éléments dans une liste&quot;.

## Affichage des informations sur les tâches dans le diagramme de Gantt de liste de projets dans un programme ou un Portfolio {#view-task-information-in-the-project-list-gantt-chart-in-a-program-or-portfolio}

Vous pouvez désormais afficher des informations sur les tâches d’un projet dans le diagramme de Gantt de liste de projets au sein d’un programme ou d’un Portfolio.

Auparavant, vous pouviez afficher les informations sur les tâches uniquement dans le diagramme de Gantt de la liste des projets de l’onglet Projets .

Pour plus d’informations, voir &quot;Affichage des informations dans le diagramme de Gantt&quot;.

## Scénarios d’hypothèses dans le diagramme de Gantt de la liste des tâches {#what-if-scenarios-in-the-task-list-gantt-chart}

Vous pouvez désormais effectuer les actions suivantes sur les tâches d’un projet lorsqu’elles s’affichent en mode d’édition du diagramme de Gantt :

Ajouter des tâches

Supprimer des tâches

Tâches de modification en ligne

Dupliquer les tâches

Réorganiser les tâches

Modifier les sous-tâches

Bien que vous puissiez voir comment vos modifications affectent la chronologie du projet, elles ne sont pas enregistrées immédiatement. Vous pouvez les enregistrer pour mettre à jour définitivement la chronologie du projet, ou vous pouvez les annuler.

Auparavant, vous ne pouviez pas prévisualiser les modifications de la liste des tâches dans le diagramme de Gantt.

Pour plus d’informations sur la modification des tâches dans le diagramme de Gantt, voir &quot;Mise à jour des informations dans le diagramme de Gantt de la liste des tâches&quot;.

## Accès au diagramme de Gantt de la liste des tâches sur les modèles {#access-the-task-list-gantt-chart-on-templates}

Vous pouvez désormais accéder au diagramme de Gantt de la liste des tâches dans un modèle de projet.

Auparavant, vous ne pouviez pas afficher le diagramme de Gantt sur la liste des tâches dans un modèle.

Pour plus d’informations, voir &quot;Prise en main du diagramme de Gantt&quot;.

## Nouvelles tailles de papier pour l’exportation du graphique Gantt {#new-paper-sizes-for-gantt-chart-export}

Vous pouvez maintenant imprimer le diagramme de Gantt sur les formats de papier A1 et A2.

Auparavant, vous pouviez uniquement exporter vers Letter, Legal, Ledger, A3 (disponible uniquement pour certaines langues) et A4.

Pour plus d’informations, voir &quot;Export du diagramme de Gantt vers PDF&quot;.

## Modification du nom de la vue Projet sur le diagramme de Gantt {#renamed-the-project-view-on-the-gantt-chart}

L’option de vue &quot;Projet&quot; du diagramme de Gantt a été renommée &quot;Ajuster tout&quot;. L’option d’affichage fonctionne toujours comme auparavant. Le nouveau nom est conçu pour être plus explicite sur ce que vous voyez lorsque l’option est sélectionnée.

Pour plus d’informations, voir &quot;Affichage des informations dans le diagramme de Gantt&quot;.

## Suppression de l’accès aux boîtes de dialogue dans le diagramme de Gantt en mode d’édition {#removed-access-to-dialog-boxes-in-the-gantt-chart-while-in-edit-mode}

Vous ne pouvez plus accéder à la boîte de dialogue Affectations avancées lorsque le graphique Gantt est en mode d’édition. Vous ne pouvez effectuer que des modifications intégrées lorsque le diagramme de Gantt de la liste des tâches est en mode d’édition.

Auparavant, vous pouviez accéder à la boîte de dialogue Affectations avancées lorsque le graphique Gantt était en mode d’édition, mais il enregistrait les modifications effectuées dans le graphique Gantt et fermait le mode d’édition.

Pour plus d’informations sur la modification du diagramme de Gantt de la liste des tâches, voir &quot;Mise à jour des informations dans le diagramme de Gantt de la liste des tâches&quot;.

## Exporter les journaux d’audit {#export-audit-logs}

Vous pouvez désormais exporter les entrées du journal d’audit vers un fichier CSV. Vous pouvez exporter jusqu’à 50 000 entrées du journal d’audit dans un fichier CSV à la fois.

Pour plus d’informations, voir &quot;Gestion des journaux d’audit&quot;.
