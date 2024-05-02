---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Erreur : l’utilisateur avec provisionnement automatique ne peut pas se connecter"
description: Si un utilisateur disposant des privilèges d’accès automatique tente de se connecter pour la première fois et reçoit une erreur indiquant que le système ne lui affecte pas de niveau d’accès, cela peut être dû au fait que votre système ne dispose pas des niveaux d’accès associés à la licence Request. La mise en service automatique utilise le type de demande de licence afin que vous puissiez résoudre ce problème en créant un niveau d’accès associé à une demande de licence.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 477f65efb09e8566dd0af88adfbe88135d6c6ae9
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 9%

---

# Erreur : l’utilisateur avec provisionnement automatique ne peut pas se connecter.

Lorsqu’un utilisateur muni d’un profil d’approvisionnement automatique tente de se connecter pour la première fois, il reçoit l’erreur suivante :

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problème

Le système n’affecte pas au nouvel utilisateur un niveau d’accès.

Par défaut, la mise en service automatique utilise le type de licence Request . S’il n’existe aucun niveau d’accès avec une licence Request , le système ne peut pas attribuer un niveau d’accès à l’utilisateur.

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
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès</td> 
   <td> <p>Vous devez être un [!DNL Workfront] administrateur. Pour plus d’informations, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Octroi d’un accès administratif complet à un utilisateur</a>.</p> <p><b>REMARQUE</b>: si vous n’avez toujours pas accès à , demandez [!DNL Workfront] s’ils définissent des restrictions supplémentaires au niveau de votre accès. Pour plus d’informations sur la manière dont une [!DNL Workfront] l’administrateur peut modifier votre niveau d’accès, voir <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solution

Créez un niveau d’accès de base avec une licence Request :

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Niveaux d’accès]**.

1. Cliquez sur **[!UICONTROL Nouveau niveau d’accès]**.
1. Saisissez un **[!UICONTROL Nom]**.
1. Dans le **[!UICONTROL Type de licence]** , sélectionnez Demander.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

Après avoir créé un niveau d’accès avec une licence de demande, demandez à l’utilisateur de se connecter avec ses informations d’identification SSO.


