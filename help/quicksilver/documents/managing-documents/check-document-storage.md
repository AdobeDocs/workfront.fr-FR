---
product-area: documents
navigation-topic: manage-documents
title: Vérifier les limites de stockage des documents
description: En tant qu’administrateur Adobe Workfront, vous pouvez afficher l’utilisation et le quota de stockage de documents sur la page Informations sur le client. L’aspect du stockage varie selon que votre entreprise utilise un stockage Workfront hérité ou un stockage d’entreprise Adobe.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7b6d24d6a5b7fd052a3e7c97034e920e771022a6
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 16%

---

# Vérifier les limites de stockage des documents

{{highlighted-preview}}

Bien qu’il n’existe aucune restriction sur les types et tailles des fichiers individuels que les utilisateurs peuvent charger vers votre instance Workfront, votre plan Workfront comprend un quota de stockage total. En tant qu’administrateur Workfront, vous surveillez l’utilisation et le quota à partir de la zone Configuration de la page Informations sur le client.

L’aspect du stockage varie selon que votre entreprise utilise un stockage Workfront hérité ou un stockage d’entreprise Adobe :

* Si vous utilisez le stockage Workfront hérité, consultez la section [Stockage Workfront hérité](#legacy-workfront-storage) dans cet article.
* Si vous utilisez le stockage d’entreprise Adobe, consultez [Stockage d’entreprise Adobe](#adobe-enterprise-storage) dans cet article.

  Pour plus d’informations sur le stockage d’entreprise, consultez [Présentation du stockage d’entreprise &#x200B;](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Plan Workfront</td> 
   <td> <p>Tout package Workfront pour gérer les documents à l’aide du stockage hérité</p>
      <p>Tout package de workflow pour gérer les documents à l’aide du stockage d’entreprise Adobe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez l’article [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Stockage Workfront hérité

Si votre entreprise utilise un stockage Workfront hérité, la page Informations sur le client affiche un quota de stockage unique pour les documents téléchargés directement vers Workfront.

Pour vérifier le stockage de documents Workfront hérité :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système** > **Infos client**.
1. Dans la section **Informations de base**, recherchez **Quota de stockage**. Vous pouvez y voir la quantité de stockage actuellement utilisée ainsi que la quantité totale de stockage incluse dans votre formule Workfront.

Le quota de stockage est actualisé tous les jours afin d’afficher le décompte le plus récent.

>[!NOTE]
>
>Cette limite ne s’applique pas aux documents que vous liez à Workfront à partir d’un autre fournisseur tiers (SharePoint, Google Drive, Webdam, Box, Dropbox ou tout autre fournisseur de gestion des ressources numériques).

<div class="preview">

## Stockage d’entreprise Adobe

<!--
If your organization uses Adobe enterprise storage, your storage quota is reported as a single pooled allocation that combines storage provisioned through your V2 Workfront SKU and any storage provisioned through a Frame.io Enterprise SKU or add-on. There's no hard cap on storage usage; users can continue uploading documents even when usage exceeds your quota.

Beginning with the May 2026 release, you can view your pooled storage quota and a usage breakdown on the Customer Info page.

-->

### Afficher l’utilisation du stockage dans les informations sur le client

Pour vérifier le stockage de documents d’entreprise d’Adobe :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système** > **Infos client**.
1. Accédez à la section **Présentation du stockage**.
1. Vérifiez votre utilisation. La présentation du stockage affiche votre quota de stockage en pool et divise l&#39;utilisation en :

   * Les projets hérités de Workfront et les projets de stockage d’entreprise Adobe s’affichent dans la barre bleue.
   * Les projets autonomes du cadre s’affichent dans la barre verte. Ces projets sont distincts de Workfront et ne sont disponibles que si vous disposez d’une licence Frame.io Enterprise.


![Utilisation du stockage d’entreprise Adobe dans les informations sur le client](assets/storage-usage.png)

Les chiffres d’utilisation sont actualisés régulièrement afin que vous puissiez voir un décompte à jour.

### Notifications par e-mail aux administrateurs

Lorsque l’utilisation dépasse 75 %, 90 % ou 100 % de votre quota de stockage, Workfront envoie une notification par e-mail aux administrateurs système.

</div>