---
title: Lier des ressources et des dossiers à l’aide du connecteur amélioré
description: Vous pouvez lier une ressource ou un dossier de Experience Manager Assets à n’importe quel objet Workfront prenant en charge les documents.
author: Courtney
draft: Probably
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 35c80f6a-419b-4237-8139-f59ab7bbd5c7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Lier des ressources et des dossiers à l’aide du connecteur amélioré

Vous pouvez lier une ressource ou un dossier de Experience Manager Assets à n’importe quel objet Workfront prenant en charge les documents. Les ressources envoyées à partir de Experience Manager Assets ne sont pas prises en compte dans le stockage global de documents dans Workfront. Les documents téléchargés et envoyés de Workfront à Experience Manager Assets sont pris en compte dans le stockage global.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Tous</p> </td> 
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
   <td> <p>Affichage de l’accès ou d’un niveau supérieur sur un document</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Conditions préalables

Avant de commencer, vous devez

* Installation de Workfront for Experience Manager Enhanced Connector

## Liaison d’une ressource à partir de Experience Manager Assets

Vous pouvez lier une ressource de Experience Manager Assets à Workfront. Une fois la ressource liée, vous pouvez

* [BAT d’une ressource liée pour Experience Manager Assets](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/enhanced-connector-proof-asset.md)
* [Télécharger une nouvelle version d’un document](../../../documents/managing-documents/upload-new-document-version.md)

Pour lier une ressource à Experience Manager Assets :

1. Accédez au **Documents** dans Workfront où vous souhaitez ajouter le document.
1. Cliquez sur **Ajouter**, puis sélectionnez l’intégration Experience Manager Assets que votre administrateur doit configurer.

   >[!NOTE]
   >
   >N’importe quel nom peut être choisi pour cette intégration. Il peut donc ne pas mentionner spécifiquement Experience Manager Assets.

1. Sélectionnez les ressources de votre choix.

   ![](assets/select-an-asset.png)

1. Cliquez sur **Lien**.

## Lier un dossier à partir de Experience Manager Assets

Les autorisations d’affichage de ressources individuelles dans un dossier dépendent des autorisations Experience Manager Assets.

Pour lier un dossier à Experience Manager Assets :

1. Accédez au **Documents** dans Workfront où vous souhaitez ajouter le document.
1. Cliquez sur **Ajouter**, puis sélectionnez l’intégration Experience Manager Assets que votre administrateur doit configurer.

   >[!NOTE]
   >
   >N’importe quel nom peut être choisi pour cette intégration. Il peut donc ne pas mentionner spécifiquement Experience Manager Assets.

1. Sélectionnez les dossiers de votre choix.

   ![](assets/select-a-folder.png)

1. Cliquez sur **Lien**.

## Lier une nouvelle version de Experience Manager Assets

Vous pouvez extraire une nouvelle ressource de Experience Manager Assets et l’ajouter à une ressource existante en tant que nouvelle version dans Workfront. Si le document est déjà lié et qu’une nouvelle version est ajoutée dans Experience Manager Assets, la nouvelle version apparaît automatiquement dans Workfront.

>[!TIP]
>
>Vous pouvez afficher toutes les versions d’une ressource si vous accédez à **Détails du document** > **Versions**.

Pour lier une nouvelle version à partir de Experience Manager Assets :

1. Accédez au **Documents** dans Workfront où vous souhaitez ajouter le document.
1. Sélectionnez la ressource à remplacer par une nouvelle version. Vous ne pouvez pas créer de version d’une ressource dans un dossier lié.
1. Cliquez sur **Ajouter**, puis sélectionnez l’intégration Experience Manager Assets que votre administrateur doit configurer.

   >[!NOTE]
   >
   >N’importe quel nom peut être choisi pour cette intégration. Il peut donc ne pas mentionner spécifiquement Experience Manager Assets.

1. Sélectionnez la ressource de votre choix.

   ![](assets/select-an-asset.png)

1. Cliquez sur **Lien**.
