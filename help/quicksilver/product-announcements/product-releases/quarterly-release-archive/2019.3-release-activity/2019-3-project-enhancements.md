---
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: Améliorations des projets (version 2019.3)
description: Cette page décrit toutes les améliorations apportées au projet avec la version 2019.3. Elle a été mise à disposition dans l’environnement de production la semaine du 19 août 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 127d695c-74e4-45f9-b5f6-55c1d05935cf
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 100%

---

# Améliorations des projets (version 2019.3)

Cette page décrit toutes les améliorations apportées au projet avec la version 2019.3. Elle a été mise à disposition dans l’environnement de production la semaine du 19 août 2019.

Pour obtenir la liste de toutes les modifications apportées à la version 2019.3, voir [Vue d’ensemble de l’activité de la version 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Modifier le type d’affichage d’un champ dans un formulaire personnalisé

Vous pouvez désormais modifier le type d’affichage d’un champ dans un formulaire personnalisé.

Par exemple, si vous avez créé un champ de cases à cocher, vous pouvez le transformer en champ de liste déroulante ou en champ de boutons radio. Ces trois types d’affichage sont interchangeables.

Si vous avez créé un champ de texte d’une seule ligne, vous pouvez également le remplacer par un champ de texte de paragraphe. Ces deux types d’affichage sont interchangeables.

Auparavant, pour modifier le type d’affichage d’un champ personnalisé, il fallait créer un champ et supprimer l’ancien. Cela nécessitait le transfert de données, ce qui prenait souvent beaucoup de temps.

>[!NOTE]
>
>Disponibilité en prévisualisation : 9 août 2019
>
>Disponibilité en production : 30 août 2019

## Créer des calendriers et des rapports de congés

Vous pouvez maintenant consulter les congés des utilisateurs et des utilisatrices pour améliorer la planification et l’exécution. Vous pouvez également ajouter de nouveaux rapports et calendriers de congés à vos tableaux de bord pour obtenir une vue en temps réel de la disponibilité des utilisateurs et des utilisatrices.

>[!NOTE]
>
>Disponibilité en prévisualisation : 9 août 2019
>
>Disponibilité en production : 30 août 2019

## Le filtre Ouvert affiche désormais plus de résultats dans une liste de problèmes.

Lorsque vous appliquez le filtre « Ouvert » à une liste de problèmes, la liste inclut des problèmes qui :

* sont au statut « Fermé - En attente d’approbation » ;
* sont associés à un objet de résolution.

Avant cette modification, ces problèmes n’étaient pas inclus dans la liste lors de l’application du filtre « Ouvert ».

## Nouvelle expérience lors de le modfication en ligne d’informations dans des listes

Lorsque vous modifiez des informations en ligne dans les nouvelles listes, les lignes qui ont été modifiées sont grisées, mais les informations restent visibles. Avant cette modification, les lignes modifiées étaient grisées et les informations n’étaient pas visibles.

Les nouvelles listes se situent dans les zones suivantes de Workfront :

* Listes de tâches et de projets
* Onglets « Heures » pour les projets, les tâches et les problèmes

## Listes mises à jour pour les onglets Heures des projets, tâches et problèmes

Les vues de liste améliorées sont désormais disponibles dans les onglets « Heures » pour les projets, les tâches et les problèmes.

Avant cette amélioration, les nouvelles listes étaient appliquées uniquement aux éléments suivants :

* Liste de tâches
* Liste de projets.

Pour plus d’informations sur l’affichage des éléments dans une liste, consultez la section [Prise en main des listes dans Adobe Workfront](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

## Modifier le graphique de Gantt sans activer un mode d’édition spécial

Vous pouvez maintenant modifier le graphique de Gantt de la liste des tâches que l’enregistrement automatique soit activé ou non. Vous ne pouvez pas annuler les modifications lorsque le bouton (bascule) d’activation/désactivation est activé. Dans ce cas, les modifications que vous apportez au projet sont enregistrées automatiquement.

Pour plus d’informations sur la modification du graphique de Gantt de la liste des tâches, consultez la section [Mettre à jour des informations dans le graphique de Gantt de la liste des tâches](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Supprimer l’onglet « Problèmes » du tableau Kanban

Nous supprimons l’onglet « Problèmes » du tableau Kanban dans la version de production 19.3. Vous pouvez toujours accéder au sous-onglet « Problèmes » à partir de la liste d’attente du tableau Kanban.

## Supprimer les onglets « Documents » et « Problèmes » de la page des détails de l’itération

>[!NOTE]
>
>Cette modification se produira dans l’environnement de production de la version 2019.3. Elle ne sera pas effectuée dans l’environnement de prévisualisation avant la version de production.

Nous supprimons les onglets Documents et Problèmes de la page détails de l’itération Agile :

* **Documents :** tous les documents stockés dans l’onglet Documents doivent être déplacés avant la version de production. Si vous ne déplacez pas vos documents, vous n’y aurez plus accès.
* **Problèmes :** cet onglet se trouve généralement sous le menu déroulant Plus. Vous pouvez toujours accéder au sous-onglet Problèmes à partir de l’onglet Éléments de travail de l’itération.

## Prendre en compte ou ignorer les congés de la personne pour les dates de la tâche

Vous pouvez maintenant décider d’autoriser ou non le planning des congés du ou de la cessionnaire principal d’une tâche afin d’ajuster les dates planifiées.

Vous pouvez prendre cette décision au niveau du système, en tant qu’administrateur ou administratrice Workfront ou au niveau du projet, en tant que personne gestionnaire de projet.

Avant cette modification, les congés de la principale personne cessionnaire ajustaient toujours les dates prévues de la tâche, si la contrainte de tâche permettait de modifier les dates.

Pour plus d’informations sur le paramètre de congés des personnes au niveau du système, voir [Configurer les préférences du projet à l’échelle du système](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Pour plus d’informations sur le paramètre de congés des personnes au niveau du projet, voir [Modifier les projets](../../../../manage-work/projects/manage-projects/edit-projects.md).

>[!NOTE]
>
>Disponibilité en prévisualisation : 22 juillet 2019
>
>Disponibilité en production : 9 août 2019

## Conditions personnalisées

Vous pouvez maintenant procéder comme suit pour personnaliser les conditions que vous utilisez pour les projets, tâches et problèmes et mieux répondre aux besoins de votre organisation :

* Créez des conditions personnalisées avec vos propres libellés et couleurs.
* Modifiez l’ordre des conditions dans les listes déroulantes dans lesquelles les personnes les sélectionnent.
* Utilisez des conditions personnalisées que vous créez à la place des conditions par défaut intégrées que Workfront attribue automatiquement aux éléments de travail.
* Modifiez les noms et les couleurs des conditions par défaut intégrées pour les projets, les tâches et les problèmes.

En outre, si vous disposez des droits de modification sur une tâche ou un problème, mais que l’objet ne vous est pas affecté (peut-être parce que vous le supervisez), vous pouvez désormais modifier sa condition à l’aide de la colonne Conditions dans une vue liste.

Auparavant, les conditions ne pouvaient pas être personnalisées ou modifiées, et seuls les utilisateurs et utilisatrices pouvaient modifier la condition d’une tâche ou d’un problème s’ils y étaient affectés.

Pour plus d’informations, voir [Conditions personnalisées](../../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).

>[!NOTE]
>
>Disponibilité en prévisualisation : 4 juillet 2019
>
>Disponibilité en production : fin septembre ou début octobre

## Nouvelle notification par e-mail pour les équipes

Il existe une nouvelle notification d’événement par e-mail pour les équipes. Les personnes membres de l’équipe reçoivent une notification par e-mail lorsqu’un projet avec des tâches affectées à leur équipe devient actif. Ce paramètre est désactivé par défaut.

Auparavant, les personnes membres de l’équipe ne pouvaient pas être averties lorsque les projets auxquels elles participaient devenaient actifs.

Pour plus d’informations, voir Notifications : informations sur les projets auxquels je participe.

>[!NOTE]
>
>Disponibilité en prévisualisation : 4 juillet 2019
>
>Disponibilité en production : 18 juillet 2019

## Les mises à jour du document apparaissent maintenant sur l’objet et le projet associés.

Lorsque vous commentez un document, votre mise à jour apparaît désormais dans l’onglet Mises à jour à la fois pour le document et pour l’objet auquel le document est associé.

Si l’objet fait partie d’un projet, votre commentaire sur le document s’affiche également dans l’onglet Mises à jour du projet.

Auparavant, les commentaires de mise à jour s’affichaient uniquement dans l’onglet Mises à jour du document.

Pour plus d’informations, voir la section [Mettre à jour le travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#updates) dans l’article [Mettre à jour le travail](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Disponibilité en prévisualisation : 6 juin 2019
>
>Disponibilité en production : 20 juin 2019

## Visibilité du planning de congés d’une personne lors de son affectation à des tâches et problèmes

Lorsque vous affectez une personne à une tâche ou à un problème, vous pouvez désormais directement voir un avertissement si la personne sélectionnée a des congés planifiés qui coïncident avec les dates planifiées de la tâche ou du problème.

Pour plus d’informations sur l’attribution de tâches, voir [Attribuer des tâches](../../../../manage-work/tasks/assign-tasks/assign-tasks-1.md).

Pour plus d’informations sur les congés, voir [Configurer les congés personnels](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

>[!NOTE]
>
>Disponibilité de la version de prévisualisation : 30 mai 2019
>
>Disponibilité de la version de production : 13 juin 2019

## Ajouter des champs représentant des objets dans les formulaires personnalisés

Nous avons créé un nouveau type de champ dans le créateur de formulaire personnalisé appelé champ de saisie semi-automatique. Ce champ vous permet d’ajouter des champs représentant des objets à vos formulaires personnalisés. Actuellement, l’objet Utilisateur ou utilisatrice est activé avec saisie semi-automatique, et d’autres objets sont à venir.

Auparavant, les administrateurs et administratrices devaient gérer manuellement les personnes en tant qu’options individuelles dans les menus déroulants de formulaire personnalisés.

>[!NOTE]
>
>Disponibilité de la version de prévisualisation : 30 mai 2019
>
>Disponibilité de la version de production : 13 juin 2019
>
>Avant la date de publication de la version de production, les nouveaux champs personnalisés ne sont pas pris en charge sur Mobile, Outlook, MS Teams et l’intégration Salesforce native.
>
>En production, Outlook et MS Teams sont désormais pris en charge. Mobile est pris en charge depuis fin juin ou début juillet et les intégrations Salesforce depuis juin.

## Le nouveau champ « Objet » de la demande a été renommé « Nom »

>[!NOTE]
>
>Cette fonctionnalité a été supprimée et ne sera pas incluse dans la version 2019.3.

Désormais, lorsque vous envoyez une nouvelle requête à une file d’attente des demandes, vous devez saisir le nom de la demande dans le champ « Nom » du nouveau formulaire de demande.

Avant cette modification, vous deviez saisir le nom de la demande dans le champ « Objet ».

Pour plus d’informations sur la création de demandes, voir [Créer et envoyer des demandes Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

