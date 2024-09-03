---
title: 22.4 Améliorations pour les administrateurs et administratrices
description: 22.4 Améliorations pour les administrateurs et administratrices
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 0876d4d47aad701d5ffadc88868217ebae7e4790
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 100%

---

# 22.4 Améliorations pour les administrateurs et administratrices

Cette page décrit toutes les améliorations pour les administrateurs et administratrices apportées à l’environnement de prévisualisation dans la version 22.4. Ces améliorations seront disponibles dans la semaine du 3 octobre 2022.

Pour obtenir la liste de toutes les modifications disponibles avec la version 22.4, voir [Vue d’ensemble de la version 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Utiliser des statuts Déverrouillé dans des processus d’approbation

>[!NOTE]
>
>Cette fonctionnalité a été introduite pour la première fois dans l’environnement de prévisualisation lors de la publication de la version 22.3. Elle est sortie en production le 15 septembre 2022.

Pour vous permettre de mieux contrôler les processus et les statuts d’approbation dans votre système, nous avons autorisé la création d’un processus d’approbation basé sur un statut de système déverrouillé. De plus, vous pouvez désormais déverrouiller tout statut déjà utilisé dans un processus d’approbation. Auparavant, un statut système utilisé dans un processus d’approbation devait être verrouillé. Cela le rendait disponible pour tous les groupes, sans possibilité de le supprimer ou de le renommer. Les équipes d’administration de groupe ne pouvaient donc pas rationaliser la liste des statuts de leur groupe en fonction de leurs besoins spécifiques.

## L’icône Plan directeur du menu principal est désormais contrôlée par le biais des modèles de disposition.

L’équipe d’administration système peut désormais ajouter ou supprimer l’icône Plan directeur dans le menu principal via la configuration du modèle de disposition. Il est ainsi plus facile de contrôler les personnes qui peuvent parcourir le catalogue de plans directeurs.

L’icône Plan directeur apparaît dans le menu principal lorsque :

* Aucun modèle de disposition n’est affecté à l’utilisateur ou à l’utilisatrice.

* Le modèle de disposition de l’utilisateur ou de l’utilisatrice dispose de l’option Plan directeur dans la liste des éléments actifs.

* Le modèle de disposition de l’utilisateur ou de l’utilisatrice contient l’option Plan directeur dans la liste Éléments disponibles ; l’icône n’apparaît pas dans le menu principal.

Les modèles de disposition existants incluent automatiquement l’icône Plan directeur, et les équipes d’administration peuvent supprimer l’icône des modèles de disposition pour limiter la visibilité du catalogue de plans directeurs. Les modèles de disposition créés après la version 22.4 incluront l’icône Plan directeur dans la liste des éléments actifs.

Pour plus d’informations, voir la section [Configurer l’accès aux plans directeurs](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Personnalisation de l’en-tête du problème

En tant qu’administrateur ou administratrice Workfront ou de groupes, vous pouvez désormais personnaliser les champs qui s’affichent dans l’en-tête d’un problème lorsque vous utilisez un modèle de disposition.

Cette mise à jour comprend les améliorations suivantes :

* Supprimez ou réorganisez les champs existants de l’en-tête du problème.

* Ajoutez de nouveaux champs non modifiables de la vue d’ensemble des problèmes. Vous ne pouvez pas ajouter de champs personnalisés ou de champs qui peuvent être modifiés. Vous pouvez également afficher les champs modifiables qui se trouvent actuellement dans l’en-tête du problème (par exemple, Statut ou Pourcentage terminé).

* L’en-tête du problème peut contenir jusqu’à cinq champs.

* Vous pouvez maintenant ajouter le champ « Résolu par » à l’en-tête du problème. Lorsqu’un objet de résolution est associé au problème, le champ « Résolu par » passe à « Résolution du problème », « Résolution de la tâche » ou « Résolution du projet », selon le type d’objet associé au problème.

Avant cette version, seuls les en-têtes de projet et de tâche pouvaient être personnalisés.



Pour plus d’informations, voir la section [Personnaliser des en-têtes d’objet à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Personnalisation de l’en-tête de tâche

En tant qu’administrateur ou administratrice de Workfront ou de groupes, vous pouvez désormais personnaliser les champs qui s’affichent dans l’en-tête d’une tâche lorsque vous utilisez un modèle de mise en page.

Cette mise à jour comprend les améliorations suivantes :

* Supprimez ou réorganisez les champs existants à partir de l’en-tête de la tâche.

* Ajoutez de nouveaux champs non modifiables de vue d’ensemble de la tâche. Vous ne pouvez pas ajouter de champs personnalisés ou de champs qui peuvent être modifiés. Vous pouvez également afficher les champs modifiables qui se trouvent actuellement dans l’en-tête de la tâche (par exemple, Statut ou Pourcentage terminé).

* L’en-tête de la tâche peut contenir jusqu’à cinq champs.

Avant cette version, seuls les en-têtes de projet pouvaient être personnalisés.

Pour plus d’informations, voir la section [Personnaliser des en-têtes d’objet à l’aide d’un modèle de disposition](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Afficher une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Inclusion anticipée des dernières fonctionnalités sur les panoramas

Nous sommes ravis d’ouvrir de nouvelles fonctionnalités de panoramas pour l’inclusion préalable des fonctionnalités. Cette option n’est pas disponible pour toutes les organisations.

Seulement un administrateur ou une administratrice Workfront peut activer les fonctionnalités anticipées. Lorsque l’administrateur ou l’administratrice active les fonctionnalités anticipées, les personnes appartenant à l’entreprise peuvent en bénéficier et les fonctionnalités supplémentaires sont activées dans votre environnement de production Workfront.

Pour plus d’informations, voir [Activation des fonctionnalités anticipées pour les panoramas Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## L’éditeur de calcul de champ de formulaire personnalisé affiche les informations d’erreur.

>[!NOTE]
>
>Cette fonctionnalité a été introduite pour la première fois dans l’environnement de prévisualisation lors de la publication de la version 22.3. Elle est publiée en production avec la version 22.4.

La modification des calculs pour les champs personnalisés est désormais plus facile avec des informations d’erreur utiles indiquées directement dans le calcul. Lorsque vous créez un champ calculé dans un formulaire personnalisé, les erreurs sont surlignées en rose. Lorsque vous pointez sur la partie mise en surbrillance, une info-bulle s’affiche pour décrire le problème.

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migration vers Adobe Unified Experience

NOTE : cette migration a été reportée au 1er et 2e trimestre 2023. Toutes les personnes concernées seront alors averties.

Si votre organisation a été intégrée à Adobe Admin Console, votre instance Workfront sera migrée vers Adobe Unified Experience avec la version 22.4.

Adobe Unified Experience comprend :

* Une seule connexion pour toutes les applications Adobe via Adobe Experience Cloud.

* Un sélecteur d’organisation à déplacer entre les organisations et les environnements Workfront.

* Une navigation avec options pour les pages Workfront, les préférences Adobe Experience Cloud et votre profil Workfront.

Pour plus d’informations, voir [Adobe Unified Experience pour Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Affichez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412388/){target=_blank}
