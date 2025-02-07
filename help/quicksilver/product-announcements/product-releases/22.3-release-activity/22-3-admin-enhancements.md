---
title: 2.2.3 Améliorations apportées aux administrateurs et administratrices
description: 2.2.3 Améliorations apportées aux administrateurs et administratrices
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 95%

---

# 2.2.3 Améliorations apportées aux administrateurs et administratrices

Cette page décrit toutes les améliorations apportées aux administrateurs et administratrices par la version 22.3 de l’environnement de prévisualisation. Ces améliorations ont été apportées la semaine du 11 juillet 2022. Pour obtenir la liste de toutes les modifications disponibles avec la version 22.3, voir [Vue d’ensemble de la version 22.3](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Intégrer Adobe Workfront avec JumpSeat

Vous pouvez désormais intégrer JumpSeat à Workfront afin de créer des conseils personnalisés et intégrés au produit à l’intention de vos utilisateurs et de vos utilisatrices. Pour activer l’intégration, vous devez disposer d’une licence d’entreprise Adobe Workfront et d’un abonnement JumpSeat actif.

Pour plus d’informations, voir [Configurer l’intégration JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Paramètres par défaut de l’épreuve déplacés vers Workfront

Vous pouvez désormais modifier les paramètres suivants de l’épreuve dans la zone de configuration de Workfront :

* Paramètres par défaut de l’épreuve

* Paramètres du statut de décision de l’épreuve

Pour plus d’informations, voir [Configurer les paramètres d’épreuve par défaut](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Utiliser des statuts Déverrouillé dans des processus d’approbation

**Note :** suppression de la version de production 2.2.3. Cette fonctionnalité devrait être mise en production le 15 septembre 2022.

Pour vous permettre de mieux contrôler les processus et les statuts d’approbation dans votre système, nous avons autorisé la création d’un processus d’approbation basé sur un statut de système déverrouillé. De plus, vous pouvez désormais déverrouiller tout statut déjà utilisé dans un processus d’approbation.

Auparavant, un statut système utilisé dans un processus d’approbation devait être verrouillé. Cela le rendait disponible pour tous les groupes, sans possibilité de le supprimer ou de le renommer. Les équipes d’administration de groupe ne pouvaient donc pas rationaliser la liste des statuts de leur groupe en fonction de leurs besoins spécifiques.

Pour plus d’informations, consultez les articles suivants :

* [Créer un processus d’approbation pour les éléments de travail](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Créer ou modifier un statut](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Statuts verrouillés et déverrouillés au niveau du système](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Ajouter un fichier PDF à un formulaire personnalisé

Nous vous aidons à rendre les formulaires personnalisés plus visuels et informatifs grâce aux nouveaux widgets de ressources que vous pouvez ajouter, tels que des images et des vidéos. Vous pouvez maintenant ajouter dans un formulaire personnalisé un lien vers un fichier PDF. Lorsque le formulaire est joint à un objet, les personnes qui l’utilisent peuvent afficher le PDF et interagir avec lui depuis le formulaire.

## L’éditeur de calcul de champ de formulaire personnalisé affiche les informations d’erreur.

>[!NOTE]
>
>Cette fonctionnalité est temporairement indisponible. Cette page sera mise à jour lorsque la fonctionnalité sera disponible.

La modification des calculs pour les champs personnalisés est désormais plus facile avec des informations d’erreur utiles indiquées directement dans le calcul. Lorsque vous créez un champ calculé dans un formulaire personnalisé, les erreurs sont surlignées en rose. Lorsque vous pointez sur la partie mise en surbrillance, une info-bulle s’affiche pour décrire le problème.

## Personnalisation de l’en-tête du projet

En tant qu’administrateur ou administratrice Workfront ou de groupes, vous pouvez désormais personnaliser les champs qui s’affichent dans l’en-tête d’un projet lorsque vous utilisez un modèle de mise en page.

Cette mise à jour comprend les améliorations suivantes :

* Supprimez les champs existants de l’en-tête du projet.

* Ajoutez de nouveaux champs de vue d’ensemble du projet non modifiables. Vous ne pouvez pas ajouter de champs personnalisés ou de champs qui peuvent être modifiés. Les champs modifiables qui se trouvent actuellement sur l’en-tête du projet peuvent rester sur l’en-tête.

* L’en-tête de l’objet peut contenir jusqu’à cinq champs.


Avant cette version, les champs des en-têtes d’objet ne pouvaient pas être personnalisés.

Pour plus d’informations, voir [Personnaliser des en-têtes d’objet à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Contrôler la création d’un projet vierge

En tant qu’administrateur ou administratrice système ou de groupes, vous pouvez désormais contrôler le fait que les personnes puissent ou non créer des projets vierges sans utiliser de modèle. Nous avons ajouté un nouveau paramètre dans la zone Préférences du projet de la configuration. Il permet de désactiver la création de projets vierges dans les zones suivantes :

* À partir de l’option Nouveau projet dans une liste de projets

* Lors de la conversion d’un problème en projet à partir de la page des problèmes


Le nouveau paramètre est « Autoriser les personnes à créer des projets sans utiliser de modèle » et est activé par défaut.

**Note :** les utilisateurs et utilisatrices peuvent toujours convertir une tâche en projet vide.

Pour plus d’informations, consultez la section [Configurer des préférences de projet à l’échelle du système](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Désactiver un groupe à partir de la page Groupes

Récemment, nous avons ajouté la possibilité de désactiver et de réactiver les groupes. Pour rendre cette action plus rapide et plus facile, nous l’avons ajoutée à la page des groupes. Désormais, après avoir cliqué sur le nom d’un groupe pour accéder à sa page, vous pouvez sélectionner le menu Plus ![icône du menu principal](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) en regard du nom du groupe, puis sélectionner Désactiver ou Réactiver.

Auparavant, vous ne pouviez désactiver ou réactiver un groupe qu’à l’aide de la case à cocher Est actif sur sa page Détails.

Pour plus d’informations, voir [Désactiver ou réactiver un utilisateur ou une utilisatrice](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Ajouter des vidéos aux formulaires personnalisés

Vous pouvez désormais ajouter un nouvel outil proposant des informations, un intérêt visuel et de la créativité à un formulaire personnalisé à l’aide d’une vidéo. Lorsque le formulaire est joint à un objet, les personnes travaillant avec l’objet peuvent lire la vidéo à tout moment.

Auparavant, vous ne pouviez ajouter que des champs textuels et des images à un formulaire personnalisé.

