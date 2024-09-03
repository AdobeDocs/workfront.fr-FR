---
content-type: release-notes
navigation-topic: product-releases-archive
title: Environnement de prévisualisation R1.4
description: Cette page décrit tous les changements disponibles dans l’environnement de prévisualisation avec la version R1.4. Les fonctionnalités de cette page ont été mises à disposition dans l’environnement de prévisualisation le 15 février 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 100%

---

# Environnement de prévisualisation R1.4

Cette page décrit tous les changements disponibles dans l’environnement de prévisualisation avec la version R1.4. Les fonctionnalités de cette page ont été mises à disposition dans l’environnement de prévisualisation le 15 février 2017.

Pour une liste de tous les changements apportés à la version R1, voir [la version R1 de Workfront](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Mise à jour des approbations des projets, des tâches et des problèmes

Lors de la création de processus d’approbation de projet, de tâche et de problème, les améliorations et modifications suivantes sont désormais disponibles :

* Les « étapes » d’approbation sont également connues sous nom de « stades » d’approbation.
* Inclut plusieurs types d’approbateurs et approbatrices par étape.\
  Il s’agit notamment des utilisateurs, des utilisatrices, des équipes et des fonctions.\
  Avant cette modification, vous ne pouviez inclure que plusieurs approbateurs et approbatrices du même type. Par exemple, vous pouviez inclure plusieurs fonctions, mais pas une fonction et une équipe.

* Les limitations préexistantes suivantes relatives à la modification des processus d’approbation globale existants ont été supprimées :

   * Le processus d’approbation modifié ne se reflète que sur les objets du système pour lesquels le processus d’approbation n’a pas encore commencé ou n’a pas été modifié. Les objets dont le processus d’approbation est déjà lancé ou dont le processus d’approbation a été modifié ne sont pas mis à jour en fonction de vos modifications.
   * Vous ne pouvez pas modifier le statut qui détermine le début de l’approbation.

* Aspect mis à jour

Pour plus d’informations sur la création de processus d’approbation, voir [Créer un processus d’approbation pour les éléments de travail](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Lors de l’association d’un processus d’approbation à un projet, une tâche ou un problème, les améliorations et modifications suivantes sont désormais disponibles :

* Aspect mis à jour
* Le diagramme d’approbation est affiché dans l’onglet Approbations et présente une représentation visuelle des étapes d’approbation précédentes, actuelles et futures.

Pour plus d’informations sur l’association d’approbations à des projets, des tâches et des problèmes, voir [Associer un processus d’approbation nouveau ou existant à un travail](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Modifier le statut d’un projet directement à partir de la page du projet

Il n’est plus nécessaire de modifier un projet pour en changer le statut. Vous pouvez désormais modifier le statut d’un projet directement à partir de la page principale du projet.

Pour plus d’informations, voir [Modifier le statut d’un projet](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Planifier la désactivation d’utilisateurs ou d’utilisatrices

Vous pouvez désormais planifier la désactivation d&#39;utilisateurs ou d’utilisatrices à une date ultérieure.

Avant cette amélioration, vous ne pouviez désactiver un utilisateur ou une utilisatrice que manuellement et immédiatement.

La planification de la désactivation d’un utilisateur ou d’une utilisatrice peut s’avérer utile dans divers scénarios. Par exemple, si vous créez des utilisateurs et utilisatrices dans Workfront qui sont embauchés temporairement, vous pouvez configurer leur désactivation à la fin de leur contrat.

Cette fonction est également disponible lors de la modification en bloc des utilisateurs et utilisatrices. 

Pour plus d’informations sur la planification de la désactivation des utilisateurs et utilisatrices, voir [Désactiver ou réactiver un utilisateur ou une utilisatrice](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) et [Ajouter des utilisateurs et des utilisatrices](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Nouvelles options de synthèse d’e-mail pour les « Actions nécessaires ».

L’option de diffusion de synthèse quotidienne est désormais disponible dans la zone « Action nécessaire » de vos paramètres de notifications.

Pour plus d’informations, voir [Modifier vos propres notifications par e-mail](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

N’oubliez pas de mettre à jour l’adresse e-mail associée à votre compte pour pouvoir tester cette fonctionnalité. Cette opération est nécessaire car l’environnement de prévisualisation de sandbox efface les adresses e-mails de l’ensemble des utilisateurs et utilisatrices.

## Amélioration de la corbeille : enregistrement dans le flux de mise à jour et réception d’une notification par e-mail

Les améliorations suivantes ont été apportées lors de la restauration de projets, de tâches et de problèmes supprimés :

* Vous recevez désormais une notification par e-mail après avoir restauré un objet.\
  En tant qu’administrateur ou administratrice Workfront, vous recevez désormais une notification par e-mail après avoir restauré un projet, une tâche ou un problème précédemment supprimé. La notification par e-mail vous informe du statut du processus de restauration.\
  Pour plus d’informations sur la restauration d’objets dans Workfront, voir [Restaurer des éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Lorsque l’objet est restauré, sa suppression et sa restauration sont désormais enregistrées dans son flux de mise à jour et dans le flux de mise à jour de l’objet parent.\
  Auparavant, seule la suppression était enregistrée dans le flux de mise à jour de l’objet parent.\
  Par exemple, lorsque la tâche est restaurée, un message est ajouté au flux de mise à jour du projet et de la tâche, indiquant que la tâche a été restaurée. (Les suppressions et les restaurations ne sont pas enregistrées dans les sous-tâches. Les informations concernant les suppressions et les restaurations des sous-tâches ne sont disponibles que pour les tâches parent).\
  Pour plus d’informations, voir [Restaurer des éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## Boîte de dialogue mise à jour pour la gestion de l’appartenance à un groupe

Il y a désormais une nouvelle interface pour la gestion des groupes et des sous-groupes qui offre une expérience plus commode et plus conviviale.

Les champs Personnes propriétaires du groupe et Personnes membres du groupe sont désormais fusionnés en un seul champ, avec une liste des personnes membres du groupe située en dessous. De plus, vous pouvez filtrer la liste des personnes membres du groupe et déterminer s’il s’agit d’une personne propriétaire ou membre. 

Pour plus d’informations sur l’ajout de sous-groupes aux groupes et sur la désignation d’utilisateurs et d’utilisatrices en tant que personnes membres ou personnes propriétaires de groupes, voir [Créer un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) et [Créer un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

 

## Copier du texte dans l’application mobile

Vous pouvez copier du texte dans les champs suivants de tous les objets visibles dans l’application mobile :

* Nom
* Description
* Numéro de référence
* Commentaires

Cette fonctionnalité a été rendue disponible dans les App Store iOS et Android au cours de la semaine du 13 février.
