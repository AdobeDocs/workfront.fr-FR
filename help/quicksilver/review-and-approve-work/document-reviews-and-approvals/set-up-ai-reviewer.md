---
product-area: documents
navigation-topic: approvals
title: Créer des réviseurs de contenu
description: Une fois qu’au moins une marque est configurée dans Workfront, vous pouvez créer plusieurs réviseurs de contenu, que vous pouvez ensuite affecter aux modèles d’approbation et aux demandes individuelles de révision et d’approbation.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 4673049e-119e-4315-95f0-f10d8b286856
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 2b3e2ac00126facab9cc45ba8fb193d8951a37ec
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 17%

---

# Créer des réviseurs de contenu

>[!NOTE]
>
>Cette fonctionnalité est actuellement en version bêta.

Une fois qu’au moins une marque est configurée dans Workfront, vous pouvez créer plusieurs réviseurs de contenu, que vous pouvez ensuite affecter aux modèles d’approbation et aux demandes individuelles de révision et d’approbation.


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

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer, vous devez configurer des directives relatives à la marque d’image dans Workfront. Pour plus d’informations, voir [Création et gestion des marques pour le réviseur de contenu](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Ajouter un réviseur de contenu

>[!NOTE]
>
>Le réviseur de contenu n’est pas conçu pour être un décideur dans le workflow de révision et d’approbation. Il ne fournit qu’un score et des recommandations pour aligner la ressource sur les exigences de marque spécifiées.

Pour ajouter un réviseur de contenu :

{{step-1-to-setup}}

1. Dans le panneau de gauche, accédez à **Révision et approbation** > **Réviseurs de contenu**.
1. Cliquez sur **Ajouter nouveau**.
1. Nommez le réviseur ou la réviseuse.
1. Sélectionnez une **marque**.
1. Sélectionnez l’une des options suivantes dans le menu déroulant **Type d’orientation** :
   * **Image** : le réviseur de contenu examine la ressource en fonction des directives de marque d’image que vous avez configurées dans Workfront.
   * **Brand Voice** : le réviseur de contenu examine la ressource en fonction des directives relatives à la voix de marque que vous avez configurées dans Workfront.
1. Cliquez sur **Créer**.

   Une fois le réviseur de contenu créé, les utilisateurs peuvent l’ajouter aux modèles d’approbation ou aux approbations individuelles.

   Pour plus d’informations, consultez les ressources suivantes :

   * [Créer un modèle de workflow d’approbation pour les documents](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
   * [Créer un workflow d’approbation de document](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)
