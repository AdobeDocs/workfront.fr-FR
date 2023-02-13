---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Prendre une décision sur un BAT dans la visionneuse de vérification
description: Vous pouvez prendre une décision sur un BAT directement dans la visionneuse de vérification.
author: Courtney
feature: Digital Content and Documents
exl-id: cf74ac54-b8c1-4404-b35f-2aa94831ecad
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 3%

---

# Prendre une décision sur un BAT dans la visionneuse de vérification

Vous pouvez prendre une décision sur un BAT directement dans la visionneuse de vérification.

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
   <td>Approbateur, réviseur et approbateur, auteur, modérateur</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Modifier l’accès aux documents</p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le rôle ou le profil d’autorisation de BAT dont vous disposez, contactez votre administrateur Workfront ou Workfront BAT.

## Prendre une décision sur un BAT dans la visionneuse de vérification

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.
1. Recherchez le BAT dont vous avez besoin, puis cliquez sur **BAT ouvert**.

1. Cliquez sur **Prendre une décision** dans le centre supérieur de la visionneuse de vérification.

1. Dans le **Décision du BAT** qui s’affiche, cliquez sur l’une des décisions suivantes :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Approuvé</td> 
      <td>Le BAT est prêt à passer à l’étape suivante du processus automatisé.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Approuvé avec des modifications</td> 
      <td>Le BAT nécessite des modifications, mais vous n’avez pas besoin de voir la révision avant qu’elle ne passe à l’étape suivante du processus automatisé.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modifications requises</td> 
      <td>Le BAT nécessite des modifications et vous devez voir une autre révision avant de passer à l’étape suivante du processus automatisé.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Non pertinent</td> 
      <td>Le BAT n'est pas pertinent pour vous et vous n'avez pas besoin de prendre une décision.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Décision personnalisée</td> 
      <td> <p>Sur les plans Select et Premium, l’administrateur Workfront ou l’administrateur Workfront BAT peut renommer, réorganiser et masquer les décisions. Pour plus d’informations, voir <a href="../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md" class="MCXref xref">Configuration des options de décision d’approbation dans le BAT Workfront</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Conditionnel) Si l’administrateur Adobe Workfront ou l’administrateur du Bon à tirer de Workfront a ajouté une section Raisons , sélectionnez les raisons applicables à votre décision. Pour plus d’informations sur la façon dont les administrateurs peuvent configurer des motifs de décision, voir  [Configuration des options de décision d’approbation dans le BAT Workfront](../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).
1. (Facultatif) Sélectionnez **M&#39;envoyer une confirmation par email** pour recevoir une confirmation par email de votre décision.
1. Cliquez sur **Prendre une décision**.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Make a decision when the proof is configured with an approval process</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can make decisions on a proof when it is configured with an approval process (within Workfront) and&nbsp;a user has sent you a document approval request, as described in <a href="../../../../review-and-approve-work/manage-approvals/request-document-approvals.md" class="MCXref xref">Request document approvals</a>.</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#make-a-workfront-approval-decision-in-a-proof" class="MCXref xref">Make a Workfront approval decision in a proof</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#change-your-workfront-approval-decision-in-a-proof" class="MCXref xref">Change your Workfront approval decision in a proof</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="make-a-workfront-approval-decision-in-a-proof">Make a Workfront approval decision in a proof</h3>
-->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Open the proof of the document that you want to make a decision on.</p>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the proofing viewer, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="change-your-workfront-approval-decision-in-a-proof">Change your Workfront approval decision in a proof</h3>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof of the document where you want to change your Workfront approval decision.</li>
<li value="2"> <p>At the top-center of the proofing viewer, click the decision you made previously.</p> </li>
<li value="3">In the <strong>Proof decision</strong> box that appears, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
</ol>
-->
