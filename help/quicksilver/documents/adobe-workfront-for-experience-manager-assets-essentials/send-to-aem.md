---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Envoyer un document vers Experience Manager Assets ou Assets Essentials
description: Vous pouvez envoyer des documents depuis Workfront vers Experience Manager Assets ou Assets Essentials. Les documents chargés et envoyés depuis Workfront vers Assets Essentials sont toujours pris en compte par rapport à votre stockage global de documents. Les ressources liées depuis Assets Essentials ne sont pas prises en compte dans le stockage global.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '919'
ht-degree: 96%

---

# Envoyer un document vers Experience Manager Assets ou Assets Essentials

Vous pouvez envoyer des documents depuis Workfront vers Experience Manager Assets ou Assets Essentials. Les documents chargés et envoyés depuis Workfront vers Assets Essentials sont toujours pris en compte par rapport à votre stockage global de documents. Les ressources liées depuis Assets Essentials ne sont pas prises en compte dans le stockage global.

Les ressources envoyées vers Experience Manager par le biais de cette intégration sont limitées à une taille de **5 Go**.

Dans l’environnement de Prévisualisation, la taille maximale d’Assets envoyé à Experience Manager par le biais de cette intégration est de 30 Go ****.

Les champs de métadonnées sont mappés pour la première fois lorsque vous envoyez une ressource de Workfront vers Experience Manager Assets ou Assets Essentials. Toutes les métadonnées configurées pour mapper des objets parent sont également envoyées. Pour plus d’informations sur la configuration du mappage des métadonnées, voir [Configurer l’intégration d’Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurer l’intégration d’Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Exemple** : lorsque vous envoyez pour la première fois une ressource jointe à une tâche, les métadonnées de la tâche sont mappées vers Experience Manager Assets ou Assets Essentials, ainsi qu’à toutes les métadonnées mappées à partir d’objets parent tels qu’un projet, un portfolio ou un programme.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer de l’accès suivant pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Plan Adobe Workfront</a> *</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Vue d’ensemble des licences héritées</a> *</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer d’Experience Manager as a Cloud Service ou d’Assets Essentials, et quelqu’un doit vous ajouter au produit en tant qu’utilisateur ou utilisatrice dans l’Admin Console.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : si vous n’avez toujours pas d’accès, demandez à votre équipe d’administration Workfront s’il existe des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès Affichage ou supérieur aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander un accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le forfait, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice Workfront.

+++

## Conditions préalables

Avant de commencer

* Votre administrateur ou administratrice Workfront doit configurer une intégration Experience Manager. Pour plus d’informations, voir [Configurer l’intégration d’Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurer l’intégration d’Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Envoyer un document depuis Workfront

Lorsqu’un utilisateur ou une utilisatrice envoie un document depuis Workfront vers Experience Manager Assets ou Assets Essentials, les métadonnées mappées sont transférées avec le document. Une fois le document envoyé, les modifications apportées aux métadonnées du document dans Workfront ne sont pas reflétées dans Assets ou Assets Essentials. Si un champ mappé dans Workfront est modifié, vous devez envoyer une nouvelle version du document avec les métadonnées mises à jour vers Assets ou Assets Essentials. Pour configurer ou modifier des métadonnées, voir [Configurer l’intégration d’Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurer l’intégration d’Experience Manager Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Pour envoyer un document, procédez comme suit :

1. Accédez à la zone **Documents** dans Workfront, puis sélectionnez le document à envoyer.
1. Cliquez sur **Envoyer à**, puis sélectionnez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >L’équipe d’administration de Workfront peut choisir n’importe quel nom pour cette intégration, qui peut donc ne pas contenir spécifiquement les mentions Assets ou Assets Essentials.

   ![Envoyer à](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Sélectionnez l’emplacement de la ressource, puis cliquez sur **Sélectionner un dossier**.
1. Lorsque vous trouvez la destination souhaitée, cliquez sur **Enregistrer**.

## Envoyer une nouvelle version

Vous pouvez ajouter une nouvelle version à un document que vous avez précédemment chargé vers Workfront. Pour plus d’informations, voir [Charger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md). Une fois la dernière version téléchargée, vous pouvez l’envoyer vers Assets Essentials. Si un champ mappé dans Workfront a été modifié, la nouvelle version met à jour les métadonnées dans Assets Essentials lors de l’envoi.

>[!IMPORTANT]
>
>Avant de charger une nouvelle version dans Workfront, nous vous recommandons de renommer le fichier. Si vous chargez une nouvelle version portant le même nom de fichier qu’une version précédente, seule la version la plus récente peut être téléchargée à partir de Workfront. Toutes les versions peuvent être téléchargées à partir d’Experience Manager Assets ou Assets Essentials, quel que soit le nom de fichier.

Pour envoyer la version la plus récente, procédez comme suit :

1. Accédez à la zone **Documents** dans Workfront, puis recherchez le document.
1. Sélectionnez **Envoyer à**, puis sélectionnez l’intégration d’Experience Manager que votre administrateur ou administratrice a configurée.

   >[!NOTE]
   >
   >L’administrateur ou l’administratrice de Workfront peut choisir n’importe quel nom pour cette intégration. Il peut donc ne pas mentionner spécifiquement Assets ou Assets Essentials.

   ![Envoyer à](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Cliquer sur **Enregistrer**. La nouvelle version enregistre au même emplacement que la version précédente.

## Déplacer un document vers un dossier lié dans Experience Manager Assets

>[!NOTE]
>
>Cette fonctionnalité est uniquement disponible pour Experience Manager Assets as a Cloud Service. Elle n’est pas disponible pour Experience Manager Assets Essentials.

Vous pouvez déplacer un document vers un dossier lié dans Experience Manager Assets si le document et le dossier lié se trouvent dans la même liste de documents (comme la zone de document d’un projet).

1. Recherchez le document à déplacer.
1. Faites glisser et déposer le document dans le dossier Experience Manager Assets lié vers lequel vous souhaitez le déplacer.

Les options du document ne sont pas disponibles lorsque le document est en cours de déplacement. Une fois le document déplacé vers Experience Manager Assets, il n’est plus visible dans la liste de documents de Workfront.

>[!NOTE]
>
> Toute action ou modification effectuée sur le document lors de son déplacement n’apparaîtra pas sur le document dans Experience Manager Assets et sera donc perdue.

