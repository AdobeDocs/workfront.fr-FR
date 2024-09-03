---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Message d’erreur : Erreur SAML 2.0 : Identifiant utilisateur introuvable"
description: Vous ne pouvez pas établir une connexion réussie à ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 92%

---

# Message d’erreur : erreur SAML 2.0 : identifiant d’utilisateur ou d’utilisatrice introuvable

## Problème

Vous ne pouvez pas établir une connexion réussie à ADFS.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Si vous établissez une connexion de test réussie et que vous rencontrez toujours des problèmes, vous pourriez avoir des mappages d’attributs incorrects ou rencontrer des problèmes avec les ID de fédération. Contactez l’assistance clientèle pour toute question.

## Cause :

Les revendications sur le serveur ADFS sont incorrectes.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Tous</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licence</td> 
   <td>
   <p>Nouveau : Standard</p>
   <p>ou</p>
   <p>Actuel : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveaux d’accès</td> 
   <td>Vous devez être administrateur ou administratrice [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus de détails sur les informations contenues dans ce tableau, consultez [Conditions d’accès préalables dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

Sur le serveur ADFS, assurez-vous qu’il existe une revendication pour l’ID de nom :

1. Sous Windows, cliquez sur **[!UICONTROL Démarrer]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion d’ADFS 2.0]**.\
   La boîte de dialogue Gestion d’ADFS 2.0 s’affiche.

1. Sélectionnez **[!UICONTROL Relation de confiance]** > **[!UICONTROL Parties de confiance]** dans le volet de gauche.

1. Cliquez avec le bouton droit de la souris sur la partie de confiance associée à Adobe Workfront, puis sélectionnez **[!UICONTROL Modifier les règles de revendication]**.
1. Vérifiez que la revendication comporte un **[!UICONTROL Type de revendication sortante]** de **[!UICONTROL ID de nom]**.

![1.png](assets/1-350x287.png)
