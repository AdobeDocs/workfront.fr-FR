---
content-type: release-notes
navigation-topic: product-releases-archive
title: Version R1 de l’environnement de prévisualisation 1 et 2
description: Cette page décrit toutes les modifications disponibles dans l’environnement de prévisualisation avec les versions R1.1 et R1.2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement de prévisualisation le 19 janvier 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 100%

---

# Version R1 de l’environnement de prévisualisation 1 et 2

Cette page décrit toutes les modifications disponibles dans l’environnement de prévisualisation avec les versions R1.1 et R1.2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement de prévisualisation le 19 janvier 2017.

Pour obtenir la liste de toutes les modifications apportées à la version R1, voir [Vue d’ensemble de l’activité de la version R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## Restaurer des projets, des tâches et des problèmes à partir de la corbeille

L’équipe d’administration de Workfront peut désormais restaurer des projets, des tâches et des problèmes qui ont été supprimés au cours des 30 derniers jours. Toutes les informations associées au projet, à la tâche ou au problème sont restaurées, y compris les documents et les données personnalisées.

De nouvelles options sont également disponibles pour configurer ce qui arrive aux heures enregistrées pour un projet, une tâche ou un problème qui est supprimé. Pour plus d’informations, voir [Configurer l’effet sur les heures lorsqu’un objet est supprimé et restauré](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Pour plus d’informations sur la restauration d’objets dans Workfront, voir [Restaurer des éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Pour plus d’informations sur l’affichage des projets, tâches et problèmes récemment restaurés, voir [Afficher l’élément restauré](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## Le diagramme d’approbation affiche la représentation visuelle des étapes d’approbation précédentes, actuelles et futures.

Désormais, lorsqu’une approbation est en attente pour un projet, une tâche ou un problème, un diagramme s’affiche. Le diagramme d’approbation affiche l’étape actuelle du processus d’approbation (en attente) et permet également d’afficher rapidement les étapes d’approbation précédentes et futures sans accéder à l’onglet Approbations.

Avant cette modification, les informations sur les étapes d’approbation n’étaient disponibles que dans l’onglet Approbations du projet, de la tâche ou du problème, et elles s’affichaient uniquement en mode Liste plutôt qu’en mode Diagramme. (Ces informations sont toujours disponibles et inchangées dans l’onglet Approbations.)

Sur les projets, les informations d’approbation s’affichent dans l’en-tête en regard du titre du projet. Pour les tâches et les problèmes, les informations d’approbation s’affichent dans le panneau de droite.

Pour plus d’informations, voir [Approuver le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md) dans  [Approuver le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Configurer les objets à mettre à jour en attente d’approbation

Lorsqu’un projet, une tâche ou un problème est en attente d’approbation, vous pouvez maintenant configurer si les utilisateurs et utilisatrices peuvent effectuer les opérations suivantes :

* Modifiez le formulaire personnalisé d’un projet, d’une tâche ou d’un problème en attente d’approbation.\
  Pour plus d’informations sur la configuration des projets, tâches et problèmes à modifier lors de l’approbation en attente, voir [Configurer des paramètres d’approbation globaux](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).

* Ajoutez des problèmes à un projet en attente d’approbation.\
  Pour plus d’informations sur la configuration des projets pour permettre aux utilisateurs et utilisatrices d’ajouter des problèmes lorsque le projet est en attente d’approbation, voir [Configurer des préférences de projet à l’échelle du système](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Modifiez les tâches et les problèmes dans un projet en attente d’approbation.\
  Pour plus d’informations sur la configuration des projets pour permettre aux utilisateurs et utilisatrices de modifier les tâches et les problèmes lorsque le projet est en attente d’approbation, voir [Configurer des préférences de projet à l’échelle du système](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Avant cette modification, les projets, tâches et problèmes en attente d’approbation ne pouvaient pas être modifiés. De plus, les problèmes ne pouvaient pas être ajoutés aux projets en attente d’approbation, et les tâches et problèmes ne pouvaient pas être modifiés dans les projets en attente d’approbation.

## Affecter des modèles de disposition à des groupes

Vous pouvez désormais attribuer des modèles de disposition à des groupes.

Avant cette modification, vous pouviez affecter des modèles de disposition aux utilisateurs et utilisatrices, aux équipes et aux fonctions. L’affectation d’un modèle de mise en page à des groupes a la priorité d’affectation de modèle de mise en page la plus basse. 

Pour plus d’informations, consultez « Créer et gérer des modèles de disposition ».

## Changements apportés aux notifications de modification en masse destinées aux utilisateurs et utilisatrices

La fonctionnalité a changé concernant la modification en masse des paramètres des notifications par e-mail destinées aux utilisateurs et utilisatrices. Lorsque vous sélectionnez plusieurs utilisateurs et utilisatrices pour modifier leurs paramètres de notification par e-mail, seules les notifications spécifiques que vous mettez à jour sont modifiées pour les utilisateurs et utilisatrices sélectionnés. Tous les paramètres de notification par e-mail inchangés restent identiques pour les utilisateurs et utilisatrices sélectionnés, même s’ils diffèrent d’un utilisateur ou d’une utilisatrice à l’autre. 

Avant cette modification, les paramètres de notification par e-mail que vous aviez sélectionnés étaient enregistrés et tous les autres paramètres de notification inchangés étaient désélectionnés lorsque vous aviez enregistré vos modifications. 

Pour plus d’informations, voir «Modifier en masse les paramètres des notifications destinées aux utilisateurs et utilisatrices » dans [Modifier vos propres notifications par e-mail](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Mise à jour de l’aspect de plusieurs notifications par e-mail

L’aspect des notifications par e-mail suivantes a été mis à jour avec une nouvelle interface utilisateur :

* Attribution de problèmes
* Modifications des dates d’engagement
* Lorsque le statut d&#39;un projet passe du statut idée/approuvé/rejeté/demandé/planifié à courant, envoyez un e-mail à l&#39;équipe
* Décision d’approbation concernant les personnes intéressées
* Achèvement d’une tâche antérieure envoyé aux tâches dépendantes
* En attente d’approbation (projet, tâche, problèmes)
* Changement de statut sur les projets, tâches, problèmes

N’oubliez pas de mettre à jour l’adresse e-mail associée à votre compte pour pouvoir tester cette fonctionnalité, car l’environnement de prévisualisation des sandbox efface les adresses e-mail de tous les utilisateurs et toutes les utilisatrices.    Pour plus d’informations sur les notifications par e-mail, voir [Notifications Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

## Nouvelles options de synthèse par e-mail pour plusieurs zones de notifications

L’option « Synthèse quotidienne » a été ajoutée dans les zones de notifications suivantes :

* Informations sur les projets auxquels je participe
* Informations sur les projets que je sponsorise.
* Informations sur l’approbation
* Informations sur le travail qui m&#39;a été affecté
* Communication

Pour plus d’informations, voir [Notifications Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  N’oubliez pas de mettre à jour l’adresse e-mail associée à votre compte pour pouvoir tester cette fonctionnalité, car l’environnement de prévisualisation des sandbox efface les adresses e-mail de tous les utilisateurs et toutes les utilisatrices.

## Rendre un groupe public

Lorsque vous rendez un groupe public, vous pouvez désormais l’ajouter à des utilisateurs ou des utilisatrices sans être propriétaire du groupe. Vous devez disposer d’un accès d’administration des utilisateurs et utilisatrices pour pouvoir modifier les utilisateurs et utilisatrices.

Pour plus d’informations sur le rendu d’un groupe public, voir la section [Créer un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) dans [Créer un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Partager l’URL d’un objet dans l’application mobile

Vous pouvez maintenant partager l’URL sur les objets suivants de l’application mobile Workfront :

* Projets
* Tâches
* Problèmes
* Feuilles de temps
* Documents

Vous pouvez partager l’URL d’un objet dans les applications suivantes :

* SMS
* E-mail
* Lecteur de stockage (par exemple, iCloud Drive)
* Une autre application installée (par exemple, Notes, Facebook)
* Vous pouvez copier un lien vers l’objet dans le presse-papiers et le coller ultérieurement dans une autre application. 

## Aide contextuelle dans la Configuration

Toutes les zones du menu Configuration ont été mises à jour avec une icône Aide dans le coin supérieur droit de la zone. Cette icône fournit un lien vers un article du site d’aide relatif à cette zone. Certaines sections des zones Configuration ont également été mises à jour avec l’icône Aide. 

## Ajouter des taux de dépenses plus précis

Vous pouvez désormais ajouter des taux de dépenses plus précis lors de la création de types de dépenses. Les taux de dépenses peuvent contenir jusqu’à 4 caractères après la virgule (par exemple, 1,0375). Cela signifie que tous les champs qui utilisent ce taux peuvent être plus précis.

Avant cette modification, les taux de dépenses ne pouvaient contenir que 2 caractères maximum après la décimale (par exemple, 1,03).

Pour plus d’informations sur la création de taux de dépenses, voir [Créer des types de dépenses personnalisés](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## Enregistrement du webinaire version R1 Prévisualisation 1 et 2

Ce webinaire a été présenté par l’équipe de préparation à la version de Workfront le 19 janvier 2017. Ce webinaire était axé sur les modifications de version de 2017 et couvrait les nouvelles fonctionnalités pouvant être testées dans la prévisualisation.
