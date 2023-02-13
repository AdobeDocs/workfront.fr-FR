---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: Affichage des métadonnées mappées pour Experience Manager Assets ou Assets Essentials
description: Vous pouvez afficher une vue en temps réel des métadonnées mappées dans le panneau Détails du document et Résumé pour les documents .
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: cfad5855-033c-4a15-b5a2-7ff32ed65fe9
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Affichage des métadonnées mappées pour Experience Manager Assets ou Assets Essentials

Vous pouvez afficher une vue en temps réel des métadonnées mappées dans le panneau Détails du document et Résumé pour les documents . Les champs de métadonnées sont d’abord mappés lorsque vous envoyez une ressource de Workfront vers Experience Manager Assets ou Assets Essentials. Si votre administrateur Workfront a activé la synchronisation des métadonnées d’objet, les champs restent à jour s’ils sont modifiés dans l’une ou l’autre des applications.

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
   <td>Requête ou supérieure
   </td>
  </tr>
  <tr>
   <td><strong>Produit</strong>
   </td>
   <td>Vous devez disposer d’Experience Manager Assets as a Cloud Service ou d’Assets Essentials, et vous devez être ajouté au produit en tant qu’utilisateur dans le Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Paramétrages du niveau d'accès*</strong>
   </td>
   <td>Modifier l’accès aux documents
<p>
<strong>Remarque : </strong>Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <strong>Création ou modification de niveaux d’accès personnalisés</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Autorisations d’objet</strong>
   </td>
   <td>Accès ou version ultérieure
<p>
Pour plus d’informations sur la demande d’accès supplémentaire, voir <strong>Demande d’accès aux objets </strong>.
   </td>
  </tr>
</table>


*Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.


## Conditions préalables

Avant de commencer,

* Votre administrateur Workfront doit configurer une intégration de Experience Manager. Pour plus d’informations, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configuration de l’intégration de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Détails du document

Pour ouvrir le panneau Métadonnées dans Détails du document :

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Passez la souris sur le document dont vous avez besoin, puis sélectionnez **Détails du document**.
1. Recherchez et développez l’objet **Métadonnées** .
   >[!NOTE]
   >
   >Vous ne pouvez pas modifier les champs de cette section. Ils sont en lecture seule.

![panneau des détails du document](assets/metadata-panel-doc-details.png)


## Résumé des documents

Pour ouvrir le panneau Métadonnées dans le panneau Résumé :

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Recherchez le document dont vous avez besoin.
1. Cliquez sur le bouton **Icône Résumé** ![icône de résumé](assets/summary-panel-icon.png), puis développez l’objet **Métadonnées** .
   >[!NOTE]
   >
   >Vous ne pouvez pas modifier les champs de cette section. Ils sont en lecture seule.

![résumé des documents](assets/metadata-panel-summary.png)
