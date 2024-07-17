---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Message d’erreur : Échec de l’authentification SAML 2.0 : identifiant utilisateur introuvable'
description: Lorsque vous utilisez SAML 2.0, l’erreur "Échec de l’authentification SAML 2.0 - Identifiant utilisateur introuvable" signifie qu’un UID ou un ID NAME n’est pas transmis des règles de demande ADFS. Dans ADFS, la Trust Party doit avoir une règle de réclamation qui transmet un UID ou une valeur d’ID NAME. Lorsque vous exécutez un  [!DNL Workfront] test de connexion, cela doit s’afficher en cas de réussite.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 25%

---

# Message d’erreur : Échec de l’authentification SAML 2.0 : identifiant utilisateur introuvable

## Problème

Cette erreur s’affiche lorsque j’utilise SAML 2.0 : &quot;Échec de l’authentification SAML 2.0 : identifiant de l’utilisateur introuvable.&quot;.

## Cause

Cela se produit lorsqu’un **UID** ou **ID NAME** n’est pas transmis par les **règles de demande ADFS**.

Dans ADFS, le **Relying Party Trust** doit avoir une **règle de réclamation** qui transmet soit une valeur **UID** ou une valeur **NAME ID**. Lorsque vous exécutez une **[!DNL Workfront]Test Connection**, elle doit l’afficher en cas de réussite.

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

1. Lors de la modification de l’ **[!UICONTROL ADFS INFO]**, dans le répertoire **[!UICONTROL Fidélisation]** > Sélectionner un objet >**[!UICONTROL Modifier les règles de demande]**.

1. L’ **[!UICONTROL attribut LDAP]** (colonne de gauche) doit comporter **[!UICONTROL Adresses de messagerie]** (ou tout identifiant unique).

1. Le **[!UICONTROL Type de réclamation sortante]** (colonne de droite) doit être **[!UICONTROL ID de nom]**.

   >[!NOTE]
   >
   >Il n’est pas nécessaire d’avoir les adresses électroniques de l’attribut LDAP. Tout identifiant unique qui identifiera l’utilisateur peut être utilisé, mais il doit être transmis dans [!DNL Adobe Workfront] en tant que **NAME ID**.
