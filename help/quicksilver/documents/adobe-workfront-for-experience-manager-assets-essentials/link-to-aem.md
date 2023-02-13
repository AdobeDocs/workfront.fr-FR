---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Lier des ressources et des dossiers à partir de Experience Manager Assets ou Assets Essentials
description: Vous pouvez lier une ressource ou un dossier de Experience Manager Assets ou Assets Essentials à n’importe quel objet Adobe Workfront prenant en charge les documents. Les ressources envoyées à partir d’Assets Essentials ne sont pas prises en compte dans le stockage global de documents dans Workfront. Les documents téléchargés et envoyés de Workfront vers Assets Essentials sont pris en compte dans le stockage global.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Lier des ressources et des dossiers à partir de Experience Manager Assets ou Assets Essentials

Vous pouvez lier une ressource ou un dossier de Experience Manager Assets ou Assets Essentials à n’importe quel objet Adobe Workfront prenant en charge les documents. Les ressources envoyées à partir d’Assets Essentials ne sont pas prises en compte dans le stockage global de documents dans Workfront. Les documents téléchargés et envoyés de Workfront vers Assets Essentials sont pris en compte dans le stockage global.

Les champs de métadonnées sont d’abord mappés lorsque vous envoyez une ressource de Workfront vers Experience Manager Assets ou Assets Essentials. Si votre administrateur Workfront a activé la synchronisation des métadonnées d’objet, les champs restent à jour s’ils sont modifiés dans l’une ou l’autre des applications.

## Exigences d’accès

Vous devez disposer des éléments suivants :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p> Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licences Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Vous devez disposer d’un Experience Manager as a Cloud Service ou Assets Essentials, et vous devez être ajouté au produit en tant qu’utilisateur dans le Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Autorisations du Experience Manager</td> 
    <td>Vous devez disposer d’un accès en écriture au dossier.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès ou version ultérieure</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de commencer,

* Votre administrateur Workfront doit configurer une intégration de Experience Manager. Pour plus d’informations, voir [Configuration de l’intégration Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configuration de l’intégration de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Liaison d’une ressource à partir de Experience Manager Assets ou Assets Essentials

Vous pouvez lier une ressource de Experience Manager Assets ou Assets Essentials à Workfront. Une fois la ressource liée, vous pouvez

* [BAT d’une ressource liée pour Experience Manager Assets ou Assets Essentials](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [Télécharger une nouvelle version d’un document](../../documents/managing-documents/upload-new-document-version.md)

1. Accédez au **Documents** dans Workfront où vous souhaitez ajouter le document.
1. Sélectionner **Ajouter**, puis sélectionnez l’intégration de Experience Manager que votre administrateur a configurée.

   >[!NOTE]
   >
   >L’administrateur de Workfront peut choisir n’importe quel nom pour cette intégration. Il peut donc ne pas mentionner spécifiquement Assets ou Assets Essentials.

1. Sélectionnez les ressources de votre choix.

   ![](assets/select-an-asset.png)

1. Cliquez sur **Sélectionner**.

## Lier un dossier à partir de Experience Manager Assets ou Assets Essentials

Les autorisations d’affichage de ressources individuelles dans un dossier dépendent des autorisations Experience Manager Assets ou Assets Essentials.

1. Accédez au **Documents** dans Workfront, où vous souhaitez placer le dossier.
1. Sélectionner **Ajouter**, puis sélectionnez l’intégration de Experience Manager que votre administrateur a configurée.

   >[!NOTE]
   >
   >L’administrateur de Workfront peut choisir n’importe quel nom pour cette intégration, de sorte qu’il ne mentionnera pas spécifiquement Ressources ou Assets Essentials.

1. Sélectionnez les dossiers de votre choix.

   ![](assets/select-a-folder.png)

1. Cliquez sur **Sélectionner**.

## Liaison d’une nouvelle version à partir de Experience Manager Assets ou d’Assets Essentials

Vous pouvez extraire une nouvelle ressource d’Assets Essentials et l’ajouter à une ressource existante en tant que nouvelle version. Si le document est déjà lié et qu’une nouvelle version est ajoutée dans Assets Essentials, la nouvelle version apparaît automatiquement dans Workfront.

Pour lier une nouvelle version à partir d’Assets Essentials :

1. Accédez au **Documents** dans Workfront où vous souhaitez ajouter le document.
1. Sélectionnez la ressource à remplacer par une nouvelle version. Vous ne pouvez pas créer de version d’une ressource dans un dossier lié.
1. Sélectionner **Ajouter** > **Version**, puis sélectionnez l’intégration de Experience Manager que votre administrateur a configurée.

   >[!NOTE]
   >
   >L’administrateur de Workfront peut choisir n’importe quel nom pour cette intégration, de sorte qu’il ne mentionnera pas spécifiquement Ressources ou Assets Essentials.

1. Sélectionnez la ressource de votre choix.

   ![](assets/select-an-asset.png)

1. Cliquez sur **Sélectionner**.

>[!TIP]
>
>Vous pouvez afficher toutes les versions d’une ressource si vous accédez à **Détails du document** > **Versions**.
