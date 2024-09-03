---
title: Améliorations apportées aux projets (version 21.4)
description: Améliorations apportées aux projets (version 21.4)
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 100%

---

# Améliorations apportées aux projets (version 21.4)

Cette page décrit toutes les améliorations apportées aux projets par la version 21.4 à l’environnement de prévisualisation. Ces améliorations sont disponibles dans l’environnement de production à partir de la semaine du 4 octobre 2021.

Pour obtenir la liste de toutes les modifications introduites par la version 21.4, consultez la section [Vue d’ensemble de la version 21.4](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Inclure des images dans les mises à jour

Dans l’onglet Mises à jour d’un objet, vous pouvez désormais ajouter des images en cliquant sur l’icône Image de la barre d’outils. Vous pouvez également glisser-déposer une image dans la zone de mise à jour. Notez que votre administrateur ou administratrice Workfront doit autoriser l’ajout d’images pour que vous puissiez voir l’icône Image.

Vous pouvez ajouter des images dans les mises à jour et les réponses. Une miniature d’image dans la mise à jour indique que les personnes destinataires peuvent prévisualiser l’image dans le navigateur ou la télécharger, et les notifications par e-mail et in-app montrent que des images sont jointes à la mise à jour.

Auparavant, la seule façon de partager une image dans Workfront était de la joindre à un objet en tant que document. Les images ajoutées dans l’onglet Mises à jour ne sont disponibles que dans cet onglet et non dans l’onglet Documents.

Pour plus d’informations, voir [Mettre à jour le travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Avant que les utilisateurs et utilisatrices de Workfront puissent inclure des images dans les mises à jour, cette fonctionnalité doit d’abord être activée par l’administrateur ou l’administratrice d’Adobe Workfront, comme décrit dans [Configurer les préférences pour les mises à jour des utilisateurs et utilisatrices](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## Algorithme mis à jour pour les affectations intelligentes

Nous avons amélioré l’algorithme utilisé pour les affectations intelligentes. Grâce à cette nouvelle amélioration, Workfront examine les 30 dernières affectations effectuées par la personne connectée pour faire des suggestions lorsqu’elle affecte des tâches et des problèmes. La liste des suggestions peut contenir jusqu’à 50 personnes.

Avant cette amélioration, Workfront prenait en compte les affectations des tâches parent et d’autres attributs d’utilisateur ou d’utilisatrice liés à ces affectations lors de la suggestion de personnes.

Pour plus d’informations sur les affectations intelligentes, voir [Vue d’ensemble des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Nouvelle expérience lors de la création d’un projet à partir d’un modèle

Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface de création d’un projet à partir d’un modèle. La fonctionnalité de création d’un projet à l’aide d’un modèle n’a pas changé. Toutefois, les améliorations suivantes ont été apportées à l’interface récemment remaniée :

* Prévisualiser les informations du modèle avant de le joindre
* Ajouter des modèles à une liste de favoris pendant le processus de création du projet

Nous avons mis à jour l’interface de création du projet, aussi bien lorsque vous le créez à partir de la zone Projets que de la zone Modèles.

Pour plus d’informations, voir [Créer un projet à l’aide d’un modèle](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Nouvelle expérience pour les modèles joints à des projets

>[!NOTE]
>
>Cette fonctionnalité n’est disponible que dans la nouvelle version d’Adobe Workfront.

Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface permettant de joindre un modèle à un projet. La fonctionnalité permettant de joindre un modèle n’a pas changé. Toutefois, les améliorations suivantes ont été apportées à l’interface récemment remaniée :

* Prévisualiser les informations du modèle avant de le joindre
* Ajouter des modèles à une liste de favoris pendant le processus d’ajout de pièce jointe
* Afficher toutes les options de gestion des paramètres des modèles et des projets sur une page continue

Pour plus d’informations, voir [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Valeurs unifiées de durée et d’unité de durée pour les tâches

Pour une expérience client plus propre et plus rationnelle, nous avons fusionné la valeur du champ Durée avec l’unité de temps de la durée. Avant cette amélioration, l’unité de temps s’affichait dans un champ déroulant distinct après le champ Durée.

En plus des champs Durée dans les zones Détails de la tâche, Modifier les tâches et Nouvelle tâche, nous mettons également à jour les champs suivants pour tenir compte de cette expérience :

* Champ Durée lors des affectations avancées
* Champ Délai de nivellement lors de la création ou de la modification d’une tâche
* Champ Fréquence lors de la création d’une tâche récurrente (bientôt disponible)
* Champ Décalage lors de l’ajout d’une tâche antérieure (bientôt disponible)

Pour plus d’informations, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## Désactiver l’ajout de problèmes en ligne sur les projets

Afin de garantir que les personnes fournissent des informations exactes lorsqu’elles ajoutent des problèmes à des projets en remplissant un formulaire de problème, nous avons introduit un nouveau paramètre qui vous permet de gérer si elles peuvent ajouter des problèmes à un projet ou à ses tâches en ligne. Ce paramètre est activé par défaut dans la zone des nouveaux paramètres de la zone Modifier le projet. Le désactiver réduit l’option Ajouter d’autres problèmes dans la section Problèmes d’un projet, de sorte que les utilisateurs et utilisatrices ne peuvent plus ajouter de problèmes à la liste. Les personnes peuvent toujours ajouter des problèmes aux projets en utilisant l’option Nouveau problème dans la section Problèmes ou en utilisant une file d’attente des demandes s’il y en a une configurée pour le projet.

>[!NOTE]
>
>Ce paramètre n’est disponible que dans la nouvelle expérience Workfront. Les personnes qui travaillent dans Workfront Classic peuvent toujours ajouter des problèmes en ligne à un projet ou à ses tâches, même si ce paramètre a été désactivé pour le projet par une personne travaillant dans la nouvelle expérience Workfront.

Pour plus d’informations, voir [Modifier les projets](../../../manage-work/projects/manage-projects/edit-projects.md).

## Amélioration de l’affichage des champs personnalisés pour les cases à cocher et les cases d’option

L’affichage et la sélection des cases à cocher et des cases d’option dans les formulaires personnalisés viennent d’être facilités. Un champ personnalisé comportant de nombreuses cases à cocher ou cases d’option s’affiche désormais dans plusieurs colonnes sur la page. Auparavant, ils s’affichaient dans une seule colonne, ce qui nécessitait un défilement supplémentaire pour les personnes qui remplissaient le formulaire.

Cela dépend de la façon dont vous positionnez les champs dans le formulaire personnalisé. Si vous placez un autre champ sur la même ligne que le champ de la case à cocher ou de la case d’option, les options peuvent n’avoir que l’espace horizontal nécessaire pour s’afficher dans une seule colonne.

Pour plus d’informations sur le remplissage d’un formulaire personnalisé, voir [Modifier les informations dans les champs des formulaires personnalisés](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

