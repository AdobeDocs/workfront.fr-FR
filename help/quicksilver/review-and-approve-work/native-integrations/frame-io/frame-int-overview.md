---
product-area: documents
navigation-topic: approvals
title: Présentation de l’intégration Frame.io
description: Présentation de l’intégration Frame.io
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 701f3fc2c885363b5f61fb9d77049c7d4c41963d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 1%

---


# Présentation de l’intégration Frame.io

L’intégration de Workfront et Frame.io permet aux coordinateurs de projet de gérer les projets et de planifier le travail dans Workfront, tandis que les créatifs, les spécialistes marketing et les parties prenantes peuvent examiner et approuver les ressources dans Frame.io.

## Basé sur la gestion du stockage d’entreprise Adobe

Au cœur de cette intégration se trouve Adobe Enterprise Storage Management (ESM), une solution de stockage dans le cloud qui sert de référentiel central pour les ressources de l’ensemble des produits d’entreprise Adobe, y compris Workfront et Frame.io.

Les principaux avantages de la gestion du stockage d’entreprise d’Adobe sont les suivants :

* Couche de stockage unifiée pour les ressources de création et de gestion de travail
* Autorisations centralisées via Adobe IMS pour un contrôle d’accès sécurisé
* Visibilité de bout en bout des ressources sur les <!--coming soon?--> d’applications Workfront, Frame.io et Creative Cloud
* Stockage évolutif et gestion des quotas pour les besoins de l&#39;entreprise

Pour plus d’informations, consultez [Présentation de la gestion du stockage d’entreprise d’Adobe](help/quicksilver/review-and-approve-work/esm-overview.md).

## Révision et approbation unifiées

L’intégration de Workfront et Frame.io utilise la fonctionnalité d’approbation unifiée de Workfront pour gérer les révisions et les approbations. Avec les validations unifiées, vous pouvez :

* Créer et gérer des révisions et des approbations directement depuis Workfront
* Suivre le statut des révisions et des validations en temps réel
* Centraliser les commentaires et les approbations au même endroit
* Vérifiez que toutes les parties prenantes ont accès aux dernières versions des ressources
* Utiliser les réviseurs d’IA pour automatiser les révisions de conformité de la marque
* et plus...

Pour plus d’informations, voir [Approbations de documents unifiés : index des articles](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Utilisation de la visionneuse Frame.io

L&#39;intégration se connecte également à la visionneuse Frame.io. La visionneuse Frame.io fournit

* Outils de balisage et de commentaires
* Historique et comparaison des versions
* Commentaires horodatés pour les révisions vidéo
* Accès mobile pour les révisions et les approbations en cours de route

Pour plus d’informations, voir [Prise en main de l’intégration Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Limites des révisions vidéo

<!--need to confirm these-->

#### Types de fichiers pris en charge dans la visionneuse Frame.io

La visionneuse Frame.io prend en charge tous les types courants de vidéos, d’images, d’audio, de PDF et de MS® Office. Pour obtenir la liste détaillée des fichiers pris en charge, voir [Types sur Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Accès et licences pour la visionneuse Frame.io

La visionneuse Frame.io est disponible pour tous les utilisateurs de Workfront disposant d’une licence payante. Aucune licence Frame.io supplémentaire n&#39;est requise pour utiliser la visionneuse Frame.io pour les révisions et les approbations avec cette intégration.

Si votre entreprise souhaite tirer parti de fonctionnalités Frame.io supplémentaires, telles que le chargement direct de ressources vers des projets dans Frame.io, vous pouvez acheter une licence d’entreprise Frame.io. <!--link to Frame.io enterprise license info or who to contacT?-->

La fonctionnalité de relecture de Workfront n&#39;est pas disponible avec cette intégration.

## Gestion de projet puissante dans Workfront

Grâce à l’intégration de Workfront et Frame.io, les coordinateurs de projet peuvent tirer parti des puissantes fonctionnalités de gestion de projet de Workfront pour planifier, suivre et gérer le travail.

Pour plus d’informations sur la gestion des projets dans Workfront, voir [Projets : index d’article](/help/quicksilver/manage-work/projects/projects-toc.md).

### Structure appliquée et conventions de nommage

Comme cette intégration est créée à l’aide d’ESM, il existe une structure appliquée et des conventions de nommage à connaître lors de la gestion des projets et des documents.

* Les noms d’objet doivent être uniques et ne peuvent pas être dupliqués
* ESM requiert des noms uniques pour les objets homologues ayant le même parent dans l’arborescence hiérarchique
* Les documents ne peuvent pas porter le même nom s&#39;ils appartiennent au même projet

Compte tenu de ces limitations, Workfront renomme automatiquement les objets ou les documents selon les besoins afin d’éviter les conflits.

### Gestion des documents dans Workfront

Les documents sont gérés au niveau du projet avec cette intégration et ne peuvent pas être chargés sur des tâches ou des événements pour le moment.

L’accès aux documents est également géré au niveau du projet. Si un utilisateur a accès à un projet, il peut accéder à tous les documents associés à ce projet.

<!--Documents can't be dragged as full folders.-->

### Limites de l’expérience du document

Comme cette intégration est créée à l’aide d’ESM, il existe certaines limites à l’expérience de document d’origine dans Workfront :

#### Limites

Les fonctionnalités suivantes ne seront pas incluses dans cette intégration :

* Fournisseurs de documents externes
* Accéder à la relecture
* Visionneuse de documents dans Workfront


#### Limitations temporaires

Pour l’instant, les fonctionnalités suivantes ne sont pas disponibles :

* Documents favoris
* Demander des documents
* Envoyer des documents à Adobe Experience Manager Assets
* Approbations en plusieurs étapes
* Chargement de documents vers des commentaires ou des mises à jour dans Workfront
* Charger des documents vers des tâches ou des événements dans Workfront



