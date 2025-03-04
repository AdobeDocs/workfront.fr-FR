---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Lier des ressources et des dossiers à partir d’Experience Manager Assets ou d’Assets Essentials
description: Vous pouvez lier une ressource ou un dossier provenant d’Experience Manager Assets ou d’Assets Essentials à n’importe quel objet Adobe Workfront prenant en charge les documents. Les ressources envoyées à partir d’Assets Essentials ne sont pas prises en compte dans le stockage global de documents de Workfront. Les documents chargés et envoyés de Workfront à Assets Essentials sont bien pris en compte dans le stockage global.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 85a2f154b3b561cdf53c68d50e66b8945f9f9823
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 98%

---

# Lier des ressources et des dossiers à partir d’Experience Manager Assets ou d’Assets Essentials

Vous pouvez lier une ressource ou un dossier provenant d’Experience Manager Assets ou d’Assets Essentials à n’importe quel objet Adobe Workfront prenant en charge les documents. Les ressources envoyées à partir d’Assets Essentials ne sont pas prises en compte dans le stockage global de documents de Workfront. Les documents chargés et envoyés de Workfront à Assets Essentials sont bien pris en compte dans le stockage global.

Les champs de métadonnées sont mappés pour la première fois lorsque vous envoyez une ressource de Workfront vers Experience Manager Assets ou Assets Essentials. Si votre équipe d’administration Workfront a activé la synchronisation des métadonnées d’objet, les champs restent à jour s’ils sont modifiés dans l’une ou l’autre des applications.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer d’Experience Manager as a Cloud Service ou d’Assets Essentials, et quelqu’un doit vous ajouter au produit en tant qu’utilisateur ou utilisatrice dans l’Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Autorisations Experience Manager</td> 
    <td>Vous devez disposer d’un accès en écriture au dossier.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher accès ou version ultérieure</p> <p>Pour plus d’informations sur les demandes d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès à des objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Conditions préalables

Avant de commencer

* Votre administrateur ou administratrice Workfront doit configurer une intégration Experience Manager. Pour plus d’informations, voir [Configurer l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurer l’intégration Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Lier une ressource à partir d’Experience Manager Assets ou d’Assets Essentials

Vous pouvez lier une ressource provenant d’Experience Manager Assets ou d’Assets Essentials à Workfront. Une fois la ressource liée, vous pouvez

* [Vérifier une ressource liée pour Experience Manager Assets ou Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Charger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md)

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez ajouter le document.
1. Sélectionnez **Ajouter**, puis choisissez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >L’équipe d’administration de Workfront peut choisir n’importe quel nom pour cette intégration, qui peut donc ne pas contenir spécifiquement les mentions Assets ou Assets Essentials.

1. Sélectionnez les ressources de votre choix.

   ![Sélectionner une ressource](assets/select-an-asset.png)

1. Cliquez sur **Sélectionner**.

## Lier un dossier à partir d’Experience Manager Assets ou d’Assets Essentials

Les autorisations d’affichage de ressources individuelles dans un dossier dépendent des autorisations Experience Manager Assets ou Assets Essentials.

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez placer le dossier.
1. Sélectionnez **Ajouter**, puis choisissez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >L’administrateur ou l’administratrice de Workfront peut choisir n’importe quel nom pour cette intégration. Il peut donc ne pas mentionner spécifiquement Assets ou Assets Essentials.

1. Sélectionnez les dossiers de votre choix.

   ![Sélectionner un dossier](assets/select-a-folder.png)

1. Cliquez sur **Sélectionner**.

## Lier une nouvelle version à partir d’Experience Manager Assets ou d’Assets Essentials

Vous pouvez extraire une nouvelle ressource d’Assets Essentials et l’ajouter à une ressource existante en tant que nouvelle version. Si le document est déjà lié et qu’une nouvelle version est ajoutée dans Assets Essentials, la nouvelle version apparaît automatiquement dans Workfront.

Pour lier une nouvelle version depuis Assets Essentials :

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez ajouter le document.
1. Sélectionnez la ressource à remplacer par une nouvelle version. Vous ne pouvez pas créer de version d’une ressource dans un dossier lié.
1. Sélectionnez **Ajouter** > **Version**, puis sélectionnez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >L’administrateur ou l’administratrice de Workfront peut choisir n’importe quel nom pour cette intégration. Il peut donc ne pas mentionner spécifiquement Assets ou Assets Essentials.

1. Sélectionnez la ressource de votre choix.

   ![Sélectionner une ressource](assets/select-an-asset.png)

1. Cliquez sur **Sélectionner**.

>[!TIP]
>
>Vous pouvez afficher toutes les versions d’une ressource en accédant à **Détails du document** > **Versions**.
