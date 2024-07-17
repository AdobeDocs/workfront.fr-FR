---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Message d’erreur : Erreur SAML 2.0 : Identifiant utilisateur introuvable"
description: Vous ne pouvez pas établir une connexion réussie à ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 34%

---

# Message d’erreur : erreur SAML 2.0 : identifiant utilisateur introuvable

## Problème

Vous ne pouvez pas établir une connexion réussie à ADFS.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Si vous établissez une connexion de test réussie et que vous rencontrez toujours des problèmes, vous pouvez rencontrer des mappages d’attributs ou des problèmes avec les ID de fédération. Contactez l’assistance clientèle pour toute question.

## Cause :

Les revendications sur le serveur ADFS sont incorrectes

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

## Solution

Sur le serveur ADFS, assurez-vous qu’il existe une demande pour l’ID de nom :

1. Sous Windows, cliquez sur **[!UICONTROL Démarrer]** > **[!UICONTROL Administration]** > **[!UICONTROL Gestion ADFS 2.0]**.\
   La boîte de dialogue Gestion ADFS 2.0 s’affiche.

1. Sélectionnez **[!UICONTROL Trust Relationship]** > **[!UICONTROL Relying Party Trtrust]** dans le volet de gauche.

1. Cliquez avec le bouton droit de la souris sur la confiance de la partie de confiance associée à Adobe Workfront, puis sélectionnez **[!UICONTROL Modifier les règles de réclamation]**.
1. Vérifiez que la demande a un **[!UICONTROL Type de demande sortante]** de **[!UICONTROL ID de nom]**.

![1.png](assets/1-350x287.png)
