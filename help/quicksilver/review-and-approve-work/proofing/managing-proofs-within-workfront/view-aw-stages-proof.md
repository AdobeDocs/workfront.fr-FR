---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Afficher les étapes du workflow automatisé sur une épreuve
description: Vous pouvez suivre facilement la progression d’une épreuve configurée avec un workflow automatisé. Vous pouvez visualiser, modifier, ajouter, démarrer et verrouiller le travail déjà effectué lors des étapes de l’épreuve.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 82%

---

# Afficher les étapes du workflow automatisé sur une épreuve

Vous pouvez suivre facilement la progression d’une épreuve configurée avec un workflow automatisé. Vous pouvez visualiser, modifier, ajouter, démarrer et verrouiller le travail déjà effectué lors des étapes de l’épreuve.

Pour plus d’informations sur l’ajout d’étapes et d’utilisateurs ou utilisatrices à une épreuve avec un workflow automatisé, voir [Ajouter des étapes et des utilisateurs ou utilisatrices à un workflow automatisé sur une épreuve](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

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
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version supérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations du niveau d’accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander un accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation d’épreuve dont vous disposez, contactez votre administrateur ou administratrice de Workfront ou Workfront Proof.

+++

## Voir le diagramme du workflow automatisé

1. Dans une liste de documents contenant le document, passez votre souris sur la ligne contenant le document, puis cliquez sur **Workflow de relecture**.

   Le diagramme du workflow automatisé s’affiche juste en dessous du titre du workflow.

   Les étapes du diagramme sont marquées comme suit :

   ![dot.png](assets/dot.png) Étape active

   ![grey_dot.png](assets/grey-dot.png) Étape inactive\
   ![sbw-key-icon.png](assets/sbw-key-icon.png) Étape privée

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png) Étape verrouillée

   Les lignes entre les étapes représentent les dépendances entre elles. Les lignes menant aux étapes inactives sont pointillées jusqu’à ce que l’étape soit activée.

   Vous pouvez passer votre souris sur une étape dans le diagramme pour afficher sa progression. Si l’étape n’est pas active et que vous disposez des droits de modification sur l’étape, vous pouvez cliquer sur le bouton Activer l’étape ![Activer l’étape](assets/activate-stage-btn.png) pour démarrer l’étape. Si l’étape est active et que vous disposez de droits de modification de l’étape, vous pouvez la verrouiller. ![Étape de verrouillage](assets/lock-stage-btn.png) Pour plus d’informations sur la barre de progression (S, O, C, D) , voir  [Afficher la progression et le statut d’une épreuve dans Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Afficher une étape

1. Dans une liste de documents contenant le document, passez votre souris sur la ligne contenant le document, puis cliquez sur **Workflow de relecture**.
1. Sur le diagramme, cliquez sur l’étape que vous souhaitez afficher.

   ![Afficher le diagramme d’étape](assets/view-stage-diagram-350x204.png)

1. Pour développer les détails d’une étape, cliquez sur la flèche latérale située sous son nom.

   ![Détails de l’étape](assets/stage-details-caret-350x167.png)

## Afficher toutes les étapes

Pour afficher toutes les étapes d’un workflow automatisé, procédez comme suit :

1. Cliquez sur le bouton Modifier l’affichage en haut de la page ![Modifier l’affichage](assets/change-view-btn.png), puis cliquez sur **Afficher toutes les étapes**.

   Toutes les étapes du workflow automatisé sont répertoriées dans la section, mais les détails sont masqués.

1. Pour développer les détails d’une étape, cliquez sur la flèche latérale située sous son nom.

## Afficher toutes les étapes en détail

Pour afficher toutes les étapes de votre workflow automatisé avec leurs détails développés :

1. Cliquez sur le bouton Modifier l’affichage en haut de la page ![Modifier l’affichage](assets/change-view-btn.png), puis cliquez sur **Afficher toutes les étapes en détail**.
1. Pour afficher les détails d’une étape, cliquez sur la flèche vers le bas située sous son nom.
