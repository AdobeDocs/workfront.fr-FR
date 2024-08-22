---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Erreur : l’utilisateur à configuration automatique ne peut pas se connecter"
description: Si un utilisateur disposant des privilèges d’accès automatique tente de se connecter pour la première fois et reçoit une erreur indiquant que le système ne lui affecte pas de niveau d’accès, cela peut être dû au fait que votre système ne dispose pas des niveaux d’accès associés à la licence Request.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 23%

---

# Erreur : l’utilisateur avec provisionnement automatique ne peut pas se connecter.

Lorsqu’un utilisateur muni d’un profil d’approvisionnement automatique tente de se connecter pour la première fois, il reçoit l’erreur suivante :

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problème

Le système n’affecte pas au nouvel utilisateur un niveau d’accès.

Par défaut, la mise en service automatique utilise le type de licence Request . S’il n’existe aucun niveau d’accès avec une licence Request , le système ne peut pas attribuer un niveau d’accès à l’utilisateur.

## Conditions d’accès

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

Créez un niveau d’accès de base avec une licence Request :

1. Accédez à **[!UICONTROL Configuration]** > **[!UICONTROL Niveaux d’accès]**.

1. Cliquez sur **[!UICONTROL New Access Level]**.
1. Saisissez un **[!UICONTROL Nom]**.
1. Dans le menu déroulant **[!UICONTROL Type de licence]**, sélectionnez Demander.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

Après avoir créé un niveau d’accès avec une licence de demande, demandez à l’utilisateur de se connecter avec ses informations d’identification SSO.


