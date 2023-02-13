---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Message d’erreur : Impossible de valider la signature numérique XML"
description: Vous ne pouvez pas établir une connexion réussie à ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Message d’erreur : Impossible de valider la signature numérique XML

## Problème

Vous ne pouvez pas établir une connexion réussie à ADFS.

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>Si vous établissez une connexion de test réussie et que vous rencontrez toujours des problèmes, vous pouvez rencontrer des mappages d’attributs ou des problèmes avec les ID de fédération. Contactez l’assistance clientèle pour toute question.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cause 1 : Le certificat est incorrect

### Solution

Récupérez manuellement le certificat de signature à partir du serveur ADFS :

1. Dans [!DNL Windows], cliquez sur **[!UICONTROL Début]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion d’ADFS 2.0]**.\
   La boîte de dialogue Gestion ADFS 2.0 s’affiche.

1. Sélectionner **[!UICONTROL Relation de confiance]** > **[!UICONTROL Confiance des parties]** dans le volet de gauche.

1. Cliquez avec le bouton droit de la souris sur **[!UICONTROL Confiance du parti de confiance]**, puis sélectionnez **[!UICONTROL Propriétés]**.

1. Cliquez sur le bouton **[!UICONTROL Signature]** .
1. Cliquez sur le nom du certificat de signature, puis sur **[!UICONTROL Affichage]**.
1. Cliquez sur Copier pour **[!UICONTROL Fichier]**... et sélectionnez **[!UICONTROL Suivant]**.

1. Sélectionner **[!UICONTROL Base-64 codée x.509 (CER)]**, puis cliquez sur **[!UICONTROL Suivant]**.

1. Indiquez le nom du fichier, puis cliquez sur **[!UICONTROL Suivant]**.
1. Cliquez sur **[!UICONTROL Terminer]**.
1. Dans [!DNL Adobe Workfront], accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Système]** > **[!UICONTROL Authentification unique (SSO)]** et chargez manuellement le certificat de signature.

## Cause 2 : Le certificat est signé à l’aide de DSA lorsque [!DNL Workfront] attend une signature RSA

### Solution

Recréez le certificat et utilisez la signature RSA au lieu de la DSA.

## Cause 3 : Données XML incorrectes

### Solution

Réexportez et réimportez les métadonnées XML à partir du système de gestion ADFS.

## Cause 4 : La requête n’a pas pu être effectuée en raison d’une erreur côté SAML.

### Solution

Contactez votre fournisseur SAML.
