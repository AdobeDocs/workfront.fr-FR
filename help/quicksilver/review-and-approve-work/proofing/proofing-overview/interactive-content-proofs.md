---
product-area: documents
navigation-topic: proofing-overview
title: Vue d’ensemble des épreuves de contenu interactif
description: Le contenu interactif fournit plusieurs méthodes pour interagir avec les spectateurs et spectatrices. Les agences peuvent mesurer le succès de leurs campagnes à l’aide des analyses collectées à partir des réponses à ce contenu.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 100%

---

# Vue d’ensemble des épreuves de contenu interactif

<!-- Audited: 01/2024 -->

Le contenu interactif fournit plusieurs méthodes pour interagir avec les spectateurs et spectatrices. Les agences peuvent mesurer le succès de leurs campagnes à l’aide des analyses collectées à partir des réponses à ce contenu.

Voici quelques exemples de contenu interactif :

* Sites web
* Vidéos incorporées ou en streaming
* Bannières interactives
* Animations HTML5
* Microsites
* E-mails interactifs

## À propos de la création d’épreuves pour le contenu interactif

Vous pouvez créer une épreuve pour le contenu interactif de l’une des manières suivantes :

* Créez une épreuve à partir d’un fichier ZIP contenant le contenu interactif.

  Adobe Workfront décompresse le contenu du fichier ZIP et le stocke sur un serveur Workfront. Ces conditions de stockage vous assurent que le contenu n’est pas altéré au cours du cycle de révision de l’épreuve.

* Spécifiez l’URL du contenu.

  Il s’agit de la méthode la plus simple pour créer une épreuve pour le contenu interactif. Il s’agit également de la seule manière pour réviser votre contenu de manière interactive, à mesure que les utilisateurs et les utilisatrices le visualisent sur Internet.

  Avec cette approche, un serveur externe inconnu pour Workfront stocke et héberge le contenu.

  Nous vous recommandons cette méthode pour les sites web volumineux, car il est difficile d’en rassembler tous les fichiers. Cependant, comme le contenu de l’épreuve est stocké en externe, Workfront ne peut pas le protéger des modifications apportées par les développeurs et les développeuses qui y travaillent. Il se peut donc que vous ne puissiez pas vous fier au fait que le contenu reste le même tout au long du cycle de révision de l’épreuve.

## À propos de la préparation de contenu interactif dans un fichier ZIP en vue de la relecture

Lorsque vous regroupez du contenu interactif dans un fichier ZIP à des fins de relecture, assurez-vous qu’il comprend les spécifications suivantes :

* Toutes les ressources, telles que CSS, JavaScript, vidéos, sons et images, doivent être incluses dans le fichier de lot.
* Le contenu interactif doit inclure le fichier principal (index.html, index.htm). Si ce fichier n’est pas placé à l’emplacement racine, l’outil recherche automatiquement le dossier pour le trouver.Le fichier principal n’a pas besoin d’être nommé index.html/index.htm, cependant, un seul fichier .html/.htm peut être placé à l’emplacement principal.
* Le fichier doit contenir au moins une page web de fichier statique.
* La taille maximale du fichier est de 500 Mo.
* Dans le cas de fichiers .zip créés dans iOS, l’outil identifie automatiquement le dossier dans lequel se trouve le contenu.
* Les projets interactifs sont pris en charge uniquement en tant qu’archives .zip. Les envois de fichiers .zip standard échoueront.
* Le site web doit être sécurisé (HTTPS).

  Il ne s’agit pas d’une exigence pour utiliser la visionneuse de relecture de bureau.

  Pour plus d’informations, consultez [Comprendre la visionneuse de relecture de bureau](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* Le site web doit être autorisé à être affiché dans un iframe.

  Il ne s’agit pas d’une exigence pour utiliser la visionneuse de relecture de bureau.

  Pour plus d’informations, consultez [Comprendre la visionneuse de relecture de bureau](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## À propos de la création d’une épreuve interactive

Une fois que vous avez préparé votre fichier de lot ZIP, créez une épreuve interactive.

Pour plus d’informations, consultez [Créer une épreuve pour le contenu interactif dans un fichier ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md).

Ou, si vous utilisez Workfront Proof, reportez-vous à la section [Générer une épreuve pour le contenu interactif](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) dans l’article [Générer des épreuves dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## À propos de la révision des épreuves interactives

Nous vous recommandons d’utiliser la visionneuse de relecture de bureau autonome comme visionneuse par défaut pour les épreuves interactives.Toutefois, si les politiques de votre entreprise n’autorisent pas l’utilisation de la visionneuse de relecture de bureau, votre administrateur ou administratrice Workfront peut configurer votre système afin que vous puissiez consulter le contenu interactif, regroupé dans un fichier de lot ZIP, dans la visionneuse de relecture web. Pour obtenir des informations comparatives sur la visionneuse de relecture de bureau et la visionneuse de relecture web, consultez [Vue d’ensemble des différences entre la visionneuse de relecture web et la visionneuse de relecture de bureau](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
