---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Message d’erreur : erreur SAML 2.0 : identifiant d’utilisateur ou d’utilisatrice introuvable'
description: Vous ne pouvez pas établir une connexion réussie à ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 95%

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

## Solution

Sur le serveur ADFS, assurez-vous qu’il existe une revendication pour l’ID de nom :

1. Sous Windows, cliquez sur **[!UICONTROL Démarrer]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion d’ADFS 2.0]**.\
   La boîte de dialogue Gestion d’ADFS 2.0 s’affiche.

1. Sélectionnez **[!UICONTROL Relation de confiance]** > **[!UICONTROL Parties de confiance]** dans le volet de gauche.

1. Cliquez avec le bouton droit de la souris sur la partie de confiance associée à Adobe Workfront, puis sélectionnez **[!UICONTROL Modifier les règles de revendication]**.
1. Vérifiez que la revendication comporte un **[!UICONTROL Type de revendication sortante]** de **[!UICONTROL ID de nom]**.

![1.png](assets/1-350x287.png)
