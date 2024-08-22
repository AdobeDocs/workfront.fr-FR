---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Message d’erreur : Échec de l’authentification SAML 2.0 : identifiant utilisateur introuvable"
description: Lorsque vous utilisez SAML 2.0, l’erreur "Échec de l’authentification SAML 2.0 - Identifiant utilisateur introuvable" signifie qu’un UID ou un ID NAME n’est pas transmis des règles de demande ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 23%

---

# Message d’erreur : Échec de l’authentification SAML 2.0 : identifiant utilisateur introuvable

## Problème

Cette erreur s’affiche lorsque j’utilise SAML 2.0 : &quot;Échec de l’authentification SAML 2.0 : identifiant de l’utilisateur introuvable.&quot;.

## Cause

Cela se produit lorsqu’un **UID** ou un **ID NAME** n’est pas transmis par les ****   des   règles de demande ADFS.

Dans ADFS, le **Relying Party Trust** doit avoir une **règle de réclamation** qui transmet soit une valeur **UID** soit une valeur **NAME ID**. Lorsque vous exécutez une **[!DNL Workfront]Test Connection**, elle doit l’afficher en cas de réussite.

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

1. Lors de la modification de l’ **[!UICONTROL ADFS INFO]**, dans le répertoire **[!UICONTROL Fidélisation]** > Sélectionner un objet >**[!UICONTROL Modifier les règles de demande]**.

1. L’ **[!UICONTROL attribut LDAP]** (colonne de gauche) doit comporter **[!UICONTROL Adresses de messagerie]** (ou tout identifiant unique).

1. Le **[!UICONTROL Type de réclamation sortante]** (colonne de droite) doit être **[!UICONTROL ID de nom]**.

   >[!NOTE]
   >
   >Il n’est pas nécessaire d’avoir les adresses électroniques de l’attribut LDAP. Tout identifiant unique qui identifiera l’utilisateur peut être utilisé, mais il doit être transmis dans [!DNL Adobe Workfront] en tant que **NAME ID**.
