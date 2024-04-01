---
product-area: documents
navigation-topic: approvals
title: Créer une demande d’approbation ou de révision de document
description: Vous pouvez demander l’approbation d’un document à d’autres utilisateurs dans Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: a02699e1-3557-47f0-89b7-dbecb507a174
source-git-commit: e8116a6778d5952ba583cfdfb94b761757adc030
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Créer une demande d’approbation ou de révision de document

<span class="preview">Les informations mises en surbrillance sur cette page font référence à des fonctionnalités qui ne sont pas encore disponibles dans l’ensemble. Elle est disponible uniquement dans l’environnement Aperçu de l’environnement de test.</span>

Vous pouvez demander l’approbation d’un document dans Adobe Workfront à d’autres utilisateurs ou équipes, ou demander à ces utilisateurs de le réviser sans avoir à l’approuver.

>[!IMPORTANT]
>
>Le contenu de cet article fait référence à la fonctionnalité d’approbation de document mise à jour, disponible uniquement pour des comptes spécifiques. Pour plus d’informations sur les processus de validation standard, reportez-vous aux articles répertoriés dans la section [Approbations de travail](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Exigences d’accès

Vous devez disposer des accès suivants pour effectuer les étapes de cet article :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Formule Adobe Workfront*</td> 
   <td> <p>Quelconque</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licence Adobe Workfront*</td> 
   <td> <p>Révision ou version ultérieure</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Paramétrages du niveau d'accès*</td> 
   <td> <p>Affichage ou accès supérieur à Projets, Tâches, Problèmes, Modèles, Portfolios, Programmes, Rapports, Tableaux de bord et Calendriers, Documents</p> <p>Remarque : Si vous n’avez toujours pas accès à , demandez à votre administrateur Workfront s’il définit des restrictions supplémentaires à votre niveau d’accès. Pour plus d’informations sur la façon dont un administrateur Workfront peut modifier votre niveau d’accès, voir <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Création ou modification de niveaux d’accès personnalisés</a>.</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Autorisations d’objet</td> 
   <td> <p>Gérer l'accès à l'objet associé à l'accès ou à la validation de la demande </p> <p>Pour plus d’informations sur la demande d’accès supplémentaire, voir <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Demande d’accès aux objets </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Pour connaître le plan, le type de licence ou l’accès dont vous disposez, contactez votre administrateur Workfront.

## Création d’une demande d’approbation ou de révision de document à partir de la page de document

1. Pointez sur le document, puis cliquez sur Détails du document.
   ![](assets/doc-details.png)


1. Près du nom du document, sélectionnez la version du document pour laquelle vous souhaitez créer une approbation dans la liste déroulante des versions. La dernière version est sélectionnée par défaut.

1. Cliquez sur **Approbations** dans le volet de gauche.

1. <span class="preview">(Facultatif) Définissez une date limite de validation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant la date limite spécifiée.</span>

1. Pour ajouter un approbateur, cliquez sur le bouton **Approbateur** et commencez à saisir le nom d’un utilisateur ou d’une équipe.

1. Pour ajouter un validant, cliquez sur le bouton **Réviseur** et commencez à saisir un nom d’utilisateur ou d’équipe.

   ![](assets/add-approver-and-deadline.png)

1. Répétez l’étape précédente pour ajouter d’autres approbateurs ou réviseurs.

## Créer une demande d’approbation ou de révision de document à partir du volet Résumé du document

1. Accédez au projet, à la tâche ou au problème qui contient le document, puis sélectionnez **Documents**.

1. Cliquez sur le document dont vous avez besoin et le volet Résumé du document de ce document s’ouvre.

1. Sélectionnez la version du document pour laquelle vous souhaitez créer une approbation dans la liste déroulante des versions. La dernière version est sélectionnée par défaut.

1. Faites défiler l’écran vers le bas jusqu’à **Approbations** dans le volet Résumé du document, puis cliquez sur **Ajouter**.

![](assets/doc-summary-add-approvers.png)

1. <span class="preview">(Facultatif) Définissez une date limite de validation. Les utilisateurs et les équipes sont avertis par e-mail 72 heures, puis 24 heures avant la date limite spécifiée.</span>

1. Pour ajouter un approbateur, cliquez sur le bouton **Approbateur** et commencez à saisir le nom d’un utilisateur ou d’une équipe.

1. Pour ajouter un validant, cliquez sur le bouton **Réviseur** et commencez à saisir un nom d’utilisateur ou d’équipe.

   ![](assets/add-approver-and-deadline.png)

1. Répétez l’étape précédente pour ajouter d’autres approbateurs ou réviseurs.

<!--
## Resubmit an approval on a new version

Document approval decisions are not automatically reset when you upload a new version. For example, if your document is approved with changes, the decision will show "changes" as the decision, even if you upload a new version with the specified changes. You can clear the decision on a new version if you manually resubmit the approval.

1. Go to the project, task, or issue that contains the document, then select **Documents**.
1. Find the document you need.

1. Scroll down to the **Approvals** section in the Summary, click the More icon, then click Resubmit.

   ![](assets/nwe-resubmit-approval-350x149.png)
-->
