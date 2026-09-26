---
title: Désactiver les intégrations de documents
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: En tant [!DNL anAdobe]’administrateur [!DNL Workfront], vous pouvez désactiver la connexion entre Workfront et tout fournisseur de documents tiers.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
TQID: 'https://experienceleague.adobe.com/3tfxxth82eJEjEmdVD3AJFxl6B1m3EVKMQP9Gy4LC24'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 91%
---
# Désactiver les intégrations de documents

En tant qu’administrateur et administratrice [!DNL Adobe] [!DNL Workfront], vous pouvez désactiver la connexion entre [!DNL Workfront] et tous les fournisseurs tiers de documents.

Lorsque vous désactivez la connexion entre [!DNL Workfront] et un fournisseur de documents, les liens vers les documents disparaissent de [!DNL Workfront]. Les utilisateurs et utilisatrices ne peuvent plus voir les documents liés, ne peuvent pas apporter de modifications aux documents via les liens [!DNL Workfront], et ne peuvent pas ajouter d’autres documents à ce fournisseur.

## Conditions d’accès

+++Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table>
  <tr>
   <td>Package Adobe Workfront
   </td>
   <td> <p>Prime ou Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Licences Adobe Workfront
   </td>
   <td><p>Standard</p>
   <p>Plan</p>
   </td>
  </tr>
   <tr>
   <td>Configurations des niveaux d’accès
   </td>
   <td>Vous devez être administrateur ou administratrice [!DNL Workfront].
   </td>
  </tr>
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Désactiver les intégrations de fournisseur de services cloud

Pour désactiver les intégrations de documents pour la [!UICONTROL gestion des actifs numériques Workfront], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM] :

1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur ou administratrice de [!DNL Workfront].

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Fournisseurs de services cloud]**.

1. Désélectionnez l’un des fournisseurs de services cloud que vous souhaitez déconnecter de [!DNL Workfront].
1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Les utilisateurs et utilisatrices ne peuvent pas se connecter au fournisseur de services cloud spécifique que vous avez désactivé et ne peuvent plus lier les documents de ce fournisseur de services cloud à Workfront.

## Désactivez l’intégration [!DNL SharePoint]

1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur ou administratrice de [!DNL Workfront].

{{step-1-to-setup}}

1. Développez **[!UICONTROL Documents]**, puis cliquez sur **[!UICONTROL [!DNL SharePoint]Intégration]**.
1. Sélectionnez l’intégration [!DNL SharePoint] que vous souhaitez désactiver.
1. Cliquez sur **[!UICONTROL Désactiver]**.\
   Les utilisateurs et utilisatrices ne peuvent pas se connecter au site [!DNL SharePoint] que vous avez désactivé et ne peuvent plus lier des documents depuis [!DNL SharePoint] à [!DNL Workfront].

## Désactiver les intégrations personnalisées

1. Connectez vous à [!DNL Workfront] en tant qu’administrateur ou administratrice.

{{step-1-to-setup}}

1. Cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Intégration personnalisée]**.
1. Sélectionnez l’intégration personnalisée que vous souhaitez désactiver.
1. Cliquez sur **[!UICONTROL Désactiver]**.

   Les utilisateurs et utilisatrices ne peuvent pas se connecter au fournisseur tiers de documents que vous avez désactivé et ne peuvent plus lier les documents de ce fournisseur de services cloud à [!DNL Workfront].
