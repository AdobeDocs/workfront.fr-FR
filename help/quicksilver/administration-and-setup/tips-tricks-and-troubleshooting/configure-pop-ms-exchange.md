---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configuration de POP dans Microsoft Exchange
description: Un compte de messagerie POP dans [!DNL Microsoft Exchange] est désactivée.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Configuration de la méthode POP [!DNL Microsoft Exchange]

## Problème

Un compte de messagerie POP dans [!DNL Microsoft Exchange] est désactivée.

## Solution

Avant de passer du temps à résoudre le problème, assurez-vous que le compte POP de l’utilisateur est correctement configuré. Si vous rencontrez des problèmes après avoir confirmé que le compte POP est correctement configuré, contactez [!DNL Microsoft] Pour obtenir de l’aide supplémentaire, contactez l’un de leurs partenaires.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

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

## Configuration de la méthode POP [!DNL Microsoft Exchange]

>[!NOTE]
>
>Les étapes suivantes peuvent être utilisées comme guide général pour configurer POP dans [!DNL Microsoft Exchange] pour une production [!DNL Workfront] système. Les étapes peuvent varier sensiblement en fonction de la version d’Exchange ou des modifications de code effectuées par Microsoft.

1. Démarrez et activez le service POP3 sur le serveur Exchange 2010.

   >[!NOTE]
   >
   >Par défaut, le service POP3 n’est pas démarré.

   1. Début [!DNL Microsoft]Gestionnaire de serveur de .
   1. Naviguer : **[!UICONTROL Gestionnaire de serveur]** > **[!UICONTROL Configuration]** >**[!UICONTROL Pare-feu Windows avec sécurité avancée]** > **[!UICONTROL Services]**.

   1. Clic droit **[!DNL Microsoft Exchange]POP3**, puis cliquez sur **[!UICONTROL Propriétés]**.

   1. (Conditionnel) Pour vous assurer que le service POP démarre automatiquement, sur la page **[!UICONTROL Général]** , définissez **[!UICONTROL Démarrage]** saisir [!UICONTROL Automatique].

1. Configurez POP3 pour le serveur.

   1. Démarrez le [!DNL Microsoft Exchange] Console de gestion.
   1. Naviguer : [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuration du serveur]** > **[!UICONTROL Accès client]**.

   1. Choisir **[!UICONTROL POP3]**.

      POP3 figure dans la liste sous [!UICONTROL POP3] et [!UICONTROL IMAP4] onglets.

   1. Sur le côté droit sous **[!UICONTROL Actions]**, sélectionnez **[!UICONTROL POP3]**, puis choisissez **[!UICONTROL Propriétés]**.

   1. Cliquez sur **[!UICONTROL Propriétés POP3]**, puis ouvrez le **[!UICONTROL Liaison]** .

      Toutes les adresses IP et numéros de port disponibles configurés pour le serveur POP3 s’affichent. La zone supérieure affiche le message Non chiffré et la zone inférieure affiche l’adresse IP et les ports pour les connexions SSL/TLS.

   1. Cliquez sur **[!UICONTROL Propriétés POP3]**, puis ouvrez le **[!UICONTROL Authentification]** .

   1. **[!UICONTROL Sélectionnez Sécurisé]** connectez-vous.

      Une connexion TLS est requise pour que le client s’authentifie auprès du serveur.

1. Activez ou autorisez les utilisateurs à se connecter au protocole POP.

   1. Démarrez le [!DNL Microsoft Exchange] Console de gestion.
   1. Naviguer : [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuration des destinataires]** > **[!UICONTROL Mailbox]**.

      Une liste de boîtes aux lettres ou d’utilisateurs s’affiche.

   1. Mettre en surbrillance l’email utilisé dans [!DNL Workfront].
   1. Sur le côté droit sous **[!UICONTROL Actions]**, sélectionnez **[!UICONTROL Propriétés]**, puis ouvrez le **[!UICONTROL Fonctionnalités de boîte aux lettres]** .

   1. (Conditionnel) Si POP3 est désactivé, cliquez sur **[!UICONTROL POP3]**, puis cliquez sur **[!UICONTROL Activer]**.

      Une liste de boîtes aux lettres ou d’utilisateurs s’affiche.

1. Configurez les connecteurs de réception.

   1. Début [!DNL Microsoft Exchange] Console de gestion.
   1. Naviguer : [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuration du serveur]** > **[!UICONTROL Transport Hub]**.

      Une liste des connecteurs de réception s’affiche.

   1. Confirmation du connecteur de réception *Client* *EX01* est activée.

      Où *Client* *EX01* est le nom de votre serveur Exchange.

   1. Sélectionner *Client EX01*, puis sur la droite sous **[!UICONTROL Actions]**, sélectionnez **[!UICONTROL Propriétés]**.

   1. Ouvrez le **[!UICONTROL Authentification]** , puis assurez-vous de **[!UICONTROL Transport Layer Security (TLS)]** est cochée.

      >[!NOTE]
      >
      >Pour disposer de l’authentification de base, vous devrez peut-être démarrer TLS et l’authentification Windows intégrée.
