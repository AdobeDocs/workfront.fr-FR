---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Envoyer un document avec le connecteur amélioré
description: Vous pouvez envoyer des documents de Workfront vers Experience Manager Assets. Les documents téléchargés et envoyés de Workfront vers Experience Manager Assets sont toujours pris en compte dans le stockage global de documents. Les ressources liées à partir de Experience Manager Assets ne sont pas prises en compte dans le stockage global.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# Envoyer un document avec le connecteur amélioré

Vous pouvez envoyer des documents de Workfront vers Experience Manager Assets. Les documents téléchargés et envoyés de Workfront vers Experience Manager Assets sont toujours pris en compte dans le stockage global de documents. Les ressources liées à partir de Experience Manager Assets ne sont pas prises en compte dans le stockage global.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Pro ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produit</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Afficher l’accès ou une version ultérieure sur les documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de commencer, vous devez

* Installez Workfront pour Experience Manager Enhanced Connector.

## Envoi d’un document à Experience Manager Assets

Lorsqu’un utilisateur envoie un document de Workfront vers Experience Manager Assets, les métadonnées mappées sont transférées le long du document. S’il est configuré, les métadonnées sont synchronisées en continu chaque fois qu’une modification est apportée.

Pour envoyer un document :

1. Accédez au **Documents** dans Workfront, puis sélectionnez le document à envoyer.
1. Cliquez sur **Envoyer à**, puis sélectionnez l’intégration Experience Manager Assets que votre administrateur doit configurer.

   >[!NOTE]
   >
   >N’importe quel nom peut être choisi pour cette intégration. Il peut donc ne pas mentionner spécifiquement Experience Manager Assets.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Sélectionnez l’emplacement où doit se rendre la ressource, puis cliquez sur **Sélectionner un dossier**.
1. Lorsque vous trouvez la destination de votre choix, cliquez sur **Enregistrer**.

## Envoi d’une nouvelle version à Experience Manager Assets

Vous pouvez ajouter une nouvelle version à un document que vous avez précédemment téléchargé vers Workfront. Pour plus d’informations, voir [Télécharger une nouvelle version d’un document](../../../documents/managing-documents/upload-new-document-version.md). Une fois la dernière version téléchargée, vous pouvez l’envoyer à Experience Manager Assets. Si un champ mappé dans Workfront a été modifié, la nouvelle version met à jour les métadonnées dans Experience Manager Assets lors de l’envoi.

Pour envoyer la version la plus récente :

1. Accédez au **Documents** dans Workfront, puis recherchez le document.
1. Cliquez sur **Envoyer à**, puis sélectionnez l’intégration Experience Manager Assets que votre administrateur doit configurer.

   >[!NOTE]
   >
   >N’importe quel nom peut être choisi pour cette intégration. Il peut donc ne pas mentionner spécifiquement Experience Manager Assets.

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Cliquer sur **Enregistrer**. La nouvelle version enregistre au même emplacement que la version précédente.
