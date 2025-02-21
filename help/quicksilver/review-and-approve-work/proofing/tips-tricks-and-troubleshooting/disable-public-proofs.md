---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: désactiver,public,partager,épreuve,public,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Désactiver le partage de l’épreuve via une URL publique ou un code intégré
description: Vous pouvez désactiver la possibilité de partager une épreuve avec une URL publique ou un code intégré sur une épreuve sur la base des épreuves ou pour des personnes.
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 93%

---

# Désactiver le partage de l’épreuve via une URL publique ou un code intégré

Vous pouvez désactiver la possibilité de partager une épreuve avec une URL publique ou un code intégré sur une épreuve sur la base des épreuves ou pour des personnes.

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

Vous devez disposer des accès suivants pour effectuer les étapes décrites dans cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Plan actuel : Pro ou version supérieure</p> <p>ou</p> <p>Formule héritée : Select ou Premium</p> <p>Pour plus d’informations sur la relecture de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accéder aux fonctionnalités de relecture dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Plan actuel : travail ou plan</p> <p>Plan hérité : n’importe lequel (la relecture doit être activée pour l’utilisateur ou l’utilisatrice)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander un accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation d’épreuve dont vous disposez, contactez votre administrateur ou administratrice Workfront ou Workfront Proof.

+++

## Désactiver par épreuve

Vous devez être la personne propriétaire ou créatrice de l’épreuve, ou avoir le rôle d’auteur ou autrice ou de modérateur ou modératrice de l’épreuve.

1. Dans le projet qui contient l’épreuve, cliquez sur **Documents** dans le panneau de gauche.
1. Pointez sur l’épreuve et sélectionnez **Détails du document**.
1. Dans le panneau de gauche, cliquez sur **Paramètres de la visionneuse de relecture**, puis désactivez la case à cocher **Autoriser le partage de l’épreuve via une URL publique ou un code incorporé**.

   ![Paramètres de la visionneuse de vérification](assets/proofing-viewer-settings-350x200.png)

1. Cliquer sur **Enregistrer**.

## Désactiver par utilisateur

Vous pouvez désactiver le paramètre Épreuve publique pour les personnes de votre instance Workfront. Pour apporter cette modification, vous devez disposer du profil d’autorisation d’épreuve de l’administrateur ou administratrice.

1. Cliquez sur l&#39;icône **Menu principal** ![icône du menu principal](assets/main-menu-icon.png) dans le coin supérieur droit d&#39;Adobe Workfront, puis cliquez sur **Vérification**.
1. Cliquez sur **Paramètres du compte** près du coin supérieur droit.
1. Cliquez sur le bouton **Utilisateurs et utilisatrices**, puis cliquez sur le nom d’un utilisateur ou d’une utilisatrice.
1. Dans la section **Paramètres d’épreuve par défaut**, désactivez la case à cocher **Partage public**.

   ![ Partage public ](assets/default-proof-settings--public-sharing-350x210.png)
