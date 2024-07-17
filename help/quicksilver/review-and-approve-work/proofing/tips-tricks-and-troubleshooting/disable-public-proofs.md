---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: disable,public,share,proof,public,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Désactiver le partage d’épreuve via une URL publique ou un code intégré
description: Vous pouvez désactiver la possibilité de partager un BAT avec une URL publique ou un code intégré sur un BAT par BAT ou pour des utilisateurs individuels.
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 19%

---

# Désactiver le partage d’épreuve via une URL publique ou un code intégré

Vous pouvez désactiver la possibilité de partager un BAT avec une URL publique ou un code intégré sur un BAT par BAT ou pour des utilisateurs individuels.

## Conditions d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Forfait Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou supérieure</p> <p>ou</p> <p>Formule héritée : sélectionnez ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Formule héritée : Toutes (la vérification doit être activée pour l’utilisateur).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront Proof.

## Désactiver par BAT

Vous devez être le propriétaire ou le créateur du BAT, ou vous devez avoir le rôle d’auteur ou de modérateur du BAT.

1. Dans le projet qui contient le BAT, cliquez sur **Documents** dans le panneau de gauche.
1. Passez la souris sur le BAT et sélectionnez **Document Details** .
1. Dans le panneau de gauche, cliquez sur **Paramètres de la visionneuse de vérification de l’évocation**, puis désactivez la case à cocher **Autoriser le partage du BAT via une URL publique ou le code incorporé** .

   ![](assets/proofing-viewer-settings-350x200.png)

1. Cliquer sur **Enregistrer**.

## Désactiver par utilisateur

Vous pouvez désactiver le paramètre BAT public pour les utilisateurs individuels de votre instance Workfront. Pour apporter cette modification, vous devez disposer d’un profil d’autorisation de BAT de l’administrateur.

1. Cliquez sur l’icône **Menu principal** ![](assets/main-menu-icon.png) dans le coin supérieur droit d’Adobe Workfront, puis cliquez sur **Vérification**.
1. Cliquez sur **Paramètres du compte** près du coin supérieur droit.
1. Cliquez sur l’onglet **Utilisateurs** , puis sur le nom d’un utilisateur.
1. Dans la section **Paramètres par défaut du BAT**, désactivez la case à cocher **Partage public** .

   ![](assets/default-proof-settings--public-sharing-350x210.png)
