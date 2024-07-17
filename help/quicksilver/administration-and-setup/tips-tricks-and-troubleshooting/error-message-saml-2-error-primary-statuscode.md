---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Message d’erreur : erreur SAML 2.0 : Principal StatusCode'
description: Vous ne pouvez pas établir une connexion réussie à ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 20%

---

# Message d’erreur : erreur SAML 2.0 : Principal StatusCode

## Problème

Vous ne pouvez pas établir une connexion réussie à ADFS.

![SAML_2.0_Error_Principal_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>Si vous établissez une connexion de test réussie et que vous rencontrez toujours des problèmes, vous pouvez rencontrer des mappages d’attributs ou des problèmes avec les ID de fédération. Contactez l’assistance clientèle pour toute question.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroyer un accès administratif intégral pour les utilisateurs et utilisatrices</a>.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas un accès, demandez à l’administration [!DNL Workfront] si elle a défini des restrictions supplémentaires dans votre niveau d’accès. Pour savoir comment un administrateur ou une administratrice [!DNL Workfront] peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Cause 1 : l’algorithme de hachage sécurisé est défini sur SHA-256

### Solution

1. Sous Windows, cliquez sur **[!UICONTROL Démarrer]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion ADFS 2.0]**.\
   La boîte de dialogue Gestion ADFS 2.0 s’affiche.

1. Sélectionnez **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trtrust]** dans le volet de gauche.

1. Cliquez avec le bouton droit de la souris sur la confiance de la partie de confiance associée à [!DNL Adobe Workfront], puis sélectionnez **[!UICONTROL Propriétés]**.
1. Cliquez sur l’onglet **[!UICONTROL Avancé]** , puis sélectionnez **[!UICONTROL SHA-1]** dans le menu déroulant **[!UICONTROL algorithme de hachage sécurisé]** .\
   ![](assets/1-350x287.png)

## Cause 2 : le certificat de signature ADFS est sur le point d’expirer et a été remplacé par un nouveau certificat avec des dates de chevauchement

### Solution

La page de configuration SSO [!DNL Workfront] répertorie la date d’expiration du certificat. Si le certificat est sur le point d’expirer, vous devez extraire manuellement le nouveau certificat de signature du serveur ADFS :

1. Sous Windows, cliquez sur **[!UICONTROL Démarrer]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion ADFS 2.0]**.\
   La boîte de dialogue Gestion ADFS 2.0 s’affiche.

1. Sélectionnez **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trtrust]** dans le volet de gauche.

1. Cliquez avec le bouton droit de la souris sur la confiance de la partie de confiance associée à [!DNL Workfront], puis sélectionnez **[!UICONTROL Propriétés]**.
1. Cliquez sur l’onglet **[!UICONTROL Signature]** .
1. Cliquez sur le nom du certificat de signature, puis sur **[!UICONTROL Afficher]**.
1. Cliquez sur Copier vers **[!UICONTROL Fichier]**... et sélectionnez **[!UICONTROL Suivant]**.

1. Sélectionnez **[!UICONTROL Base-64 codé x.509 (CER)]**, puis cliquez sur **[!UICONTROL Suivant]**.

1. Indiquez le nom du fichier, puis cliquez sur **[!UICONTROL Suivant]**.
1. Cliquez sur **[!UICONTROL Terminer]**.
1. Dans [!DNL Workfront], accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Système]** > **[!UICONTROL Connexion unique (SSO)]** et chargez manuellement le certificat de signature.

## Cause 3 : la vérification de révocation du certificat échoue

La solution dépend de la version de [!DNL Microsoft] ADFS que vous utilisez. Consultez la documentation de [!DNL Microsoft] pour obtenir les commandes appropriées à votre version.
