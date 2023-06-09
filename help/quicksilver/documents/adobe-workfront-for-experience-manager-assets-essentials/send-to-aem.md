---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Envoi d’un document à Experience Manager Assets ou Assets Essentials
description: Vous pouvez envoyer des documents de Workfront vers Experience Manager Assets ou Assets Essentials. Les documents téléchargés et envoyés depuis Workfront vers Assets Essentials sont toujours pris en compte par rapport à votre stockage global de documents. Les ressources liées à partir d’Assets Essentials ne sont pas prises en compte dans le stockage global.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 91da06fe23b464e0422d50b0db69f4eae3db642f
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# Envoi d’un document à Experience Manager Assets ou Assets Essentials


Vous pouvez envoyer des documents de Workfront vers Experience Manager Assets ou Assets Essentials. Les documents téléchargés et envoyés depuis Workfront vers Assets Essentials sont toujours pris en compte par rapport à votre stockage global de documents. Les ressources liées à partir d’Assets Essentials ne sont pas prises en compte dans le stockage global.

Les champs de métadonnées sont d’abord mappés lorsque vous envoyez une ressource de Workfront vers Experience Manager Assets ou Assets Essentials. Toutes les métadonnées configurées pour mapper des objets parents sont également envoyées. Pour plus d’informations sur la configuration du mappage des métadonnées, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configuration de l’intégration de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Exemple** Lorsque vous envoyez une ressource associée à une tâche pour la première fois, les métadonnées de la tâche sont mappées sur Experience Manager Assets ou Assets Essentials, ainsi que toutes les métadonnées mappées à partir d’objets parents tels qu’un projet, un portfolio et un programme.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Formule Adobe Workfront</a>*</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Présentation des licences héritées</a>*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer d’un Experience Manager as a Cloud Service ou Assets Essentials, et vous devez être ajouté au produit en tant qu’utilisateur dans le Admin Console.
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher l’accès ou une version ultérieure sur les documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de commencer,

* Votre administrateur Workfront doit configurer une intégration de Experience Manager. Pour plus d’informations, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configuration de l’intégration de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Envoi d’un document à partir de Workfront

Lorsqu’un utilisateur envoie un document de Workfront vers Experience Manager Assets ou Assets Essentials, les métadonnées mappées sont transférées le long du document. Une fois le document envoyé, les modifications apportées aux métadonnées du document dans Workfront ne sont pas répercutées dans Assets ou Assets Essentials. Si un champ mappé dans Workfront est modifié, vous devez envoyer une nouvelle version du document avec les métadonnées mises à jour à Assets ou Assets Essentials. Pour configurer ou modifier des métadonnées, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configuration de l’intégration de Experience Manager Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

Pour envoyer un document :

1. Accédez au **Documents** dans Workfront, puis sélectionnez le document à envoyer.
1. Cliquez sur **Envoyer à**, puis sélectionnez l’intégration de Experience Manager configurée par votre administrateur.

   >[!NOTE]
   >
   >L’administrateur de Workfront peut choisir n’importe quel nom pour cette intégration. Il peut donc ne pas mentionner spécifiquement Assets ou Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Sélectionnez l’emplacement où doit se rendre la ressource, puis cliquez sur **Sélectionner un dossier**.
1. Lorsque vous trouvez la destination de votre choix, cliquez sur **Enregistrer**.

## Envoyer une nouvelle version

Vous pouvez ajouter une nouvelle version à un document que vous avez précédemment téléchargé vers Workfront. Pour plus d’informations, voir [Télécharger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md). Une fois la dernière version téléchargée, vous pouvez l’envoyer à Assets Essentials. Si un champ mappé dans Workfront a été modifié, la nouvelle version met à jour les métadonnées dans Assets Essentials lors de l’envoi.

>[!IMPORTANT]
>
>Avant de charger une nouvelle version dans Workfront, nous vous recommandons de renommer le fichier. Si vous téléchargez une nouvelle version portant le même nom de fichier qu’une version précédente, seule la version la plus récente peut être téléchargée à partir de Workfront. Toutes les versions peuvent être téléchargées à partir de Experience Manager Assets ou d’Assets Essentials, quel que soit le nom de fichier.

Pour envoyer la version la plus récente :

1. Accédez au **Documents** dans Workfront, puis recherchez le document.
1. Sélectionner **Envoyer à**, puis sélectionnez l’intégration de Experience Manager configurée par votre administrateur.

   >[!NOTE]
   >
   >L’administrateur de Workfront peut choisir n’importe quel nom pour cette intégration, de sorte qu’il ne mentionnera pas spécifiquement Ressources ou Assets Essentials.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Cliquer sur **Enregistrer**. La nouvelle version enregistre au même emplacement que la version précédente.

## Déplacer un document vers un dossier lié dans Experience Manager Assets

>[!NOTE]
>
>Cette fonctionnalité est disponible uniquement pour Experience Manager Assets as a Cloud Service. Elle n’est pas disponible pour Experience Manager Assets Essentials.

Vous pouvez déplacer un document vers un dossier lié dans Experience Manager Assets si le document et le dossier lié se trouvent tous deux dans la même liste de documents (comme la zone de document d’un projet).

1. Recherchez le document à déplacer.
1. Faites glisser le document et déposez-le dans le dossier Experience Manager Assets lié vers lequel vous souhaitez le déplacer.

Les options du document ne sont pas disponibles lorsque le document est en cours de déplacement. Une fois le document déplacé vers Experience Manager Assets, n’est plus visible dans la liste de documents de Workfront.

>[!NOTE]
>
> Les actions ou modifications effectuées sur le document en cours de déplacement n’apparaîtront pas dans le document dans Experience Manager Assets et seront donc perdues.

