---
title: Désactiver les intégrations de documents
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: En tant qu’administrateur de  [!DNL anAdobe] [!DNL Workfront], vous pouvez désactiver la connexion entre Workfront et tous les fournisseurs de documents tiers.
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: 78281bca-1fa1-4e78-96e5-70be12142bbd
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 30%

---

# Désactiver les intégrations de documents

En tant qu&#39;administrateur [!DNL Adobe] [!DNL Workfront], vous pouvez désactiver la connexion entre [!DNL Workfront] et n&#39;importe quel fournisseur tiers de documents.

Lorsque vous désactivez la connexion entre [!DNL Workfront] et un fournisseur de documents, les liens vers les documents disparaissent de [!DNL Workfront]. Les utilisateurs ne peuvent plus voir les documents liés, ils ne peuvent pas apporter de modifications aux documents par le biais des liens [!DNL Workfront] et ils ne peuvent pas ajouter d’autres documents à ce fournisseur.

## Conditions d’accès

Vous devez disposer des éléments suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations sur les administrateurs et les administratrices [!DNL Workfront], voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Accorder à un utilisateur ou à une utilisatrice un accès administratif complet</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur ou administratrice [!DNL Workfront].

## Désactivation des intégrations de fournisseurs cloud

Pour désactiver les intégrations de documents pour [!UICONTROL Workfront DAM], [!DNL Box], [!DNL Dropbox], [!DNL Google Drive], [!DNL Microsoft OneDrive], [!DNL WebDAM] :

1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur [!DNL Workfront].
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Fournisseurs cloud]**.

1. Désélectionnez les fournisseurs cloud que vous souhaitez déconnecter de [!DNL Workfront].
1. Cliquer sur **[!UICONTROL Enregistrer]**.

   Les utilisateurs ne peuvent pas se connecter au fournisseur de cloud spécifique que vous avez désactivé et ils ne peuvent plus lier les documents de ce fournisseur de cloud à Workfront.

## Désactivation de l’intégration [!DNL SharePoint]

1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur [!DNL Workfront].
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Développez **[!UICONTROL Documents]**, puis cliquez sur **[!UICONTROL [!DNL SharePoint]Intégration]**.
1. Sélectionnez l&#39;intégration [!DNL SharePoint] que vous souhaitez désactiver.
1. Cliquez sur **[!UICONTROL Désactiver]**.\
   Les utilisateurs ne peuvent pas se connecter au site [!DNL SharePoint] que vous avez désactivé et ils ne peuvent plus lier de documents de [!DNL SharePoint] à [!DNL Workfront].

## Désactivation des intégrations personnalisées

1. Connectez-vous à [!DNL Workfront] en tant qu’administrateur.
1. Cliquez sur l’icône **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’[!DNL Adobe Workfront], puis sur **[!UICONTROL Configuration]** ![](assets/gear-icon-settings.png).

1. Cliquez sur **[!UICONTROL Documents]** > **[!UICONTROL Intégration personnalisée]**.
1. Sélectionnez l’intégration personnalisée que vous souhaitez désactiver.
1. Cliquez sur **[!UICONTROL Désactiver]**.

   Les utilisateurs ne peuvent pas se connecter au fournisseur de documents tiers que vous avez désactivé et ils ne peuvent plus lier les documents de ce fournisseur de cloud à [!DNL Workfront].
