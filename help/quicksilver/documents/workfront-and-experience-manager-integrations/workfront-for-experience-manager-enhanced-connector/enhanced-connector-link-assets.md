---
title: Lier des ressources et des dossiers à l’aide du connecteur amélioré
description: Vous pouvez lier une ressource ou un dossier provenant d’Experience Manager Assets à n’importe quel objet Workfront prenant en charge les documents.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: 3f9a824780f2ded914d461a473aef3b6ecfa8701
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 92%

---


# Lier des ressources et des dossiers à l’aide du connecteur amélioré

Vous pouvez lier une ressource ou un dossier provenant d’Experience Manager Assets à n’importe quel objet Workfront prenant en charge les documents. Les ressources envoyées à partir d’Experience Manager Assets ne sont pas prises en compte dans le stockage global de documents dans Workfront. Les documents chargés et envoyés de Workfront à Experience Assets Essentials sont bien pris en compte dans le stockage global.


>[!NOTE]
>
>Les fichiers Excel liés par le biais du connecteur amélioré ne peuvent pas être prévisualisés dans Workfront. Vous devez télécharger le fichier pour y accéder.

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
   <p>Requête ou supérieure</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produits supplémentaires</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès en lecture ou supérieur à un document</p> </td> 
  </tr> 
 </tbody> 
</table>


Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conditions préalables

Avant de commencer, vous devez

* installer le connecteur amélioré Workfront pour Experience Manager.

## Lier une ressource provenant d’Experience Manager Assets

Vous pouvez lier une ressource provenant d’Experience Manager Assets à Workfront. Une fois la ressource liée, vous pouvez

* [Relire une ressource liée pour Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [Charger une nouvelle version d’un document](../../../documents/managing-documents/upload-new-document-version.md)

Pour lier une ressource à Experience Manager Assets :

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez ajouter le document.
1. Cliquez sur **Ajouter**, puis sélectionnez l’intégration Experience Manager Assets que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >N’importe quel nom peut être choisi pour cette intégration. Experience Manager Assets peut donc ne pas être mentionné.

1. Sélectionnez les ressources de votre choix.

   ![Sélectionner une ressource](assets/select-an-asset.png)

1. Cliquez sur **Lier**.

## Lier un dossier provenant d’Experience Manager Assets

Les autorisations d’affichage de ressources individuelles dans un dossier dépendent des autorisations Experience Manager Assets.

Pour lier un dossier à Experience Manager Assets :

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez ajouter le document.
1. Cliquez sur **Ajouter**, puis sélectionnez l’intégration Experience Manager Assets que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >N’importe quel nom peut être choisi pour cette intégration. Experience Manager Assets peut donc ne pas être mentionné.

1. Sélectionnez les dossiers de votre choix.

   ![Sélectionner un dossier](assets/select-a-folder.png)

1. Cliquez sur **Lier**.

## Lier une nouvelle version provenant d’Experience Manager Assets

Vous pouvez extraire une nouvelle ressource d’Experience Manager Assets et l’ajouter à une ressource existante en tant que nouvelle version dans Workfront. Si le document est déjà lié et qu’une nouvelle version est ajoutée dans Experience Manager Assets, la nouvelle version apparaît automatiquement dans Workfront.

>[!TIP]
>
>Vous pouvez afficher toutes les versions d’une ressource en accédant à **Détails du document** > **Versions**.

Pour lier une nouvelle version provenant d’Experience Manager Assets :

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez ajouter le document.
1. Sélectionnez la ressource à remplacer par une nouvelle version. Vous ne pouvez pas créer de version d’une ressource dans un dossier lié.
1. Cliquez sur **Ajouter**, puis sélectionnez l’intégration Experience Manager Assets que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >N’importe quel nom peut être choisi pour cette intégration. Experience Manager Assets peut donc ne pas être mentionné.

1. Sélectionnez la ressource de votre choix.

   ![Sélectionner une ressource](assets/select-an-asset.png)

1. Cliquez sur **Lier**.
