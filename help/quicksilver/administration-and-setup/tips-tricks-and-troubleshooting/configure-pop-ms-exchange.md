---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configuration de POP dans Microsoft Exchange
description: Un compte de messagerie POP dans [!DNL Microsoft Exchange] est désactivé.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 16%

---

# Configurer POP dans [!DNL Microsoft Exchange]

## Problème

Un compte de messagerie POP dans [!DNL Microsoft Exchange] est désactivé.

## Solution

Avant de passer du temps à résoudre le problème, assurez-vous que le compte POP de l’utilisateur est correctement configuré. Si vous rencontrez des problèmes après avoir confirmé que le compte POP est correctement configuré, contactez le support [!DNL Microsoft] ou l&#39;un de leurs partenaires pour obtenir une aide supplémentaire.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

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

## Configurer POP dans [!DNL Microsoft Exchange]

>[!NOTE]
>
>Les étapes suivantes peuvent être utilisées comme guide général pour configurer le protocole POP dans [!DNL Microsoft Exchange] pour un système de production [!DNL Workfront]. Les étapes peuvent varier sensiblement en fonction de la version de l’Exchange ou des modifications de code effectuées par Microsoft.

1. Démarrez et activez le service POP3 sur le serveur Exchange 2010.

   >[!NOTE]
   >
   >Par défaut, le service POP3 n’est pas démarré.

   1. Démarrez le gestionnaire de serveur de [!DNL Microsoft].
   1. Accédez à : **[!UICONTROL Server Manager]** > **[!UICONTROL Configuration]** >**[!UICONTROL Pare-feu Windows avec sécurité avancée]** > **[!UICONTROL Services]**.

   1. Cliquez avec le bouton droit de la souris sur **[!DNL Microsoft Exchange]POP3**, puis cliquez sur **[!UICONTROL Propriétés]**.

   1. (Conditionnel) Pour vous assurer que le service POP démarre automatiquement, dans l’onglet **[!UICONTROL Général]**, définissez le type **[!UICONTROL Démarrage]** sur [!UICONTROL Automatique].

1. Configurez POP3 pour le serveur.

   1. Démarrez la console de gestion [!DNL Microsoft Exchange].
   1. Naviguez : [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuration du serveur]** > **[!UICONTROL Accès client]**.

   1. Sélectionnez **[!UICONTROL POP3]**.

      POP3 figure dans la liste des onglets [!UICONTROL POP3] et [!UICONTROL IMAP4] .

   1. Sur le côté droit, sous **[!UICONTROL Actions]**, sélectionnez **[!UICONTROL POP3]**, puis sélectionnez **[!UICONTROL Propriétés]**.

   1. Cliquez sur **[!UICONTROL Propriétés POP3]**, puis ouvrez l’onglet **[!UICONTROL Liaison]**.

      Toutes les adresses IP et numéros de port disponibles configurés pour le serveur POP3 s’affichent. La zone supérieure affiche le message Non chiffré et la zone inférieure affiche l’adresse IP et les ports pour les connexions SSL/TLS.

   1. Cliquez sur **[!UICONTROL POP3 Properties]**, puis ouvrez l’onglet **[!UICONTROL Authentication]**.

   1. **[!UICONTROL Sélectionnez Secure]** login.

      Une connexion TLS est requise pour que le client s’authentifie auprès du serveur.

1. Activez ou autorisez les utilisateurs à se connecter au protocole POP.

   1. Démarrez la console de gestion [!DNL Microsoft Exchange].
   1. Naviguez : [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuration du destinataire]** > **[!UICONTROL Boîte aux lettres]**.

      Une liste de boîtes aux lettres ou d’utilisateurs s’affiche.

   1. Mettez en surbrillance l’email utilisé dans [!DNL Workfront].
   1. Sur le côté droit, sous **[!UICONTROL Actions]**, sélectionnez **[!UICONTROL Propriétés]**, puis ouvrez l’onglet **[!UICONTROL Fonctionnalités de boîte aux lettres]**.

   1. (Conditionnel) Si POP3 est désactivé, cliquez sur **[!UICONTROL POP3]**, puis sur **[!UICONTROL Activer]**.

      Une liste de boîtes aux lettres ou d’utilisateurs s’affiche.

1. Configurez les connecteurs de réception.

   1. Démarrez la console de gestion [!DNL Microsoft Exchange].
   1. Naviguez : [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuration du serveur]** > **[!UICONTROL Transport Hub]**.

      Une liste des connecteurs de réception s’affiche.

   1. Vérifiez que le connecteur de réception *Client* *EX01* est activé.

      Où *Client* *EX01* est le nom de votre serveur d’Exchange.

   1. Sélectionnez *Client EX01*, puis, à droite sous **[!UICONTROL Actions]**, sélectionnez **[!UICONTROL Propriétés]**.

   1. Ouvrez l’onglet **[!UICONTROL Authentication]** , puis assurez-vous que **[!UICONTROL Transport Layer Security (TLS)]** est coché.

      >[!NOTE]
      >
      >Pour disposer de l’authentification de base, vous devrez peut-être démarrer TLS et l’authentification Windows intégrée.
