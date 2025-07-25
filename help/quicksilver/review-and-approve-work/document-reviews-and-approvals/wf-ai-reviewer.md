---
product-area: documents
navigation-topic: approvals
title: Prise en main du réviseur de l’IA dédiée à Workfront
description: Workfront AI Reviewer
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
source-git-commit: da980cee8710570f52c724053d1e0f359c6a9fe1
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 5%

---

# Prise en main du réviseur de l’IA dédiée à Workfront

Avec le réviseur de l’IA Workfront, vous pouvez augmenter la vitesse du contenu et optimiser la conformité de la marque dans le workflow de révision et d’approbation. Vous pouvez ajouter des réviseurs d’IA aux modèles d’approbation ou aux demandes individuelles de révision et d’approbation dans Workfront.

## Conditions d’accès

Pour configurer des réviseurs d’IA dans Workfront, vous devez être administrateur ou administratrice système.

Tout utilisateur peut ajouter le réviseur d’IA à une demande de révision et d’approbation.


## Conditions préalables

* Votre organisation doit avoir migré vers Adobe IMS (système Identity Management).
* Les approbations unifiées doivent être activées pour votre instance Workfront.
* Adobe doit disposer d’un contrat Adobe Gen AI signé dans ce fichier.
Pour plus d’informations sur la signature du contrat, voir [Signature du contrat Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).


## Types de fichier pris en charge {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Type de fichier non pris en charge"
>abstract="Cet outil de révision IA ne prend pas en charge le type de fichier sélectionné.Chargez un type de fichier pris en charge ou supprimez l’outil de révision IA pour envoyer la demande."

Le réviseur de l’IA peut examiner les types de fichiers suivants :

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* GIF non animé (.gif)

## Configurer des directives de marque

Le réviseur de l’IA pour Workfront utilise les directives de marque configurées dans Genstudio Foundations lors de la révision de votre contenu.

Pour en savoir plus sur les directives de la marque, voir

* [Marques GenStudio for Performance Marketing](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/guidelines/brands)
* [Ajouter des directives](https://experienceleague.adobe.com/fr/docs/genstudio-for-performance-marketing/user-guide/guidelines/add-guidelines)


## Créer des réviseurs d’IA

Une fois qu’il existe au moins une marque configurée dans GenStudio Foundations, les administrateurs Workfront peuvent commencer à créer des réviseurs d’IA dans la zone Configuration . Ces réviseurs d’IA peuvent ensuite être affectés à des modèles d’approbation et à des demandes de révision et d’approbation individuelles.

Pour plus d’informations, voir [Création de réviseurs d’IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/set-up-ai-reviewer.md).

## Ajouter des réviseurs d’IA pour réviser et approuver les demandes

Les utilisateurs peuvent ajouter des réviseurs d’IA à des modèles d’approbation existants ou à des demandes individuelles de révision et d’approbation.

### Modèles de validation

Si votre entreprise ajoute souvent les mêmes personnes aux demandes de révision et d’approbation, les utilisateurs de licences standard peuvent créer des modèles d’approbation dans la zone Configuration de Workfront .

Les utilisateurs peuvent ajouter des réviseurs d’IA aux modèles d’approbation pour vérifier automatiquement la conformité de la marque lorsqu’un modèle est utilisé pour créer une demande.

Une fois créés, les modèles d’approbation peuvent être appliqués aux ressources de la zone Documents d’un projet, d’une tâche ou d’un événement.

Pour plus d’informations, voir [Créer un modèle d’approbation pour les ressources et les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)

![liste de modèles présentant les réviseurs d’IA](assets/ai-review-templates.png)

### Demande de révision et d’approbation individuelle

Lorsque les utilisateurs créent des demandes de révision et d’approbation individuelles, ils peuvent ajouter un réviseur d’IA dans avec d’autres participants ou créer une seule demande avec uniquement le réviseur d’IA pour vérifier la conformité de la marque.

Pour plus d’informations, voir [Créer une demande de révision ou d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)


![Réviseur AI ajouté à une demande d’approbation individuelle](assets/ad-ai-reviewer-to-request.png)

## Afficher le score et le retour d’informations du réviseur de l’IA

Quelques secondes après l’envoi de la demande de révision et d’approbation avec un réviseur d’IA, le score et le retour d’informations du réviseur d’IA sont disponibles dans le panneau Résumé du document, même si d’autres participants sont toujours en train de réviser et de prendre des décisions.

Les propriétaires d’approbation reçoivent également un e-mail les informant qu’une révision de la ressource a été effectuée. Dans l’e-mail, cliquez sur **Accéder à la révision** et consultez le score et les commentaires dans Workfront.

Le réviseur de l’IA n’est pas conçu pour être un décideur dans le workflow de révision et d’approbation. Il ne fournit qu’un score et des recommandations pour aligner la ressource sur les exigences de marque spécifiées.

Si l’image répond depuis longtemps aux directives de la marque, le professionnel de la création peut charger une nouvelle version et le propriétaire de l’approbation peut créer une deuxième demande de révision et d’approbation avec le réviseur de l’IA, ce qui vous permet de passer d’une version à l’autre et de comparer les commentaires.

Pour plus d’informations sur l’affichage des scores et des commentaires, voir [Afficher le score et les commentaires des réviseurs d’IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).


![Retour d’informations du réviseur IA](assets/ai-reviewer-feedback.png)


