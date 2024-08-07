---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Afficher les étapes de workflow automatisé sur une épreuve
description: Vous pouvez facilement suivre la progression d’un BAT configuré avec un workflow automatisé. Vous pouvez afficher, modifier, ajouter, démarrer et verrouiller le travail déjà effectué sur les scènes du BAT.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: f252e3562b8ea73486d407138251b3d15d4b9f3a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 10%

---

# Afficher les étapes de workflow automatisé sur une épreuve

Vous pouvez facilement suivre la progression d’un BAT configuré avec un workflow automatisé. Vous pouvez afficher, modifier, ajouter, démarrer et verrouiller le travail déjà effectué sur les scènes du BAT.

Pour plus d’informations sur l’ajout d’étapes et d’utilisateurs à un BAT avec un workflow automatisé, voir [Ajout d’étapes et d’utilisateurs à un workflow automatisé sur un BAT](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Conditions d’accès

+++ Développez pour afficher les exigences d’accès aux fonctionnalités de cet article.

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
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront Proof.

+++

## Affichage du diagramme Processus automatisé

1. Dans une liste de documents contenant le document, passez la souris sur la ligne contenant le document, puis cliquez sur **Processus de vérification de l’intégrité**.

   Le diagramme pour le workflow automatisé s’affiche juste sous le titre du workflow.

   Les étapes du diagramme sont marquées comme suit :

   ![dot.png](assets/dot.png) Étape active

   ![gri_dot.png](assets/grey-dot.png) Etape inactive\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  Etape privée

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  Étape verrouillée

   Les lignes entre les scènes représentent les dépendances entre les scènes. Les lignes menant aux scènes inactives sont pointillées jusqu’à ce que l’étape soit activée.

   Vous pouvez positionner le pointeur de la souris sur une scène du diagramme pour afficher sa progression. Si l’étape n’est pas active et que vous disposez des droits d’édition sur l’étape, vous pouvez cliquer sur le bouton Activer l’étape ![](assets/activate-stage-btn.png) pour lancer l’étape. Si l’étape est active et que vous disposez de droits d’édition sur l’étape, vous pouvez la verrouiller. ![](assets/lock-stage-btn.png) Pour plus d’informations sur la barre de progression (S, O, C, D) , voir  [Afficher la progression et l’état d’un bon à tirer dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Affichage d’une scène

1. Dans une liste de documents contenant le document, passez la souris sur la ligne contenant le document, puis cliquez sur **Processus de vérification de l’intégrité**.
1. Sur le diagramme, cliquez sur la scène à afficher.

   ![](assets/view-stage-diagram-350x204.png)

1. Pour développer les détails d’une scène, cliquez sur la flèche latérale située sous son nom.

   ![](assets/stage-details-caret-350x167.png)

## Afficher toutes les étapes

Pour afficher toutes les étapes d’un processus automatisé :

1. Cliquez sur le bouton Modifier la vue en haut de la page ![](assets/change-view-btn.png), puis cliquez sur **Afficher toutes les étapes**.

   Toutes les étapes du processus automatisé sont répertoriées dans la section , mais les détails sont masqués.

1. Pour développer les détails d’une scène, cliquez sur la flèche latérale située sous son nom.

## Afficher toutes les étapes en détail

Pour afficher toutes les étapes de votre processus automatisé avec leurs détails étendus :

1. Cliquez sur le bouton Modifier la vue en haut de la page ![](assets/change-view-btn.png), puis cliquez sur **Afficher toutes les étapes en détail**.
1. Pour afficher les détails d’une scène, cliquez sur la flèche vers le bas située sous son nom.
