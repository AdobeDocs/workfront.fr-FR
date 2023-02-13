---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Modification des phases de BAT et des validants
description: 'Vous devez disposer des droits d’accès suivants pour effectuer les étapes de cet article : MODIFIER MOI.'
author: Courtney
feature: Digital Content and Documents
exl-id: 91549c2d-d7b1-461c-a3c4-ad0032acfb23
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 1%

---

# Modification des phases de BAT et des validants

Vous pouvez modifier les phases et les détails des réviseurs dans un BAT si vous êtes le propriétaire ou le créateur du BAT ou si le rôle du BAT approprié est attribué.

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Pro ou version ultérieure</p> <p>ou</p> <p>Plan hérité : Sélectionner ou Premium</p> <p>Pour plus d’informations sur la vérification de l’accès avec les différents plans, voir <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Accès aux fonctionnalités de vérification dans Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Formule actuelle : Travail ou plan</p> <p>Plan hérité : N’importe quel (la vérification doit être activée pour l’utilisateur)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil d'autorisation pour l'épreuve </td> 
   <td>Manager ou version ultérieure</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rôle BAT</td> 
   <td>Auteur ou modérateur </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront BAT.

## Modification d’une étape

1. Dans une liste de documents contenant le document, passez la souris sur la ligne contenant le document, puis cliquez sur **Workflow de vérification**.

   Ou

   Dans le BAT Workfront autonome, cliquez sur le bouton **Plus** (trois points) à droite du BAT, puis cliquez sur **Afficher les détails du BAT**.

1. Apportez l’une des modifications suivantes dans le **Workflow** section :

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
      <td> <p>Sélectionnez la <strong>Plus</strong> à droite du nom du validant, puis cliquez sur <strong>Supprimer</strong> dans le menu déroulant. Cliquez sur <strong>Confirmer</strong> dans la zone qui s’affiche pour retirer le validant du BAT.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suppression de plusieurs réviseurs</td> 
      <td>Cochez les cases en regard de leur nom, puis cliquez sur le bouton <strong>Supprimer</strong> près du coin supérieur droit de la section scène.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envoyer un message à tous les opérateurs validants</td> 
      <td>Sélectionnez la <strong>Plus</strong> dans le coin supérieur droit de la section scène, puis sélectionnez <strong>Message all</strong>. Configurez votre message, puis sélectionnez <strong>Envoyer</strong>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ajout d’un réviseur à l’étape</td> 
      <td>Sélectionnez la <strong>Plus</strong> dans le coin supérieur droit de la section scène, puis sélectionnez <strong>Partager</strong>. Ajoutez l’utilisateur, configurez son rôle et ses alertes par e-mail, puis répétez-les si nécessaire. Lorsque vous avez terminé, cliquez sur <strong>Partager</strong>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Supprimer l’étape</td> 
      <td> <p>Sélectionnez la <strong>Plus</strong> dans le coin supérieur droit de la section scène, sélectionnez <strong>Supprimer</strong> scène.</p> <p>Remarque : S’il n’y a qu’une seule étape, la scène ne peut pas être supprimée.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Modifier les détails du validant

1. Dans Workfront, passez la souris sur le BAT, puis cliquez sur **Détails du BAT** pour ouvrir la page Détails de la vérification.
1. Dans le **Workflow** , cliquez sur le bouton **Plus** menu ![](assets/more-button-small.png) à droite du nom du validant, puis cliquez sur **Modifier** dans le menu déroulant qui s’affiche.

1. Dans le **Modifier le validant** qui s’affiche, modifiez l’un des détails suivants :

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
      <td role="rowheader">Alertes par email</td> 
      <td>Pour modifier l’alerte email du réviseur sur le BAT, ouvrez le menu déroulant et sélectionnez l’alerte email de votre choix. Pour plus d’informations, voir dans l’article <a href="../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md" class="MCXref xref">Présentation des notifications pour les commentaires de BAT et les décisions</a>.</td> 
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

   &#42; Pour modifier ce champ, vous devez être le créateur ou le propriétaire du BAT.

1. Cliquer sur **Enregistrer**.
