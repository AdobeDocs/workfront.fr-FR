---
product-area: documents
navigation-topic: manage-documents
title: Extraire des documents
description: Vous pouvez extraire un document pour empêcher d’autres personnes de le supprimer ou d’en charger une nouvelle version. Une seule personne à la fois peut extraire un document. Vous pouvez extraire tout document chargé vers Adobe Workfront ainsi que les documents liés à des fournisseurs de documents tiers (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint ou tout autre fournisseur personnalisé).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/kkWxK2NzQtSfeRqsd0vEB-2AUYFrO6WIU3A752w7kM4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 593
ht-degree: 85%

---

# Extraire des documents

Vous pouvez récupérer un document pour empêcher d&#39;autres utilisateurs de le supprimer ou d&#39;en charger une nouvelle version. Un seul utilisateur peut extraire un document à la fois. Vous pouvez récupérer tout document chargé dans Adobe Workfront ainsi que les documents liés à des fournisseurs de documents tiers (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint ou tout autre fournisseur personnalisé). 

>[!NOTE]
>
>Cette fonctionnalité n&#39;est pas disponible dans la zone des nouveaux documents.<br>
>Si votre entreprise utilise l’espace de stockage dans le cloud d’Adobe, la nouvelle zone Documents s’affiche lorsque vous accédez aux documents dans Workfront. Pour plus d’informations sur l’espace de stockage dans le cloud Adobe, consultez [Présentation de l’espace de stockage dans le cloud Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

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
   <td> 
   <p>Contributeur ou supérieur</p>
   <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux documents</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer l’accès aux documents</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Actions autorisées sur les documents extraits

Les personnes disposant d’un accès en gestion au document peuvent effectuer les opérations suivantes :

* Modifier le document (nom du document, description, données personnalisées)
* Déplacer le document
* Partager le document
* Prévisualiser le document
* Télécharger le document

  >[!TIP]
  >
  > Bien qu’une personne puisse télécharger un document lorsqu’il est extrait par une autre personne, nous recommandons d’attendre que le document ait été réarchivé avant de le télécharger. Lorsqu’un document est extrait, cela indique souvent que le travail est toujours en cours sur le document. En attendant qu’un document soit à nouveau archivé pour le télécharger, vous avez la garantie que la personne dispose de la version la plus récente.

* Approuvez un document ou appliquez une approbation au document.
* Réviser le document dans la visionneuse de relecture

  Pour plus d’informations sur la relecture, voir [Relecture](../../review-and-approve-work/proofing/proofing.md).

## Extraire un document

Si vous disposez des autorisations de gestion sur un document, vous pouvez l’extraire pour interdire certaines actions sur le document. 

1. Accédez à la zone de stockage de votre document, puis sélectionnez le document. 

   Pour plus d’informations sur l’ajout de documents, voir [Ajouter des documents à Adobe Workfront à partir de votre système de fichiers](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Cliquez sur l’icône **Extraire** ![Extraire](assets/check-out-25x23.png).

1. Une icône de cadenas ![icône cadenas](assets/lock-icon-locked-qs.png) s’affiche à droite du nom du document. Le document reste extrait après votre déconnexion de Workfront.
1. Seule la personne qui a extrait le document ou l’administrateur ou l’administratrice Workfront peut l’archiver.

## Gérer des documents extraits

Tenez compte des points suivants concernant les documents extraits :

* Avant de pouvoir supprimer un objet dans lequel un document extrait est stocké, vous devez d’abord réarchiver ce dernier. 
* Si l’administrateur ou administratrice Workfront supprime une personne qui a extrait un document qu’elle ne possède pas, Workfront réarchive automatiquement le document.
* Si l’administrateur ou administratrice Workfront supprime une personne qui a extrait un document qu’elle possède et que le document est chargé sur un objet, le document reste extrait. Seuls les administrateurs et administratrices Workfront peuvent le réarchiver.
* Si l’administrateur ou administratrice Workfront supprime une personne qui a extrait un document qu’elle possède et que le document est chargé uniquement dans la zone Documents (et non sur un objet), le document est supprimé avec la personne.

  Pour plus d’informations sur la suppression de personnes, voir [Supprimer des personnes](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Si l’administrateur Workfront désactive un utilisateur, tous les documents qu’il a extraits restent extraits. Seul un administrateur Workfront peut les archiver à nouveau. 

## Archiver un document

Vous devez réarchiver un document avant de pouvoir charger une nouvelle version ou le supprimer. 

Pour archiver un document, procédez comme suit :

1. Accédez à la zone de stockage de votre document et sélectionnez le document. 

   Une icône de cadenas ![icône cadenas](assets/lock-icon-locked-qs.png) s’affiche à droite du nom du document.

1. Cliquez sur l’icône **Archiver** ![Icône Archiver](assets/check-in-25x22.png).
