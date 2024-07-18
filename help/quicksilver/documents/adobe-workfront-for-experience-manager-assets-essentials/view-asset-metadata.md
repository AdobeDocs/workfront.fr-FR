---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Afficher les métadonnées mappées pour Experience Manager Assets ou Assets Essentials
description: Vous pouvez afficher une vue en temps réel des métadonnées mappées dans le panneau Détails du document et Résumé pour les documents .
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: cfad5855-033c-4a15-b5a2-7ff32ed65fe9
source-git-commit: b87839d6c6dbfe978a3e14ef4b448560742f95c3
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 47%

---

# Afficher les métadonnées mappées pour Experience Manager Assets ou Assets Essentials

Vous pouvez afficher une vue en temps réel des métadonnées mappées dans le panneau Détails du document et Résumé pour les documents . Les champs de métadonnées sont d’abord mappés lorsque vous envoyez une ressource de Workfront vers Experience Manager Assets ou des Assets Essentials. Si votre administrateur Workfront a activé la synchronisation des métadonnées d’objet, les champs restent à jour s’ils sont modifiés dans l’une ou l’autre des applications.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td>Requête ou supérieure
   </td>
  </tr>
  <tr>
   <td><strong>Produit</strong>
   </td>
   <td>Vous devez disposer d’Experience Manager Assets as a Cloud Service ou d’Assets Essentials, et quelqu’un doit vous ajouter au produit en tant qu’utilisateur ou utilisatrice dans Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Configurations des niveaux d’accès*</strong>
   </td>
   <td>Accès en modification aux documents
<p>
<strong>Note :</strong> si vous ne disposez toujours pas d’un accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires ont été configurées pour votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <strong>Créer ou modifier les niveaux d’accès personnalisés</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Autorisations d’objets</strong>
   </td>
   <td>Accès ou version ultérieure
<p>
Pour plus d’informations sur la demande d’un accès supplémentaire, consultez <strong>Demander l’accès aux objets</strong>.
   </td>
  </tr>
</table>


* Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Conditions préalables

Avant de commencer

* Votre administrateur Workfront doit configurer une intégration d’Experience Manager. Pour plus d’informations, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configuration de l’intégration Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Détails du document

Pour ouvrir le panneau Métadonnées dans Détails du document :

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Passez la souris sur le document dont vous avez besoin, puis sélectionnez **Document Details**.
1. Recherchez et développez la section **Metadata** .

   >[!NOTE]
   >
   >Vous ne pouvez pas modifier les champs de cette section. Ils sont en lecture seule.

![panneau Détails du document](assets/metadata-panel-doc-details.png)


## Résumé des documents

Pour ouvrir le panneau Métadonnées dans le panneau Résumé :

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Recherchez le document dont vous avez besoin.
1. Cliquez sur l&#39;**icône de résumé** ![icône de résumé](assets/summary-panel-icon.png), puis développez la section **Métadonnées** .

   >[!NOTE]
   >
   >Vous ne pouvez pas modifier les champs de cette section. Ils sont en lecture seule.

![summary pour les documents](assets/metadata-panel-summary.png)
