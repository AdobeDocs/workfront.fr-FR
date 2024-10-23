---
product-area: documents
navigation-topic: proofing-overview
title: Vérifier le contenu interactif dans l’extension de la visionneuse de proxy web
description: L’outil de révision d’Adobe Workfront est une extension de navigateur qui vous permet de tester le contenu interactif dans un fichier ZIP ou avec une URL.
author: Courtney
feature: Digital Content and Documents
source-git-commit: def2526e2e1bb83998f0adc221b3011c471f72f8
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 1%

---


# Vérification du contenu interactif à l’aide de l’outil de révision Adobe Workfront

<span class="preview">L’outil de révision Adobe Workfront sera disponible le 1er novembre 2024.</span>

L’outil de révision d’Adobe Workfront est une extension de navigateur qui vous permet de tester le contenu interactif dans un fichier ZIP ou avec une URL. L’outil de révision Adobe Workfront est disponible dans les navigateurs suivants :

* Firefox
* Chrome
* Edge

Pour les sites web qui empêchent l’ouverture de leur site dans des iFrames, tels que Figma, nous vous recommandons d’utiliser la visionneuse de BAT pour ordinateur de bureau.

## Conditions préalables

Pour utiliser l’outil de révision web, un administrateur Workfront doit désactiver le paramètre qui ouvre automatiquement la visionneuse de vérification de l’appli de bureau pour le contenu interactif :

1. Dans le menu principal Workfront, cliquez sur **Proofing**.
1. Cliquez sur **Paramètres du compte**, puis sur l’onglet **Paramètres**.
1. Dans la section **BAT - Valeurs par défaut**, recherchez **Visionneuse de vérification de l’appli de bureau pour la vérification interactive** et cliquez sur **Configuration**.
1. Dans le menu déroulant, sélectionnez **Désactivé**.
1. Cliquer sur **Enregistrer**.

>[!IMPORTANT]
>
>Cette modification s’applique à tous les BAT interactifs dans vos environnements d’aperçu et de production. Nous vous recommandons de tester la nouvelle expérience dans votre environnement de prévisualisation avant de l’activer dans l’environnement de production. Vous pouvez facilement revenir à la visionneuse de bureau en redéfinissant le paramètre de compte sur **Activé pour tous les BAT interactifs** ou **Activé uniquement pour les BAT interactifs créés à partir d’une URL**.


## Installation de l’extension

Les réviseurs et les approbateurs doivent installer la révision Adobe Workfront dans l’un des navigateurs suivants :

* [Extension Firefox](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Extension Chrome](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)

Une fois que vous avez installé l’extension, les bons à tirer interactifs s’ouvrent automatiquement dans l’outil de révision Adobe Workfront.


Pour utiliser l’outil de révision Workfront, le paramètre permettant d’ouvrir la visionneuse de vérification de l’appli de bureau pour la vérification interactive doit être désactivé. Pour plus d’informations sur la désactivation de ce paramètre, voir la section [Conditions préalables](#prerequisites) ci-dessus.



