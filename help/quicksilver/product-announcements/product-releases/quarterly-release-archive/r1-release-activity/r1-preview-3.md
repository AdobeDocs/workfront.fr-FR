---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Preview 3
description: Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec la version R1.3. La fonctionnalité de cette page a été rendue disponible dans l’environnement Aperçu le 1er février 2017.
author: Luke
feature: Product Announcements
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# R1 Preview 3

Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec la version R1.3. La fonctionnalité de cette page a été rendue disponible dans l’environnement Aperçu le 1er février 2017.

Pour obtenir la liste de toutes les modifications apportées à R1, voir [Présentation de l’activité de version R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Méthode améliorée de liaison de fichiers externes

L’option permettant de lier des documents à partir d’une source externe (lecteur Google, boîte, Dropbox, etc.) se trouve désormais à un emplacement plus visible dans la zone Documents. 

En outre, l’autorisation d’un fournisseur de documents avant de lier pour la première fois des fichiers de ce fournisseur est désormais plus intuitive (il s’agit simplement d’une étape supplémentaire lors de la liaison de fichiers à partir d’un fournisseur externe).

Avant ces modifications, l’option permettant de lier des fichiers à partir d’une source externe se trouvait dans la boîte de dialogue Ajouter des documents de la zone Documents. Avant de lier pour la première fois un document à partir d’une source externe, l’utilisateur liant le document devait autoriser ce fournisseur de documents dans la zone Configuration .

Pour plus d’informations, voir  [Liaison de documents à partir d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Mise À Jour De L’Équipe Travaillant Sur Le Calendrier

Le calendrier Travailler sur les équipes contient désormais des fonctionnalités supplémentaires et une interface actualisée. L’équipe sur le calendrier fonctionne désormais de la même manière que l’outil de planification des ressources pour les projets.

La mise à jour du calendrier Working On (Utilisation de l’équipe) comprend les améliorations suivantes :

* Afficher les utilisateurs par ordre alphabétique ou regroupés par rôle.
* Vous pouvez filtrer la chronologie de la planification par priorités de projet, état et projets individuels. Vous pouvez également filtrer la chronologie de la planification par rôles et utilisateurs. (La zone Filtre comporte moins d’options que lors de la planification des ressources pour les projets.)
* Incluez des problèmes sur la chronologie de la planification.
* Affichez les affectations utilisateur et modifiez le nombre d’heures que les utilisateurs sont affectés à certaines tâches et à certains problèmes pour chaque jour.
* Affiche les indicateurs qui indiquent le moment où les utilisateurs sont suraffectés un jour donné.
* Indiquez si le travail terminé s’affiche dans la chronologie de planification.

Différences avec l’outil de planification des ressources lors de la planification des ressources pour les projets :

* Tous les membres de l’équipe s’affichent dans le calendrier Travail sur l’équipe.\
   Lors de la planification des ressources pour les projets, seuls les utilisateurs auxquels un rôle est associé et qui correspond au rôle d’une ou de plusieurs tâches dans la zone Non affecté s’affichent.
* L’outil de permutation n’est pas disponible dans l’équipe qui travaille sur le calendrier.
* Tout membre de l’équipe peut apporter des modifications au calendrier Travail sur l’équipe.\
   Lors de la planification des ressources pour les projets, seuls les gestionnaires de ressources peuvent prendre des décisions en matière de ressources pour le projet.
* Les problèmes s’affichent par défaut sur le calendrier Travail sur l’équipe.\
   Lors de la planification des ressources pour les projets, les problèmes ne s’affichent pas par défaut.

Pour plus d’informations sur l’utilisation du calendrier de travail de l’équipe mise à jour, voir [Planification des ressources](../../../../resource-mgmt/resource-scheduling/resource-scheduling-overview.md).

## Améliorations de la planification des ressources

La chronologie de la planification comprend les améliorations suivantes :

* [Utilisez le filtre pour contrôler quels utilisateurs s’affichent dans la chronologie de planification.](#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline)
* [Les utilisateurs restent dans la chronologie après avoir été affectés à une tâche](#users-remain-on-the-timeline-after-being-assigned-a-task)

### Utilisez le filtre pour contrôler quels utilisateurs s’affichent dans la chronologie de planification. {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

Le filtre peut désormais être utilisé pour contrôler quels utilisateurs sont affichés dans la chronologie de planification, en plus des tâches et problèmes affichés dans la zone Non affecté . Lorsque des utilisateurs sont sélectionnés dans le filtre, seuls les utilisateurs que vous sélectionnez s’affichent, qu’ils aient ou non une affectation de rôle correspondant à l’affectation de rôle des tâches dans la zone Non affecté . Toutes les tâches actuellement affectées à cet utilisateur s’affichent également.

Avant cette modification, le filtre contrôlait uniquement les tâches et problèmes affichés dans la zone Non affecté . Les utilisateurs s’affichaient dans la chronologie de planification uniquement si l’utilisateur correspondait à l’attribution du rôle d’une tâche dans la zone Non affecté .

Pour plus d’informations sur l’utilisation du filtre pour contrôler ce qui est affiché dans la chronologie de planification, voir  [Filtrage des informations dans la zone Planification](../../../../resource-mgmt/resource-scheduling/filter-scheduling-area.md), et  [Affectez manuellement des tâches et des problèmes non attribués dans les zones Planification .](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md#automatically-assigning-unassigned-tasks-and-issues) in [Affectez manuellement des tâches et des problèmes non attribués dans les zones Planification .](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Les utilisateurs restent dans la chronologie après avoir été affectés à une tâche {#users-remain-on-the-timeline-after-being-assigned-a-task}

Les utilisateurs restent dans la chronologie de la planification une fois qu’une tâche ou un problème leur a été assigné, même s’il n’y a plus aucune tâche ou problème ayant une affectation de rôle correspondante. Cela vous permet d’apporter les modifications nécessaires une fois les utilisateurs affectés.

Avant cette modification, les utilisateurs disparaissaient de la chronologie de planification immédiatement après s’être vu attribuer une tâche ou un problème s’il n’y avait plus aucune tâche ou problème dans la zone Non affecté avec une affectation de rôle correspondante.

Pour plus d’informations, voir  [Affectez manuellement des tâches et des problèmes non attribués dans les zones Planification .](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md#automatically-assigning-unassigned-tasks-and-issues) in [Affectez manuellement des tâches et des problèmes non attribués dans les zones Planification .](../../../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

## Personnalisation de la terminologie Workfront en modifiant les noms d’objet

Vous pouvez désormais personnaliser la terminologie Workfront en modifiant les noms de certains objets.\
À l’aide d’un modèle de mise en page, vous pouvez désormais modifier les noms des objets de travail suivants en fonction des besoins de votre entreprise :

* Portfolio
* Programme
* Projet
* Tâche
* Problème

Par exemple, si, dans votre organisation, vous utilisez des campagnes plutôt que des projets, vous pouvez remplacer le nom de l’objet &quot;Projet&quot; par &quot;Campagne&quot;.

Lorsque vous effectuez ce remplacement, les zones suivantes de l’application affichent le nom mis à jour des objets :

* Barre de navigation globale
* Tous les onglets
* Tous les menus 
* Créateur de rapports et éléments de création de rapports (vues, filtres et regroupements)
* Bouton Enregistrer
* Fichiers exportés
* E-mails

Les zones suivantes n’affichent pas le nom mis à jour des objets :

* Estimations de ressources
* Gestionnaire du budget des ressources
* Planificateur de capacités
* Grille des ressources
* Team Builder
* Portfolio Optimizer 
* Applications mobiles
* Module complémentaire Outlook

Pour plus d’informations sur la personnalisation de la terminologie Workfront à l’aide d’un modèle de mise en page, reportez-vous à la section Personnalisation de la terminologie dans Création et gestion des modèles de mise en page et à la section Comprendre les implications de la personnalisation des noms d’objet dans la section [Présentation des objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Inclure les dates de début et de fin d’approbation dans les rapports

Vous pouvez désormais inclure les champs suivants lors de la création ou de la modification de rapports :

* Date de début du chemin d&#39;approbation
* Date d’achèvement du chemin d’approbation

Ces champs vous permettent de savoir quand le chemin d’approbation actuel ou le plus récent a été démarré et quand il a été marqué comme terminé.

Pour plus d’informations sur ces champs, voir [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Pour plus d’informations sur les chemins d’approbation, leur création et leur déclenchement, ainsi que sur la fonction qu’ils jouent dans les processus d’approbation, voir [Créer un processus d’approbation pour les tâches](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Les champs suivants ont été supprimés de Workfront et ne peuvent plus être inclus dans les rapports (ces champs fournissaient des informations sur le projet plutôt que des informations sur les validations elles-mêmes, et ont souvent été mal utilisés) :

* Date de début prévue des approbations
* Date de début prévisionnelle pour l&#39;approbation
* Date de début estimée de l&#39;approbation

## Nouvelles options de résumé des emails pour les &quot;requêtes que j’ai effectuées&quot;

L’option de remise Résumé quotidien a été ajoutée à la zone &quot;Demandes que j’ai faites&quot; de vos paramètres de notifications.

Pour plus d’informations, voir [Activation ou désactivation de vos propres notifications d’événement](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

N’oubliez pas de mettre à jour l’adresse électronique associée à votre compte pour pouvoir tester cette fonctionnalité. Cela est nécessaire, car l’environnement de test Aperçu efface les adresses électroniques de tous les utilisateurs.

## Mise à jour de l’aspect et du sentiment des notifications électroniques d’approbation de document

L’aspect de la notification pour &quot;Approbation de document&quot; a été mis à jour avec une nouvelle interface utilisateur :

Pour plus d’informations sur les notifications électroniques, voir [Notifications Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

N’oubliez pas de mettre à jour l’adresse électronique associée à votre compte pour pouvoir tester cette fonctionnalité. Cela est nécessaire, car l’environnement de test Aperçu efface les adresses électroniques de tous les utilisateurs.

## Améliorations de la vue Milestone

La vue Milestone disponible lors de l’affichage d’une liste de projets ou d’un rapport de projet contient désormais les améliorations suivantes :

* Les dates planifiées sont modifiables.
* Pourcentage d’achèvement pour les projets et les tâches affiché

Avant cette modification, pour modifier les dates ou afficher le pourcentage terminé, vous deviez accéder à la tâche individuelle.

Pour plus d’informations, voir [Utilisation de la vue Milestone](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
