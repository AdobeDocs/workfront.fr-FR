---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Modifier les étapes d’épreuve et les réviseurs et réviseuses
description: Découvrez comment modifier les phases de BAT et les réviseurs.
author: Courtney
feature: Digital Content and Documents
exl-id: 91549c2d-d7b1-461c-a3c4-ad0032acfb23
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 9%

---

# Modifier les étapes d’épreuve et les réviseurs et réviseuses

Vous pouvez modifier les phases et les détails des réviseurs dans un BAT si vous êtes le propriétaire ou le créateur du BAT ou si le rôle du BAT approprié est attribué.

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
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rôle de BAT</td> 
   <td>Auteur ou modérateur </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurations des niveau d’accès*</td> 
   <td> <p>Accès en modification aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demander l’accès aux objets</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront Proof.

## Modification d’une étape

1. Dans une liste de documents contenant le document, passez la souris sur la ligne contenant le document, puis cliquez sur **Processus de vérification de l’intégrité**.

   Ou

   Dans le Workfront Proof autonome, cliquez sur le menu **Plus** (trois points) à droite du BAT, puis cliquez sur **Afficher les détails du BAT**.

1. Apportez l’une des modifications suivantes à la section **Workflow** :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Modifier la date limite</td> 
      <td> <p>Sélectionnez la date et choisissez une nouvelle date dans le calendrier qui s’affiche. Pour supprimer complètement l’échéance, sélectionnez la date, puis sélectionnez <strong>Effacer</strong> sous le calendrier qui s’affiche.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suppression d’un réviseur individuel</td> 
      <td> <p>Sélectionnez le menu <strong>Plus</strong> situé à droite du nom du réviseur, puis cliquez sur <strong>Supprimer</strong> dans le menu déroulant. Cliquez sur <strong>Confirmer</strong> dans la zone qui s’affiche pour supprimer le réviseur du BAT.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suppression de plusieurs réviseurs</td> 
      <td>Cochez les cases en regard de leur nom, puis cliquez sur l’icône <strong>Supprimer</strong> près du coin supérieur droit de la section d’étape.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envoyer un message à tous les opérateurs validants</td> 
      <td>Sélectionnez le menu <strong>Plus</strong> dans le coin supérieur droit de la section de scène, puis sélectionnez <strong>Message all</strong>. Configurez votre message, puis sélectionnez <strong>Envoyer</strong>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ajout d’un réviseur à l’étape</td> 
      <td>Sélectionnez le menu <strong>Plus</strong> dans le coin supérieur droit de la section de scène, puis sélectionnez <strong>Partager</strong>. Ajoutez l’utilisateur, configurez son rôle et ses alertes par e-mail, puis répétez-les si nécessaire. Lorsque vous avez terminé, cliquez sur <strong>Partager</strong>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer l’étape</td> 
      <td> <p>Sélectionnez le menu <strong>Plus</strong> dans le coin supérieur droit de la section d’étape, puis sélectionnez l’étape <strong>Supprimer</strong> .</p> <p>Remarque : S’il n’existe qu’une seule étape, celle-ci ne peut pas être supprimée.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Modifier les détails du validant

1. Dans Workfront, passez la souris sur le BAT, puis cliquez sur **Détails du BAT** pour ouvrir la page Détails du BAT.
1. Dans la section **Workflow** , cliquez sur le menu **Plus** ![](assets/more-button-small.png) situé à droite du nom du réviseur, puis cliquez sur **Modifier** dans le menu déroulant qui s’affiche.

1. Dans la zone **Modifier le réviseur** qui s’affiche, modifiez les détails suivants :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nom d’affichage*</td> 
      <td> <p>Pour modifier le nom d'affichage du validant sur le BAT, cliquez dans le champ texte et modifiez en ligne son nom.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rôle</td> 
      <td>Pour modifier le rôle du validant sur le BAT, ouvrez le menu déroulant et sélectionnez le rôle préféré. Voir pour plus d’informations.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alertes par e-mail</td> 
      <td>Pour modifier l’alerte email du réviseur sur le BAT, ouvrez le menu déroulant et sélectionnez l’alerte email de votre choix. Pour plus d’informations, reportez-vous à l’article <a href="../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md" class="MCXref xref"> Notifications pour les commentaires de BAT et la présentation des décisions </a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Décision*</td> 
      <td> <p>Pour modifier la décision du validant sur le BAT, ouvrez le menu déroulant et sélectionnez la décision souhaitée. Notez que toute décision que vous prenez au nom d’un autre utilisateur est indiquée dans la section Activité du BAT. Cette option s’affiche uniquement lorsque la révision a pris une décision.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Étape</td> 
      <td>Il n'est pas possible de déplacer les réviseurs d'une étape à l'autre. Cependant, vous pouvez supprimer et rajouter un réviseur avec un délai différent.</td> 
     </tr> 
    </tbody> 
   </table>

   &#42; Vous devez être le créateur ou le propriétaire du BAT pour modifier ce champ.

1. Cliquer sur **Enregistrer**.
