---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Message d’erreur : échec de l’authentification SAML 2.0 : identifiant utilisateur introuvable'
description: Lorsque vous utilisez SAML 2.0, l’erreur « Échec de l’authentification SAML 2.0 - Identifiant d’utilisateur introuvable » signifie qu’un UID ou un ID NAME n’est pas transmis à partir des règles de réclamation ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 81%

---

# Message d’erreur : échec de l’authentification SAML 2.0 : identifiant d’utilisateur ou d’utilisatrice introuvable

## Problème

Cette erreur s’affiche lorsque j’utilise SAML 2.0 : « Échec de l’authentification SAML 2.0 : identifiant de l’utilisateur ou l’utilisatrice introuvable ».

## Cause

Cela se produit lorsqu’un **UID** ou **NAME ID** n’est pas transmis à partir des **règles de revendication ADFS**.

Dans ADFS, la **Partie de confiance** doit disposer d’une **Règle de revendication** qui transmet soit une valeur **UID**, soit une valeur **NAME ID**. Lorsque vous exécutez une connexion de test **[!DNL Workfront]**, cela doit s’afficher en cas de réussite.

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

1. Pour modifier **[!UICONTROL ADFS INFO]**, allez à **[!UICONTROL Parties de confiance]** > Sélectionner un objet > **[!UICONTROL Modifier les règles de revendication]**.

1. L’**[!UICONTROL attribut LDAP]** (colonne de gauche) doit avoir la valeur **[!UICONTROL Adresses e-mail]** (ou tout identifiant unique).

1. La valeur **[!UICONTROL Type de revendication sortante]** (colonne de droite) doit être **[!UICONTROL ID de nom]**.

   >[!NOTE]
   >
   >Il n’est pas nécessaire que les adresses e-mail d’attribut LDAP soient indiquées. Tout identifiant unique d’une personne peut être utilisé, mais doit être transmis à [!DNL Adobe Workfront] en tant que **NAME ID**.
