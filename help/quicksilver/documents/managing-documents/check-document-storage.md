---
product-area: documents
navigation-topic: manage-documents
title: Vérifier les limites de stockage des documents
description: En tant qu’administrateur Adobe Workfront, vous pouvez afficher l’utilisation et le quota de stockage de documents sur la page Informations sur le client. L’aspect du stockage dépend de l’utilisation par votre entreprise du stockage Workfront hérité ou du stockage dans le cloud Adobe.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/vOjgBLxX5rFIGHBCHB2a6Q3Bs3KE5x-opXUMvANjI1E
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 09dff59503604894e61f2a62af7ae1c2e8a39068
workflow-type: tm+mt
source-wordcount: 491
ht-degree: 15%

---

# Vérifier les limites de stockage des documents

Bien qu’il n’existe aucune restriction sur les types et tailles des fichiers individuels que les utilisateurs peuvent charger vers votre instance Workfront, votre plan Workfront comprend un quota de stockage total. En tant qu’administrateur Workfront, vous surveillez l’utilisation et le quota à partir de la zone Configuration de la page Informations sur le client.

L’aspect du stockage varie selon que votre entreprise utilise l’ancien stockage Workfront ou l’espace de stockage cloud Adobe :

* Si vous utilisez le stockage Workfront hérité, consultez la section [Stockage Workfront hérité](#legacy-workfront-storage) dans cet article.
* Si vous utilisez l’espace de stockage cloud Adobe, consultez [Espace de stockage cloud Adobe](#adobe-cloud-storage) dans cet article.

  Pour plus d’informations sur l’espace de stockage dans le cloud Adobe, consultez [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Plan Workfront</td> 
   <td> <p>Tout package Workfront pour gérer les documents à l’aide du stockage hérité</p>
      <p>Tout package de workflow pour gérer les documents à l’aide de l’espace de stockage dans le cloud Adobe</p> </td> 
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

## Espace de stockage Adobe


Si votre entreprise utilise le stockage dans le cloud Adobe, votre quota de stockage est signalé comme une allocation de pool unique qui combine le stockage fourni par votre licence Workfront et tout stockage fourni par le biais d’un module complémentaire Frame.io Enterprise. L’utilisation du stockage n’est pas soumise à une limite stricte. Les utilisateurs peuvent continuer à charger des documents même lorsque l’utilisation dépasse votre quota.

### Afficher l’utilisation du stockage dans les informations sur le client

Pour vérifier l’espace de stockage cloud d’Adobe pour les documents :

{{step-1-to-setup}}

1. Dans le panneau de gauche, cliquez sur **Système** > **Infos client**.
1. Accédez à la section **Présentation du stockage**.
1. Vérifiez votre utilisation. La présentation du stockage affiche votre quota de stockage en pool et divise l&#39;utilisation en :

   * les projets hérités de Workfront et les projets d’espace de stockage Adobe s’affichent dans la barre bleue.
   * Les projets autonomes du cadre s’affichent dans la barre verte. Ces projets sont distincts de Workfront et ne sont disponibles que si vous disposez d’une licence Frame.io Enterprise.


![Utilisation de l’espace de stockage Adobe dans les informations sur le client](assets/storage-usage.png)

Les chiffres d’utilisation sont actualisés régulièrement afin que vous puissiez voir un décompte à jour.

### Notifications par e-mail aux administrateurs

Lorsque l’utilisation dépasse 75 %, 90 % ou 100 % de votre quota de stockage, Workfront envoie une notification par e-mail aux administrateurs système.
