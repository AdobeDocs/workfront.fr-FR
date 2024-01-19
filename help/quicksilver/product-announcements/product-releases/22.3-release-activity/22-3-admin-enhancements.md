---
title: 2.2.3 Améliorations apportées aux administrateurs
description: 2.2.3 Améliorations apportées aux administrateurs
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 2.2.3 Améliorations apportées aux administrateurs

Cette page décrit toutes les améliorations apportées par l’administrateur à la version 22.3 de l’environnement Aperçu. Ces améliorations ont été apportées à la semaine du 11 juillet 2022. Pour obtenir la liste de toutes les modifications disponibles avec la version 22.3, voir [Présentation de la version 22.3](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Intégration d’Adobe Workfront à JumpSeat

Vous pouvez désormais intégrer JumpSeat à Workfront afin de créer des conseils personnalisés et intégrés au produit à l’intention de vos utilisateurs. Pour activer l’intégration, vous devez disposer d’une licence d’entreprise Adobe Workfront et d’un abonnement JumpSeat actif.

Pour plus d’informations, voir [Configuration de l’intégration JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Paramètres par défaut du BAT déplacés vers Workfront

Vous pouvez désormais modifier les paramètres de BAT suivants dans la zone de configuration de Workfront :

* Paramètres par défaut du BAT

* Paramètres de décision de BAT

Pour plus d’informations, voir [Configuration des paramètres de BAT par défaut](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Utiliser des états déverrouillés dans un processus de validation

**Remarque :** Suppression de la version de production 2.2.3. Cette fonctionnalité devrait être mise en production le 15 septembre 2022.

Pour vous permettre de mieux contrôler les processus et les états de validation dans votre système, nous avons rendu possible la création d&#39;un processus de validation basé sur un état système déverrouillé. De plus, vous pouvez désormais déverrouiller tout statut déjà utilisé dans un processus de validation.

Auparavant, un état système utilisé dans un processus de validation devait être verrouillé. Cela l’a rendu disponible pour tous les groupes, sans possibilité de le supprimer ou de le renommer, de sorte que les administrateurs de groupes ne puissent pas rationaliser la liste des états de leur groupe en fonction de leurs besoins spécifiques.

Pour plus d’informations, voir les articles suivants :

* [Créer un processus d’approbation pour les tâches](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Création ou modification d’un état](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [États au niveau du système verrouillés et déverrouillés](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Ajout d’un fichier PDF à un formulaire personnalisé

Nous vous aidons à rendre les formulaires personnalisés plus visuels et informatifs grâce aux nouveaux widgets de ressources que vous pouvez ajouter, tels que les images et les vidéos. Vous pouvez maintenant ajouter un lien vers un fichier de PDF à un formulaire personnalisé. Lorsque le formulaire est joint à un objet, les utilisateurs qui l’utilisent peuvent afficher et interagir avec le PDF depuis le formulaire.

Pour plus d’informations, voir [Ajout ou modification d’une image ou d’un autre widget de ressource dans un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## L’éditeur de calcul de champ de formulaire personnalisé affiche les informations d’erreur

>[!NOTE]
>
>Cette fonctionnalité est temporairement indisponible. Cette page sera mise à jour lorsque la fonctionnalité sera disponible.

La modification des calculs pour les champs personnalisés est désormais plus facile avec des informations d’erreur utiles indiquées directement dans le calcul. Lorsque vous créez un champ calculé dans un formulaire personnalisé, les erreurs sont surlignées en rose. Lorsque vous passez le curseur sur la partie mise en surbrillance, une info-bulle s’affiche pour décrire le problème.

Pour plus d’informations, voir [Ajout de données calculées à un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Personnalisation de l’en-tête du projet

En tant qu’administrateur Workfront ou de groupe, vous pouvez désormais personnaliser les champs qui s’affichent dans l’en-tête d’un projet lorsque vous utilisez un modèle de mise en page.

Cette mise à jour comprend les améliorations suivantes :

* Supprimez les champs existants de l’en-tête du projet.

* Ajoutez de nouveaux champs de présentation de projet non modifiables. Vous ne pouvez pas ajouter de champs personnalisés ou de champs qui peuvent être modifiés. Les champs modifiables qui se trouvent actuellement sur l’en-tête du projet peuvent rester sur l’en-tête .

* L’en-tête de l’objet peut contenir jusqu’à cinq champs.


Avant cette version, les champs des en-têtes d’objet ne pouvaient pas être personnalisés.

Pour plus d’informations, voir [Personnalisation des en-têtes d’objet à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Contrôle de la création d’un projet vierge

En tant qu’administrateur système ou de groupe, vous pouvez désormais contrôler si les utilisateurs peuvent créer des projets vierges sans utiliser de modèle. Nous avons ajouté un nouveau paramètre dans la zone Préférences du projet de la configuration, qui vous permet de désactiver la création de projets vierges dans les zones suivantes :

* À partir de l’option Nouveau projet dans une liste de projets

* Lors de la conversion d’une publication en projet à partir de la page de problèmes


Le nouveau paramètre est &quot;Autoriser les utilisateurs à créer des projets sans utiliser de modèle&quot; et est activé par défaut.

**Remarque :** Les utilisateurs peuvent toujours convertir une tâche en projet vierge.

Pour plus d’informations, voir [Configuration des préférences de projet à l’échelle du système](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Désactivation d’un groupe à partir de la page Groupes

Récemment, nous avons ajouté la possibilité de désactiver et de réactiver les groupes. Pour rendre cette action plus rapide et plus facile, nous l’avons ajoutée à la page d’un groupe. Maintenant, après avoir cliqué sur le nom d’un groupe pour accéder à sa page, vous pouvez sélectionner le menu Plus . ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) en regard du nom du groupe, sélectionnez Désactiver ou Réactiver.

Auparavant, vous pouviez désactiver ou réactiver un groupe uniquement à l’aide de la case à cocher Est actif sur sa page Détails .

Pour plus d’informations, voir [Désactivation ou réactivation d’un groupe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Ajout de vidéos à des formulaires personnalisés

Vous pouvez désormais offrir un nouveau mode d’information, d’intérêt visuel et de créativité à un formulaire personnalisé en ajoutant une vidéo. Lorsque le formulaire est joint à un objet, les utilisateurs qui travaillent avec l’objet peuvent lire la vidéo à tout moment.

Auparavant, vous pouviez uniquement ajouter des champs textuels et des images à un formulaire personnalisé.

Pour plus d’informations, voir [Ajout ou modification d’une image ou d’un widget de ressource vidéo dans un formulaire personnalisé](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

