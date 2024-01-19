---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Preview 4
description: Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec la version R1.4. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 15 février 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# R1 Preview 4

Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec la version R1.4. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 15 février 2017.

Pour obtenir la liste de toutes les modifications apportées à R1, voir [Version Workfront R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Approbations mises à jour de projets, de tâches et de problèmes

Lors de la création de processus d’approbation pour les approbations de projet, de tâche et de problème, les améliorations et modifications suivantes sont désormais disponibles : 

* Les &quot;étapes&quot; d’approbation sont désormais appelées &quot;étapes&quot; d’approbation.
* Incluez plusieurs types d’approbateurs par étape.\
  Cela inclut les utilisateurs, les équipes et les rôles de tâche.\
  Avant cette modification, vous ne pouviez inclure que plusieurs approbateurs du même type. Par exemple, vous pouvez inclure plusieurs rôles de tâche, mais pas un rôle de tâche et une équipe.

* Les limites préexistantes suivantes liées à la modification des processus d’approbation globale existants ont été supprimées :

   * Le processus de validation modifié n’est reflété que sur les objets du système dans lesquels le processus de validation n’a pas encore commencé ou dans lesquels le processus de validation n’a pas été modifié. Les objets dans lesquels le processus de validation a déjà démarré ou dans lesquels le processus de validation a été modifié ne sont pas mis à jour avec vos modifications.
   * Vous ne pouvez pas modifier l’état qui détermine le moment où la validation commence.

* Mise à jour de l’aspect.

Pour plus d’informations sur la création de processus de validation, voir [Créer un processus d’approbation pour les tâches](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Lors de l’association d’un processus d’approbation à un projet, une tâche ou un problème, les améliorations et modifications suivantes sont désormais disponibles :

* Mise à jour de l’aspect.
* Le diagramme des validations s’affiche dans l’onglet Validations. Il affiche une représentation visuelle des étapes de validation précédentes, actuelles et futures.

Pour plus d’informations sur l’association des validations aux projets, tâches et problèmes, voir [Associer un processus d’approbation nouveau ou existant au travail](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Modification directe de l’état d’un projet à partir de la page du projet

Vous n’avez plus besoin de modifier un projet pour modifier son état. Vous pouvez désormais modifier l’état d’un projet directement à partir de la page principale du projet.

Pour plus d’informations, voir [Modification de l’état d’un projet](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Planification de la désactivation des utilisateurs

Vous pouvez maintenant planifier la désactivation des utilisateurs à une date ultérieure.

Avant cette amélioration, vous ne pouviez désactiver un utilisateur manuellement que immédiatement.

La planification de la désactivation d’un utilisateur peut s’avérer utile dans divers scénarios. Par exemple, si vous créez dans Workfront des utilisateurs qui sont engagés temporairement, vous pouvez les configurer pour qu’ils soient désactivés à la fin de leur contrat.

Cette fonctionnalité est également disponible lorsque des utilisateurs de modification en masse opèrent. 

Pour plus d’informations sur la planification de la désactivation des utilisateurs, voir [Désactivation ou réactivation d’un utilisateur](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) et [Ajout d’utilisateurs](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Nouvelles options de résumé des emails pour les &quot;actions nécessaires&quot;

L’option de remise Résumé quotidien est désormais disponible dans la zone &quot;Action requise&quot; de vos paramètres de notifications.

Pour plus d’informations, voir [Modifier vos propres notifications électroniques](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

N’oubliez pas de mettre à jour l’adresse électronique associée à votre compte pour pouvoir tester cette fonctionnalité. Cela est nécessaire, car l’environnement de test Aperçu efface les adresses électroniques de tous les utilisateurs.

## Amélioration de la Corbeille : enregistrée dans le flux de mise à jour et réception des notifications par email

Les améliorations suivantes ont été ajoutées lors de la restauration de projets, de tâches et de problèmes supprimés :

* Vous recevez désormais une notification par courrier électronique après la restauration d’un objet.\
  En tant qu’administrateur Workfront, vous recevez désormais une notification par courrier électronique après la restauration d’un projet, d’une tâche ou d’un problème qui a été supprimé précédemment. La notification par courrier électronique vous informe de l’état du processus de restauration.\
  Pour plus d’informations sur la restauration d’objets dans Workfront, voir [Restauration des éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Lorsque l’objet est restauré, la suppression et la restauration de l’objet sont désormais enregistrées dans le flux de mise à jour de l’objet lui-même et dans le flux de mise à jour de l’objet parent.\
  Auparavant, seule la suppression était enregistrée dans le flux de mise à jour de l’objet parent.\
  Par exemple, lorsque la tâche est restaurée, un message est ajouté dans le flux de mise à jour du projet et de la tâche elle-même, indiquant que la tâche a été restaurée. (Les suppressions et les restaurations ne sont pas enregistrées sur les sous-tâches. Les informations concernant les suppressions et les restaurations des sous-tâches ne sont disponibles que sur les tâches parentes.)\
  Pour plus d’informations, voir [Restauration des éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## Boîte de dialogue mise à jour pour la gestion de l’appartenance à un groupe

Il existe une nouvelle interface pour la gestion des groupes et des sous-groupes qui offre une expérience plus facile et plus conviviale.

Les champs Propriétaires de groupe et Membres du groupe sont désormais combinés en un seul champ, avec une liste des membres du groupe répertoriés ci-dessous. De plus, vous pouvez filtrer la liste des membres du groupe et modifier s’ils sont propriétaires ou membres. 

Pour plus d’informations sur l’ajout de sous-groupes aux groupes et la désignation d’utilisateurs en tant que membres ou propriétaires de groupes, voir [Création d’un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) et [Création d’un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## Copier du texte dans l’application mobile

Vous pouvez copier du texte dans les champs suivants de tous les objets visibles dans l’application mobile :

* Nom
* Description
* Numéro de référence
* Commentaires

Cette fonctionnalité doit être publiée dans les boutiques iOS et Android dès la semaine du 13 février.
