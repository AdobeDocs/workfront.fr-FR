---
product-area: documents
navigation-topic: proofing-overview
title: Vérifier le contenu interactif dans l’extension du lecteur de vérification Web
description: L’outil de révision Adobe Workfront est une extension de navigateur qui vous permet de corriger le contenu interactif dans un fichier ZIP ou avec une URL.
author: Courtney
feature: Digital Content and Documents
exl-id: 4fea13cc-2d56-466e-8851-6134782e7e80
source-git-commit: 7b02d5670ebba1456e37e6fd815e7812ec06def2
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---

# Révision de contenu interactif avec l’outil de révision Adobe Workfront

<span class="preview">L’outil de révision Adobe Workfront sera disponible le 7 novembre 2024. Cette extension est actuellement en version bêta.</span>

L’outil de révision Adobe Workfront est une extension de navigateur web qui vous permet de corriger le contenu interactif dans un fichier ZIP ou avec une URL. L’outil de révision Adobe Workfront est disponible dans les navigateurs suivants :

* Firefox
* Chrome
* Edge
* Safari

Nous vous recommandons d’utiliser le lecteur de vérification pour bureau si le contenu que vous devez réviser se trouve sur un site web qui :

* Nécessite une authentification SSO
* Empêche l&#39;ouverture de leur site dans des iFrames, comme Figma


## Installation de l’extension

### Conditions préalables

* Vous devez supprimer l’ancienne extension Visionneuse web pour utiliser l’outil Adobe Workfront Review.

### Installation de l’extension

<!--This extension is required to review conent in GS and Ex.

You must install the extension to reiew content in GenS and Express.

To review content in GS, Express, or Wou must install the extension if you are using GenStuido or Creative cloud express-->

Les réviseurs et approbateurs doivent installer l’outil de révision Adobe Workfront. dans l’un des navigateurs suivants :

* [Extension Firefox ](https://addons.mozilla.org/en-US/firefox/addon/adobe-workfront-review-tool/)

* [Extension Chrome](https://chromewebstore.google.com/detail/adobe-workfront-review-to/lhdepbgeilldghlfnankdnponhljpgml)

* [Edge](https://microsoftedge.microsoft.com/addons/detail/adobe-workfront-review-to/llhapmaiiddmcamgeapaipjpagnoijen)


Pour que les épreuves interactives s’ouvrent automatiquement dans l’outil de révision Adobe Workfront, un administrateur Workfront doit mettre à jour les paramètres de relecture dans Workfront, comme décrit dans les sections ci-dessous.

## Mettre à jour les paramètres de vérification par défaut de Workfront

### Faire de l’outil de révision Adobe Workfront la visionneuse par défaut pour les épreuves d’URL et de compression

Pour utiliser l’outil de révision web pour les épreuves d’URL et de compression, un administrateur Workfront doit ajuster le paramètre par défaut des épreuves interactives.

1. Dans le menu principal de Workfront, cliquez sur **Vérification**.
1. Cliquez sur **Paramètres du compte**, puis sur l’onglet **Paramètres**.
1. Dans la section **Valeurs par défaut de l’épreuve**, recherchez **Lecteur de vérification pour bureau pour la vérification interactive** et cliquez sur **Configurer**.
1. Dans le menu déroulant, choisissez **Désactivé**. Les épreuves interactives créées à partir d’une URL ou d’un fichier ZIP s’ouvrent désormais automatiquement dans l’outil Adobe Workfront Review, un navigateur web.
1. Cliquer sur **Enregistrer**.

>[!NOTE]
>
>Cette modification s’applique à toutes les épreuves interactives de votre instance Workfront. Nous vous recommandons de tester la nouvelle expérience dans votre environnement de prévisualisation avant de l’activer dans l’environnement de production. Vous pouvez facilement revenir à la visionneuse pour bureau en redéfinissant le paramètre de compte **Visionneuse de relecture pour bureau pour la relecture interactive** sur **Activé pour toutes les épreuves interactives**.

### Faire de l’outil de révision Adobe Workfront la visionneuse par défaut pour les épreuves ZIP uniquement

Pour utiliser l’outil de révision web pour les épreuves ZIP uniquement, un administrateur Workfront doit ajuster le paramètre par défaut pour les épreuves interactives.

1. Dans le menu principal de Workfront, cliquez sur **Vérification**.
1. Cliquez sur **Paramètres du compte**, puis sur l’onglet **Paramètres**.
1. Dans la section **Valeurs par défaut de l’épreuve**, recherchez **Lecteur de vérification pour bureau pour la vérification interactive** et cliquez sur **Configurer**.
1. Dans le menu déroulant, choisissez **Activé uniquement pour les BAT interactifs créés à partir d’une URL**. Les épreuves interactives créées à partir d’un fichier ZIP s’ouvrent désormais automatiquement dans l’outil Adobe Workfront Review, un navigateur web. Les épreuves interactives créées à partir d’une URL restent ouvertes dans le lecteur de vérification pour bureau.
1. Cliquer sur **Enregistrer**.

>[!NOTE]
>
>Cette modification s’applique à toutes les épreuves ZIP de votre instance Workfront. Nous vous recommandons de tester la nouvelle expérience dans votre environnement de prévisualisation avant de l’activer dans l’environnement de production. Vous pouvez facilement revenir à la visionneuse pour bureau en redéfinissant le paramètre de compte **Visionneuse de relecture pour bureau pour la relecture interactive** sur **Activé pour toutes les épreuves interactives**.



