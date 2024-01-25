---
product-area: documents
navigation-topic: proofing-overview
title: BAT de contenu interactif - Aperçu
description: Le contenu interactif fournit plusieurs méthodes pour interagir avec les visionneuses. Les agences peuvent mesurer le succès de leurs campagnes à l’aide des analyses collectées à partir des réponses à ce contenu.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 45dac4c5e8ff584546783d561c04d137697a03a4
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# BAT de contenu interactif - Aperçu

<!-- Audited: 01/2024 -->

Le contenu interactif fournit plusieurs méthodes pour interagir avec les visionneuses. Les agences peuvent mesurer le succès de leurs campagnes à l’aide des analyses collectées à partir des réponses à ce contenu.

Voici quelques exemples de contenu interactif :

* Sites web
* Vidéos incorporées ou en flux continu
* Bannières interactives
* animations HTML5
* Microsites
* Emails interactifs

## A propos de la création de BAT pour le contenu interactif

Vous pouvez créer un BAT pour le contenu interactif de l’une des manières suivantes :

* Créez un BAT à partir d’un fichier ZIP contenant le contenu interactif.

  Adobe Workfront décompresse le contenu du fichier ZIP et le stocke sur un serveur Workfront. Comme il est stocké de cette manière, vous pouvez vous fier au fait que le contenu reste le même tout au long du cycle de révision du BAT.

* Spécifiez l’URL du contenu.

  Il s’agit de la méthode la plus simple pour créer un BAT pour le contenu interactif. Il s’agit également de la seule manière dont vous pouvez passer en revue votre contenu de manière interactive, à mesure que les utilisateurs le visualisent sur Internet.

  Avec cette approche, un serveur externe inconnu pour Workfront stocke et héberge le contenu.

  Nous vous recommandons cette méthode pour les sites web volumineux, car il est difficile de rassembler tous les fichiers qui constituent un site web volumineux. Cependant, comme le contenu du BAT est stocké en externe, Workfront ne peut pas le protéger des modifications apportées par les développeurs qui y travaillent. Il se peut donc que vous ne puissiez pas vous fier au fait que le contenu reste le même tout au long du cycle de révision du BAT.

## A propos de la préparation de contenu interactif dans un fichier ZIP pour la vérification

Lorsque vous regroupez du contenu interactif dans un fichier ZIP à des fins de vérification, assurez-vous qu’il comprend les spécifications suivantes :

* Toutes les ressources, telles que CSS, JavaScript, vidéos, sons et images, doivent être incluses dans le fichier de bundle.
* Le contenu interactif doit inclure le fichier principal (index.html, index.htm). Si ce fichier n’est pas placé à l’emplacement racine, l’outil recherche automatiquement le dossier pour le trouver. Le fichier principal n&#39;a pas besoin d&#39;être nommé index.html/index.htm, cependant, un seul fichier .html/.htm peut être placé à l&#39;emplacement principal.
* Le fichier doit contenir au moins une page web de fichier statique.
* La taille maximale du lot est de 500 Mo.
* Dans le cas de fichiers .zip créés dans iOS, l’outil identifie automatiquement le dossier dans lequel se trouve le contenu.
* Les projets interactifs sont pris en charge uniquement en tant qu’archives .zip. Les envois de fichiers .zip standard échoueront.
* Le site web doit être sécurisé (HTTPS).

  Il ne s’agit pas d’une exigence lors de l’utilisation de la visionneuse de vérification de l’appli de bureau.

  Pour plus d’informations, voir [Présentation de la visionneuse de vérification de l’appli de bureau](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* Le site web doit être autorisé à être affiché dans un iframe.

  Il ne s’agit pas d’une exigence lors de l’utilisation de la visionneuse de vérification de l’appli de bureau.

  Pour plus d’informations, voir [Présentation de la visionneuse de vérification de l’appli de bureau](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## A propos de la création d’un BAT interactif

Une fois que vous avez préparé votre fichier de bundle ZIP, créez un BAT interactif.

Pour plus d’informations, voir [Création d’un BAT pour le contenu interactif dans un fichier ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

Ou, si vous utilisez le Bon à tirer Workfront, reportez-vous à la section [Générer un BAT pour le contenu interactif](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) dans l’article [Générer un bon à tirer dans le bon à tirer Workfront](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## A propos de la révision des BAT interactifs

Nous vous recommandons d’utiliser la visionneuse de vérification de l’appli de bureau autonome comme visionneuse par défaut pour les bons à tirer interactifs. Toutefois, si les politiques de votre entreprise n’autorisent pas l’utilisation de l’application de visionneuse de vérification de l’appli de bureau, votre administrateur Workfront peut configurer votre système afin que vous puissiez consulter le contenu interactif, regroupé dans un fichier d’archive ZIP, dans la visionneuse de vérification de l’efficacité du web. Pour obtenir des informations comparatives sur la visionneuse de vérification de l’appli de bureau et la visionneuse de vérification de l’application Web, voir [Présentation des différences entre la visionneuse de test Web et la visionneuse de test de bureau](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
