---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Activation d’Outlook pour une utilisation avec Workfront et SAML 2.0
description: Si vous activez l’authentification SAML 2.0 et souhaitez que vos utilisateurs puissent se connecter à Workfront à partir de Microsoft Outlook à l’aide de leurs informations d’identification SAML 2.0, vous devez activer SAML 2.0 pour s’authentifier dans les modules complémentaires Office.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 29%

---

# Activation d’Outlook pour une utilisation avec Workfront et SAML 2.0

Si vous activez l’authentification SAML 2.0 et souhaitez que vos utilisateurs puissent se connecter à Workfront à partir de Microsoft Outlook à l’aide de leurs informations d’identification SAML 2.0, vous devez activer SAML 2.0 pour s’authentifier dans les modules complémentaires Office.

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre entreprise utilise un portail d’authentification unique personnalisé.>
><!--
>or is enabled with Adobe IMS>
>-->
>Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront</td> 
   <td>N’importe quelle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice de Workfront.</p> <p><b>REMARQUE</b> : si vous n’avez toujours pas l’accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont un administrateur ou une administratrice Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier les niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Activation d’Outlook pour une utilisation avec Workfront et SAML 2.0

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Préférences**.

1. Dans la section **Sécurité**, assurez-vous que l’authentification **Autoriser l’authentification SAML 2.0 dans les modules complémentaires Office 365** est activée.

   Cette option permet l’incorporation de Workfront dans un Iframe uniquement pour les modules complémentaires Office 365. Cela n’ouvre pas de violation de détournement de clic, car aucun contenu cliquable n’est impliqué.

   Cette option est activée par défaut.

   >[!NOTE]
   >
   >Si vous activez l’option **Autoriser l’incorporation de Workfront dans un iframe**, l’option **Autoriser l’authentification SAML 2.0 dans les modules complémentaires Office 365** est grisée et activée.
   >
   >![](assets/if-you-enable.png)
   >

1. Cliquer sur **Enregistrer**.

   Les modifications que vous avez enregistrées ici affectent l’expérience de tous les utilisateurs dans Workfront.
