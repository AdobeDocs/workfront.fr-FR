---
product-area: documents
navigation-topic: manage-documents
title: Extraire des documents
description: Vous pouvez extraire un document pour empêcher d’autres personnes de le supprimer ou d’en charger une nouvelle version. Une seule personne à la fois peut extraire un document. Vous pouvez extraire tout document chargé vers Adobe Workfront ainsi que les documents liés à des fournisseurs de documents tiers (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint ou tout autre fournisseur personnalisé).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: 4a0448583cbcfd1f1df10d6474fdf4e77e7bff3e
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 92%

---

# Extraire des documents

Vous pouvez extraire un document pour empêcher d’autres personnes de le supprimer ou d’en charger une nouvelle version. Une seule personne à la fois peut extraire un document.Vous pouvez extraire tout document chargé vers Adobe Workfront ainsi que les documents liés à des fournisseurs de documents tiers (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint ou tout autre fournisseur personnalisé). 

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou version ultérieure</p>
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

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
  >Bien qu’une personne puisse télécharger un document lorsqu’il est extrait par une autre personne, nous recommandons d’attendre que le document ait été réarchivé avant de le télécharger. Lorsqu’un document est extrait, cela indique souvent que le travail est toujours en cours sur le document. En attendant qu’un document soit à nouveau archivé pour le télécharger, vous avez la garantie que la personne dispose de la version la plus récente.

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

* Si l’administrateur ou l’administratrice Workfront désactive une personne, tous les documents qu’elle a extraits restent extraits. Seuls les administrateurs et administratrices Workfront peuvent les réarchiver. 

## Archiver un document

Vous devez réarchiver un document avant de pouvoir charger une nouvelle version ou le supprimer. 

Pour archiver un document, procédez comme suit :

1. Accédez à la zone de stockage de votre document et sélectionnez le document. 

   Une icône de cadenas ![icône cadenas](assets/lock-icon-locked-qs.png) s’affiche à droite du nom du document.

1. Cliquez sur l’icône **Archiver** ![Icône Archiver](assets/check-in-25x22.png).
