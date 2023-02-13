---
title: 21.4 Améliorations apportées au projet
description: 21.4 Améliorations apportées au projet
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 21.4 Améliorations apportées au projet

Cette page décrit toutes les améliorations apportées aux projets avec la version 21.4 de l’environnement Aperçu. Ces améliorations seront disponibles dans l’environnement de production au cours de la semaine du 4 octobre 2021.

Pour obtenir la liste de toutes les modifications disponibles avec la version 21.4, voir [Présentation de la version 21.4](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Inclure des images dans les mises à jour

Dans l’onglet Mises à jour d’un objet, vous pouvez désormais ajouter des images en cliquant sur l’icône Image de la barre d’outils. Vous pouvez également faire glisser et déposer une image dans la zone de mise à jour. Notez que votre administrateur Workfront doit activer l’ajout d’images avant que l’icône Image ne s’affiche.

Vous pouvez ajouter des images dans les mises à jour et les réponses. Une miniature d’image dans la mise à jour indique que les destinataires peuvent prévisualiser l’image dans le navigateur ou la télécharger, et les notifications par e-mail et in-app indiquent que les images sont jointes à la mise à jour.

Auparavant, le seul moyen de partager une image dans Workfront était de la joindre à un objet en tant que document. Les images ajoutées sous l’onglet Mises à jour ne sont disponibles que dans cet onglet et non dans l’onglet Documents .

Pour plus d’informations, voir [Mise à jour du travail](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Pour que les utilisateurs de Workfront puissent inclure des images dans les mises à jour, cette fonction doit d’abord être activée par l’administrateur Adobe Workfront, comme décrit dans la section [Configuration des préférences pour les mises à jour des utilisateurs](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## Algorithme mis à jour pour les affectations intelligentes

Nous avons amélioré l’algorithme utilisé lors d’affectations intelligentes. Grâce à cette nouvelle amélioration, Workfront examine les 30 affectations les plus récentes effectuées par l’utilisateur connecté afin d’effectuer des suggestions lorsqu’il affecte des tâches et des problèmes. La liste de suggestions peut contenir jusqu’à 50 utilisateurs.

Avant cette amélioration, Workfront prenait en compte les affectations sur les tâches parents et d’autres attributs utilisateur associés à ces affectations lors de la suggestion d’utilisateurs.

Pour plus d’informations sur les affectations intelligentes, voir [Présentation des affectations intelligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Nouvelle expérience lors de la création d’un projet à partir d’un modèle

Pour que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface de création d’un projet à partir d’un modèle. La fonctionnalité de création d’un projet à l’aide d’un modèle n’a pas changé. Toutefois, voici quelques améliorations apportées à cette nouvelle interface :

* Prévisualiser les informations du modèle avant de les joindre
* Ajouter des modèles à une liste de favoris pendant le processus de création du projet

Nous avons mis à jour l’interface de création du projet, à la fois lorsque vous le créez à partir des projets et de la zone Modèles .

Pour plus d’informations, [Création d’un projet à l’aide d’un modèle](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Nouvelle expérience lors de l’association de modèles à des projets

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement dans la nouvelle expérience Adobe Workfront.

Afin que votre utilisation de Workfront soit cohérente avec la nouvelle expérience Workfront, nous avons repensé l’interface permettant de joindre un modèle à un projet. La fonctionnalité d’association d’un modèle n’a pas changé. Certaines des améliorations apportées à cette nouvelle interface ont été apportées :

* Prévisualiser les informations du modèle avant de les joindre
* Ajouter des modèles à une liste de favoris pendant le processus de pièce jointe
* Afficher toutes les options de gestion des paramètres de modèle et de projet sur une page continue

Pour plus d’informations, voir [Joindre un modèle à un projet](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Valeurs unitaires de durée et durée pour les tâches

Pour une expérience utilisateur plus propre et plus simple, nous avons fusionné la valeur du champ Durée avec l’unité de temps de durée. Avant cette amélioration, l’unité de temps affichée dans un champ déroulant distinct après le champ Durée .

Outre les champs Durée des zones Détails de la tâche, Modifier les tâches et Nouvelle tâche, nous mettons également à jour les champs suivants pour qu’ils correspondent à cette expérience :

* Champ Durée lors d’affectations avancées
* Champ de délai d&#39;ajustement lors de la création ou de la modification d&#39;une tâche
* Champ Fréquence lors de la création d&#39;une tâche récurrente (disponible prochainement)
* Champ de libellé lors de l’ajout d’un prédécesseur (disponible prochainement)

Pour plus d’informations, voir [Modifier les tâches](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## Désactivation de l’ajout de problèmes en ligne sur les projets

Pour vous assurer que les utilisateurs fournissent des informations précises lors de l’ajout de problèmes à des projets en remplissant un formulaire de problèmes, nous avons introduit un nouveau paramètre qui vous permet de gérer s’ils peuvent ajouter des problèmes à un projet ou à ses tâches intégrées. Ce paramètre est activé par défaut dans la nouvelle zone Paramètres du problème de la boîte de dialogue Modifier le projet . La désactivation réduit l’option Ajouter d’autres problèmes de la section Problèmes d’un projet afin que les utilisateurs ne puissent pas ajouter d’autres problèmes dans la liste. Les utilisateurs peuvent toujours ajouter des problèmes aux projets à l’aide de l’option Nouveau problème de la section Problèmes ou à l’aide d’une file d’attente de demandes si celle-ci est configurée pour le projet.

>[!NOTE]
>
>Ce paramètre est disponible uniquement dans la nouvelle expérience Workfront. Les utilisateurs qui travaillent dans Workfront Classic peuvent toujours ajouter des problèmes à un projet ou à ses tâches, même si ce paramètre a été désactivé pour le projet par un utilisateur qui travaille dans la nouvelle expérience Workfront.

Pour plus d’informations, voir [Modification de projets](../../../manage-work/projects/manage-projects/edit-projects.md).

## Amélioration de l’affichage des champs personnalisés pour les cases à cocher et les boutons radio

L’affichage et la sélection des options de cases à cocher et de boutons radio dans les formulaires personnalisés sont devenus plus simples : un champ personnalisé avec de nombreuses options de cases à cocher ou de boutons radio s’affiche désormais dans plusieurs colonnes sur la page. Auparavant, ils s’affichaient dans une seule colonne, ce qui nécessitait un défilement supplémentaire pour les utilisateurs qui remplissaient le formulaire.

Cela dépend de la position des champs dans le formulaire personnalisé. Si vous placez un autre champ dans la même ligne avec la case à cocher ou le champ de bouton radio, les options peuvent n’avoir qu’un espace horizontal suffisant pour s’afficher dans une seule colonne.

Pour plus d’informations sur le remplissage d’un formulaire personnalisé, voir [Modifier les informations dans les champs de formulaire personnalisés](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

Pour plus d’informations sur la création d’une case à cocher ou d’un champ de bouton radio dans un formulaire personnalisé, reportez-vous aux sections [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) et [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) dans l’article [Création ou modification d’un formulaire personnalisé](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

