---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Création d’un dossier lié à Experience Manager Assets ou Assets Essentials
description: Vous pouvez créer un dossier lié à Experience Manager Assets ou Assets Essentials dans Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: eb2b3b21-bc0b-45d3-85fa-1715cf927cb7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Création d’un dossier lié à Experience Manager Assets ou Assets Essentials

Vous pouvez créer un dossier lié à Experience Manager Assets ou Assets Essentials dans Workfront. Comme le dossier est lié, toute ressource ajoutée au dossier s’affichera automatiquement dans Workfront et Experience Manager. Vous n’avez pas à envoyer manuellement la ressource si elle se trouve dans un dossier lié.


## Exigences d’accès

Vous devez disposer des éléments suivants :

<table>
  <tr>
   <td><strong>Formule Adobe Workfront*</strong>
   </td>
   <td>Tous
   </td>
  </tr>
  <tr>
   <td><strong>Licences Adobe Workfront*</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>Produit</strong>
   </td>
   <td>Vous devez disposer d’Experience Manager Assets as a Cloud Service ou d’Assets Essentials, et vous devez être ajouté au produit en tant qu’utilisateur.
   </td>
  </tr>
  <tr>
   <td><strong>Autorisations des Experience Manager</strong>
   </td>
   <td>Vous devez disposer d’un accès en écriture au dossier de destination dans l’intégration d’Experience Manager.
   </td>
  </tr>
  <tr>
   <td><strong>Paramétrages du niveau d'accès</strong>
   </td>
   <td>Vous devez être un administrateur Workfront. Pour plus d’informations sur les administrateurs Workfront, voir <strong>Octroi d’un accès administratif complet à un utilisateur</strong>.
   </td>
  </tr>
</table>


*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.


## Conditions préalables

Avant de commencer,

* Votre administrateur Workfront doit configurer une intégration de Experience Manager. Pour plus d’informations, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configuration de l’intégration de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Création d’un dossier lié

Le dossier lié est créé à l’emplacement spécifié par l’administrateur Workfront lors de la configuration de l’intégration. Chaque intégration ne peut avoir qu’un seul emplacement de dossier pour les dossiers liés.

Le nom du dossier lié est automatiquement créé en fonction du Portfolio, du programme, du projet auquel il est associé et ne peut pas être modifié. Si le projet n’est associé à aucun Portfolio ou programme, le dossier lié affiche le nom du projet et sa date de création.

Pour créer un dossier lié :



1. Accédez au projet dans lequel vous souhaitez placer le dossier.
1. Sélectionner **Ajouter**, puis accédez à l’ intégration Experience Manager configurée par votre administrateur.
   >[!NOTE]
   >
   >L’administrateur de Workfront peut choisir n’importe quel nom pour cette intégration, de sorte qu’il ne mentionnera pas spécifiquement Experience Manager Assets ou Assets Essentials.

1. Sélectionner **Créer un dossier lié**. Le système crée automatiquement un dossier dans Experience Manager en fonction de l’emplacement spécifié lors de la configuration de l’intégration.
   ![créer un dossier lié ;](assets/linked-folder.png)
