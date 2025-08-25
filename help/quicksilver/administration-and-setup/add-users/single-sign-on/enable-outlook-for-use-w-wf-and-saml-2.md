---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Activer Outlook à utiliser avec Workfront et SAML 2.0
description: Si vous activez l’authentification SAML 2.0 et que vous souhaitez que vos utilisateurs et utilisatrices puissent se connecter à Workfront à partir de Microsoft Outlook en utilisant leurs informations d’identification SAML 2.0, vous devez activer SAML 2.0 pour l’authentification dans les modules complémentaires d’Office.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8a55d364-962a-4eef-8968-b2233a71cf31
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 70%

---

# Activer Outlook pour une utilisation avec Workfront et SAML 2.0

>[!IMPORTANT]
>
>[Microsoft est en train de désactiver la prise en charge des jetons Exchange Online hérités](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) actuellement utilisés par le complément Workfront Outlook pour l&#39;authentification. Cette modification apportée par Microsoft a déjà commencé à affecter les clients et continuera à être déployée par phases jusqu’en octobre 2025.
>
>* **Une fois que Microsoft a complètement désactivé ces jetons, l’intégration de Workfront pour Microsoft Outlook ne fonctionne plus.**
>
>Dans le cadre de cette modification, Microsoft a pris la décision de modifier la manière dont les jetons sont réactivés. Après le **30 juin 2025**, les administrateurs ne pourront plus réactiver les jetons eux-mêmes. Seule la prise en charge de Microsoft peut accorder des exceptions. **Le 1er octobre 2025, les jetons hérités seront désactivés pour tous les clients. Les exceptions ne seront pas accordées.**

Si vous activez l’authentification SAML 2.0 et que vous souhaitez que vos utilisateurs et utilisatrices puissent se connecter à Workfront à partir de Microsoft Outlook en utilisant leurs informations d’identification SAML 2.0, vous devez activer SAML 2.0 pour l’authentification dans les modules complémentaires d’Office.

>[!NOTE]
>
>Cette option n’est pas disponible si l’instance Workfront de votre organisation utilise un portail SSO personnalisé.>
><!--
>or is enabled with Adobe IMS>
>-->
>Consultez votre administrateur ou administratrice réseau ou informatique si vous avez besoin de plus d’informations.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td> <p>Vous devez être un administrateur ou une administratrice Workfront.</p> <p><b>NOTE</b> : si vous n’avez toujours pas accès, demandez à votre administrateur ou administratrice Workfront si des restrictions supplémentaires à votre niveau d’accès ont été appliquées. Pour plus d’informations sur la façon dont l’administration Workfront peut modifier votre niveau d’accès, consultez la section <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Créer ou modifier des niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Activer Outlook pour une utilisation avec Workfront et SAML 2.0

{{step-1-to-setup}}

1. Cliquez sur **Système** > **Préférences**.

1. Dans la section **Sécurité**, assurez-vous que l’option **Autoriser l’authentification SAML 2.0 dans les modules complémentaires Office 365** est activée.

   Cette option permet d’intégrer Workfront dans un iframe uniquement pour les modules complémentaires d’Office 365. Cela n’ouvre pas une brèche au piratage par clic, car il n’y a pas de contenu cliquable.

   Cette option est activée par défaut.

   >[!NOTE]
   >
   >Si vous activez l’option **Autoriser l’incorporation de Workfront dans un iframe**, l’option **Autoriser l’authentification SAML 2.0 dans les modules complémentaires Office 365** est grisée et activée.
   >
   >![Option Autoriser l’incorporation](assets/if-you-enable.png)
   >

1. Cliquer sur **Enregistrer**.

   Les modifications que vous avez enregistrées ici affectent l’expérience de l’ensemble des utilisateurs et utilisatrices de Workfront.
