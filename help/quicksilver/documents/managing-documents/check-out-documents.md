---
product-area: documents
navigation-topic: manage-documents
title: Vérifier les documents
description: Vous pouvez extraire un document pour empêcher d’autres utilisateurs de le supprimer ou de télécharger une nouvelle version. Un seul utilisateur peut extraire un document à la fois. Vous pouvez extraire tout document téléchargé vers Adobe Workfront ainsi que les documents liés à des fournisseurs de documents tiers (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint ou tout autre fournisseur personnalisé).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: 9aa6822c9c1ecade776d4c71b113c1afd997f40c
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 15%

---

# Vérifier les documents

Vous pouvez extraire un document pour empêcher d’autres utilisateurs de le supprimer ou de télécharger une nouvelle version. Un seul utilisateur peut extraire un document à la fois. Vous pouvez extraire tout document téléchargé vers Adobe Workfront ainsi que les documents liés à des fournisseurs de documents tiers (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint ou tout autre fournisseur personnalisé). 

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>N’importe quelle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou supérieur</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer l’accès au document</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Actions autorisées sur les documents extraits

Les utilisateurs disposant d’un accès de gestion au document peuvent effectuer les opérations suivantes :

* Modifier le document (nom du document, description, données personnalisées)
* Déplacer le document
* Partage du document
* Aperçu du document
* Télécharger le document

  >[!TIP]
  >
  > Bien qu’un utilisateur puisse télécharger un document lorsqu’il est extrait par un autre utilisateur, nous recommandons aux utilisateurs d’attendre que le document ait été réarchivé avant de le télécharger. Lorsqu’un document est extrait, cela indique souvent que le travail est toujours en cours sur le document. En attendant qu’un document soit à nouveau archivé pour le télécharger, vous avez la garantie que l’utilisateur dispose de la version la plus récente.

* Approuvez un document ou apportez une validation au document.
* Vérifier le document dans la visionneuse de vérification

  Pour plus d&#39;informations sur la vérification, voir [Vérification](../../review-and-approve-work/proofing/proofing.md)

## Extraction d’un document

Si vous disposez des autorisations de gestion d’un document, vous pouvez l’extraire pour interdire certaines actions sur le document. 

1. Accédez à la zone de stockage de votre document, puis sélectionnez le document. 

   Pour plus d’informations sur l’ajout de documents, voir [Ajout de documents à Adobe Workfront à partir de votre système de fichiers](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Cliquez sur l’icône **Extraire** ![](assets/check-out-25x23.png) .

1. Une icône de verrouillage ![](assets/lock-icon-locked-qs.png) s’affiche à droite du nom du document. Le document reste extrait une fois que vous vous êtes déconnecté de Workfront.
1. Seul l’utilisateur qui a extrait le document ou l’administrateur Workfront peut l’archiver.

## Gestion des documents extraits

Tenez compte des points suivants concernant les documents extraits :

* Avant de pouvoir supprimer un objet dans lequel un document extrait est stocké, vous devez d’abord le réarchiver. 
* Si l’administrateur Workfront supprime un utilisateur qui a extrait un document qu’il ne possède pas, Workfront l’extrait automatiquement.
* Si l’administrateur de Workfront supprime un utilisateur qui a extrait un document qu’il possède et que le document est téléchargé sur un objet, le document reste extrait. Seul un administrateur Workfront peut le réarchiver.
* Si l’administrateur de Workfront supprime un utilisateur qui a extrait un document qu’il possède et que le document est téléchargé uniquement dans la zone Documents (et non sur un objet), le document est supprimé avec l’utilisateur.

  Pour plus d’informations sur la suppression d’utilisateurs, voir [Suppression d’utilisateurs](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Si l’administrateur Workfront désactive un utilisateur, tous les documents qu’il a extraits restent extraits. Seul un administrateur Workfront peut les archiver à nouveau. 

## Archiver un document

Vous devez réarchiver un document avant de pouvoir télécharger une nouvelle version ou de la supprimer. 

Pour archiver un document :

1. Accédez à la zone de stockage de votre document et sélectionnez le document. 

   Une icône de verrouillage ![](assets/lock-icon-locked-qs.png) s’affiche à droite du nom du document.

1. Cliquez sur l’icône **Check In** ![](assets/check-in-25x22.png) .
