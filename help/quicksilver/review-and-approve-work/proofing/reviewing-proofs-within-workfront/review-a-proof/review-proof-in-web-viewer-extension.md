---
product-area: documents
navigation-topic: proofing-overview
title: Vérifier le contenu interactif dans l’extension de la visionneuse de proxy web
description: L’outil de révision d’Adobe Workfront est une extension de navigateur qui vous permet de tester le contenu interactif dans un fichier ZIP ou avec une URL.
author: Courtney
feature: Digital Content and Documents
source-git-commit: 5650ebfbf115908cbf2b89ffeab0551a4ecacc2d
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---


# Vérification du contenu interactif à l’aide de l’outil de révision Adobe Workfront

<span class="preview">L’outil de révision Adobe Workfront sera disponible le 7 novembre 2024. Cette extension est actuellement en version bêta.</span>

L’outil de révision d’Adobe Workfront est une extension de navigateur web qui vous permet de tester le contenu interactif dans un fichier ZIP ou avec une URL. L’outil de révision Adobe Workfront est disponible dans les navigateurs suivants :

* Firefox
* Chrome
* Edge

Pour les sites web qui empêchent l’ouverture de leur site dans des iFrames, tels que Figma, nous vous recommandons d’utiliser la visionneuse de BAT pour ordinateur de bureau.


## Faire de l’outil de révision Adobe Workfront la visionneuse par défaut pour les BAT d’URL et de ZIP

Pour utiliser l’outil de révision web pour les BAT URL et ZIP, un administrateur Workfront doit ajuster le paramètre par défaut pour les BAT interactifs.

1. Dans le menu principal Workfront, cliquez sur **Proofing**.
1. Cliquez sur **Paramètres du compte**, puis sur l’onglet **Paramètres**.
1. Dans la section **BAT - Valeurs par défaut**, recherchez **Visionneuse de vérification de l’appli de bureau pour la vérification interactive** et cliquez sur **Configuration**.
1. Dans le menu déroulant, sélectionnez **Désactivé**. Les bons à tirer interactifs créés à partir d’une URL ou d’un fichier ZIP s’ouvrent désormais automatiquement dans l’outil de révision Adobe Workfront, qui est un navigateur Web.
1. Cliquer sur **Enregistrer**.

>[!NOTE]
>
>Cette modification s’applique à tous les BAT interactifs dans vos environnements d’aperçu et de production. Nous vous recommandons de tester la nouvelle expérience dans votre environnement de prévisualisation avant de l’activer dans l’environnement de production. Vous pouvez facilement revenir à la visionneuse de bureau en redéfinissant le paramètre de compte sur **Activé pour tous les bons à tirer interactifs**.

## Faire de l’outil de révision Adobe Workfront la visionneuse par défaut pour les BAT ZIP uniquement

Pour utiliser l’outil de révision web uniquement pour les BAT ZIP, un administrateur Workfront doit ajuster le paramètre par défaut pour les BAT interactifs.

1. Dans le menu principal Workfront, cliquez sur **Proofing**.
1. Cliquez sur **Paramètres du compte**, puis sur l’onglet **Paramètres**.
1. Dans la section **BAT - Valeurs par défaut**, recherchez **Visionneuse de vérification de l’appli de bureau pour la vérification interactive** et cliquez sur **Configuration**.
1. Dans le menu déroulant, sélectionnez **Activé uniquement pour les BAT interactifs créés à partir d’une URL**. Les bons à tirer interactifs créés à partir d’un fichier ZIP s’ouvrent désormais automatiquement dans l’outil de révision d’Adobe Workfront, qui est un navigateur Web. Les bons à tirer interactifs créés à partir d’une URL restent ouverts dans la visionneuse de vérification de l’appli de bureau.
1. Cliquer sur **Enregistrer**.

>[!NOTE]
>
>Cette modification s’applique à tous les BAT interactifs dans vos environnements d’aperçu et de production. Nous vous recommandons de tester la nouvelle expérience dans votre environnement de prévisualisation avant de l’activer dans l’environnement de production. Vous pouvez facilement revenir à la visionneuse de bureau en redéfinissant le paramètre de compte sur **Activé pour tous les bons à tirer interactifs**.

## Installation de l’extension

Les réviseurs et les approbateurs doivent installer l’outil de révision Adobe Workfront. dans l’un des navigateurs suivants :

* [Extension Firefox](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Extension Chrome](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

Une fois que vous avez installé l’extension, les bons à tirer interactifs s’ouvrent automatiquement dans l’outil de révision Adobe Workfront.

>[!IMPORTANT]
>
>Vous devez supprimer l’extension de visionneuse web héritée pour utiliser l’outil de révision Adobe Workfront.




