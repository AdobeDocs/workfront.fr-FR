---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Aperçu 1 et 2
description: Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec les versions R1.1 et R1.2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 19 janvier 2017.
author: Luke
feature: Product Announcements
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 2%

---

# R1 Aperçu 1 et 2

Cette page décrit toutes les modifications disponibles dans l’environnement Aperçu avec les versions R1.1 et R1.2. Les fonctionnalités de cette page ont été rendues disponibles dans l’environnement Aperçu le 19 janvier 2017.

Pour obtenir la liste de toutes les modifications apportées à R1, voir [Présentation de l’activité de version R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Restauration de projets, de tâches et de problèmes à partir de la corbeille 

Les administrateurs de Workfront peuvent désormais restaurer des projets, des tâches et des problèmes qui ont été supprimés au cours des 30 derniers jours. Toutes les informations associées au projet, à la tâche ou au problème sont restaurées, y compris les documents et les données personnalisées.

De nouvelles options sont également disponibles pour configurer ce qui arrive aux heures enregistrées par rapport à un projet, une tâche ou un problème qui est supprimé. Pour plus d’informations, voir [Configurer l’effet sur les heures lorsqu’un objet est supprimé et restauré](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Pour plus d’informations sur la restauration d’objets dans Workfront, voir [Restauration des éléments supprimés](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Pour plus d’informations sur l’affichage des projets, tâches et problèmes récemment restaurés, voir [Afficher l’élément restauré](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## Diagramme d’approbation Affiche la représentation visuelle des étapes d’approbation précédentes, actuelles et futures.

Désormais, lorsqu’une approbation est en attente sur un projet, une tâche ou un problème, un diagramme s’affiche. Le diagramme d&#39;approbation affiche l&#39;étape en cours du processus de validation (en attente) et permet également d&#39;afficher rapidement les étapes de validation précédentes et futures sans accéder à l&#39;onglet Validations .

Avant cette modification, les informations sur les étapes de validation n’étaient disponibles que dans l’onglet Validations du projet, de la tâche ou du problème, et elles s’affichaient uniquement en mode Liste plutôt qu’en mode Diagramme. (Ces informations sont toujours disponibles et inchangées dans l’onglet Validations .)

Sur les projets, les informations de validation s’affichent dans l’en-tête en regard du titre du projet. Pour les tâches et les problèmes, les informations de validation s’affichent dans le panneau de droite.

Pour plus d’informations, voir [Valider le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md) in  [Valider le travail](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Configurer les objets à mettre à jour en attente d’approbation

Lorsqu’un projet, une tâche ou un problème est en attente d’approbation, vous pouvez maintenant configurer si les utilisateurs peuvent :

* Modifiez le formulaire personnalisé d’un projet, d’une tâche ou d’un problème en attente d’approbation.\
   Pour plus d’informations sur la configuration des projets, tâches et problèmes à modifier lors de l’approbation en attente, voir [Configuration des paramètres d’approbation globaux](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Ajoutez des problèmes à un projet en attente d’approbation.\
   Pour plus d’informations sur la configuration des projets pour permettre aux utilisateurs d’ajouter des problèmes lorsque le projet est en attente d’approbation, voir [Configuration des préférences de projet à l’échelle du système](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Modifiez les tâches et les problèmes dans un projet en attente d’approbation.\
   Pour plus d’informations sur la configuration des projets pour permettre aux utilisateurs de modifier les tâches et les problèmes lorsque le projet est en attente d’approbation, voir [Configuration des préférences de projet à l’échelle du système](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Avant cette modification, les projets, tâches et problèmes en attente d’approbation n’ont pas pu être modifiés. en outre, les problèmes n’ont pas pu être ajoutés aux projets en attente d’approbation, et les tâches et problèmes n’ont pas pu être modifiés dans les projets en attente d’approbation.

## Affectation de modèles de mise en page à des groupes

Vous pouvez désormais attribuer des modèles de mise en page à des groupes.

Avant cette modification, vous pouviez affecter des modèles de mise en page aux utilisateurs, aux équipes et aux rôles de tâche. L’affectation d’un modèle de mise en page à des groupes a la priorité d’affectation de modèle de mise en page la plus basse. 

Pour plus d’informations, voir &quot;Création et gestion des modèles de mise en page&quot;.

## Modifications apportées aux notifications utilisateur de modification en bloc

La fonctionnalité a changé lors de la modification en masse des paramètres de notification électronique des utilisateurs. Lorsque vous sélectionnez plusieurs utilisateurs pour modifier leurs paramètres d’e-mail de notification, seules les notifications spécifiques que vous mettez à jour sont modifiées pour tous les utilisateurs sélectionnés. Tous les paramètres de notification électronique inchangés restent identiques pour tous les utilisateurs sélectionnés, même s’ils diffèrent d’un utilisateur à l’autre. 

Avant cette modification, les paramètres de notification électronique que vous avez sélectionnés étaient enregistrés et tous les autres paramètres de notification inchangés étaient désélectionnés lorsque vous avez enregistré vos modifications. 

Pour plus d’informations, voir &quot;Modification des paramètres de notification utilisateur en bloc&quot; dans [Activation ou désactivation de vos propres notifications d’événement](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Mise à jour de l’aspect de plusieurs notifications par courrier électronique

L’aspect des notifications par e-mail suivantes a été mis à jour avec une nouvelle interface utilisateur :

* Assignation du problème
* Modifications de date de validation
* Lorsque le statut d&#39;un projet passe du statut idée/approuvé/rejeté/demandé/planifié à courant, envoyez un e-mail à l&#39;équipe
* Décision d’approbation des parties intéressées
* Une tâche de prédécesseur terminée pour les dépendances de tâche
* En attente d’approbation (projet, tâche, problèmes)
* Changement d’état sur les projets, tâches, problèmes

N’oubliez pas de mettre à jour l’adresse électronique associée à votre compte pour pouvoir tester cette fonctionnalité, car l’environnement de test Aperçu permet d’effacer les adresses électroniques de tous les utilisateurs.    Pour plus d’informations sur les notifications électroniques, voir [Notifications Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## Nouvelles options de résumé des emails pour plusieurs zones de notifications

L’option &quot;Daily Digest&quot; a été ajoutée dans les zones de notifications suivantes :

* Informations sur les projets sur lesquels je travaille
* Informations sur les projets dont je suis le sponsor
* Informations d&#39;approbation
* Informations sur le travail qui m&#39;a été affecté
* Communication

Pour plus d’informations, voir [Notifications Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  N’oubliez pas de mettre à jour l’adresse électronique associée à votre compte pour pouvoir tester cette fonctionnalité, car l’environnement de test Aperçu permet d’effacer les adresses électroniques de tous les utilisateurs. 

## Rendre un groupe public

Lorsque vous rendez un groupe public, vous pouvez désormais l’ajouter à des utilisateurs sans être propriétaire d’un groupe. Vous devez disposer d’un accès d’administration utilisateur pour pouvoir modifier les utilisateurs.

Pour plus d’informations sur la publication d’un groupe, voir la section [Création d’un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) dans [Création d’un groupe](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Partage de l’URL d’un objet dans l’application mobile 

Vous pouvez maintenant partager l’URL sur les objets suivants de l’application mobile Workfront :

* Projets
* Tâches
* Événements
* Feuilles de temps
* Documents

Vous pouvez partager une URL d’un objet dans les applications suivantes :

* Message texte
* E-mail
* Lecteur de stockage (par exemple, iCloud Drive)
* Une autre application installée (par exemple, Notes, Facebook)
* Vous pouvez copier un lien vers l’objet dans le presse-papiers et le coller ultérieurement dans une autre application. 

## Aide contextuelle dans la configuration

Toutes les zones du menu Configuration ont été mises à jour avec une icône Aide dans le coin supérieur droit de la zone. Cette icône fournit un lien vers un article du site d’aide relatif à cette zone. Certaines sections des zones Configuration ont également été mises à jour à l’aide de l’icône Aide. 

## Ajouter des taux de dépenses plus précis

Vous pouvez désormais ajouter des taux de dépenses plus exacts lors de la création de types de dépenses. Les taux de dépenses peuvent contenir jusqu’à 4 caractères après la virgule (par exemple, 1,0375). Cela signifie que tous les champs qui utilisent ce taux peuvent être plus précis.

Avant cette modification, les taux de dépenses ne pouvaient contenir que 2 caractères au maximum après la décimale (par exemple, 1,03).

Pour plus d’informations sur la création de taux de dépenses, voir [Création de types de dépenses personnalisés](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## Enregistrement du webinaire sur l’aperçu 1 et la version 2 de R1

Ce webinaire a été présenté par l’équipe Préparation à la publication de Workfront le 19 janvier 2017. Ce webinaire a été consacré aux modifications de version de 2017 et a couvert les nouvelles fonctionnalités qui peuvent être testées dans l’aperçu.
