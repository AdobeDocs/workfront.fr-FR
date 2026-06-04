---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Envoyer un document avec le connecteur amélioré
description: Vous pouvez envoyer des documents de Workfront vers Experience Manager Assets. Les documents chargés et envoyés de Workfront vers Experience Manager Assets sont toujours pris en compte dans le stockage global de documents. Les ressources liées à partir d’Experience Manager Assets ne sont pas prises en compte dans le stockage global.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
TQID: https://experienceleague.adobe.com/tu4blsoJGh2ilDeTIwqdx4xtmuC-1OOnZ2QySDNnQpI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 409
ht-degree: 96%

---

# Envoyer un document avec le connecteur amélioré

Vous pouvez envoyer des documents de Workfront vers Experience Manager Assets. Les documents chargés et envoyés de Workfront vers Experience Manager Assets sont toujours pris en compte dans le stockage global de documents. Les ressources liées à partir d’Experience Manager Assets ne sont pas prises en compte dans le stockage global.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Package Adobe Workfront</td> 
   <td> <p>Tous</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td> 
   <p>Contributeur ou supérieur</p>
   <p>Requête ou supérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produits supplémentaires</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> s=« MCXref xref »&gt;Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Accès Affichage ou supérieur aux documents</p></td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Conditions préalables

Avant de commencer, vous devez

* Installer le connecteur amélioré Workfront pour Experience Manager

## Envoyer un document à Experience Manager Assets

Lorsqu’un utilisateur ou une utilisatrice envoie un document de Workfront vers Experience Manager Assets, les métadonnées mappées sont transférées avec le document. Si cela a été configuré, les métadonnées sont synchronisées en continu chaque fois qu’une modification est apportée.

Pour envoyer un document, procédez comme suit :

1. Accédez à la zone **Documents** dans Workfront, puis sélectionnez le document à envoyer.
1. Cliquez sur **Envoyer à**, puis sélectionnez l’intégration Experience Manager Assets que votre équipe d’administration a configurée.

   >[!NOTE]
   >
   >N’importe quel nom peut être choisi pour cette intégration. Experience Manager Assets peut donc ne pas être mentionné.

   ![Envoyer à](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Sélectionnez l’emplacement de la ressource, puis cliquez sur **Sélectionner un dossier**.
1. Lorsque vous avez trouvé la destination de votre choix, cliquez sur **Enregistrer**.

## Envoyer une nouvelle version à Experience Manager Assets

Vous pouvez ajouter une nouvelle version à un document que vous avez précédemment chargé vers Workfront. Pour plus d’informations, voir [Charger une nouvelle version d’un document](../../../documents/managing-documents/upload-new-document-version.md). Une fois la dernière version chargée, vous pouvez l’envoyer à Experience Manager Assets. Si un champ mappé dans Workfront a été modifié, la nouvelle version met à jour les métadonnées dans Experience Manager Assets lors de l’envoi.

Pour envoyer la version la plus récente, procédez comme suit :

1. Accédez à la zone **Documents** dans Workfront, puis recherchez le document.
1. Cliquez sur **Envoyer à**, puis sélectionnez l’intégration Experience Manager Assets que votre équipe d’administration a configurée.

   >[!NOTE]
   >
   >N’importe quel nom peut être choisi pour cette intégration. Experience Manager Assets peut donc ne pas être mentionné.

   ![Envoyer à](assets/copy-of-send-to-in-toolbar-350x149.png)

1. Cliquer sur **Enregistrer**. La nouvelle version enregistre au même emplacement que la version précédente.
