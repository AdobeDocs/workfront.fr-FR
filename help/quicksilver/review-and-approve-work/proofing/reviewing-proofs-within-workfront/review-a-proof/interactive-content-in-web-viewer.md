---
product-area: documents
navigation-topic: review-a-proof
title: Configuration de la vérification de contenu interactif dans la visionneuse de Web Proofing
description: Nous vous recommandons de consulter tout le contenu interactif à l’aide de la visionneuse de vérification de l’appli de bureau. Toutefois, si les politiques de votre entreprise l’empêchent, votre administrateur Workfront peut configurer votre système pour utiliser la visionneuse de Web Proofing (Web Proofing Viewer) à des fins de vérification interactive. Pour obtenir des informations comparatives sur ces deux visionneuses, reportez-vous à la section Différences entre la visionneuse de test Web et la visionneuse de test de bureau .
author: Courtney
feature: Digital Content and Documents
exl-id: daddc225-62df-4e1a-98fd-8bb7c7c5553b
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Configuration de la vérification de contenu interactif dans la visionneuse de Web Proofing

Nous vous recommandons de consulter tout le contenu interactif à l’aide de la visionneuse de vérification de l’appli de bureau. Toutefois, si les politiques de votre entreprise l’empêchent, votre administrateur Workfront peut configurer votre système pour utiliser la visionneuse de Web Proofing (Web Proofing Viewer) à des fins de vérification interactive. Pour obtenir des informations comparatives sur ces deux visionneuses, voir [Présentation des différences entre la visionneuse de test Web et la visionneuse de test de bureau](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

Une fois que l’administrateur de Workfront a configuré votre système pour la vérification de l’intégrité interactive dans la visionneuse Web Proofing, vous devez télécharger une extension afin d’ajouter des commentaires et des balises aux bons à tirer interactifs :

## Limites

La visionneuse de test Web présente les limites suivantes :

* Ne prend pas en charge les BAT d’URL (ne prend en charge que les fichiers d’archive ZIP).
* Ne prend pas en charge Safari et Internet Explorer.
* N’émule pas le contenu à l’aide des spécifications de l’interface sur les appareils mobiles, telles que la couleur des boutons, mais permet d’afficher le contenu interactif tel qu’il apparaît dans les résolutions des différents appareils.

>[!IMPORTANT]
>
>Vous devez installer le module externe de navigateur hérité pour ajouter des commentaires aux bons à tirer interactifs dans la visionneuse de test Web. Ce module externe n’est disponible que dans Firefox dans la variable [Magasin de modules complémentaires Firefox](https://addons.mozilla.org/en-US/firefox/addon/proofhq-rich-media-review/).

## Configuration de la vérification de contenu interactif dans la visionneuse de Web Proofing

1. Ouvrez un BAT créé à partir d’un fichier ZIP contenant du contenu interactif.

   Pour plus d’informations, voir [A propos de la préparation de contenu interactif dans un fichier ZIP pour la vérification](../../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) in [BAT de contenu interactif - Aperçu](../../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

   Voir aussi [Création d’un BAT pour le contenu interactif dans un fichier ZIP](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md).

1. Cliquez sur **Ajouter un commentaire**.

   Un message vous invite à télécharger l’extension de navigateur pour le contenu interactif.

1. Cliquez sur **Ajouter au navigateur** pour accéder à la page de téléchargement de l’extension dans la boutique de votre navigateur, puis téléchargez l’extension.
1. Dans la visionneuse Web Proofing, cliquez sur **Recharger le BAT**.

Une fois l’extension installée sur votre navigateur, la visionneuse de correctifs effectue une capture d’écran statique de votre contenu chaque fois que vous cliquez sur . **Ajouter un commentaire**. Cette capture d’écran vous permet d’ajouter des commentaires avec des annotations.

 
