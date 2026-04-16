---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Lier des ressources et des dossiers à partir d’Experience Manager Assets Essentials
description: Vous pouvez lier une ressource ou un dossier de Experience Manager Assets Essentials à tout objet Adobe Workfront prenant en charge les documents. Les ressources envoyées à partir d’Assets Essentials ne sont pas prises en compte dans le stockage global de documents de Workfront. Les documents chargés et envoyés de Workfront à Assets Essentials sont bien pris en compte dans le stockage global.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: a9dfc5c7838668bd3007c157a4e1a53ab4bd86f5
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 52%

---

# Lier des ressources et des dossiers à partir d’Experience Manager Assets Essentials

Vous pouvez lier une ressource ou un dossier de Experience Manager Assets Essentials à tout objet Adobe Workfront prenant en charge les documents.

Pour lier des ressources et des dossiers à partir de Experience Manager Assets à l’aide de la fonction de conseil, consultez [Lier des ressources et des dossiers à la fonction de conseil optimisée par Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).


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

* Votre administrateur ou administratrice Workfront doit configurer une intégration Experience Manager. Pour plus d’informations, voir [Configuration de l’intégration de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Lier une ressource à partir de Experience Manager Assets Essentials

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez ajouter le document.
1. Sélectionnez **Ajouter**, puis choisissez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >L’administrateur Workfront peut choisir n’importe quel nom pour cette intégration et ne pas mentionner spécifiquement Experience Manager Assets Essentials.

1. Sélectionnez les ressources de votre choix.

   ![Sélectionner une ressource](assets/select-an-asset.png)

1. Cliquez sur **Sélectionner**.

## Lier une nouvelle version de Experience Manager Assets Essentials

Vous pouvez extraire une nouvelle ressource de Experience Manager Assets Essentials et l’ajouter à une ressource existante en tant que nouvelle version. Si le document est déjà lié et qu’une nouvelle version est ajoutée dans Experience Manager Assets Essentials, la nouvelle version s’affiche automatiquement dans Workfront.

Pour lier une nouvelle version :

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez ajouter le document.
1. Sélectionnez la ressource à remplacer par une nouvelle version. Vous ne pouvez pas créer de version d’une ressource dans un dossier lié.
1. Sélectionnez **Ajouter** > **Version**, puis sélectionnez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >L’administrateur Workfront peut choisir n’importe quel nom pour cette intégration, de sorte qu’il peut ne pas mentionner spécifiquement Experience Manager Assets Essentials.

1. Sélectionnez la ressource à lier.

1. Cliquez sur **Sélectionner**.

## Lier un dossier depuis Experience Manager Assets Essentials

Les autorisations d’affichage de ressources individuelles dans un dossier reposent sur les autorisations de Experience Manager Assets Essentials.

1. Accédez à la zone **Documents** dans Workfront, dans laquelle vous souhaitez placer le dossier.
1. Sélectionnez **Ajouter**, puis choisissez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >L’administrateur Workfront peut choisir n’importe quel nom pour cette intégration, de sorte qu’il peut ne pas mentionner spécifiquement Experience Manager Assets Essentials.

1. Sélectionnez les dossiers de votre choix.

   ![Sélectionner un dossier](assets/select-a-folder.png)

1. Cliquez sur **Sélectionner**.

## Considérations

* La fonctionnalité de gestionnaire d’accès n’est pas disponible pour Assets Essentials. Pour lier des ressources et des dossiers à l’aide du gestionnaire d’accès, consultez [Lier des ressources et des dossiers au gestionnaire d’accès optimisé par Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem.md).

* Les ressources envoyées à partir d’Assets Essentials ne sont pas prises en compte dans le stockage global de documents de Workfront. Les documents chargés et envoyés de Workfront à Assets Essentials sont bien pris en compte dans le stockage global.

* Les champs de métadonnées sont d’abord mappés lorsque vous envoyez une ressource de Workfront vers Experience Manager Assets Essentials. Si votre équipe d’administration Workfront a activé la synchronisation des métadonnées d’objet, les champs restent à jour s’ils sont modifiés dans l’une ou l’autre des applications.
