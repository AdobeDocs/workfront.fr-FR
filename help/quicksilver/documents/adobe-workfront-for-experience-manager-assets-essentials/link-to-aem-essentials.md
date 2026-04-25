---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Lier des ressources et des dossiers à partir d’Experience Manager Assets Essentials
description: You can link an asset or folder from Experience Manager Assets Essentials to any Adobe Workfront object that supports documents. Les ressources envoyées à partir d’Assets Essentials ne sont pas prises en compte dans le stockage global de documents de Workfront. Les documents chargés et envoyés de Workfront à Assets Essentials sont bien pris en compte dans le stockage global.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 0b93f6f6-cf4b-4077-a464-be7f19f7cd25
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 51%

---

# Lier des ressources et des dossiers à partir d’Experience Manager Assets Essentials

You can link an asset or folder from Experience Manager Assets Essentials to any Adobe Workfront object that supports documents.

To link assets and folders from Experience Manager Assets using Content Advisor, see [Link assets and folders with Content Advisor powered by Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

If you are on enterprise storage, see [Use the Adobe Experience Manager with the Frame.io integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou supérieur</p> 
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produits supplémentaires</td> 
   <td>Vous devez disposer d’Experience Manager as a Cloud Service ou d’Assets Essentials, et quelqu’un doit vous ajouter au produit en tant qu’utilisateur ou utilisatrice dans l’Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Autorisations Experience Manager</td> 
    <td>Vous devez disposer d’un accès en écriture au dossier.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Accès en modification aux documents</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher accès ou version ultérieure</p> </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur le contenu de ce tableau, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer :

* Votre administrateur ou administratrice Workfront doit configurer une intégration Experience Manager. For more information, see [Configure the Experience Manager Assets Essentials integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Link an asset from Experience Manager Assets Essentials

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez ajouter le document.
1. Sélectionnez **Ajouter**, puis choisissez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it may not specifically mention Experience Manager Assets Essentials.

1. Sélectionnez les ressources de votre choix.

   ![Select an asset](assets/select-an-asset.png)

1. Cliquez sur **Sélectionner**.

## Link a new version from Experience Manager Assets Essentials

You can pull a new asset over from Experience Manager Assets Essentials and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets Essentials, the new version appears automatically in Workfront.

To link a new version:

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez ajouter le document.
1. Sélectionnez la ressource à remplacer par une nouvelle version. Vous ne pouvez pas créer de version d’une ressource dans un dossier lié.
1. Sélectionnez **Ajouter** > **Version**, puis sélectionnez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets Essentials.

1. Select the asset you want to link.

1. Cliquez sur **Sélectionner**.

## Link a folder from Experience Manager Assets Essentials

Permissions to view individual assets inside of a folder rely on Experience Manager Assets Essentials permissions.

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez placer le dossier.
1. Sélectionnez **Ajouter**, puis choisissez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets Essentials.

1. Sélectionnez les dossiers de votre choix.

   ![Select a folder](assets/select-a-folder.png)

1. Cliquez sur **Sélectionner**.

## Considérations

* Content Advisor functionality is not available for Assets Essentials. To link assets and folders using Content Advisor, see [Link assets and folders with Content Advisor powered by Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

* Les ressources envoyées à partir d’Assets Essentials ne sont pas prises en compte dans le stockage global de documents de Workfront. Les documents chargés et envoyés de Workfront à Assets Essentials sont bien pris en compte dans le stockage global.

* Metadata fields are first mapped when you send an asset from Workfront to Experience Manager Assets Essentials. Si votre équipe d’administration Workfront a activé la synchronisation des métadonnées d’objet, les champs restent à jour s’ils sont modifiés dans l’une ou l’autre des applications.
