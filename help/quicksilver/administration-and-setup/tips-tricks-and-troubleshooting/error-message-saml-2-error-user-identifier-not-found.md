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
ht-degree: 28%

---

# Message d’erreur : erreur SAML 2.0 : identifiant utilisateur introuvable

## Problème

Vous ne pouvez pas établir une connexion réussie à ADFS.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Si vous établissez une connexion de test réussie et que vous rencontrez toujours des problèmes, vous pouvez rencontrer des mappages d’attributs ou des problèmes avec les ID de fédération. Contactez l’assistance clientèle pour toute question.

## Cause :

Les revendications sur le serveur ADFS sont incorrectes.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td>
   <p>Nouvelle : standard</p>
   <p>ou</p>
   <p>Actuelle : formule</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td>Vous devez être un administrateur ou une administratrice [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Pour plus d’informations sur ce tableau, consultez [Conditions d’accès requises dans la documentation Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solution

Sur le serveur ADFS, assurez-vous qu’il existe une demande pour l’ID de nom :

1. Sous Windows, cliquez sur **[!UICONTROL Démarrer]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion ADFS 2.0]**.\
   La boîte de dialogue Gestion ADFS 2.0 s’affiche.

1. Sélectionnez **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trtrust]** dans le volet de gauche.

1. Cliquez avec le bouton droit de la souris sur la confiance de la partie de confiance associée à Adobe Workfront, puis sélectionnez **[!UICONTROL Modifier les règles de réclamation]**.
1. Vérifiez que la demande a un **[!UICONTROL Type de demande sortante]** de **[!UICONTROL ID de nom]**.

![1.png](assets/1-350x287.png)
