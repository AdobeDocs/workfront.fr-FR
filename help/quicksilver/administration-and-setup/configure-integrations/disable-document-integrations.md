---
title: Désactivation des intégrations de documents
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: As [!DNL anAdobe] [!DNL Workfront] administrateur, vous pouvez désactiver la connexion entre Workfront et l’un des fournisseurs tiers de documents.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 1%

---

# Désactivation des intégrations de documents

En tant que [!DNL Adobe] [!DNL Workfront] administrateur, vous pouvez désactiver la connexion entre [!DNL Workfront] et tous les fournisseurs tiers de documents.

Lorsque vous désactivez la connexion entre [!DNL Workfront] et un fournisseur de documents, les liens vers les documents disparaissent de [!DNL Workfront]. Les utilisateurs ne peuvent plus voir les documents liés, ils ne peuvent pas apporter de modifications aux documents via le [!DNL Workfront] et ne peuvent pas ajouter d’autres documents à ce fournisseur.

## Exigences d’accès

Les étapes de cet article doivent être les suivantes :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations sur [!DNL Workfront] administrateurs, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre [!DNL Workfront] administrateur.

## Désactivation des intégrations de fournisseurs cloud

Pour désactiver les intégrations de documents pour [!UICONTROL Gestion des actifs numériques Workfront], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM]:

1. Connectez-vous à [!DNL Workfront] as a [!DNL Workfront] administrateur.
1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Fournisseurs cloud]**.

1. Désélectionnez l’un des fournisseurs de cloud dont vous souhaitez vous déconnecter. [!DNL Workfront].
1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Les utilisateurs ne peuvent pas se connecter au fournisseur de cloud spécifique que vous avez désactivé et ils ne peuvent plus lier les documents de ce fournisseur de cloud à Workfront.

## Désactivez le [!DNL SharePoint] integration

1. Connectez-vous à [!DNL Workfront] as a [!DNL Workfront] administrateur.
1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Développer **[!UICONTROL Documents]**, puis cliquez sur **[!UICONTROL [!DNL SharePoint]Intégration]**.
1. Sélectionnez la [!DNL SharePoint] intégration que vous souhaitez désactiver.
1. Cliquez sur **[!UICONTROL Désactiver]**.\
   Les utilisateurs ne peuvent pas se connecter au [!DNL SharePoint] que vous avez désactivé et qu’ils ne peuvent plus lier des documents depuis [!DNL SharePoint] to [!DNL Workfront].

## Désactivation des intégrations personnalisées

1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur.
1. Cliquez sur le bouton **[!UICONTROL Menu Principal]** icon ![](assets/main-menu-icon.png) dans le coin supérieur droit de [!DNL Adobe Workfront], puis cliquez sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Intégration personnalisée]**.
1. Sélectionnez l’intégration personnalisée que vous souhaitez désactiver.
1. Cliquez sur **[!UICONTROL Désactiver]**.

   Les utilisateurs ne peuvent pas se connecter au fournisseur de documents tiers que vous avez désactivé et ils ne peuvent plus lier les documents de ce fournisseur de cloud à [!DNL Workfront].
