---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: Améliorations des projets (version 2019.3)
description: Cette page décrit toutes les modifications apportées au projet avec la version 2019.3. Elle a été rendue disponible dans l’environnement de production dans la semaine du 19 août 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 2%

---

# Améliorations des projets (version 2019.3)

Cette page décrit toutes les modifications apportées au projet avec la version 2019.3. Elle a été rendue disponible dans l’environnement de production dans la semaine du 19 août 2019.

Pour obtenir la liste de toutes les modifications apportées en 2019.3, consultez la [présentation de l’activité de version 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Modifier le type d’affichage d’un champ dans un formulaire personnalisé

Vous pouvez désormais modifier le type d’affichage d’un champ dans un formulaire personnalisé.

Par exemple, si vous avez créé un champ de cases à cocher, vous pouvez le transformer en champ de liste déroulante ou en champ de boutons radio. Ces trois types d’affichage de champ sont interchangeables.

Si vous avez créé un champ de texte d’une seule ligne, vous pouvez également le remplacer par un champ de texte de paragraphe. Ces deux types d’affichage de champ sont interchangeables.

Auparavant, pour modifier le type d’affichage d’un champ personnalisé, vous deviez créer un nouveau champ et supprimer l’ancien champ. Il fallait pour cela transférer des données, ce qui prenait souvent du temps.

>[!NOTE]
>
>Disponibilité de l’aperçu : 9 août 2019
>
>Disponibilité de la production : 30 août 2019

## Créer des calendriers et des rapports de temps d’expiration

Vous pouvez désormais voir le temps de pause de l’utilisateur pour une meilleure planification et une meilleure exécution. Vous pouvez également ajouter de nouveaux rapports et calendriers de désactivation à vos tableaux de bord pour une vue en temps réel de la disponibilité des utilisateurs.

>[!NOTE]
>
>Disponibilité de l’aperçu : 9 août 2019
>
>Disponibilité de la production : 30 août 2019

## Le filtre Ouvrir affiche désormais d’autres résultats dans une liste de problèmes.

Lorsque vous appliquez le filtre Ouvrir à une liste de problèmes, la liste inclut des problèmes qui :

* Sont dans un état Fermé - En attente d’approbation
* Sont associés à un objet de résolution

Avant cette modification, ces problèmes n’étaient pas inclus dans la liste lors de l’application du filtre Ouvrir.

## Nouvelle expérience lors de l’édition en ligne d’informations dans des listes

Lorsque vous insérez des informations d’édition dans les nouvelles listes, les lignes qui ont été modifiées sont grisées, mais les informations restent visibles. Avant cette modification, les lignes modifiées étaient grisées et les informations n’étaient pas visibles.

Vous trouverez les nouvelles listes dans les zones suivantes de Workfront :

* Listes Projets et tâches
* Onglet Heures pour les projets, les tâches et les problèmes

## Listes mises à jour pour les onglets Projet, Tâche et Heures de publication

Les vues de liste améliorées sont désormais disponibles dans les onglets Heures pour les projets, les tâches et les problèmes.

Avant cette amélioration, les nouvelles listes étaient appliquées uniquement aux éléments suivants :

* Liste des tâches
* Liste des projets

Pour plus d’informations sur l’affichage des éléments dans une liste, voir [Prise en main des listes dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Modifier Gantt sans activer un mode de modification spécial

Vous pouvez maintenant modifier le diagramme de Gantt de la liste des tâches lorsque l’enregistrement automatique est activé ou non. Vous ne pouvez pas annuler les modifications lorsque le bouton activer/désactiver est activé. Dans ce cas, les modifications que vous apportez au projet sont enregistrées automatiquement.

Pour plus d’informations sur la modification du diagramme de Gantt de la liste des tâches, voir [Mise à jour d’informations dans le diagramme de Gantt de la liste des tâches](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Suppression de l’onglet Problèmes du panorama Kanban

Nous supprimons l’onglet Problèmes du panorama Kanban de la version de production 19.3. Vous pouvez toujours accéder au sous-onglet Problèmes à partir du journal sur le panorama Kanban.

## Suppression des onglets Documents et Problèmes de la page Détails de l’itération

>[!NOTE]
>
>Cette modification se produira dans Production avec la version 2019.3. Elle ne sera pas effectuée dans l’environnement Aperçu avant la version de production.

Nous supprimons les onglets Documents and Issues de la page Agile iteration details :

* **Documents :** Tous les documents stockés dans l’onglet Documents doivent être déplacés avant la version de production. Si vous ne parvenez pas à déplacer vos documents, vous n’y aurez plus accès.
* **Problèmes :** Cet onglet se trouve généralement sous le menu déroulant Plus. Vous pouvez toujours accéder au sous-onglet Problèmes à partir de l’onglet Éléments de travail de l’itération.

## Envisager ou ignorer le délai d’expiration de l’utilisateur pour les dates de la tâche

Vous pouvez maintenant décider d’autoriser ou non le délai de remise d’une tâche au cessionnaire Principal d’une tâche afin d’ajuster les dates prévues.

Vous pouvez prendre cette décision au niveau du système, en tant qu’administrateur Workfront ou au niveau du projet, en tant que chef de projet.

Avant cette modification, le temps de pause du cessionnaire Principal ajustait toujours les dates planifiées de la tâche, si la contrainte de tâche permettait de modifier les dates.

Pour plus d’informations sur le paramètre de délai de désactivation de l’utilisateur au niveau du système, voir [Configuration des préférences du projet à l’échelle du système](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Pour plus d’informations sur le paramètre de délai de désactivation au niveau du projet, voir [Modification de projets](../../../../manage-work/projects/manage-projects/edit-projects.md).

>[!NOTE]
>
>Disponibilité de l’aperçu : 22 juillet 2019
>
>Disponibilité de la production : 9 août 2019

## Conditions personnalisées

Vous pouvez maintenant procéder comme suit pour personnaliser les Conditions que vous utilisez pour les projets, tâches et problèmes et mieux répondre aux besoins de votre organisation :

* Créez des conditions personnalisées avec vos propres libellés et couleurs.
* Modifiez l’ordre des Conditions dans les listes déroulantes dans lesquelles les utilisateurs les sélectionnent.
* Utilisez des conditions personnalisées que vous créez à la place des conditions par défaut intégrées que Workfront attribue automatiquement aux éléments de travail.
* Modifiez les noms et les couleurs des conditions par défaut intégrées pour les projets, les tâches et les problèmes.

En outre, si vous disposez des droits de modification d’une tâche ou d’un problème, mais que vous ne lui êtes pas assigné (peut-être parce que vous la supervoyez), vous pouvez désormais modifier sa condition à l’aide de la colonne Conditions dans un mode Liste.

Auparavant, les conditions ne pouvaient pas être personnalisées ou modifiées, et seuls les utilisateurs pouvaient modifier la condition d’une tâche ou d’un problème s’ils y étaient affectés.

Pour plus d’informations, voir [Conditions personnalisées](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>Disponibilité de l’aperçu : 4 juillet 2019
>
>Disponibilité de la production : fin septembre ou début octobre

## Nouvelle notification électronique pour les équipes

Il existe une nouvelle notification d’événement par e-mail pour les équipes. Les membres de l’équipe reçoivent une notification par e-mail lorsqu’un projet avec des tâches affectées à leur équipe devient actif. Ce paramètre est désactivé par défaut.

Auparavant, les membres de l’équipe ne pouvaient pas être avertis lorsque les projets sur lesquels ils étaient actifs.

Pour plus d’informations, voir Notifications : informations sur les projets sur lesquels je travaille.

>[!NOTE]
>
>Disponibilité de l’aperçu : 4 juillet 2019
>
>Disponibilité de la production : 18 juillet 2019

## Les mises à jour du document apparaissent maintenant sur l’objet et le projet associés.

Lorsque vous commentez un document, votre mise à jour s’affiche désormais dans l’onglet Mises à jour du document et de l’objet auquel le document est joint.

Si l’objet fait partie d’un projet, votre commentaire sur le document s’affiche également dans l’onglet Mises à jour du projet.

Auparavant, les commentaires de mise à jour s’affichaient uniquement dans l’onglet Mises à jour du document.

Pour plus d’informations, reportez-vous à la section [Mise à jour du travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) de l’article [Mise à jour du travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Disponibilité de l’aperçu : 6 juin 2019
>
>Disponibilité de la production : 20 juin 2019

## Visibilité dans le planning de désactivation d’un utilisateur lors de son attribution aux tâches et aux problèmes

Lorsque vous affectez un utilisateur à une tâche ou à un problème, vous pouvez maintenant voir un avertissement en ligne si l’utilisateur sélectionné a un délai d’expiration planifié entre les dates prévues de la tâche ou du problème.

Pour plus d’informations sur l’affectation de tâches, voir [Affecter des tâches](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md)

Pour plus d&#39;informations sur les heures de congé, voir [Configuration de l&#39;heure personnelle](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

>[!NOTE]
>
>Disponibilité de l’aperçu : 30 mai 2019
>
>Disponibilité de la production : 13 juin 2019

## Ajout de champs représentant des objets dans Forms personnalisé

Nous avons créé un nouveau type de champ dans le créateur de formulaires personnalisé appelé Typeforward. Ce champ vous permet d’ajouter des champs qui représentent des objets à vos formulaires personnalisés. Actuellement, l’objet User est activé avec Typeforward, et d’autres objets sont à venir.

Auparavant, les administrateurs devaient gérer manuellement les utilisateurs en tant qu’options individuelles dans les menus déroulants de formulaire personnalisés.

>[!NOTE]
>
>Disponibilité de l’aperçu : 30 mai 2019
>
>Disponibilité de la production : 13 juin 2019
>
>Avant la date de publication de la version de production, les nouveaux champs personnalisés ne sont pas pris en charge sur Mobile, Outlook, les équipes MS et l’intégration Salesforce native.
>
>En production, Outlook et les équipes MS sont désormais pris en charge. Mobile est pris en charge à compter de fin juin ou début juillet ; les intégrations Salesforce sont prises en charge à compter de juin.

## Le nouveau champ &quot;Objet&quot; de la requête a été renommé &quot;Nom&quot;

>[!NOTE]
>
>Cette fonctionnalité a été supprimée et ne sera pas incluse dans la version 2019.3.

Désormais, lorsque vous envoyez une nouvelle requête à une file d’attente de requêtes, vous saisissez le nom de la requête dans le champ &quot;Nom&quot; du nouveau formulaire de requête.

Avant cette modification, vous devez saisir le nom de la requête dans le champ &quot;Objet&quot;.

Pour plus d’informations sur la création de requêtes, voir [Création et envoi de requêtes Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

