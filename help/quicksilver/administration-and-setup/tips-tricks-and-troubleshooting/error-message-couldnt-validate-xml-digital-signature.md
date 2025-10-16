---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Message d’erreur : impossible de valider la signature numérique XML'
description: Vous ne pouvez pas établir une connexion réussie à ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 97%

---

# Message d’erreur : impossible de valider la signature numérique XML

## Problème

Vous ne pouvez pas établir une connexion réussie à ADFS.

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>Si vous établissez une connexion de test réussie et que vous rencontrez toujours des problèmes, vous pourriez avoir des mappages d’attributs incorrects ou rencontrer des problèmes avec les ID de fédération. Contactez l’assistance clientèle pour toute question.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquet</td> 
   <td><p>Tous</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licence</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configurations des niveaux d’accès</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations, voir [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cause 1 : le certificat est incorrect.

### Solution

Récupérez manuellement le certificat de signature à partir du serveur ADFS :

1. Dans [!DNL Windows], cliquez sur **[!UICONTROL Démarrer]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion d’ADFS 2.0]**.\
   La boîte de dialogue Gestion d’ADFS 2.0 s’affiche.

1. Sélectionnez **[!UICONTROL Relation de confiance]** > **[!UICONTROL Parties de confiance]** dans le volet de gauche.

1. Cliquez avec le bouton droit sur **[!UICONTROL Parties de confiance]**, puis sélectionnez **[!UICONTROL Propriétés]**.

1. Cliquez sur l’onglet **[!UICONTROL Signature]**.
1. Cliquez sur le nom du certificat de signature, puis sur **[!UICONTROL Afficher]**.
1. Cliquez sur Copier vers **[!UICONTROL Fichier]**... et sélectionnez **[!UICONTROL Suivant]**.

1. Sélectionnez **[!UICONTROL Base-64 encodée x.509 (CER)]**, puis cliquez sur **[!UICONTROL Suivant]**.

1. Indiquez le nom du fichier, puis cliquez sur **[!UICONTROL Suivant]**.
1. Cliquez sur **[!UICONTROL Terminer]**.
1. Dans [!DNL Adobe Workfront], accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Système]** > **[!UICONTROL Authentification unique (SSO)]** et chargez manuellement le certificat de signature.

## Cause 2 : le certificat est signé à l’aide de DSA alors que [!DNL Workfront] attend une signature RSA.

### Solution

Recréez le certificat et utilisez la signature RSA au lieu de DSA.

## Cause 3 : les données XML sont incorrectes.

### Solution

Exportez et importez à nouveau les métadonnées XML à partir du système de gestion ADFS.

## Cause 4 : la requête n’a pas pu être exécutée en raison d’une erreur côté SAML.

### Solution

Contactez votre fournisseur SAML.
