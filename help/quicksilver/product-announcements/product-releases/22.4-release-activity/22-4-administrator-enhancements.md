---
title: Améliorations apportées à l’administration (version 22.4)
description: Améliorations apportées à l’administration (version 22.4)
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 0876d4d47aad701d5ffadc88868217ebae7e4790
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 7%

---

# Améliorations apportées à l’administration (version 22.4)

Cette page décrit toutes les améliorations apportées par l’administrateur à la version 22.4 de l’environnement Aperçu. Ces améliorations seront disponibles la semaine du 3 octobre 2022.

Pour obtenir la liste de toutes les modifications disponibles avec la version 22.4, consultez la [présentation de la version 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Utiliser des états déverrouillés dans un processus de validation

>[!NOTE]
>
>Cette fonctionnalité a été introduite pour la première fois dans l’environnement Aperçu au cours de la période de publication de la version 22.3. Il est publié en production le 15 septembre 2022.

Pour vous permettre de mieux contrôler les processus et les états de validation dans votre système, nous avons rendu possible la création d&#39;un processus de validation basé sur un état système déverrouillé. De plus, vous pouvez désormais déverrouiller tout statut déjà utilisé dans un processus de validation. Auparavant, un état système utilisé dans un processus de validation devait être verrouillé. Cela l’a rendu disponible pour tous les groupes, sans possibilité de le supprimer ou de le renommer, de sorte que les administrateurs de groupes ne puissent pas rationaliser la liste des états de leur groupe en fonction de leurs besoins spécifiques.

## L’icône Plan directeur du menu principal est désormais contrôlée par le biais des modèles de mise en page.

Les administrateurs système peuvent désormais ajouter ou supprimer l’icône Plan directeur dans le menu principal via la configuration du modèle de mise en page. Cela permet de mieux contrôler qui peut parcourir le catalogue de plans directeurs.

L’icône Plan directeur apparaît dans le menu principal lorsque :

* Aucun modèle de mise en page n’est affecté à l’utilisateur.

* Le modèle de disposition de l’utilisateur dispose de l’option Plan directeur dans la liste des éléments actifs.

* Le modèle de mise en page de l’utilisateur dispose de l’option Plan directeur dans la liste Éléments disponibles ; l’icône n’apparaît pas dans le menu principal.

Les modèles de mise en page existants incluent automatiquement l’icône Plan directeur, et les administrateurs peuvent supprimer l’icône des modèles de mise en page pour limiter la visibilité du catalogue de plans directeurs. Les nouveaux modèles de mise en page créés après la version 22.4 incluront l’icône Plan directeur dans la liste des éléments actifs.

Pour plus d’informations, voir [Configuration de l’accès aux plans directeurs](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Voir une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Personnalisation de l’en-tête du problème

En tant qu’administrateur Workfront ou de groupe, vous pouvez désormais personnaliser les champs qui s’affichent dans l’en-tête d’un problème lorsque vous utilisez un modèle de mise en page.

Cette mise à jour comprend les améliorations suivantes :

* Supprimez ou réorganisez les champs existants de l’en-tête du problème.

* Ajoutez de nouveaux champs de présentation des problèmes non modifiables. Vous ne pouvez pas ajouter de champs personnalisés ou de champs qui peuvent être modifiés. Vous pouvez également afficher les champs modifiables qui se trouvent actuellement dans l’en-tête du problème (par exemple, État ou Pourcentage terminé).

* L’en-tête de problème peut contenir jusqu’à cinq champs.

* Vous pouvez maintenant ajouter le champ &quot;Résolu par&quot; à l’en-tête du problème. Lorsqu’un objet de résolution est associé au problème, le champ &quot;Résolu par&quot; passe à &quot;Résolution du problème&quot;, &quot;Résolution de la tâche&quot; ou &quot;Résolution du projet&quot;, selon le type d’objet associé au problème.

Avant cette version, seuls les en-têtes de projet et de tâche pouvaient être personnalisés.



Pour plus d’informations, consultez la section [Personnaliser les en-têtes d’objet à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Voir une démonstration vidéo de cette fonctionnalité](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Personnalisation de l’en-tête de tâche

En tant qu’administrateur Workfront ou de groupe, vous pouvez désormais personnaliser les champs qui s’affichent dans l’en-tête d’une tâche lorsque vous utilisez un modèle de mise en page.

Cette mise à jour comprend les améliorations suivantes :

* Supprimez ou réorganisez les champs existants de l’en-tête de la tâche.

* Ajoutez de nouveaux champs non modifiables Présentation de la tâche . Vous ne pouvez pas ajouter de champs personnalisés ou de champs qui peuvent être modifiés. Vous pouvez également afficher les champs modifiables qui se trouvent actuellement dans l’en-tête de la tâche (par exemple, État ou Pourcentage terminé).

* L’en-tête de la tâche peut contenir jusqu’à cinq champs.

Avant cette version, seuls les en-têtes de projet pouvaient être personnalisés.

Pour plus d’informations, voir [Personnalisation des en-têtes d’objet à l’aide d’un modèle de mise en page](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Regardez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Inclusion anticipée des dernières fonctionnalités sur les panoramas

Nous sommes ravis d’ouvrir de nouvelles fonctionnalités de panoramas pour l’accord préalable des fonctionnalités. Cet outil facultatif est disponible pour toutes les organisations.

Seul un administrateur Workfront peut souscrire aux premières fonctionnalités. Lorsque l’administrateur choisit de se connecter aux nouvelles fonctionnalités, tous les utilisateurs de l’entreprise y sont inscrits et les fonctionnalités supplémentaires sont activées dans votre environnement Workfront de production.

Pour plus d’informations, reportez-vous à la section [Fonctionnalité d’opt-in anticipée pour les panoramas Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Regardez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## L’éditeur de calcul de champ de formulaire personnalisé affiche les informations d’erreur

>[!NOTE]
>
>Cette fonctionnalité a été introduite pour la première fois dans l’environnement Aperçu au cours de la période de publication de la version 22.3. Il est publié en production avec la version 22.4.

La modification des calculs pour les champs personnalisés est désormais plus facile avec des informations d’erreur utiles indiquées directement dans le calcul. Lorsque vous créez un champ calculé dans un formulaire personnalisé, les erreurs sont surlignées en rose. Lorsque vous passez le curseur sur la partie mise en surbrillance, une info-bulle s’affiche pour décrire le problème.

[Regardez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migration vers l’Adobe d’une expérience unifiée

REMARQUE : Cette migration a été reportée au 1er et 2e trimestre de 2023. Tous les clients concernés seront alors avertis.

Si votre organisation a été intégrée à Adobe Admin Console, votre instance Workfront sera migrée vers l’Adobe Expérience unifiée avec la version 22.4.

L’expérience unifiée Adobe comprend :

* Une seule connexion pour toutes les applications Adobe via Adobe Experience Cloud

* Sélecteur d’organisation à déplacer entre les organisations et les environnements Workfront

* Navigation avec options pour les pages Workfront, les préférences Adobe Experience Cloud et votre profil Workfront

Pour plus d’informations, voir [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Regardez une démonstration vidéo de cette fonctionnalité.](https://video.tv.adobe.com/v/3412388/){target=_blank}
