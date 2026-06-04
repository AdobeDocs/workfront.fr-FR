---
product-area: documents
navigation-topic: approvals
title: Créer des outils de révision IA
description: Une fois qu’au moins une marque est configurée dans Workfront, vous pouvez créer plusieurs réviseurs d’IA, que vous pouvez ensuite affecter aux modèles d’approbation et aux demandes individuelles de révision et d’approbation.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
exl-id: 4673049e-119e-4315-95f0-f10d8b286856
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sfM3OtA-DVqywr3Up8VGjcycLRs5WtF22dcpXzRlnvQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 290
ht-degree: 18%

---

# Créer des outils de révision IA

>[!NOTE]
>
>Cette fonctionnalité est actuellement en version bêta.

Une fois qu’au moins une marque est configurée dans Workfront, vous pouvez créer plusieurs réviseurs d’IA, que vous pouvez ensuite affecter aux modèles d’approbation et aux demandes individuelles de révision et d’approbation.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur système.</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer, vous devez configurer des directives relatives à la marque d’image dans Workfront. Pour plus d’informations, voir [Création et gestion des marques pour le réviseur de contenu](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Ajouter un réviseur d’IA

>[!NOTE]
>
>Le réviseur de l’IA n’est pas conçu pour être un décideur dans le workflow de révision et d’approbation. Il ne fournit qu’un score et des recommandations pour aligner la ressource sur les exigences de marque spécifiées.

Pour ajouter un réviseur de contenu :

{{step-1-to-setup}}

1. Dans le panneau de gauche, accédez à **Révision et approbation** > **Réviseurs AI**.
1. Cliquez sur **Ajouter nouveau**.
1. Nommez le réviseur ou la réviseuse.
1. Sélectionnez une **marque**.
1. Sélectionnez l’une des options suivantes dans le menu déroulant **Type d’orientation** :
   * **Image** : le réviseur de l’IA examinera la ressource par rapport aux directives de marque d’image que vous avez configurées dans Workfront.
   * **Brand Voice** : le réviseur de l’IA examinera la ressource par rapport aux directives relatives à la voix de marque que vous avez configurées dans Workfront.
1. Cliquez sur **Créer**.

   Une fois le réviseur de l’IA créé, les utilisateurs peuvent l’ajouter aux modèles d’approbation ou aux approbations individuelles.

   Pour plus d’informations, consultez les ressources suivantes :

   * [Créer un modèle de workflow d’approbation pour les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
   * [Créer un workflow d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)
