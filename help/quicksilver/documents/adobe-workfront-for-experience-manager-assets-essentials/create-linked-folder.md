---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Créer un dossier lié à Experience Manager Assets ou à Assets Essentials
description: Vous pouvez créer un dossier lié à Experience Manager Assets ou à Assets Essentials dans Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: b87839d6c6dbfe978a3e14ef4b448560742f95c3
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 100%

---

# Créer un dossier lié à Experience Manager Assets ou à Assets Essentials

Vous pouvez créer un dossier lié à Experience Manager Assets ou à Assets Essentials dans Workfront. Comme le dossier est lié, toute ressource ajoutée au dossier s’affichera automatiquement dans Workfront et Experience Manager. Vous n’avez pas à envoyer manuellement la ressource si elle se trouve dans un dossier lié.


## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>Plan Adobe Workfront*</strong>
   </td>
   <td>Tous
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
   <td>Vous devez disposer d’Experience Manager Assets as a Cloud Service ou d’Assets Essentials et faire l’objet d’un ajout au produit en tant qu’utilisateur ou utilisatrice.
   </td>
  </tr>
  <tr>
   <td><strong>Autorisations pour Experience Manager</strong>
   </td>
   <td>Vous devez disposer d’un accès en écriture au dossier de destination dans l’intégration d’Experience Manager.
   </td>
  </tr>
  <tr>
   <td><strong>Configurations du niveau d’accès</strong>
   </td>
   <td>Pour configurer une intégration d’Experience Manager, vous devez être un administrateur ou une administratrice de Workfront. Une fois la configuration effectuée, les utilisateurs et utilisatrices disposant d’une licence de plan peuvent configurer des dossiers liés sur des projets individuels.
   </td>
  </tr>
</table>


*Pour connaître la formule, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Conditions préalables

Avant de commencer

* Votre administrateur ou administratrice Workfront doit configurer une intégration Experience Manager. Pour plus d’informations, consultez la section [Configurer l’intégration d’Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurer l’intégration d’Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Créer un dossier lié

Le dossier lié est créé à l’emplacement spécifié par l’administration de Workfront lors de la configuration de l’intégration. Chaque intégration ne peut avoir qu’un seul emplacement de dossier pour les dossiers liés.

Le nom du dossier lié est automatiquement créé en fonction du portfolio, du programme, du projet auquel il est associé et ne peut pas être modifié. Si le projet n’est associé à aucun portfolio ou programme, le dossier lié affiche le nom du projet et sa date de création.

Pour créer un dossier lié, procédez comme suit :

1. Accédez au projet dans lequel vous souhaitez placer le dossier.
1. Sélectionner **Ajouter nouveau**, puis accédez à l’intégration d’Experience Manager configurée par votre administrateur ou administratrice.

   >[!NOTE]
   >
   >L’administration de Workfront peut choisir le nom de cette intégration. Il se peut donc qu’il ne fasse pas référence de manière explicite à Experience Manager Assets ou Assets Essentials.

1. Sélectionnez **Créer un dossier lié**. Le système crée automatiquement un dossier dans Experience Manager en fonction de l’emplacement spécifié lors de la configuration de l’intégration.
   ![Création d’un dossier lié](assets/linked-folder.png)
