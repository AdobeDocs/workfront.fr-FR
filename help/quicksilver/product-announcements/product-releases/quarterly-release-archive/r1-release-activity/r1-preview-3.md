---
content-type: release-notes
navigation-topic: product-releases-archive
title: Version R1 de l’environnement de prévisualisation, 3
description: Cette page décrit toutes les modifications disponibles dans l’environnement de prévisualisation avec la version R1.3. La fonctionnalité de cette page a été rendue disponible dans l’environnement de prévisualisation le 1er février 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 100%

---

# Version R1 de l’environnement de prévisualisation, 3

Cette page décrit toutes les modifications disponibles dans l’environnement de prévisualisation avec la version R1.3. La fonctionnalité de cette page a été rendue disponible dans l’environnement de prévisualisation le 1er février 2017.

Pour obtenir la liste de toutes les modifications apportées à la version R1, voir [Vue d’ensemble de l’activité de la version R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## Méthode améliorée de liaison de fichiers externes

L’option permettant de lier des documents à partir d’une source externe (Google Drive, Box, Dropbox, etc.) se trouve désormais à un emplacement plus visible dans la zone Documents. 

En outre, l’autorisation d’un fournisseur de documents avant de lier pour la première fois des fichiers de ce fournisseur est désormais plus intuitive (il s’agit simplement d’une étape supplémentaire lors de la liaison de fichiers provenant d’un fournisseur externe).

Avant ces modifications, l’option permettant de lier des fichiers à partir d’une source externe se trouvait dans la boîte de dialogue Ajouter des documents de la zone Documents. Avant de lier pour la première fois un document à partir d’une source externe, la personne liant le document devait autoriser ce fournisseur de documents dans la zone Configuration.

Pour plus d’informations, voir [Lier des documents provenant d’applications externes](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Mise à jour du calendrier En train de travailler sur de l’équipe

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Le calendrier En train de travailler sur disponible pour les équipes contient désormais des fonctionnalités supplémentaires et spn aspect a été mis à jour. Le calendrier En train de travailler sur de l’équipe fonctionne désormais de la même manière que l’outil de planification des ressources pour les projets.

La mise à jour du calendrier En train de travailler sur de l’équipe comprend les améliorations suivantes :

* Affichez les personnes par ordre alphabétique ou par rôle.
* Vous pouvez filtrer la chronologie de la planification par priorités de projet, statut et projets individuels. Vous pouvez également filtrer la chronologie de la planification par rôles et personnes. (La zone Filtre comporte moins d’options que lors de la planification des ressources pour les projets.)
* Incluez des problèmes sur la chronologie de la planification.
* Affichez les affectations de personnes et modifiez le nombre d’heures qui leur sont attribuées pour certaines tâches et certains problèmes pour chaque jour.
* Affiche les indicateurs qui montrent le moment où les personnes sont suraffectées un jour donné.
* Indiquez si le travail terminé doit s’afficher dans la chronologie de planification.

Différences avec l’outil de planification des ressources lors de la planification des ressources pour les projets :

* Toutes les personnes membres de l’équipe s’affichent dans le calendrier En train de travailler sur de l’équipe.\
  Lors de la planification des ressources pour les projets, seules les personnes auxquelles un rôle est associé et qui correspond au rôle d’une ou de plusieurs tâches dans la zone Non affecté s’affichent.
* L’outil Permuter n’est pas disponible dans le calendrier En train de travailler sur de l’équipe.
* Toute personne membre de l’équipe peut apporter des modifications au calendrier En train de travailler sur de l’équipe.\
  Lors de la planification des ressources pour les projets, seules les personnes gestionnaires de ressources peuvent prendre des décisions en matière de ressources pour le projet.
* Les problèmes s’affichent par défaut sur le calendrier En train de travailler sur de l’équipe.\
  Lors de la planification des ressources pour les projets, les problèmes ne s’affichent pas par défaut.

Pour plus d’informations sur l’utilisation du calendrier En train de travailler sur de l’équipe mis à jour, voir « Planification des ressources ».

## Amélioration de la planification des ressources

La chronologie de la planification comprend les améliorations suivantes :

* « Utilisation du filtre pour contrôler quelles personnes s’affichent dans la chronologie de planification ».
* « Les personnes restent sur la chronologie après avoir été affectées à une tâche. »

### Utiliser le filtre pour contrôler quelles personnes s’affichent dans la chronologie de planification. {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>Les outils de planification des ressources ont été retirés de Workfront avec la version 23.1. Pour plus d’informations sur la planification des ressources à l’aide de l’équilibreur de charge de travail, voir [Vue d’ensemble de l’équilibreur de charge de travail](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Le filtre peut maintenant être utilisé pour contrôler quelles personnes sont affichées dans la chronologie de planification, en plus des tâches et problèmes affichés dans la zone Non affecté. Lorsque des personnes sont sélectionnées dans le filtre, seules les personnes que vous sélectionnez s’affichent, qu’elles aient ou non une affectation de rôle correspondant à l’affectation de rôle des tâches dans la zone Non affecté. Toutes les tâches actuellement affectées à cette personne s’affichent également.

Avant cette modification, le filtre contrôlait uniquement les tâches et problèmes affichés dans la zone Non affecté. Les personnes s’affichaient dans la chronologie de planification uniquement si elles correspondaient à l’attribution du rôle d’une tâche dans la zone Non affecté.

Pour plus d’informations sur l’utilisation du filtre afin de contrôler ce qui s’affiche dans la chronologie de planification, voir « Filtrer les informations dans la zone Planification » et « Affecter manuellement des tâches et des problèmes non affectés dans les zones Planification ».

### Les utilisateurs et utilisatrices restent dans la chronologie après avoir été affectés à une tâche. {#users-remain-on-the-timeline-after-being-assigned-a-task}

Les utilisateurs et utilisatrices restent dans la chronologie de la planification une fois qu’un élément (tâche ou problème) leur a été affecté, même s’il n’y a plus aucune tâche ni aucun problème ayant une affectation de rôle correspondante. Cela vous permet d’apporter les modifications nécessaires une fois les utilisateurs et utilisatrices affectés.

Avant cette modification, les utilisateurs et utilisatrices disparaissaient de la chronologie de planification immédiatement après s’être vu affecter une tâche ou un problème s’il n’y avait plus aucune tâche ni aucun problème dans la zone Non affecté avec une affectation de rôle correspondante.

Pour plus d’informations, voir « Attribuer manuellement des tâches et des problèmes non assignés dans les zones de planification ».

## Personnaliser la terminologie Workfront en modifiant les noms d’objet

Vous pouvez désormais personnaliser la terminologie Workfront en modifiant les noms de certains objets.\
À l’aide d’un modèle de mise en page, vous pouvez désormais modifier les noms des objets de travail suivants en fonction des besoins de votre entreprise :

* Portfolio
* Programme
* Projet
* Tâche
* Problème

Par exemple, si, dans votre organisation, vous utilisez des campagnes plutôt que des projets, vous pouvez remplacer le nom de l’objet « Projet » par « Campagne ».

Lorsque vous effectuez ce remplacement, les zones suivantes de l’application affichent le nom mis à jour des objets :

* Barre de navigation globale
* Tous les onglets
* Tous les menus
* Les éléments de Report Builder et de création de rapports (vues, filtres et regroupements)
* Boutons Enregistrer
* Fichiers exportés
* E-mails

Les zones suivantes n’affichent pas le nom mis à jour des objets :

* Estimations de ressources
* Gestionnaire du budget des ressources
* Planificateur de capacités
* Grille des ressources
* Team Builder
* Optimisateur de portfolio
* Applications mobiles
* Module complémentaire Outlook

Pour plus d’informations sur la personnalisation de la terminologie Workfront à l’aide d’un modèle de mise en page, voir la section « Personnaliser la terminologie » dans « Créer et gérer des modèles de mise en page » et la section « Présentation des implications de la personnalisation des noms d’objet » dans [Présentation des objets dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Inclure les dates de début et de fin d’approbation dans les rapports

Vous pouvez désormais inclure les champs suivants lors de la création ou de la modification de rapports :

* Date de début du chemin d&#39;approbation
* Date d’achèvement du chemin d’approbation

Ces champs vous permettent de savoir quand le chemin d’approbation actuel ou le plus récent a été démarré et quand il a été marqué comme terminé.

Pour plus d’informations sur ces champs, voir [Glossaire de la terminologie Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Pour plus d’informations sur les chemins d’approbation, leur création et leur déclenchement, ainsi que sur la fonction qu’ils jouent dans les processus d’approbation, voir [Créer un processus d’approbation pour les éléments de travail](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Les champs suivants ont été supprimés de Workfront et ne peuvent plus être inclus dans les rapports (ces champs fournissaient des informations sur le projet plutôt que des informations sur les approbations, et ont souvent été mal utilisés) :

* Date de début prévue des approbations
* Date de début prévisionnelle pour l&#39;approbation
* Date de début estimée de l&#39;approbation

## Nouvelles options de synthèse des e-mails pour les « Demandes que j’ai effectuées »

L’option de diffusion Synthèse quotidienne a été ajoutée à la zone « Demandes que j’ai effectuées » de vos paramètres de notifications.

Pour plus d’informations, consultez la section [Modifier vos propres notifications par e-mail](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

N’oubliez pas de mettre à jour l’adresse e-mail associée à votre compte pour pouvoir tester cette fonctionnalité. Cette opération est nécessaire car l’environnement de prévisualisation de sandbox efface les adresses e-mails de l’ensemble des utilisateurs et utilisatrices.

## Mise à jour de l’aspect des notifications par e-mail d’approbation de document

L’aspect des notification pour l’approbation de document a été mis à jour avec une nouvelle interface utilisateur :

Pour plus d’informations sur les notifications par e-mail, voir [Notifications Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

N’oubliez pas de mettre à jour l’adresse e-mail associée à votre compte pour pouvoir tester cette fonctionnalité. Cette opération est nécessaire car l’environnement de prévisualisation de sandbox efface les adresses e-mails de l’ensemble des utilisateurs et utilisatrices.

## Améliorations apportées à la vue Jalon

La vue Jalon disponible lors de l’affichage d’une liste de projets ou d’un rapport de projet contient désormais les améliorations suivantes :

* Les dates prévues sont modifiables.
* Le pourcentage terminé pour les projets et les tâches est affiché.

Avant cette modification, pour modifier les dates ou afficher le pourcentage terminé, vous deviez accéder à la tâche individuelle.

Pour plus d’informations, voir [Utiliser la vue Jalon](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
