---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Message d''erreur : Échec de l’authentification SAML 2.0 : Identifiant utilisateur introuvable"'
description: Lorsque vous utilisez SAML 2.0, l’erreur "Échec de l’authentification SAML 2.0 - Identifiant utilisateur introuvable" signifie qu’un UID ou un ID NAME n’est pas transmis des règles de demande ADFS. Dans ADFS, la Trust Party doit avoir une règle de réclamation qui transmet un UID ou une valeur d’ID NAME. Lorsque vous exécutez une [!DNL Workfront] Tester la connexion, cela doit s’afficher en cas de réussite.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---

# Message d’erreur : Échec de l’authentification SAML 2.0 : Identifiant utilisateur introuvable

## Problème

Je reçois cette erreur lors de l’utilisation de SAML 2.0 : &quot;Échec de l’authentification SAML 2.0 : Identifiant utilisateur introuvable.&quot;

## Cause

Cela se produit lorsqu’une **UID** ou **Identifiant NOM** n’est pas transmis à partir de la fonction **Règles de demande ADFS**.

Dans ADFS, la variable **Confiance du parti de confiance** doit disposer d’un **Règle de demande** qui transmet **UID** ou **Identifiant NOM** . Lorsque vous exécutez une **[!DNL Workfront]Tester la connexion**, cela doit s’afficher en cas de réussite.

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

## Solution

1. Lors de la modification de la variable **[!UICONTROL INFORMATIONS SUR LES ADFS]**, dans la variable **[!UICONTROL Confiance des parties]** > Sélectionner un objet >**[!UICONTROL Modifier des règles de demande]**.

1. Le **[!UICONTROL Attribut LDAP]** (colonne de gauche) doit avoir la valeur **[!UICONTROL Adresses électroniques]** (ou tout identifiant unique).

1. Le **[!UICONTROL Type de demande sortante]** (colonne de droite) doit être **[!UICONTROL ID de nom]**.

   >[!NOTE]
   >
   >Il n’est pas nécessaire d’avoir les adresses électroniques de l’attribut LDAP. Tout identifiant unique qui identifiera l’utilisateur peut être utilisé, mais doit être transmis. [!DNL Adobe Workfront] comme la propriété **Identifiant NOM**.
