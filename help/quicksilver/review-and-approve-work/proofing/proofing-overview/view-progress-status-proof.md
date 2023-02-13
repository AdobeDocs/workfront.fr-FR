---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Présentation de l’état et de la progression du BAT
description: Vous pouvez afficher des informations sur l’avancement d’un BAT tout au long du processus de révision et un résumé global de l’état de décision du BAT dans la zone Documents .
author: Courtney
feature: Digital Content and Documents
exl-id: 78e81070-ff82-4d82-90a3-6e0cd176b290
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 2%

---

# Présentation de l’état et de la progression du BAT

Vous pouvez afficher des informations sur l’avancement d’un BAT tout au long du processus de révision et un résumé global de l’état de décision du BAT dans la zone Documents .

## Présentation de la progression du BAT

La progression de la preuve indique le travail effectué sur un BAT depuis le moment où vous envoyez le BAT aux destinataires jusqu’au moment où ils prennent une décision sur le BAT. Les icônes de progression, S, O, C et D, apparaissent à côté du nom du BAT et fournissent des informations sur la progression du BAT.

![](assets/proof-edit-existing-progress-350x62.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Icône Progression</strong> </p> </td> 
   <td> <p><strong>Description</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt=""> </p> <p><strong>Envoyé</strong> </p> </td> 
   <td> <p>Le BAT a été envoyé aux destinataires affectés.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Ouvert</strong> </p> </td> 
   <td> <p>Tous les destinataires attribués ouvrent la page des détails du BAT ou du BAT.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Commentaires</strong> </p> </td> 
   <td> <p>Tous les destinataires assignés font au moins un commentaire sur le BAT.</p> <p>Si aucun opérateur validant n'est affecté au BAT, la variable <strong>C</strong> n’apparaît pas dans la barre de progression.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt=""> </p> <p><strong>Décision prise</strong> </p> </td> 
   <td> <p>Tous les approbateurs affectés prennent une décision sur le BAT, Tous les approbateurs affectés prennent une décision sur le BAT, sauf si le créateur du BAT indique qu’une seule décision est nécessaire.</p> <p>Si aucun approbateur (décideur) n’est désigné pour le BAT, la variable <strong>D</strong> n’apparaît pas dans la barre de progression. </p> </td> 
  </tr> 
 </tbody> 
</table>

Les icônes de progression peuvent apparaître dans les couleurs suivantes pour indiquer certaines informations sur la progression du BAT :

* **Vert**: Terminé.
* **Blanc**: Non terminé.
* **Orange**: non terminé et délai inférieur à 24 heures.
* **Rouge**: Ne pas terminer et dépasser la date limite.

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Levels of proof progress</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof uses the progress icons to track a proof's progress at each of the following levels:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each reviewer, based on that person's activity on the proof.&nbsp;</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each stage, based on the progress the reviewer on the stage who is most behind in the proofing process.&nbsp;To learn more about stages, see <a href="../../../review-and-approve-work/proofing/proofing-overview/stages.md" class="MCXref xref">Automated Workflow Stages overview</a>.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For the proof, based on the progress of the stage (group of reviewers) who is the most behind in the proofing process.</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For an example of how Workfront Proof determines progress using the reviewer or stage that is most behind,&nbsp;suppose three reviewers on a proof need to make a&nbsp;decision. If two of them have made their&nbsp;decision&nbsp;but the third has not, the progress bar for the proof does not show&nbsp;the D in green because of the outstanding&nbsp;decision.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If the Primary Decision Maker setting is selected on a proof and the primary decision maker submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Similarly, if the Only One Decision Required setting is selected on a proof and any reviewer submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

## Aperçu de l’état du BAT

Le statut du BAT affiche le statut des décisions requises pour le BAT. Le statut du BAT dépend du participant au &quot;pire cas&quot;. Par exemple, supposons qu’il y ait trois décisions sur le BAT : deux ont le statut de **Acceptée** et l’un a le statut de **Rejetés**. La décision &quot;la pire des situations&quot; de **Rejetés** sur-règlemente les autres décisions et le statut global du BAT est affiché comme **Rejetés**. 

![](assets/proof-edit-existing-progress-350x62.png)

Les options d’état standard sont les suivantes :

* En attente
* Approuvé
* Approuvé avec des modifications
* Modifications requises
* Non pertinent

Si des décisions personnalisées sont configurées dans votre compte, les options d’état reflètent vos paramètres de décision personnalisés.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Viewing proof progress and status</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You can view the progress and status of proofs for individual documents. </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-progress-and-status-for-a-document" class="MCXref xref">View proof progress and status&nbsp;for a document</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-approval-information-in-home" class="MCXref xref">View proof approval information&nbsp;in Home</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-progress-and-status-for-a-document">View proof progress and status&nbsp;for a document</h3>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">If a proof has not already been generated for the document in Adobe Workfront, generate it, as described in the articles.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Documents area, under the proof's name, click <strong>Proof Details</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Proofing Details</strong> box that appears, the proof's progress for each stage, then click <strong>Done</strong>.</li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Under the proof's name, click <strong>Proofing Workflow</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <img src="assets/click-proofing-workflow-qs-350x149.png" style="width: 350;height: 149;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
   -->
<!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   These screenshots will need to change with new terminology ("Review Workflow" for this one?)
   </MadCap:conditionalText>
   <br> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Workflow information that appears, scroll down to see the proof's progress for each stage:</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/scroll-to-see-socd-for-stages-qs-350x152.png" style="width: 350;height: 152;"> </p>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-approval-information-in-home">View proof approval information&nbsp;in Home</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can view information about proofs that you have submitted for approval. Proof approval information is displayed in the Home area only while the proof is pending approval.&nbsp;For information about how to view information about proof approvals in the Home area, see&nbsp;<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a>.</p>
-->
