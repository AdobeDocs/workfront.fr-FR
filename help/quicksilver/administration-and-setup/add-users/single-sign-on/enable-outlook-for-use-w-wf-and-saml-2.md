---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Activation d’Outlook pour une utilisation avec Workfront et SAML 2.0
description: Si vous activez l’authentification SAML 2.0 et souhaitez que vos utilisateurs puissent se connecter à Workfront à partir de Microsoft Outlook à l’aide de leurs informations d’identification SAML 2.0, vous devez activer SAML 2.0 pour s’authentifier dans les modules complémentaires Office.
author: Caroline, Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---

# Activation d’Outlook pour une utilisation avec Workfront et SAML 2.0

Si vous activez l’authentification SAML 2.0 et souhaitez que vos utilisateurs puissent se connecter à Workfront à partir de Microsoft Outlook à l’aide de leurs informations d’identification SAML 2.0, vous devez activer SAML 2.0 pour s’authentifier dans les modules complémentaires Office.

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre entreprise utilise un portail d’authentification unique personnalisé.>
><!--
>or is enabled with Adobe IMS>
>-->
>Si vous avez besoin d’informations supplémentaires, contactez votre administrateur réseau ou informatique.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès</td> 
   <td> <p>Vous devez être un administrateur Workfront.</p> <p><b>REMARQUE</b>: Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Activation d’Outlook pour une utilisation avec Workfront et SAML 2.0

1. Cliquez sur **Configuration** près du coin supérieur droit d’Adobe Workfront dans la barre de navigation globale.
1. Cliquez sur **Système** > **Préférences**.

1. Dans le **Sécurité** , assurez-vous que la variable **Autorisation de l’authentification SAML 2.0 dans les modules complémentaires Office 365** est activée.

   Cette option permet l’incorporation de Workfront dans un Iframe uniquement pour les modules complémentaires Office 365. Cela n’ouvre pas de violation de détournement de clic, car aucun contenu cliquable n’est impliqué.

   Cette option est activée par défaut.

   >[!NOTE]
   >
   >Si vous activez l’option **Autorisation de l’incorporation de Workfront dans un iframe**, l’option **Autorisation de l’authentification SAML 2.0 dans les modules complémentaires Office 365** est grisée et activée.
   >
   >![](assets/if-you-enable.png)

1. Cliquer sur **Enregistrer**.

   Les modifications que vous avez enregistrées ici affectent l’expérience de tous les utilisateurs dans Workfront.
