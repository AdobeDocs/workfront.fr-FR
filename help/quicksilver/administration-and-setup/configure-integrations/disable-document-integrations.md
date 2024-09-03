---
title: Désactiver les intégrations de documents
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: En tant qu’administrateur et administratrice  [!DNL anAdobe] [!DNL Workfront], vous pouvez désactiver la connexion entre Workfront et l’un des fournisseurs tiers de documents.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
author: Courtney, Becky
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 98%

---

# Désactiver les intégrations de documents

En tant qu’administrateur et administratrice [!DNL Adobe] [!DNL Workfront], vous pouvez désactiver la connexion entre [!DNL Workfront] et tous les fournisseurs tiers de documents.

Lorsque vous désactivez la connexion entre [!DNL Workfront] et un fournisseur de documents, les liens vers les documents disparaissent de [!DNL Workfront]. Les utilisateurs et utilisatrices ne peuvent plus voir les documents liés, ne peuvent pas apporter de modifications aux documents via les liens [!DNL Workfront], et ne peuvent pas ajouter d’autres documents à ce fournisseur.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations sur les administrateurs et les administratrices [!DNL Workfront], voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à un utilisateur ou à une utilisatrice un accès administratif complet</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez l’administration [!DNL Workfront].

+++

## Désactiver les intégrations de fournisseur de documents

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
