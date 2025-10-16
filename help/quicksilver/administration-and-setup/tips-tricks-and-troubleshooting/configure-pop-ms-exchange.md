---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configurer POP dans Microsoft Exchange
description: Un compte e-mail POP dans  [!DNL Microsoft Exchange]  est désactivé.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 99%

---

# Configurer POP dans [!DNL Microsoft Exchange]

## Problème

Un compte e-mail POP dans [!DNL Microsoft Exchange] est désactivé.

## Solution

Avant de passer du temps à résoudre le problème, assurez-vous que le compte POP de la personne est correctement configuré. Si vous continuez à rencontrer des problèmes après avoir confirmé que le compte POP est correctement configuré, contactez l’assistance de [!DNL Microsoft] ou l’un de ses partenaires pour obtenir une aide supplémentaire.

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

## Configurer POP dans [!DNL Microsoft Exchange]

>[!NOTE]
>
>Les étapes suivantes peuvent servir de guide général pour la configuration de POP dans [!DNL Microsoft Exchange] pour un système de production [!DNL Workfront]. Les étapes peuvent différer de manière significative en fonction de la version d’Exchange ou des modifications de code apportées par Microsoft.

1. Commencez par activer le service POP3 sur le serveur Exchange 2010.

   >[!NOTE]
   >
   >Par défaut, le service POP3 n’est pas activé.

   1. Démarrez le gestionnaire de serveur de [!DNL Microsoft].
   1. Accédez à : **[!UICONTROL Gestionnaire de serveur]** > **[!UICONTROL Configuration]** > **[!UICONTROL Pare-feu Windows avec sécurité avancée]** > **[!UICONTROL Services]**.

   1. Cliquez avec le bouton droit de la souris sur **[!DNL Microsoft Exchange]POP3**, puis cliquez sur **[!UICONTROL Propriétés]**.

   1. (Le cas échéant) Pour garantir le démarrage automatique du service POP, dans l’onglet **[!UICONTROL Général]**, définissez le type de **[!UICONTROL Démarrage]** sur [!UICONTROL Automatique].

1. Configurer POP3 pour le serveur.

   1. Démarrez la console de gestion [!DNL Microsoft Exchange].
   1. Accédez à : [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuration du serveur]** > **[!UICONTROL Accès client]**.

   1. Choisissez **[!UICONTROL POP3]**.

      POP3 figure dans la liste sous les onglets [!UICONTROL POP3] et [!UICONTROL IMAP4].

   1. Sur le côté droit, sous **[!UICONTROL Actions]**, sélectionnez **[!UICONTROL POP3]**, puis **[!UICONTROL Propriétés]**.

   1. Cliquez sur **[!UICONTROL Propriétés POP3]**, puis ouvrez l’onglet **[!UICONTROL Liaison]**.

      Toutes les adresses IP disponibles et tous les numéros de port configurés pour le serveur POP3 s’affichent. La zone du haut indique les connexions non chiffrées et la zone du bas indique l’IP et les ports pour les connexions SSL/TLS.

   1. Cliquez sur **[!UICONTROL Propriétés POP3]**, puis ouvrez l’onglet **[!UICONTROL Authentification]**.

   1. **[!UICONTROL Sélectionnez une connexion Sécurisée]**.

      Une connexion TLS est nécessaire pour que le client ou la cliente puisse s’authentifier auprès du serveur.

1. Activez ou autorisez les personnes à se connecter à POP.

   1. Démarrez la console de gestion [!DNL Microsoft Exchange].
   1. Accédez à : [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuration des personnes destinataires]** > **[!UICONTROL Boîte aux lettres]**.

      Une liste de boîtes de réception ou d’utilisateurs et utilisatrices s’affiche.

   1. Mettez en surbrillance l’e-mail utilisé dans [!DNL Workfront].
   1. Sur le côté droit, sous **[!UICONTROL Actions]**, sélectionnez **[!UICONTROL Propriétés]**, puis ouvrez l’onglet **[!UICONTROL Caractéristiques de la boîte de réception]**.

   1. (Le cas échéant) Si POP3 est désactivé, cliquez sur **[!UICONTROL POP3]**, puis sur **[!UICONTROL Activer]**.

      Une liste de boîtes de réception ou d’utilisateurs et utilisatrices s’affiche.

1. Configurez les connecteurs de réception.

   1. Démarrez la console de gestion [!DNL Microsoft Exchange].
   1. Accédez à : [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuration du serveur]** > **[!UICONTROL Hub Transport]**.

      Une liste des connecteurs de réception s’affiche.

   1. Confirmez que le connecteur de réception *Client* *EX01* est activé.

      Où *Client* *EX01* est le nom de votre serveur Exchange.

   1. Sélectionnez *Client EX01*, puis à droite sous **[!UICONTROL Actions]**, sélectionnez **[!UICONTROL Propriétés]**.

   1. Ouvrez l’onglet **[!UICONTROL Authentification]**, puis assurez-vous que l’option **[!UICONTROL Transport Layer Security (TLS)]** est cochée.

      >[!NOTE]
      >
      >Pour disposer de l’authentification de base, vous devrez peut-être lancer TLS et l’authentification intégrée de Windows.
