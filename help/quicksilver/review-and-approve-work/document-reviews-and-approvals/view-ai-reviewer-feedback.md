---
product-area: documents
navigation-topic: approvals
title: Afficher le score et les commentaires de l’outil de révision IA
description: Quelques secondes après l’envoi de la demande d’approbation, vous pouvez afficher le score et le retour d’informations du réviseur de l’IA dans le panneau Résumé du document .
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 838e8f3d-0ea6-4844-a261-ef7b0e78a755
TQID: 'https://experienceleague.adobe.com/iPlcSTaPI-zhmWvRvO81RKFYnIzUoJqzM70mNcxrVbs'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 3%
---
# Afficher le score et les commentaires de l’outil de révision IA

Quelques secondes après l’envoi de la demande de révision et d’approbation, vous pouvez afficher le score et le retour d’informations du réviseur de l’IA dans le panneau Résumé du document .

Le réviseur de l’IA n’est pas conçu pour être un décideur dans le workflow de révision et d’approbation. Il ne fournit qu’un score et des recommandations pour aligner la ressource sur les exigences de marque spécifiées.

![Retour d’informations du réviseur IA](assets/ai-reviewer-output.png)

## Comprendre comment les scores sont calculés

Le réviseur de l’IA calcule les scores différemment selon le type de révision :

* Révision de l’image : ce score reflète le ratio des directives approuvées par rapport aux directives ayant échoué.
* Copier la révision : Ce score utilise une pondération équilibrée des résultats subjectifs et objectifs. Les directives objectives (affichées sous « Corriger ») sont pondérées trois fois plus que les directives subjectives (affichées sous « Considérer »).

Étant donné que les directives objectives ont plus de poids dans les critiques de copie, nous vous recommandons d&#39;écrire des directives concrètes et mesurables dans votre marque. Pour plus d’informations, consultez la section [&#x200B; Bonnes pratiques pour la rédaction de directives relatives aux marques &#x200B;](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md#best-practices-for-writing-brand-guidelines) de l’article Création et gestion des marques pour l’AI Reviewer .

## Afficher le score et le retour d’informations

Vous pouvez afficher le score et les commentaires du réviseur de l’IA dans le panneau Résumé du document ou dans l’onglet Approbations de la page Détails du document .

1. Dans l’e-mail de notification Workfront, cliquez sur **Accéder à la révision**.

   Ou

   Accédez à la zone Documents où le document est chargé, puis ouvrez le panneau Résumé du document .
1. Cliquez sur **Score**.
   ![afficher le score du document](assets/view-score.png)

Dans la fenêtre de score et de commentaires, le réviseur de l’IA explique comment la ressource ne répond pas aux instructions spécifiées.
![Le retour d’informations du réviseur d’AI requiert votre attention](assets/ai-reviewer-needs-attention.png)

## Chargez une nouvelle version et ajoutez à nouveau un réviseur d’IA.

Si vous devez ajuster la ressource en fonction des commentaires du réviseur de l’IA, vous pouvez charger une nouvelle version et démarrer une nouvelle révision.

Pour plus d’informations, voir [Charger une nouvelle version du document et demander une approbation](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md).
