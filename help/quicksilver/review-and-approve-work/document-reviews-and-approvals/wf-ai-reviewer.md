---
product-area: documents
navigation-topic: approvals
title: Prise en main du réviseur de l’IA dédiée à Workfront
description: Utilisez le réviseur Workfront AI pour évaluer le contenu par rapport aux directives de la marque lors des workflows de révision et d’approbation.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/5nwapHAbb8wRWqen7a49QfpsAMLPZNEfJUJ2vm4R7SA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 3%
---
# Prise en main du réviseur de l’IA dédiée à Workfront

Le réviseur d’IA est un collaborateur d’IA, un type d’agent d’IA qui peut être ajouté à vos projets, tâches et documents. Les collaborateurs de l’IA peuvent être configurés dans la zone Configuration et affectés comme les utilisateurs.

Dans Workfront, AI Reviewer contribue à accroître la vitesse du contenu et à améliorer la conformité de la marque tout au long du processus de révision et d’approbation. Vous pouvez ajouter des réviseurs d’IA aux modèles d’approbation ou les inclure dans des demandes individuelles de révision et d’approbation.

## Conditions d’accès

Pour configurer des réviseurs d’IA dans Workfront, vous devez être administrateur ou administratrice système.

Tout utilisateur peut ajouter le réviseur d’IA à une demande de révision et d’approbation.

## Conditions

* Les approbations unifiées doivent être activées pour votre instance Workfront.
* Votre organisation doit disposer de GenStudio Foundation.
  * AI Reviewer dans Workfront fournit les fonctionnalités disponibles dans GenStudio Foundation pour les workflows de révision et d’approbation de ressources. Vous n’avez pas besoin d’accéder directement à GenStudio Foundation pour terminer votre travail. Votre accès aux fonctionnalités de GenStudio Foundation par le biais de l’IA Reviewer est soumis aux conditions de votre contrat Workfront.
* Adobe doit disposer d’un contrat Adobe Gen AI signé dans ce fichier.
Pour plus d’informations sur la signature du contrat, voir [Signature du contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).
* AI Reviewer n’est pas disponible dans les environnements Sandbox.


## Types de fichier pris en charge {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Type de fichier non pris en charge"
>abstract="Cet outil de révision IA ne prend pas en charge le type de fichier sélectionné. Chargez un type de fichier pris en charge ou supprimez l’AI Reviewer pour envoyer la demande."

Le réviseur de l’IA peut examiner les types de fichiers suivants :

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* GIF non animé (.gif)
* PDF (.pdf)
* PPT (.ppt, .pptx)
* DOC (.doc, .docx)

Si vous téléchargez un type de fichier non pris en charge, l’option Réviseur AI n’est pas disponible lors de la création d’un workflow d’approbation.

## Configurer des directives de marque

Le réviseur de l’IA Workfront applique les directives de la marque lors de la révision de votre contenu. Les administrateurs Workfront peuvent définir des directives de marque dans la zone Configuration de Workfront . Les marques créées dans GenStudio Foundation sont également disponibles dans Workfront.

Pour configurer les directives de la marque, les administrateurs système doivent :

1. [Octroi de l’accès aux autorisations de marque](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [Créer et gérer des marques pour l’AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## Créer des outils de révision IA

Une fois qu’au moins une marque est configurée, les administrateurs de Workfront peuvent commencer à créer des réviseurs d’IA dans la zone Configuration . Vous pouvez créer plusieurs réviseurs d’IA axés sur différents conseils :

* **Image** : ce réviseur d’IA examinera la ressource par rapport aux directives de marque d’image que vous avez configurées dans Workfront. [!BADGE Beta]{type=Positive tooltip="Cette fonctionnalité est actuellement en version bêta."}
  * Les administrateurs système doivent signer l’accord bêta pour activer cette fonctionnalité.
* **Brand Voice** : le réviseur de l’IA examinera la ressource par rapport aux directives relatives à la voix de marque que vous avez configurées dans Workfront.

Les réviseurs d’IA peuvent ensuite être affectés à des modèles d’approbation et à des demandes de révision et d’approbation individuelles.

Pour plus d’informations, voir [Configuration des collaborateurs d’IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Ce qu’évalue AI Reviewer {#what-ai-reviewer-evaluates}

Le réviseur de l’IA évalue le contenu différemment selon le type de consigne : image ou voix de marque.

### Image

Le réviseur d’IA évalue :

* **Composition** : Point focal, arrière-plan, recadrage, cadrage créatif
* **Éclairage et humeur** : Utilisation de la lumière, de la vitalité, de l&#39;optimisme
* **Diversité et inclusion** : représentation des personnes (race, sexe, âge, capacité)

AI Reviewer n’évalue pas :

* **Utilisation du logo** : emplacement, espace libre, dimensionnement, version correcte du logo
* **Palette de couleurs** : conformité des couleurs de la marque, évitement des couleurs non approuvées
* **Typographie** : famille de polices, poids, espacement, alignement
* **Style d’illustration** : cohérence avec l’approche d’illustration de la marque
* **Accessibilité** : conformité du contraste, lisibilité

### Voix de marque

Le réviseur d’IA évalue :

* **Ton de la voix** : Conversationnel, clair, humain, aligné avec la personnalité de la marque
* **Jargon/formalité** : évitement des mots à la mode, de l’élitisme ou d’une formalité excessive
* **Message** : Encouragement, honnêteté, positionnement responsable (par exemple, pour les sujets liés à l’IA)

AI Reviewer n’évalue pas :

* **Juridique/conformité** : utilisation des marques, clauses de non-responsabilité, règles de localisation

Pour obtenir des conseils sur la rédaction de directives de marque conformes à ce que l’évaluateur d’IA évalue, voir [&#x200B; Créer et gérer des marques pour l’évaluateur d’IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Ajouter des réviseurs d’IA pour réviser et approuver les demandes

Les utilisateurs peuvent ajouter des réviseurs AI aux modèles d’approbation existants ou à des demandes individuelles de révision et d’approbation.

### Modèles d’approbation

Si votre entreprise ajoute souvent les mêmes personnes aux demandes de révision et d’approbation, les utilisateurs de licences standard peuvent créer des modèles d’approbation dans la zone Configuration de Workfront .

Les utilisateurs peuvent ajouter des réviseurs d’IA aux modèles d’approbation pour vérifier automatiquement la conformité de la marque lorsqu’un modèle est utilisé pour créer une demande.

Une fois créés, les modèles d’approbation peuvent être appliqués aux ressources de la zone Documents d’un projet, d’une tâche ou d’un événement.

Pour plus d’informations, voir [Création d’un modèle de workflow d’approbation pour les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

![liste de modèles présentant les réviseurs d’IA](assets/ai-review-templates.png)

### Demande de révision et d’approbation individuelle

Lorsque les utilisateurs créent des demandes de révision et d’approbation individuelles, ils peuvent ajouter un réviseur d’IA dans avec d’autres participants ou créer une seule demande avec uniquement le réviseur d’IA pour vérifier la conformité de la marque.

Pour plus d’informations, voir [Créer un processus d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).


![Réviseur AI ajouté à une demande d’approbation individuelle](assets/new-stage.png)

## Afficher le score et les commentaires de l’outil de révision IA

Quelques secondes après l’envoi de la demande de révision et d’approbation avec un réviseur d’IA, le score et le retour d’informations du réviseur d’IA sont disponibles dans le panneau Résumé du document, même si d’autres participants sont toujours en train de réviser et de prendre des décisions.

Les propriétaires d’approbation reçoivent également un e-mail les informant qu’une révision de la ressource a été effectuée. Dans l’e-mail, cliquez sur **Accéder à la révision** et consultez le score et les commentaires dans Workfront.

Le réviseur de l’IA n’est pas conçu pour être un décideur dans le workflow de révision et d’approbation. Il ne fournit qu’un score et des recommandations pour aligner la ressource sur les exigences de marque spécifiées.

Si la ressource ne répond pas aux directives de la marque, le contenu créatif peut charger une nouvelle version et le propriétaire de l’approbation peut créer une deuxième demande de révision et d’approbation avec le réviseur de l’IA.

Pour plus d’informations sur l’affichage des scores et des commentaires, voir [Afficher le score et les commentaires des réviseurs d’IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).

