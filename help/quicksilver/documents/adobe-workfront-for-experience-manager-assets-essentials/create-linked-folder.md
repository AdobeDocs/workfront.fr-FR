---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Créer un dossier lié à Experience Manager Assets ou Assets Essentials
description: Vous pouvez créer un dossier lié à Experience Manager Assets ou aux Assets Essentials dans Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: 1744e6f2b78c64ba2fa4856d9c6a0611404e4458
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 14%

---

# Créer un dossier lié à Experience Manager Assets ou Assets Essentials

Vous pouvez créer un dossier lié à Experience Manager Assets ou aux Assets Essentials dans Workfront. Comme le dossier est lié, toute ressource ajoutée au dossier s’affichera automatiquement dans Workfront et Experience Manager. Vous n’avez pas à envoyer manuellement la ressource si elle se trouve dans un dossier lié.


## Conditions d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>Formules Adobe Workfront*</strong>
   </td>
   <td>N’importe quelle
   </td>
  </tr>
  <tr>
   <td><strong>Licences Adobe Workfront*</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>Produit</strong>
   </td>
   <td>Vous devez disposer d’Assets Essentials as a Cloud Service Experience Manager Assets et vous ajouter au produit en tant qu’utilisateur.
   </td>
  </tr>
  <tr>
   <td><strong>Autorisations des Experience Manager</strong>
   </td>
   <td>Vous devez disposer d’un accès en écriture au dossier de destination dans l’intégration d’Experience Manager.
   </td>
  </tr>
  <tr>
   <td><strong> Configurations de niveau d’accès</strong>
   </td>
   <td>Pour configurer une intégration d’Experience Manager, vous devez être un administrateur Workfront. Une fois configuré, les utilisateurs disposant d’une licence Plan peuvent configurer des dossiers liés sur des projets individuels.
   </td>
  </tr>
</table>


* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.


## Conditions préalables

Avant de commencer

* Votre administrateur Workfront doit configurer une intégration d’Experience Manager. Pour plus d’informations, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configuration de l’intégration Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Création d’un dossier lié

Le dossier lié est créé à l’emplacement spécifié par l’administrateur Workfront lors de la configuration de l’intégration. Chaque intégration ne peut avoir qu’un seul emplacement de dossier pour les dossiers liés.

Le nom du dossier lié est automatiquement créé en fonction du Portfolio, du programme, du projet auquel il est associé et ne peut pas être modifié. Si le projet n’est associé à aucun Portfolio ou programme, le dossier lié affiche le nom du projet et sa date de création.

Pour créer un dossier lié :



1. Accédez au projet dans lequel vous souhaitez placer le dossier.
1. Sélectionnez **Ajouter nouveau**, puis accédez à l’intégration Experience Manager configurée par votre administrateur.

   >[!NOTE]
   >
   >L’administrateur de Workfront peut choisir n’importe quel nom pour cette intégration. Il se peut donc qu’il ne mentionne pas spécifiquement Experience Manager Assets ou les Assets Essentials.

1. Sélectionnez **Créer un dossier lié**. Le système crée automatiquement un dossier dans Experience Manager en fonction de l’emplacement spécifié lors de la configuration de l’intégration.
   ![créer un dossier lié](assets/linked-folder.png)
