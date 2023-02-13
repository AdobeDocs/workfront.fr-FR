---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Message d''erreur : Erreur SAML 2.0 : Principal StatusCode'''
description: Vous ne pouvez pas établir une connexion réussie à ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Message d’erreur : Erreur SAML 2.0 : Principal StatusCode

## Problème

Vous ne pouvez pas établir une connexion réussie à ADFS.

![SAML_2.0_Error_Principal_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

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

## Cause 1 : L’algorithme de hachage sécurisé est défini sur SHA-256

### Solution

1. Sous Windows, cliquez sur **[!UICONTROL Début]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion d’ADFS 2.0]**.\
   La boîte de dialogue Gestion ADFS 2.0 s’affiche.

1. Sélectionner **[!UICONTROL Relation de confiance]** > **[!UICONTROL Confiance des parties]** dans le volet de gauche.

1. Clic droit sur la confiance de la partie de confiance liée à [!DNL Adobe Workfront], puis sélectionnez **[!UICONTROL Propriétés]**.
1. Cliquez sur le bouton **[!UICONTROL Avancé]** , puis sélectionnez **[!UICONTROL SHA-1]** de la **[!UICONTROL Algorithme de hachage sécurisé]** menu déroulant.\
   ![](assets/1-350x287.png)

## Cause 2 : Le certificat de signature ADFS est sur le point d’expirer et a été remplacé par un nouveau certificat avec des dates de chevauchement

### Solution

Le [!DNL Workfront] La page de configuration SSO répertorie la date d’expiration du certificat. Si le certificat est sur le point d’expirer, vous devez extraire manuellement le nouveau certificat de signature du serveur ADFS :

1. Sous Windows, cliquez sur **[!UICONTROL Début]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion d’ADFS 2.0]**.\
   La boîte de dialogue Gestion ADFS 2.0 s’affiche.

1. Sélectionner **[!UICONTROL Relation de confiance]** > **[!UICONTROL Confiance des parties]** dans le volet de gauche.

1. Clic droit sur la confiance de la partie de confiance liée à [!DNL Workfront], puis sélectionnez **[!UICONTROL Propriétés]**.
1. Cliquez sur le bouton **[!UICONTROL Signature]** .
1. Cliquez sur le nom du certificat de signature, puis sur **[!UICONTROL Affichage]**.
1. Cliquez sur Copier pour **[!UICONTROL Fichier]**... et sélectionnez **[!UICONTROL Suivant]**.

1. Sélectionner **[!UICONTROL Base-64 codée x.509 (CER)]**, puis cliquez sur **[!UICONTROL Suivant]**.

1. Indiquez le nom du fichier, puis cliquez sur **[!UICONTROL Suivant]**.
1. Cliquez sur **[!UICONTROL Terminer]**.
1. Dans [!DNL Workfront], accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Système]** > **[!UICONTROL Authentification unique (SSO)]** et chargez manuellement le certificat de signature.

## Cause 3 : Échec de la vérification de révocation du certificat

La solution dépend de la version de [!DNL Microsoft] ADFS que vous utilisez. Consulter [!DNL Microsoft]Documentation de pour obtenir les commandes appropriées pour votre version.
