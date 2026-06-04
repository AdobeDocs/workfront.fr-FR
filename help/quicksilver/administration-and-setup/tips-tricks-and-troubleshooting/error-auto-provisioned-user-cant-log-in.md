---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Erreur : l''utilisateur affecté automatiquement ne peut pas se connecter'
description: Si un utilisateur configuré automatiquement tente de se connecter pour la première fois et reçoit une erreur indiquant que le système ne lui affecte pas de niveau d’accès, cela peut être dû au fait que votre système ne dispose pas des niveaux d’accès associés à la licence Request.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
TQID: https://experienceleague.adobe.com/jUBGb9lqH9QL34Rw-oEhjty3l3wAf8avcLgtVe1-VSg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 200
ht-degree: 74%

---

# Erreur : la personne auto-allouée ne peut pas se connecter.

Lorsqu’une personne auto-allouée tente de se connecter pour la première fois, elle reçoit l’erreur suivante :

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problème

Le système n’affecte pas de niveau d’accès au nouvel utilisateur ou à la nouvelle utilisatrice.

Par défaut, l’auto-allocation utilise le type de licence Demande. Lorsqu’il n’existe aucun niveau d’accès avec une licence Demande, le système ne peut pas affecter de niveau d’accès à l’utilisateur ou à l’utilisatrice.

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

Créer un niveau d’accès de base avec une licence Demande :

1. Accédez à **[!UICONTROL Configurer]** > **[!UICONTROL Niveaux d’accès]**.

1. Cliquez sur **[!UICONTROL Nouveau niveau d’accès]**.
1. Saisissez un **[!UICONTROL nom]**.
1. Dans le menu déroulant **[!UICONTROL Type de licence]**, sélectionnez Demande.
1. Cliquez sur **[!UICONTROL Enregistrer les modifications]**.

Après avoir créé un niveau d’accès avec une licence Demande, demandez à l’utilisateur ou l’utilisatrice de se connecter avec ses identifiants SSO.


