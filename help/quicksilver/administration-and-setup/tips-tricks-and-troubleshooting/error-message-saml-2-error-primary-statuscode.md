---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Message d’erreur : erreur SAML 2.0 : Principal StatusCode'
description: Vous ne pouvez pas établir une connexion réussie à ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 97%

---

# Message d’erreur : Erreur SAML 2.0 : Code de statut principal

## Problème

Vous ne pouvez pas établir une connexion réussie à ADFS.

![SAML_2.0_Error_Primary_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

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

## Cause 1 : l’algorithme de hachage sécurisé est défini sur SHA-256.

### Solution

1. Sous Windows, cliquez sur **[!UICONTROL Démarrer]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion d’ADFS 2.0]**.\
   La boîte de dialogue Gestion d’ADFS 2.0 s’affiche.

1. Sélectionnez **[!UICONTROL Relation de confiance]** > **[!UICONTROL Parties de confiance]** dans le volet de gauche.

1. Cliquez avec le bouton droit de la souris sur sur la partie de confiance liée à [!DNL Adobe Workfront], puis sélectionnez **[!UICONTROL Propriétés]**.
1. Cliquez sur l’onglet **[!UICONTROL Avancé]**, puis sélectionnez **[!UICONTROL SHA-1]** dans le menu déroulant **[!UICONTROL Algorithme de hachage sécurisé]**.
   ![SHA-1](assets/1-350x287.png)

## Cause 2 : le certificat de signature ADFS est sur le point d’expirer et a été remplacé par un nouveau certificat avec des chevauchements de dates.

### Solution

La page de configuration SSO de [!DNL Workfront] répertorie la date d’expiration du certificat. Si le certificat est sur le point d’expirer, vous devez extraire manuellement le nouveau certificat de signature du serveur ADFS :

1. Sous Windows, cliquez sur **[!UICONTROL Démarrer]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion d’ADFS 2.0]**.\
   La boîte de dialogue Gestion d’ADFS 2.0 s’affiche.

1. Sélectionnez **[!UICONTROL Relation de confiance]** > **[!UICONTROL Parties de confiance]** dans le volet de gauche.

1. Cliquez avec le bouton droit de la souris sur la partie de confiance liée à [!DNL Workfront], puis sélectionnez **[!UICONTROL Propriétés]**.
1. Cliquez sur l’onglet **[!UICONTROL Signature]**.
1. Cliquez sur le nom du certificat de signature, puis sur **[!UICONTROL Afficher]**.
1. Cliquez sur Copier vers **[!UICONTROL Fichier]**... et sélectionnez **[!UICONTROL Suivant]**.

1. Sélectionnez **[!UICONTROL Base-64 encodée x.509 (CER)]**, puis cliquez sur **[!UICONTROL Suivant]**.

1. Indiquez le nom du fichier, puis cliquez sur **[!UICONTROL Suivant]**.
1. Cliquez sur **[!UICONTROL Terminer]**.
1. Dans [!DNL Workfront], accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Système]** > **[!UICONTROL Authentification unique (SSO)]** et chargez manuellement le certificat de signature.

## Cause 3 : la vérification de révocation du certificat a échoué.

La solution dépend de la version de l’ADFS de [!DNL Microsoft] que vous utilisez. Consultez la documentation de [!DNL Microsoft] pour obtenir les commandes appropriées pour votre version.
