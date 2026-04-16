---
product-area: documents
navigation-topic: approvals
title: Prise en main du Workfront Content Reviewer
description: Utilisez le collaborateur IA de réviseur de contenu de Workfront pour évaluer le contenu par rapport aux directives de la marque lors des workflows de révision et d’approbation.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 99048cf2b9320b7f00e1de3bae3f48bc145af5f0
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 1%

---

# Prise en main du Workfront Content Reviewer

Le réviseur de contenu est un collaborateur d’IA, un type d’agent d’IA qui peut être ajouté à vos projets, tâches et documents. Les collaborateurs de l’IA peuvent être configurés dans la zone Configuration et affectés comme les utilisateurs.

Dans Workfront, le réviseur de contenu permet d’augmenter la vitesse du contenu et d’améliorer la conformité de la marque tout au long du processus de révision et d’approbation. Vous pouvez ajouter des réviseurs de contenu aux modèles d’approbation ou les inclure dans des demandes individuelles de révision et d’approbation.

## Conditions d’accès

Pour configurer des réviseurs de contenu dans Workfront, vous devez être administrateur ou administratrice système.

Tout utilisateur peut ajouter le réviseur de contenu à une demande de révision et d’approbation.

## Conditions

* Les approbations unifiées doivent être activées pour votre instance Workfront.
* Votre organisation doit disposer de GenStudio Foundation.
   * Content Reviewer dans Workfront fournit les fonctionnalités disponibles dans GenStudio Foundation pour les workflows de révision et d’approbation de ressources. Vous n’avez pas besoin d’accéder directement à GenStudio Foundation pour terminer votre travail. Votre accès à la fonctionnalité GenStudio Foundation par l’intermédiaire de l’analyseur de contenu est soumis aux conditions de votre contrat Workfront.
* Adobe doit disposer d’un contrat Adobe Gen AI signé dans ce fichier.
Pour plus d’informations sur la signature du contrat, voir [Signature du contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Types de fichier pris en charge {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Type de fichier non pris en charge"
>abstract="Ce réviseur de contenu ne prend pas en charge le type de fichier sélectionné. Chargez un type de fichier pris en charge ou supprimez le réviseur de contenu pour envoyer la demande."

Le réviseur de contenu peut examiner les types de fichiers suivants :

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* GIF non animé (.gif)
* PDF (.pdf)
* PPT (.ppt, .pptx)
* DOC (.doc, .docx)

Si vous téléchargez un type de fichier non pris en charge, l’option Réviseur de contenu n’est pas disponible lors de la création d’un workflow d’approbation.

## Configurer des directives de marque

Le réviseur de contenu Workfront applique les directives de la marque lors de la révision de votre contenu. Les administrateurs Workfront peuvent définir des directives de marque dans la zone Configuration de Workfront . Les marques créées dans GenStudio Foundation sont également disponibles dans Workfront.

Pour configurer les directives de la marque, les administrateurs système doivent :

1. [Octroi de l’accès aux autorisations de marque](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [Créer et gérer des marques pour le réviseur de contenu](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## Créer des réviseurs de contenu

Une fois qu’au moins une marque est configurée, les administrateurs Workfront peuvent commencer à créer des réviseurs de contenu dans la zone Configuration . Vous pouvez créer plusieurs réviseurs de contenu axés sur différents conseils :

* **Image** : ce réviseur de contenu examinera la ressource par rapport aux directives de marque d’image que vous avez configurées dans Workfront. [!BADGE Beta]{type=Positive tooltip="Cette fonctionnalité est actuellement en version bêta."}
   * Les administrateurs système doivent signer l’accord bêta pour activer cette fonctionnalité.
* **Brand Voice** : le réviseur de contenu examine la ressource en fonction des directives relatives à la voix de marque que vous avez configurées dans Workfront.

Les réviseurs de contenu peuvent ensuite être affectés à des modèles d’approbation et à des demandes individuelles de révision et d’approbation.

Pour plus d’informations, voir [Configuration des collaborateurs d’IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Ajout de réviseurs de contenu aux demandes de révision et d’approbation

Les utilisateurs peuvent ajouter des réviseurs de contenu aux modèles d’approbation existants ou à des demandes individuelles de révision et d’approbation.

### Modèles d’approbation

Si votre entreprise ajoute souvent les mêmes personnes aux demandes de révision et d’approbation, les utilisateurs de licences standard peuvent créer des modèles d’approbation dans la zone Configuration de Workfront .

Les utilisateurs peuvent ajouter des réviseurs de contenu aux modèles d’approbation afin de vérifier automatiquement la conformité de la marque lorsqu’un modèle est utilisé pour créer une demande.

Une fois créés, les modèles d’approbation peuvent être appliqués aux ressources de la zone Documents d’un projet, d’une tâche ou d’un événement.

Pour plus d’informations, voir [Création d’un modèle de workflow d’approbation pour les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

![liste de modèles présentant les réviseurs d’IA](assets/ai-review-templates.png)

### Demande de révision et d’approbation individuelle

Lorsque les utilisateurs créent des demandes de révision et d’approbation individuelles, ils peuvent ajouter un réviseur de contenu dans avec d’autres participants ou créer une seule demande avec uniquement le réviseur de contenu pour vérifier la conformité de la marque.

Pour plus d’informations, voir [Créer un processus d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).


![Le réviseur de contenu a été ajouté à la demande de validation individuelle](assets/new-stage.png)

## Afficher le score et les commentaires des réviseurs de contenu

Quelques secondes après l’envoi de la demande de révision et d’approbation avec un réviseur de contenu, le score et les commentaires du réviseur de contenu sont disponibles dans le panneau Résumé du document, même si d’autres participants procèdent toujours à la révision et prennent des décisions.

Les propriétaires d’approbation reçoivent également un e-mail les informant qu’une révision de la ressource a été effectuée. Dans l’e-mail, cliquez sur **Accéder à la révision** et consultez le score et les commentaires dans Workfront.

Le réviseur de contenu n’est pas conçu pour être un décideur dans le workflow de révision et d’approbation. Il ne fournit qu’un score et des recommandations pour aligner la ressource sur les exigences de marque spécifiées.

Si la ressource ne répond pas aux directives de la marque, le contenu créatif peut charger une nouvelle version et le propriétaire de l’approbation peut créer une deuxième demande de révision et d’approbation auprès du réviseur du contenu.

Pour plus d’informations sur l’affichage des scores et des commentaires, voir [Afficher le score et les commentaires des réviseurs de contenu](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).

